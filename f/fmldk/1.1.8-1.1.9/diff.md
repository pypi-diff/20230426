# Comparing `tmp/fmldk-1.1.8.tar.gz` & `tmp/fmldk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmldk-1.1.8.tar", last modified: Tue Apr  4 18:41:17 2023, max compression
+gzip compressed data, was "fmldk-1.1.9.tar", last modified: Wed Apr 26 08:01:25 2023, max compression
```

## Comparing `fmldk-1.1.8.tar` & `fmldk-1.1.9.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.658231 fmldk-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-04-04 18:41:17.658231 fmldk-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-04-04 18:41:04.000000 fmldk-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.642230 fmldk-1.1.8/ctfr/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/ctfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/ctfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/ctfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/ctfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/ctfr_models_v0.1.29.py
--rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfr/ctfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.642230 fmldk-1.1.8/ctfrv2/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfrv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfrv2/ctfrv2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfrv2/ctfrv2_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfrv2/ctfrv2_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    85749 2023-04-04 18:41:04.000000 fmldk-1.1.8/ctfrv2/ctfrv2_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.646231 fmldk-1.1.8/eda/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-04 18:41:04.000000 fmldk-1.1.8/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-04-04 18:41:04.000000 fmldk-1.1.8/eda/eda_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-04 18:41:04.000000 fmldk-1.1.8/eda/eda_lib_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-04-04 18:41:04.000000 fmldk-1.1.8/eda/eda_lib_v0.1.19.py
--rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-04-04 18:41:04.000000 fmldk-1.1.8/eda/eda_lib_v0.1.37.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.646231 fmldk-1.1.8/fmldk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-04-04 18:41:17.000000 fmldk-1.1.8/fmldk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-04 18:41:17.000000 fmldk-1.1.8/fmldk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:41:17.000000 fmldk-1.1.8/fmldk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-04 18:41:17.000000 fmldk-1.1.8/fmldk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 18:41:17.000000 fmldk-1.1.8/fmldk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.646231 fmldk-1.1.8/sage/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/sage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    62668 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/sage_data_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/sage_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/sage_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/sage_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    79131 2023-04-04 18:41:04.000000 fmldk-1.1.8/sage/sage_model_old.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 18:41:17.658231 fmldk-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-04 18:41:04.000000 fmldk-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.646231 fmldk-1.1.8/stctn/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-04 18:41:04.000000 fmldk-1.1.8/stctn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-04-04 18:41:04.000000 fmldk-1.1.8/stctn/stctn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-04 18:41:04.000000 fmldk-1.1.8/stctn/stctn_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-04 18:41:04.000000 fmldk-1.1.8/stctn/stctn_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-04-04 18:41:04.000000 fmldk-1.1.8/stctn/stctn_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.654231 fmldk-1.1.8/tfr/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.14.py
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.15.py
--rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.16.py
--rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.18.py
--rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_data_v0.1.21.py
--rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_local_block_sparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_local_block_sparse_attention_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_local_block_sparse_attention_v0.1.12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_models_v0.1.10.py
--rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_models_v0.1.11.py
--rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_models_v0.1.23.py
--rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-04-04 18:41:04.000000 fmldk-1.1.8/tfr/tfr_models_v0.1.31.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:41:17.658231 fmldk-1.1.8/tft/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_data_v1.1.3.py
--rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_data_v1.1.7.py
--rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_global_scaled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_losses_bkp.py
--rw-r--r--   0 runner    (1001) docker     (123)    81746 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_model_v0.1.26.py
--rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_model_v0.1.31.py
--rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-04-04 18:41:04.000000 fmldk-1.1.8/tft/tft_model_v1.1.3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.819284 fmldk-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-04-26 08:01:25.819284 fmldk-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-04-26 08:01:12.000000 fmldk-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/ctfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55520 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113137 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105725 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_models_v0.1.29.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111862 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfr/ctfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/ctfrv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55580 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42022 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86435 2023-04-26 08:01:12.000000 fmldk-1.1.9/ctfrv2/ctfrv2_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22984 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib_v0.1.19.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-04-26 08:01:12.000000 fmldk-1.1.9/eda/eda_lib_v0.1.37.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.807284 fmldk-1.1.9/fmldk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 08:01:25.000000 fmldk-1.1.9/fmldk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.811284 fmldk-1.1.9/sage/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46583 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_global_scaled_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_losses_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86777 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83909 2023-04-26 08:01:12.000000 fmldk-1.1.9/sage/sage_model_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:01:25.819284 fmldk-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 08:01:12.000000 fmldk-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.811284 fmldk-1.1.9/stctn/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55190 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-04-26 08:01:12.000000 fmldk-1.1.9/stctn/stctn_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.815284 fmldk-1.1.9/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55577 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37924 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46425 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.16.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54017 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.18.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55773 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_data_v0.1.21.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107319 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_local_block_sparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93067 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97067 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_losses_bkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113988 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.10.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100101 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.11.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109483 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.23.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114250 2023-04-26 08:01:12.000000 fmldk-1.1.9/tfr/tfr_models_v0.1.31.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:25.819284 fmldk-1.1.9/tft/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46581 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55578 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data_v1.1.3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62667 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_data_v1.1.7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42019 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_global_scaled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84122 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64043 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model_v0.1.26.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65090 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model_v0.1.31.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-04-26 08:01:12.000000 fmldk-1.1.9/tft/tft_model_v1.1.3.py
```

### Comparing `fmldk-1.1.8/PKG-INFO` & `fmldk-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.1.8
+Version: 1.1.9
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.1.8/README.md` & `fmldk-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfr/ctfr_data.py` & `fmldk-1.1.9/ctfr/ctfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfr/ctfr_losses.py` & `fmldk-1.1.9/ctfr/ctfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfr/ctfr_losses_bkp.py` & `fmldk-1.1.9/ctfr/ctfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfr/ctfr_models.py` & `fmldk-1.1.9/ctfr/ctfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfr/ctfr_models_v0.1.29.py` & `fmldk-1.1.9/ctfr/ctfr_models_v0.1.29.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfr/ctfr_models_v0.1.31.py` & `fmldk-1.1.9/ctfr/ctfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfrv2/ctfrv2_data.py` & `fmldk-1.1.9/ctfrv2/ctfrv2_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfrv2/ctfrv2_global_scaled_data.py` & `fmldk-1.1.9/ctfrv2/ctfrv2_global_scaled_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfrv2/ctfrv2_losses.py` & `fmldk-1.1.9/ctfrv2/ctfrv2_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/ctfrv2/ctfrv2_models.py` & `fmldk-1.1.9/ctfrv2/ctfrv2_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import shutil
 import pickle
 import absl.logging
 absl.logging.set_verbosity(absl.logging.ERROR)
 import pandas as pd
-
+import os
 
 # Distribution Sampling functions
 
 # negbin
 def negbin_sample(mu, alpha, n_samples=1):
     tol = 1e-5
     r = 1.0 / alpha
@@ -1687,33 +1687,50 @@
                  num_heads,
                  kernel_sizes,
                  d_model,
                  forecast_horizon,
                  max_inp_len,
                  loss_type,
                  num_quantiles,
-                 decoder_lags='Default',
-                 dropout_rate=0.1):
+                 decoder_lags=1,
+                 dropout_rate=0.1,
+                 seed=None,
+                 deterministic_ops=False):
         
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.kernel_sizes = kernel_sizes
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.decoder_lags = decoder_lags
         self.dropout_rate = dropout_rate
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
-    
+        self.seed = seed
+        self.allow_deterministic_ops = deterministic_ops
+
+    def set_seed(self):
+        tf.keras.utils.set_random_seed(self.seed)
+        if self.allow_deterministic_ops:
+            print("Deterministic Ops enabled.")
+            os.environ["TF_DETERMINISTIC_OPS"] = "True"
+            os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+
     def build(self):
         tf.keras.backend.clear_session()
+        if self.seed is None:
+            print("No seed set for deterministic weights initialization")
+        else:
+            print("Using seed {} for weights initialization".format(self.seed))
+            self.set_seed()
+
         self.model = ConvVarTransformer_Model(self.col_index_dict,
                                   self.vocab_dict,
                                   self.num_layers,
                                   self.num_heads,
                                   self.kernel_sizes,
                                   self.d_model,
                                   self.forecast_horizon,
```

### Comparing `fmldk-1.1.8/eda/eda_lib.py` & `fmldk-1.1.9/eda/eda_lib.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/eda/eda_lib_v0.1.18.py` & `fmldk-1.1.9/eda/eda_lib_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/eda/eda_lib_v0.1.19.py` & `fmldk-1.1.9/eda/eda_lib_v0.1.19.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/eda/eda_lib_v0.1.37.py` & `fmldk-1.1.9/eda/eda_lib_v0.1.37.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/fmldk.egg-info/PKG-INFO` & `fmldk-1.1.9/fmldk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmldk
-Version: 1.1.8
+Version: 1.1.9
 Summary: Forecast ML library
 Author: Rahul Sinha
 Author-email: rahul.sinha@unilever.com
 Description-Content-Type: text/markdown
 
 ### A library to easily build & train Transformer models for forecasting.
```

### Comparing `fmldk-1.1.8/fmldk.egg-info/SOURCES.txt` & `fmldk-1.1.9/fmldk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 fmldk.egg-info/SOURCES.txt
 fmldk.egg-info/dependency_links.txt
 fmldk.egg-info/requires.txt
 fmldk.egg-info/top_level.txt
 sage/__init__.py
 sage/sage_data.py
 sage/sage_data_old.py
-sage/sage_global_scaled_data.py
+sage/sage_global_scaled_data_old.py
 sage/sage_losses.py
+sage/sage_losses_old.py
 sage/sage_model.py
 sage/sage_model_old.py
 stctn/__init__.py
 stctn/stctn_data.py
 stctn/stctn_losses.py
 stctn/stctn_losses_bkp.py
 stctn/stctn_models.py
@@ -51,16 +52,16 @@
 tfr/tfr_models.py
 tfr/tfr_models_v0.1.10.py
 tfr/tfr_models_v0.1.11.py
 tfr/tfr_models_v0.1.23.py
 tfr/tfr_models_v0.1.31.py
 tft/__init__.py
 tft/tft_data.py
+tft/tft_data_old.py
 tft/tft_data_v1.1.3.py
 tft/tft_data_v1.1.7.py
 tft/tft_global_scaled_data.py
 tft/tft_losses.py
-tft/tft_losses_bkp.py
 tft/tft_model.py
 tft/tft_model_v0.1.26.py
 tft/tft_model_v0.1.31.py
 tft/tft_model_v1.1.3.py
```

### Comparing `fmldk-1.1.8/sage/sage_data.py` & `fmldk-1.1.9/sage/sage_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/sage/sage_data_old.py` & `fmldk-1.1.9/tft/tft_data_v1.1.7.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from bokeh.palettes import Category10, Category20, Colorblind
 from bokeh.io import reset_output
 from bokeh.models.ranges import DataRange1d
 
 # COMMAND ----------
 
 
-class sage_dataset:
+class tft_dataset:
     def __init__(self, 
                  col_dict, 
                  window_len, 
                  fh, 
                  batch, 
                  min_nz,
                  scaling_method='mean_scaling',
```

### Comparing `fmldk-1.1.8/sage/sage_global_scaled_data.py` & `fmldk-1.1.9/sage/sage_global_scaled_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/sage/sage_losses.py` & `fmldk-1.1.9/sage/sage_losses_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/sage/sage_model.py` & `fmldk-1.1.9/sage/sage_model_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/sage/sage_model_old.py` & `fmldk-1.1.9/sage/sage_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# Databricks notebook source
+#!/usr/bin/env python
+# coding: utf-8
+
+
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import shutil
 import pickle
 import absl.logging
 absl.logging.set_verbosity(absl.logging.ERROR)
 import pandas as pd
 import gc
-
+import os
 
 # Distribution Sampling functions
 
 # negbin
 def negbin_sample(mu, alpha, n_samples=1):
     tol = 1e-5
     r = 1.0 / alpha
@@ -57,14 +60,17 @@
 def GumbelSample(a, b, n_samples=1):
     dist = tfd.Gumbel(loc=a, scale=b)
     return tf.reduce_mean(tf.stop_gradient(dist.sample(sample_shape=n_samples)), axis=0)
 
 def min_power_of_2(x):
     return m.ceil(m.log2(x))
 
+
+# Model Class - Dense Transformer w/ Variable Selection
+
 # Positional Encoding
 
 def get_angles(pos, i, d_model):
     angle_rates = 1 / np.power(10000, (2 * (i//2)) / np.float32(d_model))
     return pos * angle_rates
   
 @tf.function
@@ -245,41 +251,14 @@
 # Point-wise FFN
 
 def point_wise_feed_forward_network(d_model, dff):
     return tf.keras.Sequential([tf.keras.layers.Dense(dff, activation='relu'),  # (batch_size, seq_len, dff)
                                 tf.keras.layers.Dense(d_model)  # (batch_size, seq_len, d_model)
                                ])
     
-# Encoder Layer - Conv Attention
-
-class ConvEncoderLayer(tf.keras.layers.Layer):
-    def __init__(self, d_model, num_heads, kernel_sizes, dff, rate):
-        super(ConvEncoderLayer, self).__init__()
-
-        self.mha = MultiHeadConvAttention(d_model, num_heads, kernel_sizes)
-        self.ffn = point_wise_feed_forward_network(d_model, dff)
-
-        self.layernorm1 = tf.keras.layers.LayerNormalization(epsilon=1e-6)
-        self.layernorm2 = tf.keras.layers.LayerNormalization(epsilon=1e-6)
-    
-        self.dropout1 = tf.keras.layers.Dropout(rate)
-        self.dropout2 = tf.keras.layers.Dropout(rate)
-    
-    def call(self, x, mask, training):
-
-        attn_output, _ = self.mha(x, x, x, mask, training=training)  # (batch_size, input_seq_len, d_model)
-        attn_output = self.dropout1(attn_output, training=training)
-        out1 = self.layernorm1(x + attn_output)                      # (batch_size, input_seq_len, d_model)
-    
-        ffn_output = self.ffn(out1, training=training)               # (batch_size, input_seq_len, d_model)
-        ffn_output = self.dropout2(ffn_output, training=training)
-        out2 = self.layernorm2(out1 + ffn_output)                    # (batch_size, input_seq_len, d_model)
-    
-        return out2
-
 
 # Decoder Layer - Conv Attention
 
 class ConvDecoderLayer(tf.keras.layers.Layer):
     def __init__(self, d_model, num_heads, kernel_sizes, dff, rate):
         super(ConvDecoderLayer, self).__init__()
 
@@ -301,68 +280,29 @@
     
         ffn_output = self.ffn(out1, training=training)  # (batch_size, target_seq_len, d_model)
         ffn_output = self.dropout2(ffn_output, training=training)
         out2 = self.layernorm2(ffn_output + out1)  # (batch_size, target_seq_len, d_model)
     
         return out2, attn_weights_block1
 
-
-# Conv Encoder Module
-
-class ConvEncoder(tf.keras.layers.Layer):
-    def __init__(self, num_layers, d_model, num_heads, kernel_sizes, dff, maximum_position_encoding, rate):
-        super(ConvEncoder, self).__init__()
-
-        self.d_model = d_model
-        self.num_layers = num_layers
-    
-        self.pos_encoding = positional_encoding(maximum_position_encoding, self.d_model)
-        
-        self.enc_layers = [ConvEncoderLayer(d_model, num_heads, kernel_sizes, dff, rate) for _ in range(num_layers)]
-  
-        self.dropout = tf.keras.layers.Dropout(rate)
-        
-    def call(self, x, mask, training):
-
-        seq_len = tf.shape(x)[1]
-    
-        # adding position encoding.
-        x += self.pos_encoding[:, :seq_len, :]
-        
-        x = self.dropout(x, training=training)
-    
-        for i in range(self.num_layers):
-            x = self.enc_layers[i](x, mask, training=training)
-    
-        return x  # (batch_size, input_seq_len, d_model)
-
 # Conv Decoder Module
 
 class ConvDecoder(tf.keras.layers.Layer):
-    def __init__(self, num_layers, d_model, num_heads, kernel_sizes, dff, maximum_position_encoding, rate):
+    def __init__(self, num_layers, d_model, num_heads, kernel_sizes, dff, rate):
         super(ConvDecoder, self).__init__()
 
         self.d_model = d_model
         self.num_layers = num_layers
-    
-        self.pos_encoding = positional_encoding(maximum_position_encoding, d_model)
-        
         self.dec_layers = [ConvDecoderLayer(d_model, num_heads, kernel_sizes, dff, rate) for _ in range(num_layers)]
         
-        self.dropout = tf.keras.layers.Dropout(rate)
-    
     def call(self, x, look_ahead_mask, padding_mask, training):
 
         seq_len = tf.shape(x)[1]
         attention_weights = {}
-    
-        x += self.pos_encoding[:, -seq_len:, :]
-    
-        x = self.dropout(x, training=training)
-
+        
         for i in range(self.num_layers):
             x, block1 = self.dec_layers[i](x, look_ahead_mask, padding_mask, training=training)
       
         attention_weights['decoder_layer{}_block1'.format(i+1)] = block1
         
         return x, attention_weights
     
@@ -522,31 +462,58 @@
                                                                         additional_context=False, 
                                                                         return_gate=False)
     def call(self, inputs, training):
         static_var_select_vec = self.static_context_variable_selection(inputs, training=training)
         return static_var_select_vec
       
 class static_enrichment_layer(tf.keras.layers.Layer):
-    def __init__(self, hidden_layer_size, dropout_rate):
+    def __init__(self, hidden_layer_size, context, dropout_rate):
         super(static_enrichment_layer, self).__init__()
 
         self.hidden_layer_size = hidden_layer_size
         self.dropout_rate = dropout_rate
+        self.context = context
         self.grn_enrich = gated_residual_network(hidden_layer_size=self.hidden_layer_size,
                                                  output_size=None,
                                                  dropout_rate=self.dropout_rate,
                                                  use_time_distributed=True,
-                                                 additional_context=True,
+                                                 additional_context=self.context,
                                                  return_gate=False)
-    def call(self,inputs, training):
-        # inputs: [temporal_features, static_enrichment_vec]
-        x,c = inputs
-        c = tf.expand_dims(c, axis=1)
-        enriched = self.grn_enrich([x,c], training=training)
+    def call(self, inputs, training):
+        if self.context:
+            x,c = inputs
+            c = tf.expand_dims(c, axis=1)
+            enriched = self.grn_enrich([x,c], training=training)
+        else:
+            x = inputs
+            enriched = self.grn_enrich(x, training=training)
+            
         return enriched
+
+# LSTM Layer
+
+class lstm_layer(tf.keras.layers.Layer):
+    def __init__(self, hidden_layer_size, rnn_layers, dropout_rate):
+        super(lstm_layer, self).__init__()
+
+        self.rnn_layers = rnn_layers
+        self.hidden_layer_size = hidden_layer_size
+        self.dropout_rate = dropout_rate
+        self.temporal_layer = tf.keras.layers.LSTM(units=hidden_layer_size, return_state=True, return_sequences=True)
+        self.gate = apply_gating_layer(hidden_layer_size=self.hidden_layer_size, dropout_rate=self.dropout_rate, use_time_distributed=True,activation=None)
+        self.add_norm = add_norm_layer()
+
+    def call(self, inputs, training):
+        decoder_in, init_states = inputs
+        lstm_out, enc_h, enc_c = self.temporal_layer(decoder_in, initial_state=init_states, training=training)
+        # Apply gating layer
+        lstm_out, _ = self.gate(lstm_out, training=training)
+        temporal_features = self.add_norm([lstm_out, decoder_in], training=training)
+        return temporal_features
+
       
 class lstm_init_states(tf.keras.layers.Layer):
     """
     Takes static_vec as input
     """
     def __init__(self, hidden_layer_size, output_size, dropout_rate):
         super(lstm_init_states, self).__init__()
@@ -609,30 +576,25 @@
             mlp_outputs = self.grn_flat([flatten,context], training=training) #[batch,time_steps,num_vars]
         else:
             inputs = x
             flatten = tf.concat(inputs, axis=-1) #[batch,time_steps,sum_of_var_dims]
             mlp_outputs = self.grn_flat(flatten, training=training) #[batch,time_steps,num_vars]
         
         dynamic_weights = tf.keras.layers.TimeDistributed(tf.keras.layers.Activation('softmax'))(mlp_outputs) #[batch,time_steps,num_vars]
-        #weights = tf.expand_dims(dynamic_weights, axis=2) #[batch,time_steps,1,num_vars]
         weights = tf.expand_dims(dynamic_weights, axis=-1) #[batch,time_steps,num_vars,1]
         
         trans_emb_list = []
         for i in range(self.num_vars):
             e = self.grn_var[i](inputs[i], training=training)
             trans_emb_list.append(e)
         
-        #trans_embedding = tf.stack(trans_emb_list, axis=-1) #[batch,time_steps,hidden_layer_size,num_vars]
         trans_embedding = tf.stack(trans_emb_list, axis=2) #[batch,time_steps,num_vars,hidden_layer_size]
-        
         combined = tf.keras.layers.Multiply()([weights, trans_embedding])
-        #tfr_input = tf.reduce_sum(combined, axis=-1) #[batch,time_steps,hidden_layers_size]
         tfr_input = tf.reduce_sum(combined, axis=2) #[batch,time_steps,hidden_layers_size]
-        
-        #print("tfr_input shape:, dynamic_wts shape: ", tfr_input.shape, dynamic_weights.shape)
+       
         return tfr_input, dynamic_weights
       
 class all_variable_select_concat_layer(tf.keras.layers.Layer):
     def __init__(self, hidden_layer_size, output_size, dropout_rate):
         super(all_variable_select_concat_layer, self).__init__()
         
         self.hidden_layer_size = hidden_layer_size
@@ -669,14 +631,35 @@
         trans_embedding = tf.stack(trans_emb_list, axis=2) #[batch,time_steps,num_vars,hidden_layer_size]
         
         combined = tf.keras.layers.Multiply()([weights, trans_embedding]) #[batch,time_steps,num_vars,hidden_layer_size]
         batch_size, timesteps = tf.shape(combined)[0], tf.shape(combined)[1]
         tfr_input = tf.reshape(combined, [batch_size, timesteps, -1]) #[batch,time_steps,hidden_layers_size]
         
         return tfr_input, dynamic_weights   
+    
+    
+class final_gating_layer(tf.keras.layers.Layer):
+    def __init__(self, hidden_layer_size, dropout_rate):
+        super(final_gating_layer, self).__init__()
+        self.hidden_layer_size = hidden_layer_size
+        self.dropout_rate = dropout_rate
+        self.gate = apply_gating_layer(hidden_layer_size=self.hidden_layer_size,
+                                       dropout_rate=self.dropout_rate,
+                                       use_time_distributed=True,
+                                       activation=None)
+        self.add_norm = add_norm_layer()
+
+    def call(self, inputs, training):
+
+        attn_out, temporal_features = inputs
+        # final gating layer
+        attn_out, _ = self.gate(attn_out, training=training)
+        # final add & norm
+        out = self.add_norm([attn_out, temporal_features], training=training)
+        return out
 
 
 class CausalConvEncoder(tf.keras.layers.Layer):
     def __init__(self, d_model, num_layers):
         super(CausalConvEncoder, self).__init__()
         self.layers = []
         for i in range(num_layers):
@@ -685,49 +668,44 @@
           
     def call(self, inputs, training):
         x = inputs
         for layer in self.layers:
             x = layer(x, training=training)
         state = x #[:,-1:,:] # return last hidden state 
         return state
-
-
+    
+    
 class CausalConvResidualLayer(tf.keras.layers.Layer):
     def __init__(self, d_model, seq_len, dropout_rate):
         super(CausalConvResidualLayer, self).__init__()
         self.seq_len = seq_len
         num_causal_layers = int(min_power_of_2(self.seq_len))
-
-        self.conv1x1 = tf.keras.layers.Conv1D(filters=d_model, kernel_size=1)
+        
+        
+        self.conv1x1 = tf.keras.layers.Conv1D(filters=d_model, kernel_size=1) 
         self.causalconvlayer1 = CausalConvEncoder(d_model=d_model, num_layers=num_causal_layers)
-
         self.conv_dropout1 = tf.keras.layers.Dropout(dropout_rate)
-
         self.conv_layernorm1 = tf.keras.layers.LayerNormalization(epsilon=1e-6)
-
         self.conv_activation1 = tf.keras.layers.Activation('selu')
-
         self.conv_add = tf.keras.layers.Add()
-
+        
     def call(self, inputs, training):
         x = inputs
-
+        
         y = self.conv1x1(x)
-
         x = self.causalconvlayer1(x)
         x = self.conv_layernorm1(x)
         x = self.conv_activation1(x)
         x = self.conv_dropout1(x)
-
-        out = self.conv_add([x, y])
-
+        
+        out = self.conv_add([x,y])
+        
         return out
 
-
-# Variable Weighted Transformer Model
+# Sage Model
 
 class SageTransformer(tf.keras.Model):
     def __init__(self,
                  static_variables,
                  num_layers,
                  d_model,
                  num_heads,
@@ -742,31 +720,34 @@
         
         self.hist_len = hist_len
         self.f_len = f_len
         self.loss_fn = loss_fn
         self.stat_variables = static_variables
         self.num_quantiles = num_quantiles
         self.seq_len = int(hist_len + f_len)
-        
-        self.decoder = ConvDecoder(num_layers, d_model, num_heads, kernel_sizes, dff, self.seq_len, rate)
+        self.num_causal_layers = int(min_power_of_2(self.seq_len)) 
         
         if self.stat_variables:
             self.static_input_layer = static_variable_selection_layer(hidden_layer_size=d_model, output_size=None, dropout_rate=rate)
             self.static_context_layer = static_contexts(hidden_layer_size=d_model, output_size=None, dropout_rate=rate)
-            self.static_enrich_layer = static_contexts(hidden_layer_size=d_model, output_size=None, dropout_rate=rate)
-            self.decoder_enrich = add_norm_layer()
+            self.enrich_vector_layer = static_contexts(hidden_layer_size=d_model, output_size=None, dropout_rate=rate)
+            self.init_states_layer = lstm_init_states(hidden_layer_size=d_model, output_size=d_model, dropout_rate=rate)
         
+        self.static_enrich_layer = static_enrichment_layer(hidden_layer_size=d_model, context=self.stat_variables, dropout_rate=rate)
         self.decoder_input_layer = temporal_variable_selection_layer(hidden_layer_size=d_model, output_size=None, context=self.stat_variables, dropout_rate=rate)
+        self.recurrent_layer = lstm_layer(hidden_layer_size=d_model, rnn_layers=1, dropout_rate=rate)
+        self.decoder = ConvDecoder(num_layers, d_model, num_heads, kernel_sizes, dff, rate)
+        self.pff_layer = final_gating_layer(hidden_layer_size=d_model, dropout_rate=rate)
         
         if self.loss_fn == 'Point':
             self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1))
-        elif self.loss_fn == 'Binary':
-            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='sigmoid'))
+        elif self.loss_fn == 'Tweedie':
+            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='linear'))
         elif self.loss_fn == 'Poisson':
-            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='softplus'))
+            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='linear'))
         elif self.loss_fn == 'Quantile':
             self.proj_intrcpt = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation=None))
             if self.num_quantiles > 1:
                 self.proj_incrmnt = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=self.num_quantiles-1, activation='softplus'))
         elif self.loss_fn == 'Normal':
             self.m_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1))
             self.s_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='softplus'))
@@ -784,102 +765,107 @@
         mask: TensorShape(batch,hist+fh_timesteps,1)
         scale: TensorShape(batch,1,1)
         '''
         if self.stat_variables:
             static_vars_list, decoder_vars_list, mask, scale = inputs
         else:
             decoder_vars_list, mask, scale = inputs
+            
+        # scale
+        scale = scale[:,-1:,:]
+        s_dim = scale.shape.as_list()[-1] 
         
-        # scale -- old
-        #scale = scale[:,-1:,:]
-
-        # scale -- new
-        scale = scale[:, -1:, :]
-        s_dim = scale.shape.as_list()[-1]
-
         if s_dim == 2:
-            # print("standard scaling used")
             scaler = 'standard_scaler'
-            scale_mean = scale[:, :, 0:1]
-            scale_std = scale[:, :, 1:2]
+            scale_mean = scale[:,:,0:1]
+            scale_std = scale[:,:,1:2]
         else:
-            # print("mean scaling used")
             scaler = 'mean_scaler'
-            scale_mean = scale[:, :, 0:1]
-            scale_std = scale[:, :, 0:1]
-
+            scale_mean = scale[:,:,0:1]
+            scale_std = scale[:,:,0:1]
+        
         # static var selection 
         if self.stat_variables:
             static_vec, static_weights = self.static_input_layer(static_vars_list, training=training)
             context = self.static_context_layer(static_vec, training=training)
-            static_enrichment_vec = self.static_enrich_layer(static_vec, training=training)
-            static_enrichment_vec = tf.expand_dims(static_enrichment_vec, axis=1)
-
+            enrichment_vec = self.enrich_vector_layer(static_vec, training=training)
+            init_h, init_c = self.init_states_layer(static_vec)            
             # dec input prep
             target_d, decoder_weights = self.decoder_input_layer([decoder_vars_list, context], training=training)
-            target_d = self.decoder_enrich([target_d, static_enrichment_vec])
+
         else:
             static_weights = None
             target_d, decoder_weights = self.decoder_input_layer(decoder_vars_list, training=training)
-          
+            init_h, init_c = tf.zeros([batch_size, self.hidden_layer_size], dtype=tf.float32), tf.zeros([batch_size, self.hidden_layer_size], dtype=tf.float32)
+            
+        # lstm init states
+        init_states = [init_h, init_c]
+        
+        # recurrent_layer
+        temporal_features = self.recurrent_layer([target_d, init_states], training=training)
+        
+        # static feature enrichment
+        if self.stat_variables:
+            enriched_features = self.static_enrich_layer([temporal_features, enrichment_vec], training=training)
+        else:
+            enriched_features = self.static_enrich_layer(temporal_features, training=training)
+        
+        # masks
         padding_mask = create_padding_mask(mask[:,:self.seq_len,0])
         look_ahead_mask = create_look_ahead_mask(self.seq_len)
-        dec_output, _ = self.decoder(target_d, look_ahead_mask, padding_mask, training=training)
+        
+        # attention stack
+        dec_output, _ = self.decoder(enriched_features, look_ahead_mask, padding_mask, training=training)
+        
+        # final_gating_layer
+        dec_output = self.pff_layer([dec_output, temporal_features], training=training)
+        
         dec_output = dec_output[:,-self.f_len:,:]
         decoder_weights = decoder_weights[:, -self.f_len:, :]
         
         if self.loss_fn == 'Point':
             out = self.final_layer(dec_output, training=training)
-        elif self.loss_fn == 'Binary':
+        elif self.loss_fn == 'Tweedie':
             out = self.final_layer(dec_output, training=training)
         elif self.loss_fn == 'Poisson':
-            if scaler == 'mean_scaler':
-                mean = self.final_layer(dec_output, training=training) * scale
-            elif scaler == 'standard_scaler':
-                mean = self.final_layer(dec_output, training=training) * scale_std + scale_mean
-            #mean = self.final_layer(dec_output, training=training)*scale -- old
-            parameters = mean
-            out = poisson_sample(mu=mean)
+            out = self.final_layer(dec_output, training=training)
         elif self.loss_fn == 'Quantile':
             if self.num_quantiles > 1:
                 out = tf.math.cumsum(tf.concat([self.proj_intrcpt(dec_output, training=training), self.proj_incrmnt(dec_output, training=training)], axis=-1), axis=-1)
             else:
                 out = self.proj_intrcpt(dec_output, training=training)
         elif self.loss_fn == 'Normal':
             if scaler == 'mean_scaler':
-                mean = self.m_layer(dec_output, training=training) * scale  # (batch, f_len, 1)
-                stddev = self.s_layer(dec_output, training=training) * scale  # (batch, f_len, 1)
+                mean = self.m_layer(dec_output, training=training)*scale       # (batch, f_len, 1)
+                stddev = self.s_layer(dec_output, training=training)*scale      # (batch, f_len, 1)
             elif scaler == 'standard_scaler':
-                mean = self.m_layer(dec_output, training=training) * scale_std + scale_mean  # (batch, f_len, 1)
-                stddev = self.s_layer(dec_output, training=training) * scale_std  # (batch, f_len, 1)
-            #mean = self.m_layer(dec_output, training=training)*scale       # (batch, f_len, 1)  -- old
-            #stddev = self.s_layer(dec_output, training=training)*scale      # (batch, f_len, 1) -- old
+                mean = self.m_layer(dec_output, training=training)*scale_std + scale_mean       # (batch, f_len, 1)
+                stddev = self.s_layer(dec_output, training=training)*scale_std     # (batch, f_len, 1)     
             parameters = tf.concat([mean, stddev], axis=-1)
             out = normal_sample(mean, stddev)
         elif self.loss_fn == 'Negbin':
             if scaler == 'mean_scaler':
-                mean = self.m_layer(dec_output, training=training) * scale  # (batch, f_len, 1)
-                alpha = self.a_layer(dec_output, training=training) * tf.sqrt(scale)  # (batch, f_len, 1)
+                mean = self.m_layer(dec_output, training=training)*scale       # (batch, f_len, 1)
+                alpha = self.a_layer(dec_output, training=training)*tf.sqrt(scale)      # (batch, f_len, 1)
             elif scaler == 'standard_scaler':
-                mean = self.m_layer(dec_output, training=training) * scale_std + scale_mean  # (batch, f_len, 1)
-                alpha = self.a_layer(dec_output, training=training) * tf.sqrt(scale_std)  # (batch, f_len, 1)
-            #mean = self.m_layer(dec_output, training=training)*scale       # (batch, f_len, 1) -- old
-            #alpha = self.a_layer(dec_output, training=training)*tf.sqrt(scale)      # (batch, f_len, 1) -- old
+                mean = self.m_layer(dec_output, training=training)*scale_std + scale_mean       # (batch, f_len, 1)
+                alpha = self.a_layer(dec_output, training=training)*tf.sqrt(scale_std)      # (batch, f_len, 1)
             parameters = tf.concat([mean, alpha], axis=-1)
             out = negbin_sample(mean, alpha)
         else:
             raise ValueError('Invalid Loss Function.')
-
-        if self.loss_fn == 'Point' or self.loss_fn == 'Quantile':
+       
+        if self.loss_fn in ['Point','Quantile','Tweedie','Poisson']:
             return out, scale, static_weights, decoder_weights
         else:
             return out, parameters, static_weights, decoder_weights
 
 
-# SageTransformer Wrapper
+
+# SAGE Wrapper
 
 class SageTransformer_Model(tf.keras.Model):
     def __init__(self,
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
@@ -895,15 +881,14 @@
         
         self.hist_len = int(max_inp_len-1)
         self.f_len = int(forecast_horizon)
         self.loss_type = loss_type
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         
-        self.num_causal_layers = int(min_power_of_2(self.hist_len+self.f_len)) 
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.kernel_sizes = kernel_sizes
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.dropout_rate = dropout_rate
@@ -914,15 +899,15 @@
             self.static_variables = True
         
         self.model = SageTransformer(static_variables = self.static_variables,
                                     num_layers = num_layers,
                                     d_model = d_model,
                                     num_heads = num_heads, 
                                     kernel_sizes = kernel_sizes,
-                                    dff = int(2*d_model),
+                                    dff = d_model,
                                     hist_len = self.hist_len, 
                                     f_len = self.f_len,
                                     loss_fn = self.loss_type,
                                     num_quantiles = num_quantiles,
                                     rate = dropout_rate)
         
         # Create static cat embedding layers
@@ -936,15 +921,15 @@
             for i,(colname, values, emb) in enumerate(zip(stat_col_names, stat_col_vocab, stat_col_emb_dim)):
                 values = tf.convert_to_tensor(values, dtype=tf.string)
                 cat_indices = tf.range(len(values), dtype = tf.int64)
                 cat_init = tf.lookup.KeyValueTensorInitializer(values, cat_indices)
                 cat_lookup_table = tf.lookup.StaticVocabularyTable(cat_init, 1)
                 self.stat_lookup_tables[colname] = cat_lookup_table
                 self.stat_embed_layers[colname] = tf.keras.layers.Embedding(input_dim = len(values) + 1, 
-                                                                            output_dim = emb,
+                                                                            output_dim = d_model,
                                                                             name = "embedding_layer_{}".format(colname))
         # Create temporal known cat embedding layers
         self.temporal_known_col_details = vocab_dict.get('temporal_known_cat_indices', None)
         if self.temporal_known_col_details:
             self.temporal_known_lookup_tables = {}
             self.temporal_known_embed_layers = {}
             temporal_known_col_names = self.temporal_known_col_details[0]
@@ -953,70 +938,67 @@
             for i,(colname, values, emb) in enumerate(zip(temporal_known_col_names, temporal_known_col_vocab, temporal_known_col_emb_dim)):
                 values = tf.convert_to_tensor(values, dtype=tf.string)
                 cat_indices = tf.range(len(values), dtype = tf.int64)
                 cat_init = tf.lookup.KeyValueTensorInitializer(values, cat_indices)
                 cat_lookup_table = tf.lookup.StaticVocabularyTable(cat_init, 1)
                 self.temporal_known_lookup_tables[colname] = cat_lookup_table
                 self.temporal_known_embed_layers[colname] = tf.keras.layers.Embedding(input_dim = len(values) + 1, 
-                                                                                      output_dim = emb,
+                                                                                      output_dim = d_model,
                                                                                       name = "embedding_layer_{}".format(colname))
         
         # columns names & indices
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
         self.stat_num_col_names, self.stat_num_indices = self.col_index_dict.get('static_num_indices')
         self.stat_cat_col_names, self.stat_cat_indices = self.col_index_dict.get('static_cat_indices')
         self.known_num_col_names, self.known_num_indices = self.col_index_dict.get('temporal_known_num_indices')
         self.unknown_num_col_names, self.unknown_num_indices = self.col_index_dict.get('temporal_unknown_num_indices')
         self.known_cat_col_names, self.known_cat_indices = self.col_index_dict.get('temporal_known_cat_indices')
         self.unknown_cat_col_names, self.unknown_cat_indices = self.col_index_dict.get('temporal_unknown_cat_indices')
         
         # Create Numerical Embedding (Linear Transform) Layers
         
-        self.target_linear_transform_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=d_model, use_bias=False)) 
-        #self.scale_linear_transform_layer = tf.keras.layers.Dense(units=d_model, use_bias=False)
-        self.hist_encode_layer = CausalConvEncoder(d_model=d_model, num_layers=self.num_causal_layers)
-        #self.hist_encode_layer = CausalConvResidualLayer(d_model=d_model, seq_len=int(self.hist_len+self.f_len), dropout_rate=dropout_rate)
-
+        self.target_linear_transform_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=d_model, use_bias=False))
+        #self.hist_encode_layer = tf.keras.layers.LSTM(units=d_model, return_state=False, return_sequences=True) 
+      
         if len(self.stat_num_col_names)>0:
             self.stat_linear_transform_layers = {}
             for colname in self.stat_num_col_names:
                 self.stat_linear_transform_layers[colname] = tf.keras.layers.Dense(units=d_model, use_bias=False)
         
         if len(self.known_num_col_names)>=0:
             self.known_linear_transform_layers = {}
             for colname in self.known_num_col_names + ['rel_age']:
                 self.known_linear_transform_layers[colname] = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=d_model, use_bias=False))
                 
     def call(self, inputs, training):
-
+        
         # total_dim
-        t_dim = inputs.shape.as_list()[-1] - 3  # reduce 2 dims for mask,rel_age,scale
+        t_dim = inputs.shape.as_list()[-1] - 3 # reduce 2 dims for mask,rel_age,scale
         dim_counter = 0
         
         # target
         target = tf.strings.to_number(inputs[:,:,self.target_index:self.target_index+1], out_type=tf.dtypes.float32)
         dim_counter += 1
-
+        
         # transform to model dim
         target = self.target_linear_transform_layer(target)
         
         # ordered col names list
         stat_cols_ordered_list = []
         future_cols_ordered_list = []
         
         # stat, encoder, decoder tensor lists
         static_vars_list = []
         decoder_vars_list = [target[:,:-1,:]] # left-shifted actuals
         future_cols_ordered_list = future_cols_ordered_list + [self.target_col_name]
         
         # recurrent state encoding w/ causal conv encoder
-        recurrent_state = self.hist_encode_layer(target[:,:-1,:]) # (batch, seq_len-1, d_model)
-        decoder_vars_list.append(recurrent_state) # encoded state till current timestep
-       
-        future_cols_ordered_list = future_cols_ordered_list + ['{}_past_encoding'.format(self.target_col_name)]
+        #recurrent_state = self.hist_encode_layer(target[:,:-1,:]) # (batch, seq_len-1, d_model)
+        #decoder_vars_list.append(recurrent_state) # encoded state till current timestep
+        #future_cols_ordered_list = future_cols_ordered_list + ['{}_past_encoding'.format(self.target_col_name)]
         
         # static numeric
         if len(self.stat_num_indices)>0:
             stat_cols_ordered_list = stat_cols_ordered_list + self.stat_num_col_names
             for col, i in zip(self.stat_num_col_names, self.stat_num_indices):
                 stat_var = tf.strings.to_number(inputs[:,-1,i:i+1], out_type=tf.dtypes.float32)
                 stat_var = self.stat_linear_transform_layers[col](stat_var)
@@ -1030,15 +1012,15 @@
             for col, i in zip(self.stat_cat_col_names, self.stat_cat_indices):
                 stat_var = inputs[:,:,i]
                 stat_var_id = self.stat_lookup_tables.get(col).lookup(stat_var)
                 stat_var_embeddings = self.stat_embed_layers.get(col)(stat_var_id)
                 # append
                 static_vars_list.append(stat_var_embeddings[:,-1,:])
                 dim_counter += 1
-
+                
         # known numeric 
         if len(self.known_num_indices)>0:
             future_cols_ordered_list = future_cols_ordered_list + self.known_num_col_names
             for col, i in zip(self.known_num_col_names, self.known_num_indices):
                 num_vars = tf.strings.to_number(inputs[:,1:,i:i+1], out_type=tf.dtypes.float32)
                 num_vars = self.known_linear_transform_layers[col](num_vars)
                 # append
@@ -1051,161 +1033,225 @@
             for col, i in zip(self.known_cat_col_names, self.known_cat_indices):
                 cat_var = inputs[:,1:,i]
                 cat_var_id = self.temporal_known_lookup_tables.get(col).lookup(cat_var)
                 cat_var_embeddings = self.temporal_known_embed_layers.get(col)(cat_var_id)
                 # append
                 decoder_vars_list.append(cat_var_embeddings)
                 dim_counter += 1
-
+                
+        # unsued cols for this model
+        if len(self.unknown_num_indices)>0:
+            for col, i in zip(self.unknown_num_col_names, self.unknown_num_indices):
+                dim_counter += 1
+        
+        if len(self.unknown_cat_indices)>0:
+            for col, i in zip(self.unknown_cat_col_names, self.unknown_cat_indices):
+                dim_counter += 1
+                
         # remaining_dim
         r_dim = t_dim - dim_counter
 
         # default scale
-        scale = tf.strings.to_number(inputs[:, :-1, -2:-1], out_type=tf.dtypes.float32)
-
-        if r_dim == 2:  # standard scaling used (mean,std)
-            # print(" standard r_dim")
+        scale = tf.strings.to_number(inputs[:,:-1,-2:-1], out_type=tf.dtypes.float32)
+        
+        if r_dim == 2: # standard scaling used (mean,std)
+            #print(" standard r_dim")
             # rel_age
-            rel_age = tf.strings.to_number(inputs[:, :-1, -4:-3], out_type=tf.dtypes.float32)
+            rel_age = tf.strings.to_number(inputs[:,:-1,-4:-3], out_type=tf.dtypes.float32)
             rel_age_dec = self.known_linear_transform_layers['rel_age'](rel_age)
-
             # append
             decoder_vars_list.append(rel_age_dec)
-
             # scale
-            scale = tf.strings.to_number(inputs[:,:-1, -3:-1], out_type=tf.dtypes.float32)
-            #scale_log = scale[:,:,0:1] #tf.math.log(tf.math.sqrt(tf.abs(scale[:,:,0:1]))) # mean
+            scale = tf.strings.to_number(inputs[:,:-1,-3:-1], out_type=tf.dtypes.float32)
+            #scale_log = scale[:,:,0:1] #tf.math.log(tf.math.sqrt(scale[:,:,0:1]))
             #scale_log = self.scale_linear_transform_layer(scale_log[:,-1,:])
             # append
             #static_vars_list.append(scale_log)
-
         elif r_dim == 1:
-            # print(" mean r_dim")
-            # rel_age
-            rel_age = tf.strings.to_number(inputs[:, :-1, -3:-2], out_type=tf.dtypes.float32)
+            #print(" mean r_dim")
+             # rel_age
+            rel_age = tf.strings.to_number(inputs[:,:-1,-3:-2], out_type=tf.dtypes.float32)
             rel_age_dec = self.known_linear_transform_layers['rel_age'](rel_age)
-
             # append
             decoder_vars_list.append(rel_age_dec)
-
             # scale
-            scale = tf.strings.to_number(inputs[:, :-1, -2:-1], out_type=tf.dtypes.float32)
-            #scale_log = scale #tf.math.log(tf.math.sqrt(scale))
+            scale = tf.strings.to_number(inputs[:,:-1,-2:-1], out_type=tf.dtypes.float32)
+            #scale_log = tf.math.log(tf.math.sqrt(scale))
             #scale_log = self.scale_linear_transform_layer(scale_log[:,-1,:])
             # append
             #static_vars_list.append(scale_log)
-        
+            
         # Append additional columns
         #stat_cols_ordered_list = stat_cols_ordered_list + ['scale']
         future_cols_ordered_list = future_cols_ordered_list + ['rel_age']
         
         # mask
         mask = tf.strings.to_number(inputs[:,:-1,-1:], out_type=tf.dtypes.float32)
         
+        
         # model process
         if self.static_variables:
             o, s, s_wts, f_wts = self.model([static_vars_list, decoder_vars_list, mask, scale], training=training)
         else:
             o, s, s_wts, f_wts = self.model([decoder_vars_list, mask, scale], training=training)
 
         # Retain period-wise importance
         bs = tf.shape(f_wts)[0]
         f_wts = tf.reshape(f_wts, [bs*(self.f_len), -1])
               
         return o, s, ([stat_cols_ordered_list,future_cols_ordered_list], [s_wts, f_wts])
     
     
 def SageTransformer_Train(model,
+                      target_index,
                       train_dataset, 
                       test_dataset, 
                       loss_type,
                       loss_function, 
                       metric, 
                       learning_rate,
                       max_epochs, 
                       min_epochs,
                       prefill_buffers,
                       num_train_samples,
                       num_test_samples,
-                      train_batch_size,       
+                      train_batch_size,
+                      test_batch_size,
                       train_steps_per_epoch,
                       test_steps_per_epoch,
                       patience,
                       weighted_training,
                       model_prefix,
                       logdir,
                       opt=None,
-                      clipnorm=None):
+                      clipnorm=None,
+                      min_delta=0.0001,
+                      shuffle=True):
     """
      train_dataset, test_dataset: tf.data.Dataset iterator for train & test datasets 
      loss_type: One of ['Point','Quantile','Normal','Poisson','Negbin']
      loss_function: One of the supported loss functions in loss library
      metric: 'MAE' or 'MSE' 
      max_epochs: Max. training epochs
      min_epochs: Min. Training epochs
      *_steps_per_epoch: batches per epoch 
      weighted_training: True/False
      model_prefix: relative or absolute model path with a prefix for a model name
      logdir: tensorflow training logs for tensorboard
         
     """
+   
     @tf.function
     def trainstep(model, optimizer, x_train, y_train, scale, wts, training):
         with tf.GradientTape() as tape:
             o, s, f = model(x_train, training=training)
-            out_len = s.shape.as_list()[1] #tf.shape(s)[1]
-            s_dim = scale.shape.as_list()[-1] #tf.shape(scale)[-1]
-            if loss_type in ['Normal','Poisson','Negbin']:
+            out_len = tf.shape(s)[1]
+            s_dim = tf.shape(scale)[-1]
+            if loss_type in ['Normal','Negbin']:
                 if s_dim == 1:
                     if weighted_training:
-                        loss = loss_function(y_train * scale[:, -out_len:, :], [s, wts])
+                        loss = loss_function(y_train*scale[:,-out_len:,:], [s, wts])
                     else:
-                        loss = loss_function(y_train * scale[:, -out_len:, :], s)
+                        loss = loss_function(y_train*scale[:,-out_len:,:], s)
                 else:
-                    s_mean = scale[:, -out_len:, 0:1]
-                    s_std = scale[:, -out_len:, 1:2]
+                    s_mean = scale[:,-out_len:,0:1]
+                    s_std = scale[:,-out_len:,1:2]
                     if weighted_training:
-                        loss = loss_function(y_train * s_std + s_mean, [s, wts])
+                        loss = loss_function(y_train*s_std + s_mean, [s, wts])
                     else:
-                        loss = loss_function(y_train * s_std + s_mean, s)
-            elif loss_type in ['Point','Binary']:
-                if weighted_training:                               
-                    loss = loss_function(y_train, [o, wts])
+                        loss = loss_function(y_train*s_std + s_mean, s)
+            elif loss_type in ['Tweedie','Poisson']:
+                if s_dim == 1:
+                    if weighted_training:                               
+                        loss = loss_function(y_train*scale[:,-out_len:,:], [o*scale[:,-out_len:,:], wts])
+                    else:
+                        loss = loss_function(y_train*scale[:,-out_len:,:], o*scale[:,-out_len:,:])
                 else:
-                    loss = loss_function(y_train, o)
+                    s_mean = scale[:,-out_len:,0:1]
+                    s_std = scale[:,-out_len:,1:2]
+                    if weighted_training:
+                        loss = loss_function(y_train*s_std + s_mean, [o*s_std + s_mean, wts])
+                    else:
+                        loss = loss_function(y_train*s_std + s_mean, o*s_std + s_mean)
+            elif loss_type in ['Point']:
+                    if weighted_training:                               
+                        loss = loss_function(y_train, [o, wts])
+                    else:
+                        loss = loss_function(y_train, o)
             elif loss_type in ['Quantile']:
                 if weighted_training:                               
                     loss = loss_function(y_train, [o, wts])
                 else:
                     loss = loss_function(y_train, o)                                   
             else:
                 raise ValueError("Invalid loss_type specified!")
         grads = tape.gradient(loss, model.trainable_variables)
         optimizer.apply_gradients((grad, var) for (grad, var) in zip(grads, model.trainable_variables) if grad is not None)
         return loss, o
-    
-    @tf.function
+
     def teststep(model, x_test, y_test, scale, wts, training):
-        o, s, f = model(x_test, training=training)
-        out_len = s.shape.as_list()[1]  # tf.shape(s)[1]
-        s_dim = scale.shape.as_list()[-1]  # tf.shape(scale)[-1]
-        if loss_type in ['Normal','Poisson','Negbin']:
+        out_len = y_test.shape.as_list()[1]
+        s_dim = scale.shape.as_list()[-1]
+        hist_len = x_test.shape.as_list()[1] - out_len
+        
+        if s_dim == 1:
+            scale_mean = scale[:,-1:,-1]
+        else:
+            scale_mean = scale[:,-1:,0]
+            scale_std = scale[:,-1:,1]
+            
+        # recursive predict
+        output = []
+        
+        for i in range(out_len):
+            o, s, f = model(x_test, training=training)
+            infer_arr = x_test.numpy()
+            # update target
+            if loss_type in ['Normal','Negbin']:
+                output.append(s[:,i:i+1,:])
+                if s_dim == 1:
+                    infer_arr[:,hist_len+i:hist_len+i+1,target_index] = o[:,i:i+1,0]/scale_mean
+                else:
+                    infer_arr[:,hist_len+i:hist_len+i+1,target_index] = np.nan_to_num((o[:,i:i+1,0] - scale_mean)/scale_std)
+
+            elif loss_type in ['Point','Quantile','Tweedie','Poisson']:
+                output.append(o[:,i:i+1,:])
+                infer_arr[:,hist_len+i:hist_len+i+1,target_index] = o[:,i:i+1,0] # append q=0.5 value assuming it's the first in sequence
+
+            # feedback updated hist + fh tensor
+            x_test = tf.convert_to_tensor(np.char.decode(infer_arr.astype(np.bytes_), 'UTF-8'), dtype=tf.string) 
+        
+        o = tf.concat(output, axis=1)
+        if loss_type in ['Normal','Negbin']:
             if s_dim == 1:
                 if weighted_training:
-                    loss = loss_function(y_test * scale[:, -out_len:, :], [s, wts])
+                    loss = loss_function(y_test*scale[:,-out_len:,:], [s, wts])
+                else:
+                    loss = loss_function(y_test*scale[:,-out_len:,:], s)
+            else:
+                s_mean = scale[:,-out_len:,0:1]
+                s_std = scale[:,-out_len:,1:2]
+                if weighted_training:
+                    loss = loss_function(y_test*s_std + s_mean, [s, wts])
                 else:
-                    loss = loss_function(y_test * scale[:, -out_len:, :], s)
+                    loss = loss_function(y_test*s_std + s_mean, s)
+        elif loss_type in ['Tweedie','Poisson']:
+            if s_dim == 1:
+                if weighted_training:                               
+                    loss = loss_function(y_test*scale[:,-out_len:,:], [o*scale[:,-out_len:,:], wts])
+                else:
+                    loss = loss_function(y_test*scale[:,-out_len:,:], o*scale[:,-out_len:,:])
             else:
-                s_mean = scale[:, -out_len:, 0:1]
-                s_std = scale[:, -out_len:, 1:2]
+                s_mean = scale[:,-out_len:,0:1]
+                s_std = scale[:,-out_len:,1:2]
                 if weighted_training:
-                    loss = loss_function(y_test * s_std + s_mean, [s, wts])
+                    loss = loss_function(y_test*s_std + s_mean, [o*s_std + s_mean, wts])
                 else:
-                    loss = loss_function(y_test * s_std + s_mean, s)
-        elif loss_type in ['Point','Binary']:
+                    loss = loss_function(y_test*s_std + s_mean, o*s_std + s_mean)
+        elif loss_type in ['Point']:
             if weighted_training:                               
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)
         elif loss_type in ['Quantile']:
             if weighted_training:                               
                 loss = loss_function(y_test, [o, wts])
@@ -1262,15 +1308,15 @@
 
     vocab_dict_file = model_prefix + '_vocab_dict.pkl'
     with open(vocab_dict_file, 'wb') as f:
         pickle.dump(model.vocab_dict, f)
     
     model_tracker_file = open(model_prefix + '_tracker.txt', mode='w', encoding='utf-8')
 
-    model_tracker_file.write('SageTransformer Training started with following Model Parameters ... \n')
+    model_tracker_file.write('Feature Weighted ConvTransformer Training started with following Model Parameters ... \n')
     model_tracker_file.write('----------------------------------------\n')
     model_tracker_file.write('num_layers ' + str(model.num_layers) + '\n')
     model_tracker_file.write('num_heads ' + str(model.num_heads) + '\n')
     model_tracker_file.write('d_model ' + str(model.d_model) + '\n')
     model_tracker_file.write('forecast_horizon ' + str(model.forecast_horizon) + '\n')
     model_tracker_file.write('max_inp_len ' + str(model.max_inp_len) + '\n')
     model_tracker_file.write('dropout_rate ' + str(model.dropout_rate) + '\n')
@@ -1282,30 +1328,43 @@
     
     model_list = []
     best_model = None
     time_since_improvement = 0
     
     ######################################################### train loop -- pre-filled tensor buffers
     
+    def shuffle_arrays(arrays, set_seed=-1):
+      """Shuffles arrays in-place, in the same order, along axis=0
+      arrays : List of NumPy arrays.
+      set_seed : Seed value if int >= 0, else seed is random.
+      """
+      assert all(len(arr) == len(arrays[0]) for arr in arrays)
+      seed = np.random.randint(0, 2**(32 - 1) - 1) if set_seed < 0 else set_seed
+      for arr in arrays:
+        rstate = np.random.RandomState(seed)
+        rstate.shuffle(arr)
+    
     if prefill_buffers:
       print("prefetching training samples ... ")
       # get batch size
       batch_size = 0
       for x,y,s,w in train_dataset.take(1):
         batch_size = int(x.shape[0])
 
       x_train = []
       y_train = []
       train_scale = []
       train_wts = []
+      #num_train_batches = 0
       for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
         x_train.append(x_batch)
         y_train.append(y_batch)
         train_scale.append(scale)
         train_wts.append(wts)
+        #num_train_batches = num_train_batches + m.floor(batch_size/train_batch_size)
         if (step+1)*batch_size >= num_train_samples:
           break
        
       # concat
       x_train = tf.concat(x_train, axis=0)
       y_train = tf.concat(y_train, axis=0)
       train_scale = tf.concat(train_scale, axis=0)
@@ -1313,65 +1372,81 @@
       print("Training Samples Gathered: ", x_train.shape[0])
       
       print("prefetching test samples ... ")
       x_test = []
       y_test = []
       test_scale = []
       test_wts = []
+      #num_test_batches = 0
       for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
         x_test.append(x_batch)
         y_test.append(y_batch)
         test_scale.append(scale)
         test_wts.append(wts)
+        #num_test_batches = num_test_batches + m.floor(batch_size/train_batch_size)
         if (step+1)*batch_size >= num_test_samples:
           break
 
       # concat
       x_test = tf.concat(x_test, axis=0)
       y_test = tf.concat(y_test, axis=0)
       test_scale = tf.concat(test_scale, axis=0)
       test_wts = tf.concat(test_wts, axis=0)
       print("Test Samples Gathered: ", x_test.shape[0])
-      
+        
       num_train_batches = int(x_train.shape[0]//train_batch_size)
-      num_test_batches = int(x_test.shape[0]//train_batch_size)
+      num_test_batches = int(x_test.shape[0]//test_batch_size)
 
       for epoch in range(max_epochs):
           print("Epoch {}/{}". format(epoch, max_epochs))
+          # shuffle Training data only,if shuffle=True
+          if shuffle:
+            #shuffle_arrays([x_train, y_train, train_scale, train_wts])
+            indices = tf.range(start=0, limit=tf.shape(x_train)[0], dtype=tf.int32)
+            shuffled_indices = tf.random.shuffle(indices)
+            x_train = tf.gather(x_train, shuffled_indices)
+            y_train = tf.gather(y_train, shuffled_indices)
+            train_scale = tf.gather(train_scale, shuffled_indices)
+            train_wts = tf.gather(train_wts, shuffled_indices)
+
           for i in range(num_train_batches):
             x_batch = x_train[i*train_batch_size:(i+1)*train_batch_size]
             y_batch = y_train[i*train_batch_size:(i+1)*train_batch_size]
             scale = train_scale[i*train_batch_size:(i+1)*train_batch_size]
             wts = train_wts[i*train_batch_size:(i+1)*train_batch_size]
             train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
             out_len = tf.shape(train_out)[1]
             train_loss_avg.update_state(train_loss)
-            if loss_type in ['Normal','Poisson','Negbin']:
+            if loss_type in ['Normal','Negbin']:
               train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-            elif loss_type in ['Point','Quantile']:
+            elif loss_type in ['Point','Tweedie','Poisson']:
               train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
+            elif loss_type in ['Quantile']:
+              train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
             with train_summary_writer.as_default():
-              tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
-              tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
+              tf.summary.scalar('loss', train_loss_avg.result(), step=(i+1)*(epoch+1))
+              tf.summary.scalar('accuracy', train_metric.result(), step=(i+1)*(epoch+1))
 
           for i in range(num_test_batches):
             x_batch = x_test[i*train_batch_size:(i+1)*train_batch_size]
             y_batch = y_test[i*train_batch_size:(i+1)*train_batch_size]
             scale = test_scale[i*train_batch_size:(i+1)*train_batch_size]
             wts = test_wts[i*train_batch_size:(i+1)*train_batch_size]
             test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
             out_len = tf.shape(test_out)[1]
             test_loss_avg.update_state(test_loss)
-            if loss_type in ['Normal','Poisson','Negbin']:
+            if loss_type in ['Normal','Negbin']:
               test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-            elif loss_type in ['Point','Quantile']:
+            elif loss_type in ['Point','Tweedie','Poisson']:
               test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
+            elif loss_type in ['Quantile']:
+              test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
             with test_summary_writer.as_default():
-              tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
-              tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
+              tf.summary.scalar('loss', test_loss_avg.result(), step=(i+1)*(epoch+1))
+              tf.summary.scalar('accuracy', test_metric.result(), step=(i+1)*(epoch+1))
 
           print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch, 
                                                                                                       train_loss_avg.result().numpy(),
                                                                                                       test_loss_avg.result().numpy(),
                                                                                                       train_metric.result().numpy(),
                                                                                                       test_metric.result().numpy()))
 
@@ -1386,17 +1461,25 @@
           train_metric.reset_states()
           test_loss_avg.reset_states()
           test_metric.reset_states()
 
           # Save Model
           model_path = model_prefix + '_' + str(epoch) 
           model_list.append(model_path)
+          
+          if epoch == 0:
+            prev_min_loss = np.min(test_loss_results)
+          else:
+            prev_min_loss = np.min(test_loss_results[:-1])
+          current_min_loss = np.min(test_loss_results)
+          delta = current_min_loss - prev_min_loss
 
+          print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
           # track & save best model
-          if test_loss_results[epoch]==np.min(test_loss_results):
+          if ((test_loss_results[epoch]==np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
               best_model = model_path
               tf.keras.models.save_model(model, model_path)
               # reset time_since_improvement
               time_since_improvement = 0
           else:
               time_since_improvement += 1
 
@@ -1427,36 +1510,40 @@
           for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
               if step > train_steps_per_epoch:
                   break
               else:
                   train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
                   out_len = tf.shape(train_out)[1]
                   train_loss_avg.update_state(train_loss)
-                  if loss_type in ['Normal','Poisson','Negbin']:
+                  if loss_type in ['Normal','Negbin']:
                       train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-                  elif loss_type in ['Point','Quantile']:
+                  elif loss_type in ['Point','Tweedie','Poisson']:
                       train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
+                  elif loss_type in ['Quantile']:
+                      train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
                   with train_summary_writer.as_default():
-                      tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
-                      tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
+                      tf.summary.scalar('loss', train_loss_avg.result(), step=(step+1)*(epoch+1))
+                      tf.summary.scalar('accuracy', train_metric.result(), step=(step+1)*(epoch+1))
 
           for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
               if step > test_steps_per_epoch:
                   break
               else:
                   test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
                   out_len = tf.shape(test_out)[1]
                   test_loss_avg.update_state(test_loss)
-                  if loss_type in ['Normal','Poisson','Negbin']:
+                  if loss_type in ['Normal','Negbin']:
                       test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-                  elif loss_type in ['Point','Quantile']:
+                  elif loss_type in ['Point','Tweedie','Poisson']:
                       test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
+                  elif loss_type in ['Quantile']:
+                      test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out[:,-out_len:,0:1]*scale[:,-out_len:,:])
                   with test_summary_writer.as_default():
-                      tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
-                      tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
+                      tf.summary.scalar('loss', test_loss_avg.result(), step=(step+1)*(epoch+1))
+                      tf.summary.scalar('accuracy', test_metric.result(), step=(step+1)*(epoch+1))
 
           print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch, 
                                                                                                       train_loss_avg.result().numpy(),
                                                                                                       test_loss_avg.result().numpy(),
                                                                                                       train_metric.result().numpy(),
                                                                                                       test_metric.result().numpy()))
 
@@ -1471,17 +1558,25 @@
           train_metric.reset_states()
           test_loss_avg.reset_states()
           test_metric.reset_states()
 
           # Save Model
           model_path = model_prefix + '_' + str(epoch) 
           model_list.append(model_path)
-
+          
+          if epoch == 0:
+            prev_min_loss = np.min(test_loss_results)
+          else:
+            prev_min_loss = np.min(test_loss_results[:-1])
+          current_min_loss = np.min(test_loss_results)
+          delta = current_min_loss - prev_min_loss
+         
+          print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
           # track & save best model
-          if test_loss_results[epoch]==np.min(test_loss_results):
+          if ((test_loss_results[epoch]==np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
               best_model = model_path
               tf.keras.models.save_model(model, model_path)
               # reset time_since_improvement
               time_since_improvement = 0
           else:
               time_since_improvement += 1
 
@@ -1503,137 +1598,174 @@
               break
 
           # write after each epoch
           model_tracker_file.flush()
         
     return best_model
         
-
+ 
         
 def SageTransformer_InferRecursive(model, inputs, loss_type, hist_len, f_len, target_index, num_quantiles):
     infer_tensor, scale, id_arr, date_arr = inputs
-
     s_dim = scale.shape[-1]
-
+    
     if s_dim == 1:
-        scale = scale[:, -1:, -1]
+        scale = scale[:,-1:,-1]
     else:
-        scale_mean = scale[:, -1:, 0]
-        scale_std = scale[:, -1:, 1]
-
-    #scale = scale[:,-1:,-1]  # old
+        scale_mean = scale[:,-1:,0]
+        scale_std = scale[:,-1:,1]
+        
     window_len = hist_len + f_len
     output = []
     stat_wts_df = None 
     decoder_wts_df = None
         
     for i in range(f_len):
         out, dist, feature_wts = model(infer_tensor, training=False)
             
         # update target
-        if loss_type in ['Normal','Poisson','Negbin']:
+        if loss_type in ['Normal','Negbin']:
             dist = dist.numpy()
-            output.append(dist[:,i:i+1,0])
+            output.append(out[:,i:i+1,0])
             infer_arr = infer_tensor.numpy()
-            #infer_arr[:,hist_len:hist_len+i+1,target_index] = out[:,0:i+1,0]/scale
             if s_dim == 1:
-                infer_arr[:, hist_len:hist_len + i + 1, target_index] = out[:, 0:i + 1, 0] / scale
+                infer_arr[:,hist_len+i:hist_len+i+1,target_index] = out[:,i:i+1,0]/scale
             else:
-                infer_arr[:, hist_len:hist_len + i + 1, target_index] = np.nan_to_num((out[:, 0:i + 1, 0] - scale_mean) / scale_std)
-        elif loss_type in ['Point','Quantile','Binary']:
+                infer_arr[:,hist_len+i:hist_len+i+1,target_index] = np.nan_to_num((out[:,i:i+1,0] - scale_mean)/scale_std)
+        elif loss_type in ['Point','Quantile','Tweedie','Poisson']:
             out = out.numpy()
-            output.append(out[:,i:i+1,0])
+            output.append(out[:,i:i+1,:])
             infer_arr = infer_tensor.numpy()
-            infer_arr[:,hist_len:hist_len+i+1,target_index] = out[:,0:i+1,0]
+            infer_arr[:,hist_len+i:hist_len+i+1,target_index] = out[:,i:i+1,0] # feedback q=0.5 percentile
             
         # feedback updated hist + fh tensor
         infer_tensor = tf.convert_to_tensor(np.char.decode(infer_arr.astype(np.bytes_), 'UTF-8'), dtype=tf.string)
             
         if i == (f_len - 1):
             column_names_list, wts_list = feature_wts
             stat_columns, decoder_columns = column_names_list
             stat_columns_string = []
             decoder_columns_string = []
             for col in stat_columns:
                 stat_columns_string.append(col.numpy().decode("utf-8")) 
             for col in decoder_columns:
                 decoder_columns_string.append(col.numpy().decode("utf-8"))
-
+                
+            #print(" decoder_columns_string: ",  decoder_columns_string)
             stat_wts, decoder_wts = wts_list
             # Average feature weights across time dim
             decoder_wts = decoder_wts.numpy()
             # convert wts to df    
             decoder_wts_df = pd.DataFrame(decoder_wts, columns=decoder_columns_string)    
             if stat_wts is not None:
                 stat_wts = stat_wts.numpy()
                 stat_wts_df = pd.DataFrame(stat_wts, columns=stat_columns_string)   
             
     output_arr = np.concatenate(output, axis=1) 
         
     # rescale if necessary
-    if loss_type in ['Normal','Poisson','Negbin']:
+    if loss_type in ['Normal','Negbin']:
         output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr), axis=1))
-    elif loss_type in ['Point','Quantile','Binary']:
-        #output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr*scale.reshape(-1,1)), axis=1))
-        # new
+        output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
+        output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
+    elif loss_type in ['Point','Tweedie','Poisson']:
         if s_dim == 1:
-            output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output_arr * scale.reshape(-1, 1)), axis=1))
+            output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr[:,:,0]*scale.reshape(-1,1)), axis=1))
         else:
-            output_arr = output_arr * scale_std.reshape(-1, 1) + scale_mean.reshape(-1, 1)
-            output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output_arr), axis=1))
-    output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
-    output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
-        
+            output_arr = output_arr[:,:,0]*scale_std.reshape(-1,1) + scale_mean.reshape(-1,1)
+            output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1), output_arr), axis=1))
+        output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
+        output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
+    elif loss_type in ['Quantile']:
+        df_list = []
+        for i in range(num_quantiles):
+            if s_dim == 1:
+                output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr[:,:,i]*scale.reshape(-1,1)), axis=1))
+                output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value': f"forecast_{i}"})
+                output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
+                df_list.append(output_df)
+            else:
+                output = output_arr[:,:,i]* scale_std.reshape(-1, 1) + scale_mean.reshape(-1, 1)
+                output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output), axis=1))
+                output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0: 'id', 'value': f"forecast_{i}"})
+                output_df = output_df.rename_axis('index').sort_values(by=['id', 'index']).reset_index(drop=True)
+                df_list.append(output_df)
+        output_df = pd.concat(df_list, axis=1)
+        output_df = output_df.loc[:,~output_df.columns.duplicated()]
+            
     # merge date_columns
     date_df = pd.DataFrame(date_arr.reshape(-1,)).rename(columns={0:'period'})
     forecast_df = pd.concat([date_df, output_df], axis=1)
-    forecast_df['forecast'] = forecast_df['forecast'].astype(np.float32)
+    if loss_type in ['Quantile']:
+        for i in range(num_quantiles):
+            forecast_df[f"forecast_{i}"] = forecast_df[f"forecast_{i}"].astype(np.float32)
+    else:
+        forecast_df['forecast'] = forecast_df['forecast'].astype(np.float32)
         
     # weights df merge with id
     stat_wts_df = pd.concat([pd.DataFrame(id_arr.reshape(-1,1)), stat_wts_df], axis=1)
     
     decoder_wts_df = pd.concat([date_df, decoder_wts_df], axis=1)
     fid_df = pd.DataFrame(np.repeat(id_arr.reshape(-1,1), f_len, axis=0))
     fid_df.columns = ['id']
     decoder_wts_df = pd.concat([fid_df, decoder_wts_df], axis=1) 
     
     print(stat_wts_df.shape, decoder_wts_df.shape)
         
     return forecast_df, stat_wts_df, decoder_wts_df
 
 
+
+
 class SageModel:
     def __init__(self, 
                  col_index_dict,
                  vocab_dict,
                  num_layers,
                  num_heads,
                  kernel_sizes,
                  d_model,
                  forecast_horizon,
                  max_inp_len,
                  loss_type,
                  num_quantiles,
-                 dropout_rate=0.1):
+                 dropout_rate=0.1,
+                 seed=None,
+                 deterministic_ops=False):
         
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.kernel_sizes = kernel_sizes
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.dropout_rate = dropout_rate
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
+        self.seed = seed
+        self.allow_deterministic_ops = deterministic_ops
     
+    def set_seed(self):
+        tf.keras.utils.set_random_seed(self.seed)
+        if self.allow_deterministic_ops:
+            print("Deterministic Ops enabled.")
+            os.environ["TF_DETERMINISTIC_OPS"] = "True"
+            os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+        
     def build(self):
         tf.keras.backend.clear_session()
+        if self.seed is None:
+            print("No seed set for deterministic weights initialization")
+        else:
+            print("Using seed {} for weights initialization".format(self.seed))
+            self.set_seed()
+            
         self.model = SageTransformer_Model(self.col_index_dict,
                                   self.vocab_dict,
                                   self.num_layers,
                                   self.num_heads,
                                   self.kernel_sizes,
                                   self.d_model,
                                   self.forecast_horizon,
@@ -1642,72 +1774,80 @@
                                   self.num_quantiles,
                                   self.dropout_rate)
         
     def train(self, 
               train_dataset, 
               test_dataset,
               loss_function, 
-              metric='MSE',
-              learning_rate=0.0001,
-              max_epochs=100,
-              min_epochs=10,
-              prefill_buffers=False,
-              num_train_samples=200000,
-              num_test_samples=50000,
-              train_batch_size=64,
-              train_steps_per_epoch=200,
-              test_steps_per_epoch=100,
-              patience=10,
-              weighted_training=False,
-              model_prefix='./sage_model',
-              logdir='/tmp/sage_logs',
+              metric, 
+              learning_rate,
+              max_epochs, 
+              min_epochs,
+              prefill_buffers,
+              num_train_samples,
+              num_test_samples,
+              train_batch_size,
+              test_batch_size,
+              train_steps_per_epoch,
+              test_steps_per_epoch,
+              patience,
+              weighted_training,
+              model_prefix,
+              logdir,
               load_model=None,
               opt=None,
-              clipnorm=None):
-
+              clipnorm=None,
+              min_delta=0.0001,
+              shuffle=True):
+        
         if load_model is None:
             # Initialize Weights
-            for x, y, s, w in train_dataset.take(1):
+            for x,y,s,w in train_dataset.take(1):
                 self.model(x, training=False)
         else:
             # Initialize Weights
-            for x, y, s, w in train_dataset.take(1):
+            for x,y,s,w in train_dataset.take(1):
                 self.model(x, training=False)
             saved_model = tf.keras.models.load_model(load_model)
             self.model.set_weights(saved_model.get_weights())
             del saved_model
             gc.collect()
             print("Saved model: {} loaded. Continuing training ...".format(load_model))
         
         best_model = SageTransformer_Train(self.model,
+                                          self.target_index,    
                                           train_dataset, 
                                           test_dataset, 
                                           self.loss_type,
                                           loss_function, 
                                           metric, 
                                           learning_rate,
                                           max_epochs, 
                                           min_epochs,
                                           prefill_buffers,
                                           num_train_samples,
                                           num_test_samples,
                                           train_batch_size,
+                                          test_batch_size,
                                           train_steps_per_epoch,
                                           test_steps_per_epoch,
                                           patience,
                                           weighted_training,
                                           model_prefix,
                                           logdir,
                                           opt,
-                                          clipnorm)
+                                          clipnorm,
+                                          min_delta,
+                                          shuffle)
         return best_model
     
     def load(self, model_path):
         tf.keras.backend.clear_session()
         self.model = tf.keras.models.load_model(model_path)
         
     def infer(self, inputs):
         forecast, stat_wts_df, decoder_wts_df = SageTransformer_InferRecursive(self.model, inputs, self.loss_type, self.max_inp_len, self.forecast_horizon, self.target_index, self.num_quantiles)
         
         return forecast, [stat_wts_df, decoder_wts_df]
     
     
+
```

### Comparing `fmldk-1.1.8/setup.py` & `fmldk-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The directory containing this file
 this_directory = Path(__file__).parent
 long_description  = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="fmldk",
-    version="1.1.8",
+    version="1.1.9",
     description="Forecast ML library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rahul Sinha",
     author_email="rahul.sinha@unilever.com",
     packages=["sage","tfr","tft","stctn","ctfr","ctfrv2","eda"],
     include_package_data=True,
```

### Comparing `fmldk-1.1.8/stctn/stctn_data.py` & `fmldk-1.1.9/stctn/stctn_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/stctn/stctn_losses.py` & `fmldk-1.1.9/stctn/stctn_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/stctn/stctn_losses_bkp.py` & `fmldk-1.1.9/stctn/stctn_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/stctn/stctn_models.py` & `fmldk-1.1.9/stctn/stctn_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data.py` & `fmldk-1.1.9/tfr/tfr_data.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.11.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.12.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.14.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.14.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.15.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.15.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.16.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.16.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.18.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.18.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_data_v0.1.21.py` & `fmldk-1.1.9/tfr/tfr_data_v0.1.21.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_local_block_sparse_attention.py` & `fmldk-1.1.9/tfr/tfr_local_block_sparse_attention.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_local_block_sparse_attention_v0.1.10.py` & `fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_local_block_sparse_attention_v0.1.12.py` & `fmldk-1.1.9/tfr/tfr_local_block_sparse_attention_v0.1.12.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_losses.py` & `fmldk-1.1.9/tfr/tfr_losses.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_losses_bkp.py` & `fmldk-1.1.9/tfr/tfr_losses_bkp.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_models.py` & `fmldk-1.1.9/tfr/tfr_models.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_models_v0.1.10.py` & `fmldk-1.1.9/tfr/tfr_models_v0.1.10.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_models_v0.1.11.py` & `fmldk-1.1.9/tfr/tfr_models_v0.1.11.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_models_v0.1.23.py` & `fmldk-1.1.9/tfr/tfr_models_v0.1.23.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tfr/tfr_models_v0.1.31.py` & `fmldk-1.1.9/tfr/tfr_models_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tft/tft_data.py` & `fmldk-1.1.9/tft/tft_data_old.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tft/tft_data_v1.1.3.py` & `fmldk-1.1.9/tft/tft_data_v1.1.3.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tft/tft_data_v1.1.7.py` & `fmldk-1.1.9/tft/tft_global_scaled_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# Databricks notebook source
+#!/usr/bin/env python
+# coding: utf-8
+
+# In[ ]:
+
+
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import pandas as pd
 import numpy as np
 from joblib import Parallel, delayed
 import itertools
@@ -19,28 +24,29 @@
 from bokeh.plotting import figure, output_file, show, output_notebook, save
 from bokeh.models import ColumnDataSource, HoverTool, Div, FactorRange
 from bokeh.layouts import gridplot, column, row
 from bokeh.palettes import Category10, Category20, Colorblind
 from bokeh.io import reset_output
 from bokeh.models.ranges import DataRange1d
 
-# COMMAND ----------
 
+# In[ ]:
 
-class tft_dataset:
+
+class tft_gs_dataset:
     def __init__(self, 
                  col_dict, 
                  window_len, 
                  fh, 
                  batch, 
                  min_nz,
-                 scaling_method='mean_scaling',
+                 scaling_method = 'mean_scaling',
                  interleave=1, 
-                 PARALLEL_DATA_JOBS=4,
-                 PARALLEL_DATA_JOBS_BATCHSIZE=128,
+                 PARALLEL_DATA_JOBS=1, 
+                 PARALLEL_DATA_JOBS_BATCHSIZE=64, 
                  WORKDIR='/tmp/'):
         """
         col_dict: dictionary of various column groups {id_col:'',
                                                        target_col:'',
                                                        time_index_col:'',
                                                        datetime_format:'',
                                                        static_num_col_list:[],
@@ -52,23 +58,23 @@
                                                        strata_col_list:[],
                                                        sort_col_list:[],
                                                        wt_col:''}
         window_len: history_len + forecast_horizon
         fh: forecast_horizon
         batch: batch_size (per strata)
         min_nz: min. no. of non-zeros in the target input series to be eligible for train/test batch
-        
+        scaling_method = 'mean_scaling','standard_scaling','no_scaling'
         """
         self.col_dict = col_dict
         self.window_len = window_len
         self.fh = fh
         self.batch = batch
         self.min_nz = min_nz
-        self.scaling_method = scaling_method
         self.interleave = interleave
+        self.scaling_method = scaling_method
         self.PARALLEL_DATA_JOBS = PARALLEL_DATA_JOBS
         self.PARALLEL_DATA_JOBS_BATCHSIZE = PARALLEL_DATA_JOBS_BATCHSIZE
         self.workdir = str(WORKDIR).rstrip('/\\').strip()
        
         # extract columnsets from col_dict
         self.id_col = self.col_dict.get('id_col', None)
         self.target_col = self.col_dict.get('target_col', None)
@@ -160,170 +166,91 @@
         """
         n_jobs = min(len(keys_dict),4)
         sample_id = Parallel(n_jobs=n_jobs, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.dict_sampler)(v1,v2) for (k1,v1),(k2,v2) in zip(keys_dict.items(), wts_dict.items()) )
         sample_id = list(itertools.chain.from_iterable(sample_id))
         random.shuffle(sample_id)
         return sample_id
 
-    def select_arrs(self, df):
+    def select_arrs(self, df, mode):
         """
         Extract train/test samples from each sampled Id as 2-D arrays [window_len, num_columns]
         """
         groups = df.groupby([self.id_col])
-        sampled_arr = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.df_sampler)(gdf) for _,gdf in groups)
+        sampled_arr = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.df_sampler)(gdf, mode) for _,gdf in groups)
         arr_list = [tup[0] for tup in sampled_arr]
         pad_list = [tup[1] for tup in sampled_arr]
+        scale_list = [tup[2] for tup in sampled_arr]
         arr = np.stack(arr_list, axis=0)
         pad_arr = np.stack(pad_list, axis=0)
-        return arr, pad_arr
-    
-    def static_arrs(self, df, use_memmap, prefix):
-        """
-        Use for creating static train/test datasets i.e. non-generator based training
-        """
-        groups = df.groupby([self.id_col])
-        sliding_arrs = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.extract_windows)(gdf.values, use_memmap) for _, gdf in groups)
-        
-        if use_memmap:
-            print("Id specific memmap files creation completed. Beginning merge ...")
-            sample_arr = np.memmap(sliding_arrs[0][0], dtype='<U32', mode='r', shape=sliding_arrs[0][1])
-            x_size = sum([tup[1][0] for tup in sliding_arrs])
-            y_size = self.window_len
-            z_size = sliding_arrs[0][1][2]
-            f_name = self.workdir + '/' + str(prefix) + str(sample_arr[0,0,0]) +'_full.dat'
-    
-            arr = np.memmap(f_name, dtype='<U32', mode='w+', shape=(x_size, y_size, z_size))
-        
-            init_size = 0
-            for mem_arr in [(np.memmap(tup[0], dtype='<U32', mode='r', shape=tup[1]), tup[1]) for tup in sliding_arrs]:
-                shape = mem_arr[1][0]
-                arr[init_size:init_size + shape,:,:] = mem_arr[0]
-                init_size += shape
-            arr.flush()
-            f_shape = arr.shape
-            pad_arr = np.vstack([tup[2] for tup in sliding_arrs]).reshape(-1,)
-            print("Memmap merge completed.")
-        
-            # cleanup individual memfiles
-            try:
-                [os.remove(tup[0]) for tup in sliding_arrs]
-            except:
-                pass
-            del arr
-            gc.collect()
-            return f_name, f_shape, pad_arr
-        else:
-            arr = np.vstack([tup[0] for tup in sliding_arrs])
-            pad_arr = np.vstack([tup[1] for tup in sliding_arrs]).reshape(-1,)
-            return arr, pad_arr
+        scale_arr = np.stack(scale_list, axis=0)
+        return arr, pad_arr, scale_arr
 
-        
-    def static_infer_arrs(self, df):
-        """
-        Use for creating static train/test datasets i.e. non-generator based training
-        """
-        groups = df.groupby([self.id_col])
-        sliding_arrs = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.extract_infer_windows)(gdf[self.col_list].values, gdf[self.time_index_col].values) for _, gdf in groups)
-        
-        arr_list = [tup[0] for tup in sliding_arrs]
-        pad_list = [tup[1] for tup in sliding_arrs]
-        date_list = [tup[2] for tup in sliding_arrs]
-        
-        arr = np.concatenate(arr_list, axis=0) # 3-D array
-        pad_arr = np.concatenate(pad_list, axis=0) # 1-D array
-        date_arr = np.concatenate(date_list, axis=0) # 1-D array
-        id_arr = arr[:,-1:,0] 
-        
-        return arr, pad_arr, id_arr, date_arr
-    
-    def extract_windows(self, array, use_memmap):
-        """
-        Writes out 3-D numpy arrays (num_series, seq_len, num_cols) to memmap files to be merged later
-        """
-        # pad if array size < window_size i.e
-        array_size = array.shape[0]
-        pad_len = 0
-        if array_size >= self.window_len:
-            max_records = int(array.shape[0] - self.window_len + 1)
-        else:
-            max_records = 1
-            pad_len = int(self.window_len - array_size)
-            array = np.pad(array, pad_width=((pad_len,0),(0,0)), mode='constant', constant_values=0)
-        
-        sub_windows = (np.expand_dims(np.arange(self.window_len), 0) + np.expand_dims(np.arange(max_records, step=self.interleave), 0).T)
-    
-        array = array[sub_windows]
-        pad_array = (np.zeros((array.shape[0],), dtype=np.int32) + pad_len).reshape(-1,1)
-        
-        if use_memmap:
-            # memfile
-            f_name = self.workdir + '/' + str(array[0,0,0]) + '.dat'
-            shape = array.shape
-            fp = np.memmap(f_name, dtype='<U32', mode='w+', shape=shape)
-            fp[:] = array[:]
-            fp.flush()
-            del array
-            gc.collect()     
-            return (f_name, shape, pad_array)
-        else:
-            return (array, pad_array)
-        
-    def extract_infer_windows(self, array, date_array):
-        # pad if array size < window_size i.e
-        array_size = array.shape[0]
-        pad_len = 0
-        if array_size >= self.window_len:
-            max_records = int(array.shape[0] - self.window_len + 1)
-        else:
-            max_records = 1
-            pad_len = int(self.window_len - array_size)
-            array = np.pad(array, pad_width=((pad_len,0),(0,0)), mode='constant', constant_values=0)
-            date_array = np.pad(date_array, pad_width=((pad_len,0),), mode='constant', constant_values=0)
-        
-        sub_windows = (np.expand_dims(np.arange(self.window_len), 0) + np.expand_dims(np.arange(max_records, step=self.interleave), 0).T)
-    
-        arr = array[sub_windows]
-        date_arr = date_array[sub_windows]
-        date_arr = date_arr[:,-self.fh:]
-        pad_arr = np.zeros((arr.shape[0],), dtype=np.int32) + pad_len
-        
-        return (arr, pad_arr, date_arr)
-    
-    
-    def df_sampler(self, gdf):
+    def df_sampler(self, gdf, mode):
         """
         Helper function for select_arrs
         
         gdf = gdf.reset_index(drop=True)
         first_nonzero_index = gdf[self.target_col].ne(0).idxmax()
         gdf = gdf.iloc[first_nonzero_index:,:]
         gdf = gdf.reset_index(drop=True)
         
         """
+        
+        scale_gdf = gdf[gdf[self.time_index_col]<=self.train_till].reset_index(drop=True)
+        
+        if self.scaling_method == 'mean_scaling':
+            scale = [scale_gdf[self.target_col].mean() + 1.0]
+        elif self.scaling_method == 'standard_scaling':
+            scale_mu = scale_gdf[self.target_col].mean()
+            scale_std = np.maximum(scale_gdf[self.target_col].std(), 0.0001)
+            scale = [scale_mu, scale_std]
+        elif self.scaling_method == 'no_scaling':
+            scale = [1.0]
+        
+        if mode == 'train':
+            gdf = gdf[gdf[self.time_index_col]<=self.train_till].reset_index(drop=True)
+        elif mode == 'test':
+            test_len = int(gdf[(gdf[self.time_index_col]>self.train_till) & (gdf[self.time_index_col]<=self.test_till)].groupby(self.id_col)[self.target_col].count().max())
+            test_len = test_len + (self.window_len - self.fh)
+            gdf = gdf[gdf[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-test_len:]).reset_index(drop=True)
+            
         gdf = gdf.reset_index(drop=True)
         delta = len(gdf) - self.window_len
+        
         if delta<0:
             arr = gdf.loc[:,self.col_list].reset_index(drop=True).values
             # left pad to window_len with 0
             pad_len = np.abs(delta)
             arr = np.pad(arr,pad_width=((pad_len,0),(0,0)), mode='constant', constant_values=0)
         elif delta==0:
             pad_len = 0
             rand_start = 0
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
         else:
             pad_len = 0
             rand_start = random.randrange(delta)
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
-        return (arr, pad_len)
+            
+        return (arr, pad_len, scale)
     
     def df_infer_sampler(self, gdf):
         """
         Helper function for select_all_arrs
         """
+        scale_gdf = gdf[gdf[self.time_index_col]<=self.history_till].reset_index(drop=True)
+        
+        if self.scaling_method == 'mean_scaling':
+            scale = [scale_gdf[self.target_col].mean() + 1.0]
+        elif self.scaling_method == 'standard_scaling':
+            scale_mu = scale_gdf[self.target_col].mean()
+            scale_std = np.maximum(scale_gdf[self.target_col].std(), 0.0001)
+            scale = [scale_mu, scale_std]
+        elif self.scaling_method == 'no_scaling':
+            scale = [1.0]
+        
         gdf = gdf.reset_index(drop=True)
         delta = len(gdf) - self.window_len
         if delta<0:
             arr = gdf.loc[:,self.col_list].reset_index(drop=True).values
             pad_len = np.abs(delta)
             arr = np.pad(arr,pad_width=((pad_len,0),(0,0)), mode='constant', constant_values=0)
             date_arr = gdf.loc[:,self.time_index_col].reset_index(drop=True).values
@@ -335,31 +262,34 @@
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
             date_arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.time_index_col].reset_index(drop=True).tail(self.fh).values
         else:
             pad_len = 0
             rand_start = random.randrange(delta)
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
             date_arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.time_index_col].reset_index(drop=True).tail(self.fh).values
-        return (arr, pad_len, date_arr)
+        return (arr, pad_len, date_arr, scale)
     
     def select_all_arrs(self, data):
         """
         Use for inference dataset
         """
         groups = data.groupby([self.id_col])
         sampled_arr = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.df_infer_sampler)(gdf) for _,gdf in groups)
         arr_list = [tup[0] for tup in sampled_arr]
         pad_list = [tup[1] for tup in sampled_arr]
         date_list = [tup[2] for tup in sampled_arr]
+        scale_list = [tup[3] for tup in sampled_arr]
+        
         arr = np.stack(arr_list, axis=0)
         pad_arr = np.stack(pad_list, axis=0)
         date_arr = np.stack(date_list, axis=0)
+        scale_arr = np.stack(scale_list, axis=0)
         id_arr = arr[:,-1:,0]
         
-        return arr, pad_arr, id_arr, date_arr
+        return arr, pad_arr, id_arr, date_arr, scale_arr
     
     def sort_dataset(self, data):
         """
         sort pandas dataframe by provided col list & order
         """
         if len(self.sort_col_list) > 0:
             data = data.sort_values(by=self.sort_col_list, ascending=True)
@@ -380,177 +310,42 @@
         if len(null_cols)>0:
             null_status == True
         else:
             null_status == False
         
         return null_status, null_cols
     
-    def data_generator(self, data):
+    def data_generator(self, data, mode):
         """
         outputs:
         --------
         arr: [batch,window_len,len(col_list)]
         pad_arr as list: [pad_len_arr1, pad_len_arr2, ...]
 
         """
+        
+        train_data, test_data = self.split_train_test(data)
+        
         keys_dict, wts_dict = self.get_keys(data)
         self.train_test_batch_size = int(self.batch*len(keys_dict))
-        # accomodate larger batch sizes than no. of keys
-        cycles = int(m.ceil(self.batch/len(keys_dict)))
+       
         while True:
             sample_id = self.select_ids(keys_dict, wts_dict)
             df = data.query("{}==@sample_id".format(self.id_col))
-            arr, pad_arr = self.select_arrs(df)
-                
+            arr, pad_arr, scale_arr = self.select_arrs(df, mode)
+            
+            #print("data gen: ", scale_arr.shape)
             # -- done for @tf.function retracing reason. May revisit later
             #valid_indices = np.where(np.count_nonzero(arr[:,:self.window_len-self.fh,self.target_index].astype(np.float32)>0,axis=1)>=self.min_nz)
             #arr = arr[valid_indices]
             #pad_arr = pad_arr[valid_indices]
             
-            model_in, model_out, scale, weights  = self.preprocess(arr, pad_arr)
+            model_in, model_out, scale, weights  = self.preprocess(arr, pad_arr, scale_arr)
             yield model_in.astype(str), model_out.astype(np.float32), scale.astype(np.float32), weights.astype(np.float32)
             
-    def fill_buffer(self, data):
-        
-        keys_dict, wts_dict = self.get_keys(data)
-        self.train_test_batch_size = int(self.batch*len(keys_dict))
-        
-        # get max no. of keys 
-        if len(self.strata_col_list)>0:
-            max_keys = data.groupby(self.strata_col_list)[self.id_col].nunique().max()
-        else:
-            max_keys = data[self.id_col].nunique()
-            
-        # calculate interleave value required to meet max_samples requirement
-        #max_samples_count = data.groupby(self.id_col)[self.target_col].apply(lambda x: max(0,x.count()-self.window_len)).sum()
-        #self.interleave = m.ceil(max_samples_count/self.max_samples_required)
-            
-        # create arrays 
-        model_in = []
-        model_out =[]
-        scale = []
-        weights =[]
-        
-        for i in range(0, max_keys, self.batch):
-            sample_id = []
-            for k,v in keys_dict.items():
-                v = list(v)
-                if len(v) < max_keys:
-                    shortby = m.ceil(max_keys/len(v))
-                    v *= shortby        
-                sample_id += v[i:i+self.batch]
-            random.shuffle(sample_id)
-            
-            # extract rows for these sample_ids in parallel
-            df = data[self.col_list].query("{}==@sample_id".format(self.id_col))
-            arr, pad_arr = self.static_arrs(df, use_memmap=False, prefix='fill_buffer') 
-            valid_indices = np.where(np.count_nonzero(arr[:,:self.window_len-self.fh,self.target_index].astype(np.float32)>=0,axis=1)>=self.min_nz)
-            arr = arr[valid_indices]
-            pad_arr = pad_arr[valid_indices]
-            m_in, m_out, s, w  = self.preprocess(arr, pad_arr)
-            
-            # add to lists
-            model_in.append(m_in)
-            model_out.append(m_out)
-            scale.append(s)
-            weights.append(w)
-            
-        model_in = np.vstack(model_in)
-        model_out = np.vstack(model_out)
-        scale = np.vstack(scale)
-        weights = np.vstack(weights)   
-        
-        # shuffle
-        p = np.random.permutation(len(model_in))
-        model_in, model_out, scale, weights = model_in[p], model_out[p], scale[p], weights[p]
-        
-        return model_in.astype(str), model_out.astype(np.float32), scale.astype(np.float32), weights.astype(np.float32)
-        
-            
-    def static_dataset(self, data, batchsize, use_memmap, prefix='train'):
-        """
-        piecewise processing using np.memmap; works with arrays much larger than available memory
-        
-        """
-        
-        if use_memmap:
-            f_name, f_shape, pad_arr = self.static_arrs(data[self.col_list], use_memmap, prefix)
-            fp = np.memmap(f_name, dtype='<U32', mode='r', shape=f_shape)
-            num_batches = int((len(fp) // batchsize) + (1 if (len(fp) % batchsize)!=0 else 0))
-        
-            model_in_files = {}
-            model_out_files = {}
-            scale_files = {}
-            weights_files = {}
-        
-            for i in range(num_batches):
-                fp_batch, pad_batch = fp[i*batchsize:(i+1)*batchsize], pad_arr[i*batchsize:(i+1)*batchsize]
-            
-                # filter
-                valid_indices = np.where(np.count_nonzero(fp_batch[:,:self.window_len-self.fh,self.target_index].astype(np.float32)>0, axis=1)>=self.min_nz)
-                fp_batch = fp_batch[valid_indices]
-                pad_batch = pad_batch[valid_indices]
-            
-                # shuffle
-                p = np.random.permutation(len(fp_batch))
-                fp_batch, pad_batch = fp_batch[p], pad_batch[p]
-                model_in_batch, model_out_batch, scale_batch, weights_batch  = self.preprocess(fp_batch, pad_batch)
-            
-                # write to memmap
-                model_in_batch_name = self.workdir + '/' + str(prefix) + str(fp_batch[0,0,0]) + '_' + str(i) + '_model_in.dat'
-                model_in_mmap = np.memmap(model_in_batch_name, dtype='<U32', mode='w+', shape=model_in_batch.shape)
-                model_in_mmap[:] = model_in_batch[:]
-                model_in_mmap.flush()
-            
-                model_out_batch_name = self.workdir + '/' + str(prefix) + str(fp_batch[0,0,0]) + '_' + str(i) + '_model_out.dat'
-                model_out_mmap = np.memmap(model_out_batch_name, dtype='<U32', mode='w+', shape=model_out_batch.shape)
-                model_out_mmap[:] = model_out_batch[:]
-                model_out_mmap.flush()
-            
-                scale_batch_name = self.workdir + '/' + str(prefix) + str(fp_batch[0,0,0]) + '_' + str(i) + '_scale.dat'
-                scale_mmap = np.memmap(scale_batch_name, dtype='<U32', mode='w+', shape=scale_batch.shape)
-                scale_mmap[:] = scale_batch[:]
-                scale_mmap.flush()
-            
-                wts_batch_name = self.workdir + '/' + str(prefix) + str(fp_batch[0,0,0]) + '_' + str(i) + '_weights.dat'
-                wts_mmap = np.memmap(wts_batch_name, dtype='<U32', mode='w+', shape=weights_batch.shape)
-                wts_mmap[:] = weights_batch[:]
-                wts_mmap.flush()
-         
-                model_in_files[model_in_batch_name] = model_in_batch.shape
-                model_out_files[model_out_batch_name] = model_out_batch.shape
-                scale_files[scale_batch_name] = scale_batch.shape
-                weights_files[wts_batch_name] = weights_batch.shape
-        
-            del fp, pad_arr
-            gc.collect()
-        
-            try:
-                os.remove(f_name)
-            except:
-                pass
-        
-            return model_in_files, model_out_files, scale_files, weights_files
-        else:
-            arr, pad_arr = self.static_arrs(data[self.col_list], use_memmap, prefix)
-            
-            # filter
-            valid_indices = np.where(np.count_nonzero(arr[:,:self.window_len-self.fh,self.target_index].astype(np.float32)>0,axis=1)>=self.min_nz)
-            arr = arr[valid_indices]
-            pad_arr = pad_arr[valid_indices]
-            
-            # shuffle
-            p = np.random.permutation(len(arr))
-            arr, pad_arr = arr[p], pad_arr[p]
-            
-            model_in, model_out, scale, weights  = self.preprocess(arr, pad_arr)
-            del arr, pad_arr
-            gc.collect()
-            
-            return model_in.astype(str), model_out.astype(np.float32), scale.astype(np.float32), weights.astype(np.float32)
             
     def vocab_list(self, data):
         """
         Function to generate default embedding dimensions for categorical vars as 3rd root of no. of unique values.
         
         vocab_dict = {}
         embed_dict = {}
@@ -572,54 +367,52 @@
                         emb_dim = max(m.ceil(len(col_unique_vals)**0.33),2)       
                         cols_val_list.append(col_unique_vals)
                         cols_dim_list.append(emb_dim)
                     vocab_dict[k] = [d[0], cols_val_list, cols_dim_list]
                            
         return vocab_dict
     
-    def preprocess(self, sample_arr, pad_arr):
+    def preprocess(self, sample_arr, pad_arr, scale_arr):
         """
         Preprocess_samples Tensorflow Ops & outputs resp.
         """
         sequence_len = int(self.window_len)
         max_input_len = int(self.window_len - self.fh)
         
         sid =  sample_arr[..., [self.id_index]].astype(str)
         target = sample_arr[..., [self.target_index]].astype(float)
         
         # target outlier correction
         SU = np.maximum(3.0*np.quantile(target[:,:max_input_len,:], q=0.97, axis=1, keepdims=True), 0)
         SL = np.minimum(np.quantile(target[:,:max_input_len,:], q=0.01, axis=1, keepdims=True), 0)
         target = np.clip(target, a_min=SL, a_max=SU)
         
-        # scale target : target/target_mean -- old
-        #target_nz_count = np.maximum(np.count_nonzero(np.abs(target[:,:max_input_len,:]), axis=1).reshape(-1,1,1), 1.0)
-        #target_sum = np.sum(np.abs(target[:,:max_input_len,:]), axis=1, keepdims=True)
-        #target_nz_mean = np.divide(target_sum, target_nz_count) + 1.0
-        #target_scaled = np.divide(target, target_nz_mean)
-
-        # scale target : target/target_mean -- new
-        if self.scaling_method == 'mean_scaling':
-            target_nz_count = np.maximum(np.count_nonzero(np.abs(target[:, :max_input_len, :]), axis=1).reshape(-1, 1, 1), 1.0)
-            target_sum = np.sum(np.abs(target[:, :max_input_len, :]), axis=1, keepdims=True)
-            target_nz_mean = np.divide(target_sum, target_nz_count) + 1.0
+        # scale target : target/target_mean
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+            #target_nz_count = np.maximum(np.count_nonzero(np.abs(target[:,:max_input_len,:]), axis=1).reshape(-1,1,1), 1.0)
+            #target_sum = np.sum(np.abs(target[:,:max_input_len,:]), axis=1, keepdims=True)
+            #target_nz_mean = np.divide(target_sum, target_nz_count) + 1.0
+            target_nz_mean = scale_arr.reshape(-1,1,1)
             target_scaled = np.divide(target, target_nz_mean)
         elif self.scaling_method == 'standard_scaling':
-            target_mean = np.mean(target[:, :max_input_len, :], axis=1, keepdims=True)
-            target_stddev = np.maximum(np.std(target[:, :max_input_len, :], axis=1, keepdims=True), 0.001)
+            #target_mean = np.mean(target[:,:max_input_len,:], axis=1, keepdims=True)
+            #target_stddev = np.maximum(np.std(target[:,:max_input_len,:], axis=1, keepdims=True), 0.001)
+            target_mean = scale_arr[:,0].reshape(-1,1,1)
+            target_stddev = scale_arr[:,1].reshape(-1,1,1)
             target_scaled = np.divide(np.subtract(target, target_mean), target_stddev)
-            target_scaled = np.nan_to_num(target_scaled)  # correct where stddev is 0
-        elif self.scaling_method == 'no_scaling':
-            target_nz_mean = 1.0
-            target_scaled = np.divide(target, target_nz_mean)
-
+            target_scaled = np.nan_to_num(target_scaled) # correct where stddev is 0
+       
         # build model_in array  
         model_in = np.concatenate((sid, target_scaled), axis=-1)
         model_out = target_scaled[:,-self.fh:,:]
-
+        
+        # make model_in target values zero for the fh
+        #target_scaled[:,-self.fh:, :] = 0
+        #model_in = np.concatenate((sid, target_scaled), axis=-1)
+        
         if len(self.static_num_indices) > 0:
             static_num = sample_arr[..., self.static_num_indices].astype(float)
             # scale
             #static_nz_count = np.maximum(np.count_nonzero(np.abs(static_num), axis=1).reshape(-1,1,len(self.static_num_indices)), 1.0)
             #static_sum = np.sum(np.abs(static_num), axis=1, keepdims=True)
             #static_nz_mean = np.divide(static_sum, static_nz_count) + 1.0
             #static_num = np.divide(static_num, static_nz_mean)
@@ -629,61 +422,47 @@
         if len(self.static_cat_indices) > 0:
             static_cat = sample_arr[..., self.static_cat_indices].astype(str)
             # merge
             model_in = np.concatenate((model_in, static_cat), axis=-1)
 
         if len(self.temporal_known_num_indices) > 0:
             known_num = sample_arr[..., self.temporal_known_num_indices].astype(float)
-            # scale -- old
-            #known_nz_count = np.maximum(np.count_nonzero(np.abs(known_num), axis=1).reshape(-1,1,len(self.temporal_known_num_indices)), 1.0)
-            #known_sum = np.sum(np.abs(known_num), axis=1, keepdims=True)
-            #known_nz_mean = np.divide(known_sum, known_nz_count) + 1.0
-            #known_num = np.divide(known_num, known_nz_mean)
-            # scale -- new
+            # scale
             if self.scaling_method == 'mean_scaling':
-                known_nz_count = np.maximum(np.count_nonzero(np.abs(known_num), axis=1).reshape(-1, 1, len(self.temporal_known_num_indices)),1.0)
+                known_nz_count = np.maximum(np.count_nonzero(np.abs(known_num), axis=1).reshape(-1,1,len(self.temporal_known_num_indices)), 1.0)
                 known_sum = np.sum(np.abs(known_num), axis=1, keepdims=True)
                 known_nz_mean = np.divide(known_sum, known_nz_count) + 1.0
                 known_num = np.divide(known_num, known_nz_mean)
             elif self.scaling_method == 'standard_scaling':
                 known_mean = np.mean(known_num, axis=1, keepdims=True)
                 known_stddev = np.maximum(np.std(known_num, axis=1, keepdims=True), 0.001)
                 known_num = np.divide(np.subtract(known_num, known_mean), known_stddev)
                 known_num = np.nan_to_num(known_num)
             elif self.scaling_method == 'no_scaling':
-                known_nz_count = np.maximum(np.count_nonzero(np.abs(known_num), axis=1).reshape(-1, 1, len(self.temporal_known_num_indices)),1.0)
-                known_sum = np.sum(np.abs(known_num), axis=1, keepdims=True)
-                known_nz_mean = np.divide(known_sum, known_nz_count) + 1.0
-                known_num = np.divide(known_num, known_nz_mean)
+                pass
+            
             # merge
             model_in = np.concatenate((model_in, known_num), axis=-1)
 
         if len(self.temporal_unknown_num_indices) > 0:
             unknown_num = sample_arr[..., self.temporal_unknown_num_indices].astype(float)
-            # scale -- old
-            #unknown_nz_count = np.maximum(np.count_nonzero(np.abs(unknown_num[:,:max_input_len,:]), axis=1).reshape(-1,1,len(self.temporal_unknown_num_indices)), 1.0)
-            #unknown_sum = np.sum(np.abs(unknown_num[:,:max_input_len,:]), axis=1, keepdims=True)
-            #unknown_nz_mean = np.divide(unknown_sum, unknown_nz_count) + 1.0
-            #unknown_num = np.divide(unknown_num, unknown_nz_mean)
-            # scale -- new
+            # scale
             if self.scaling_method == 'mean_scaling':
-                unknown_nz_count = np.maximum(np.count_nonzero(np.abs(unknown_num[:, :max_input_len, :]), axis=1).reshape(-1, 1, len(self.temporal_unknown_num_indices)),1.0)
-                unknown_sum = np.sum(np.abs(unknown_num[:, :max_input_len, :]), axis=1, keepdims=True)
+                unknown_nz_count = np.maximum(np.count_nonzero(np.abs(unknown_num[:,:max_input_len,:]), axis=1).reshape(-1,1,len(self.temporal_unknown_num_indices)), 1.0)
+                unknown_sum = np.sum(np.abs(unknown_num[:,:max_input_len,:]), axis=1, keepdims=True)
                 unknown_nz_mean = np.divide(unknown_sum, unknown_nz_count) + 1.0
                 unknown_num = np.divide(unknown_num, unknown_nz_mean)
             elif self.scaling_method == 'standard_scaling':
-                unknown_mean = np.mean(unknown_num[:, :max_input_len, :], axis=1, keepdims=True)
-                unknown_stddev = np.maximum(np.std(unknown_num[:, :max_input_len, :], axis=1, keepdims=True), 0.001)
+                unknown_mean = np.mean(unknown_num[:,:max_input_len,:], axis=1, keepdims=True)
+                unknown_stddev = np.maximum(np.std(unknown_num[:,:max_input_len,:], axis=1, keepdims=True), 0.001)
                 unknown_num = np.divide(np.subtract(unknown_num, unknown_mean), unknown_stddev)
                 unknown_num = np.nan_to_num(unknown_num)
             elif self.scaling_method == 'no_scaling':
-                unknown_nz_count = np.maximum(np.count_nonzero(np.abs(unknown_num[:, :max_input_len, :]), axis=1).reshape(-1, 1, len(self.temporal_unknown_num_indices)),1.0)
-                unknown_sum = np.sum(np.abs(unknown_num[:, :max_input_len, :]), axis=1, keepdims=True)
-                unknown_nz_mean = np.divide(unknown_sum, unknown_nz_count) + 1.0
-                unknown_num = np.divide(unknown_num, unknown_nz_mean)
+                pass
+            
             # merge
             model_in = np.concatenate((model_in, unknown_num), axis=-1)
    
         if len(self.temporal_known_cat_indices) > 0:
             known_cat = sample_arr[..., self.temporal_known_cat_indices].astype(str)
             # merge
             model_in = np.concatenate((model_in, known_cat), axis=-1)
@@ -692,63 +471,49 @@
             unknown_cat = sample_arr[..., self.temporal_unknown_cat_indices].astype(str)
             # merge
             model_in = np.concatenate((model_in, unknown_cat), axis=-1)
             
         rel_age = np.broadcast_to((np.arange(0,sequence_len,1)/sequence_len).reshape(-1,1), target.shape)
         model_in = np.concatenate((model_in, rel_age), axis=-1) 
         
-        # scale -- old
-        #scale_in = np.broadcast_to(target_nz_mean, target.shape)
-        #model_in = np.concatenate((model_in, scale_in), axis=-1)
-        #scale_out = np.broadcast_to(target_nz_mean, model_out.shape)
-
-        # scale -- new
-        if self.scaling_method == 'mean_scaling':
+        # scale
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
             scale_in = np.broadcast_to(target_nz_mean, target.shape)
         elif self.scaling_method == 'standard_scaling':
             scale_mean = np.broadcast_to(target_mean, target.shape)
             scale_std = np.broadcast_to(target_stddev, target.shape)
             scale_in = np.concatenate((scale_mean, scale_std), axis=-1)
-        elif self.scaling_method == 'no_scaling':
-            scale_in = np.broadcast_to(target_nz_mean, target.shape)
-
+            
         model_in = np.concatenate((model_in, scale_in), axis=-1)
-
-        if self.scaling_method == 'mean_scaling':
+        
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
             scale_out = np.broadcast_to(target_nz_mean, model_out.shape)
         elif self.scaling_method == 'standard_scaling':
             scale_mean_out = np.broadcast_to(target_mean, model_out.shape)
             scale_std_out = np.broadcast_to(target_stddev, model_out.shape)
             scale_out = np.concatenate((scale_mean_out, scale_std_out), axis=-1)
-        elif self.scaling_method == 'no_scaling':
-            scale_out = np.broadcast_to(target_nz_mean, model_out.shape)
-
+            
         mask_list = []
         for pad_len in pad_arr:
             if pad_len > 0:
                 mask = np.concatenate((-1*np.ones((1,pad_len)), np.ones((1,sequence_len-pad_len))), axis=1)
             else:
                 mask = np.ones((1,sequence_len))
             mask_list.append(mask)
 
         # mask & relative age
         mask = np.vstack(mask_list).reshape(-1,sequence_len,1)
         model_in = np.concatenate((model_in, mask), axis=-1)
 
-        # sample weights -- old
-        #weights = np.around(np.log10(np.squeeze(target_nz_mean) + 10),2) #/np.quantile(np.squeeze(target_nz_mean), q=0.8)
-        # sample weights -- new
-        if self.scaling_method == 'mean_scaling':
-            weights = np.around(np.log10(np.squeeze(target_nz_mean) + 10), 2)  # /np.quantile(np.squeeze(target_nz_mean), q=0.8)
+        # sample weights
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+            weights = np.around(np.log10(np.squeeze(target_nz_mean) + 10),2) #/np.quantile(np.squeeze(target_nz_mean), q=0.8)
         elif self.scaling_method == 'standard_scaling':
-            weights = np.around(np.log10(np.squeeze(target_mean) + 10), 2)
-        elif self.scaling_method == 'no_scaling':
-            weights = np.around(np.log10(np.squeeze(target_nz_mean) + 10), 2)
-
-        weights = np.clip(weights, a_min=1.0, a_max=5.0)
+            weights = np.around(np.log10(np.squeeze(target_mean) + 10),2)
+        weights = np.clip(weights, a_min=1.0, a_max=2.0)
         weights = weights.reshape(-1,1)
         #weights = np.expand_dims(weights.reshape(-1,1), axis=-1)
         #weights = np.tile(weights, [1,sequence_len,1])
         
         return model_in, model_out, scale_out, weights
     
     def split_train_test(self, data):
@@ -760,185 +525,74 @@
             # check if test_till - train_till > window_len
             test_len = int(data[(data[self.time_index_col]>self.train_till) & (data[self.time_index_col]<=self.test_till)].groupby(self.id_col)[self.target_col].count().max())
             test_len = test_len + (self.window_len - self.fh)
             test_data = data[data[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-test_len:]).reset_index(drop=True)
             #test_data = data[data[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True) #original
         return train_data, test_data
     
-    def train_test_dataset(self, data, train_till, test_till, low_memory=True, use_memmap=True, fill_buffer=False):
+    def train_test_dataset(self, data, train_till, test_till):
         
-        if self.datetime_format is not None:
-            data[self.time_index_col] = pd.to_datetime(data[self.time_index_col], format=self.datetime_format)
-            self.train_till = pd.to_datetime(train_till, format=self.datetime_format)
-            self.test_till = pd.to_datetime(test_till, format=self.datetime_format)
-        else:
-            self.train_till = train_till
-            self.test_till = test_till
+        self.train_till = train_till
+        self.test_till = test_till
             
         # check null
         null_status, null_cols = self.check_null(data)
         if null_status:
             print("NaN column(s): ", null_cols)
             raise ValueError("Column(s) with NaN detected!")
         
         # sort
         data = self.sort_dataset(data)
         
-        # infer frequency
-        if self.datetime_format is not None:
-            sample_id = data[self.id_col].unique().tolist()[0]
-            freq = pd.infer_freq(data[data[self.id_col]==sample_id][self.time_index_col])
-            if freq == 'H':
-                self.train_test_timedelta = int((self.test_till - self.train_till).dt.seconds/3600)
-            elif freq == 'D':
-                self.train_test_timedelta = int((self.test_till - self.train_till).dt.days)
-            elif freq == '7D':
-                self.train_test_timedelta = int((self.test_till - self.train_till).dt.days/7)
-            elif freq == 'M':
-                self.train_test_timedelta = int(12*(self.test_till.dt.year - self.train_till.dt.year) + (self.test_till.dt.month - self.train_till.dt.month))
-        
-        # split into train, test dfs
-        train_data, test_data = self.split_train_test(data)
-        
         # check samples
-        check_gen = self.data_generator(train_data)
+        check_gen = self.data_generator(data=data, mode='train')
         x, y, s, w = next(check_gen)
         num_features = x.shape[-1]
         scale_dims = s.shape[-1]
         
-        if low_memory and (not fill_buffer):
-            print("low_memory: {} and fill_buffer: {}. Use generator".format(low_memory, fill_buffer))
-            trainset = tf.data.Dataset.from_generator(lambda: self.data_generator(train_data),
+        trainset = tf.data.Dataset.from_generator(lambda: self.data_generator(data=data, mode='train'),
                                                       output_signature=(tf.TensorSpec(shape=(None, self.window_len, num_features), dtype=tf.string),
                                                                         tf.TensorSpec(shape=(None, self.fh, 1), dtype=tf.float32),
                                                                         tf.TensorSpec(shape=(None, self.fh, scale_dims), dtype=tf.float32),
                                                                         tf.TensorSpec(shape=(None, 1), dtype=tf.float32)))
         
-            testset = tf.data.Dataset.from_generator(lambda: self.data_generator(test_data),
+        testset = tf.data.Dataset.from_generator(lambda: self.data_generator(data=data, mode='test'),
                                                      output_signature=(tf.TensorSpec(shape=(None, self.window_len, num_features), dtype=tf.string),
                                                                        tf.TensorSpec(shape=(None, self.fh, 1), dtype=tf.float32),
                                                                        tf.TensorSpec(shape=(None, self.fh, scale_dims), dtype=tf.float32),
                                                                        tf.TensorSpec(shape=(None, 1), dtype=tf.float32)))
-        elif (not low_memory) and use_memmap:
-            print("low_memory: {} and use_memmap: {}. Use memmap".format(low_memory, use_memmap))
-            SHUFFLE_BUFFER_SIZE = int(m.ceil(train_data[self.id_col].nunique()*0.01)*self.batch)
-            BATCH_SIZE = self.batch
-            
-            train_x, train_y, train_z, train_w = self.static_dataset(train_data, batchsize=self.batch*max(m.ceil(train_data[self.id_col].nunique()*0.01), 200), use_memmap=use_memmap, prefix='train')
-            test_x, test_y, test_z, test_w = self.static_dataset(test_data, batchsize=self.batch*max(m.ceil(test_data[self.id_col].nunique()*0.01), 200), use_memmap=use_memmap, prefix='test')
-               
-            def train_data_generator():
-                train_datasets = []
-                for (k1,v1), (k2,v2), (k3,v3), (k4,v4) in zip(train_x.items(), train_y.items(), train_z.items(), train_w.items()):
-                    model_in = np.memmap(k1, dtype='<U32', mode='r', shape=v1)
-                    model_out = np.memmap(k2, dtype='<U32', mode='r', shape=v2)
-                    scale = np.memmap(k3, dtype='<U32', mode='r', shape=v3)
-                    weights = np.memmap(k4, dtype='<U32', mode='r', shape=v4)
-                    ds = tf.data.Dataset.from_tensor_slices((model_in.astype(str), model_out.astype(np.float32), scale.astype(np.float32), weights.astype(np.float32)))
-                    train_datasets.append(ds)
-                return train_datasets
-                
-            def test_data_generator():
-                test_datasets = []
-                for (k1,v1), (k2,v2), (k3,v3), (k4,v4) in zip(test_x.items(), test_y.items(), test_z.items(), test_w.items()):
-                    model_in = np.memmap(k1, dtype='<U32', mode='r', shape=v1)
-                    model_out = np.memmap(k2, dtype='<U32', mode='r', shape=v2)
-                    scale = np.memmap(k3, dtype='<U32', mode='r', shape=v3)
-                    weights = np.memmap(k4, dtype='<U32', mode='r', shape=v4)
-                    ds = tf.data.Dataset.from_tensor_slices((model_in.astype(str), model_out.astype(np.float32), scale.astype(np.float32), weights.astype(np.float32)))
-                    test_datasets.append(ds)
-                return test_datasets
-                
-            train_datasets = train_data_generator()
-            test_datasets = test_data_generator()
-            
-            if tf.__version__ < "2.7.0":
-                trainset = tf.data.experimental.sample_from_datasets(train_datasets).batch(BATCH_SIZE, drop_remainder=True) #num_parallel_calls=self.PARALLEL_DATA_JOBS)
-                testset = tf.data.experimental.sample_from_datasets(test_datasets).batch(BATCH_SIZE, drop_remainder=False) #num_parallel_calls=self.PARALLEL_DATA_JOBS)
-            else:
-                trainset = tf.data.Dataset.sample_from_datasets(train_datasets).batch(BATCH_SIZE, drop_remainder=True) #num_parallel_calls=self.PARALLEL_DATA_JOBS)
-                testset = tf.data.Dataset.sample_from_datasets(test_datasets).batch(BATCH_SIZE, drop_remainder=False) #num_parallel_calls=self.PARALLEL_DATA_JOBS)
-        
-        elif (not low_memory) and (not use_memmap):
-            print("low_memory: {} and use_memmap: {}. Use static_dataset".format(low_memory, use_memmap))
-            SHUFFLE_BUFFER_SIZE = int(m.ceil(train_data[self.id_col].nunique()*0.1)*self.batch)
-            
-            model_in_x, model_out_x, scale_x, weights_x = self.static_dataset(train_data, batchsize=self.batch*max(m.ceil(train_data[self.id_col].nunique()*0.01), 200), use_memmap=use_memmap, prefix='train')
-            model_in_y, model_out_y, scale_y, weights_y = self.static_dataset(test_data, batchsize=self.batch*max(m.ceil(test_data[self.id_col].nunique()*0.01), 200), use_memmap=use_memmap, prefix='test')
-            
-            if tf.__version__ < "2.7.0":
-                trainset = tf.data.Dataset.from_tensor_slices((model_in_x, model_out_x, scale_x, weights_x)).shuffle(SHUFFLE_BUFFER_SIZE, reshuffle_each_iteration=True).batch(self.batch, drop_remainder=True)
-                testset = tf.data.Dataset.from_tensor_slices((model_in_y, model_out_y, scale_y, weights_y)).batch(self.batch, drop_remainder=False)
-            else:
-                trainset = tf.data.Dataset.from_tensor_slices((model_in_x, model_out_x, scale_x, weights_x)).shuffle(SHUFFLE_BUFFER_SIZE, reshuffle_each_iteration=True).batch(self.batch, drop_remainder=True, num_parallel_calls=self.PARALLEL_DATA_JOBS)
-                testset = tf.data.Dataset.from_tensor_slices((model_in_y, model_out_y, scale_y, weights_y)).batch(self.batch, drop_remainder=False, num_parallel_calls=self.PARALLEL_DATA_JOBS)
-        
-        elif fill_buffer:
-            print("low_memory: {}, fill_buffer: {}. Fill buffer".format(low_memory, fill_buffer))
-            #avg_train_samples = max(1, int((train_data.groupby(self.id_col).size().mean() - self.window_len)/self.interleave))
-            #num_train_observations = avg_train_samples*train_data[self.id_col].nunique()
-            
-            #avg_test_samples = max(1, int((test_data.groupby(self.id_col).size().mean() - self.window_len)))
-            #num_test_observations = avg_test_samples*test_data[self.id_col].nunique()
-            
-            model_in_x, model_out_x, scale_x, _ = self.fill_buffer(train_data) # , num_observations=num_train_observations)
-            model_in_y, model_out_y, scale_y, _ = self.fill_buffer(test_data) # , num_observations=num_test_observations)
-            
-            # weights over entire dataset based on scale
-            weights_x = np.around(np.log10(np.squeeze(scale_x[:,-1:,:])+10),2)
-            weights_x = weights_x.reshape(-1,1)
-            
-            weights_y = np.around(np.log10(np.squeeze(scale_y[:,-1:,:])+10),2)
-            weights_y = weights_y.reshape(-1,1)
-            
-            TRAIN_SHUFFLE_BUFFER_SIZE = model_in_x.shape[0] # num_train_observations
-            TEST_SHUFFLE_BUFFER_SIZE = model_in_y.shape[0] # num_test_observations
-            
-            if tf.__version__ < "2.7.0":
-                trainset = tf.data.Dataset.from_tensor_slices((model_in_x, model_out_x, scale_x, weights_x)).shuffle(TRAIN_SHUFFLE_BUFFER_SIZE, reshuffle_each_iteration=False).batch(self.train_test_batch_size, drop_remainder=True)
-                testset = tf.data.Dataset.from_tensor_slices((model_in_y, model_out_y, scale_y, weights_y)).shuffle(TEST_SHUFFLE_BUFFER_SIZE, reshuffle_each_iteration=False).batch(self.train_test_batch_size, drop_remainder=True)
-            else:
-                trainset = tf.data.Dataset.from_tensor_slices((model_in_x, model_out_x, scale_x, weights_x)).shuffle(TRAIN_SHUFFLE_BUFFER_SIZE, reshuffle_each_iteration=False).batch(self.train_test_batch_size, drop_remainder=True, num_parallel_calls=self.PARALLEL_DATA_JOBS)
-                testset = tf.data.Dataset.from_tensor_slices((model_in_y, model_out_y, scale_y, weights_y)).shuffle(TEST_SHUFFLE_BUFFER_SIZE, reshuffle_each_iteration=False).batch(self.train_test_batch_size, drop_remainder=True, num_parallel_calls=self.PARALLEL_DATA_JOBS)
-         
+
         return trainset, testset
         
 
-    def infer_dataset(self, data, history_till, future_till, low_memory=True):
+    def infer_dataset(self, data, history_till, future_till):
         self.history_till = history_till
         self.future_till = future_till
         
         # check null
         null_status, null_cols = self.check_null(data)
         if null_status:
             print("NaN column(s): ", null_cols)
             raise ValueError("Column(s) with NaN detected!")
             
         # sort & filter to recent context
         data = self.sort_dataset(data)
         data = data[data[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
+
+        arr, pad_arr, id_arr, date_arr, scale_arr = self.select_all_arrs(data)
         
-        if low_memory:
-            arr, pad_arr, id_arr, date_arr = self.select_all_arrs(data)
-        else:
-            arr, pad_arr, id_arr, date_arr = self.static_infer_arrs(data)
-        
-        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr)
+        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr, scale_arr)
         input_tensor = tf.convert_to_tensor(model_in.astype(str), dtype=tf.string)
         
-        # for evaluation -- old
-        #actuals_arr = model_out*scale
-        # for evaluation -- new
-        if self.scaling_method == 'mean_scaling':
-            actuals_arr = model_out * scale
+        # for evaluation
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+            actuals_arr = model_out*scale
         elif self.scaling_method == 'standard_scaling':
-            actuals_arr = model_out * scale[:, :, 1:2] + scale[:, :, 0:1]
-        elif self.scaling_method == 'no_scaling':
-            actuals_arr = model_out * scale
-        
+            actuals_arr = model_out*scale[:,:,1:2] + scale[:,:,0:1]
+            
         if len(self.static_cat_col_list)>0:
             stat_arr_list = []
             for col, i in zip(self.static_cat_col_list, self.static_cat_indices):
                 stat_arr = model_in[:,-1:,i].astype(str)
                 stat_arr_list.append(stat_arr)    
             stat_arr = np.concatenate(stat_arr_list, axis=1)        
             actuals_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1), stat_arr, actuals_arr.reshape(-1,self.fh)), axis=1))
@@ -961,15 +615,15 @@
             # merge with forecast period dates
             date_df = pd.DataFrame(date_arr.reshape(-1,)).rename(columns={0:'period'})
             actuals_df = pd.concat([actuals_df, date_df], axis=1)
             actuals_df['actual'] = actuals_df['actual'].astype(np.float32)
          
         return [input_tensor, scale, id_arr, date_arr], actuals_df
     
-    def baseline_infer_dataset(self, data, history_till, future_till, ignore_cols, ignore_pad_values, low_memory=True):
+    def baseline_infer_dataset(self, data, history_till, future_till, ignore_cols, ignore_pad_values):
         self.history_till = history_till
         self.future_till = future_till
         
         # check null
         null_status, null_cols = self.check_null(data)
         if null_status:
             print("NaN column(s): ", null_cols)
@@ -979,20 +633,17 @@
         data = self.sort_dataset(data)
         data = data[data[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
         
         # mask out columns in ignore_cols for baseline forecast
         for col,val in zip(ignore_cols, ignore_pad_values):
             data[col] = np.where(data[self.time_index_col]>self.history_till, val, data[col])
         
-        if low_memory:
-            arr, pad_arr, id_arr, date_arr = self.select_all_arrs(data)
-        else:
-            arr, pad_arr, id_arr, date_arr = self.static_infer_arrs(data)
-            
-        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr)
+        arr, pad_arr, id_arr, date_arr, scale_arr = self.select_all_arrs(data)
+     
+        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr, scale_arr)
         input_tensor = tf.convert_to_tensor(model_in.astype(str), dtype=tf.string)
         
         return [input_tensor, scale, id_arr, date_arr]
     
     def acf(self, series):
         # https://stackoverflow.com/questions/43344406/is-there-a-bokeh-version-of-pandas-autocorrelation-plot-method
         n = len(series)
@@ -1187,10 +838,13 @@
             layout = column(sup_title, grid, sizing_mode="stretch_both")
             layouts.append(layout)
             i += 1
         
         supergrid = gridplot(layouts, ncols=1)
         show(supergrid)
 
-# COMMAND ----------
+
+# In[ ]:
+
+
```

### Comparing `fmldk-1.1.8/tft/tft_global_scaled_data.py` & `fmldk-1.1.9/sage/sage_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[ ]:
-
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import pandas as pd
 import numpy as np
 from joblib import Parallel, delayed
@@ -25,18 +23,15 @@
 from bokeh.models import ColumnDataSource, HoverTool, Div, FactorRange
 from bokeh.layouts import gridplot, column, row
 from bokeh.palettes import Category10, Category20, Colorblind
 from bokeh.io import reset_output
 from bokeh.models.ranges import DataRange1d
 
 
-# In[ ]:
-
-
-class tft_gs_dataset:
+class sage_dataset:
     def __init__(self, 
                  col_dict, 
                  window_len, 
                  fh, 
                  batch, 
                  min_nz,
                  scaling_method = 'mean_scaling',
@@ -58,15 +53,15 @@
                                                        strata_col_list:[],
                                                        sort_col_list:[],
                                                        wt_col:''}
         window_len: history_len + forecast_horizon
         fh: forecast_horizon
         batch: batch_size (per strata)
         min_nz: min. no. of non-zeros in the target input series to be eligible for train/test batch
-        scaling_method = 'mean_scaling','standard_scaling','no_scaling'
+        
         """
         self.col_dict = col_dict
         self.window_len = window_len
         self.fh = fh
         self.batch = batch
         self.min_nz = min_nz
         self.interleave = interleave
@@ -170,23 +165,30 @@
         random.shuffle(sample_id)
         return sample_id
 
     def select_arrs(self, df, mode):
         """
         Extract train/test samples from each sampled Id as 2-D arrays [window_len, num_columns]
         """
+        # filter out ids with insufficient timestamps (at least one datapoint should be before train cutoff period)
+        df = df.groupby(self.id_col).filter(lambda x: x[self.time_index_col].min()<self.train_till)
+
         groups = df.groupby([self.id_col])
         sampled_arr = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.df_sampler)(gdf, mode) for _,gdf in groups)
         arr_list = [tup[0] for tup in sampled_arr]
         pad_list = [tup[1] for tup in sampled_arr]
         scale_list = [tup[2] for tup in sampled_arr]
+        known_scale_list = [tup[3] for tup in sampled_arr]
+        unknown_scale_list = [tup[4] for tup in sampled_arr]
         arr = np.stack(arr_list, axis=0)
         pad_arr = np.stack(pad_list, axis=0)
         scale_arr = np.stack(scale_list, axis=0)
-        return arr, pad_arr, scale_arr
+        known_scale_arr = np.stack(known_scale_list, axis=0)
+        unknown_scale_arr = np.stack(unknown_scale_list, axis=0)
+        return arr, pad_arr, scale_arr, known_scale_arr, unknown_scale_arr
 
     def df_sampler(self, gdf, mode):
         """
         Helper function for select_arrs
         
         gdf = gdf.reset_index(drop=True)
         first_nonzero_index = gdf[self.target_col].ne(0).idxmax()
@@ -194,27 +196,61 @@
         gdf = gdf.reset_index(drop=True)
         
         """
         
         scale_gdf = gdf[gdf[self.time_index_col]<=self.train_till].reset_index(drop=True)
         
         if self.scaling_method == 'mean_scaling':
-            scale = [scale_gdf[self.target_col].mean() + 1.0]
+            target_nz_count = np.maximum(np.count_nonzero(np.abs(scale_gdf[self.target_col])), 1.0)
+            target_sum = np.sum(np.abs(scale_gdf[self.target_col]))
+            scale = [np.divide(target_sum, target_nz_count) + 1.0]
+            
+            if len(self.temporal_known_num_indices) > 0:
+              known_nz_count = np.maximum(np.count_nonzero(np.abs(scale_gdf[self.temporal_known_num_col_list].values), axis=0), 1.0)
+              known_sum = np.sum(np.abs(scale_gdf[self.temporal_known_num_col_list].values), axis=0)
+              known_scale = [np.divide(known_sum, known_nz_count) + 1.0]
+            else:
+              known_scale = [1]
+
+            if len(self.temporal_unknown_num_indices) > 0:
+              unknown_nz_count = np.maximum(np.count_nonzero(np.abs(scale_gdf[self.temporal_unknown_num_col_list].values), axis=0), 1.0)
+              unknown_sum = np.sum(np.abs(scale_gdf[self.temporal_unknown_num_col_list].values), axis=0)
+              unknown_scale = [np.divide(unknown_sum, unknown_nz_count) + 1.0]
+            else:
+              unknown_scale = [1]
+
         elif self.scaling_method == 'standard_scaling':
             scale_mu = scale_gdf[self.target_col].mean()
             scale_std = np.maximum(scale_gdf[self.target_col].std(), 0.0001)
             scale = [scale_mu, scale_std]
-        elif self.scaling_method == 'no_scaling':
+
+            if len(self.temporal_known_num_indices) > 0:
+              known_mean = np.mean(scale_gdf[self.temporal_known_num_col_list].values, axis=0)
+              known_stddev = np.maximum(np.std(scale_gdf[self.temporal_known_num_col_list].values, axis=0), 0.0001)
+              known_scale = [known_mean, known_stddev]
+            else:
+              known_scale = [0, 1]
+
+            if len(self.temporal_unknown_num_indices) > 0:
+              unknown_mean = np.mean(scale_gdf[self.temporal_unknown_num_col_list].values, axis=0)
+              unknown_stddev = np.maximum(np.std(scale_gdf[self.temporal_unknown_num_col_list].values, axis=0), 0.0001)
+              unknown_scale = [unknown_mean, unknown_stddev]
+            else:
+              unknown_scale = [0, 1]
+
+        elif self.scaling_method == 'no_scaling' or self.scaling_method == 'log_scaling':
             scale = [1.0]
+            known_scale = [1.0]
+            unknown_scale = [1.0]
         
         if mode == 'train':
             gdf = gdf[gdf[self.time_index_col]<=self.train_till].reset_index(drop=True)
         elif mode == 'test':
             test_len = int(gdf[(gdf[self.time_index_col]>self.train_till) & (gdf[self.time_index_col]<=self.test_till)].groupby(self.id_col)[self.target_col].count().max())
-            test_len = test_len + (self.window_len - self.fh)
+            test_len = test_len + (self.window_len - self.fh) 
             gdf = gdf[gdf[self.time_index_col]<=self.test_till].groupby(self.id_col).apply(lambda x: x[-test_len:]).reset_index(drop=True)
             
         gdf = gdf.reset_index(drop=True)
         delta = len(gdf) - self.window_len
         
         if delta<0:
             arr = gdf.loc[:,self.col_list].reset_index(drop=True).values
@@ -226,32 +262,69 @@
             rand_start = 0
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
         else:
             pad_len = 0
             rand_start = random.randrange(delta)
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
             
-        return (arr, pad_len, scale)
+        return (arr, pad_len, scale, known_scale, unknown_scale)
     
     def df_infer_sampler(self, gdf):
         """
         Helper function for select_all_arrs
         """
-        scale_gdf = gdf[gdf[self.time_index_col]<=self.history_till].reset_index(drop=True)
+        scale_gdf = gdf[gdf[self.time_index_col]<=self.train_till].reset_index(drop=True)
         
         if self.scaling_method == 'mean_scaling':
-            scale = [scale_gdf[self.target_col].mean() + 1.0]
+            target_nz_count = np.maximum(np.count_nonzero(np.abs(scale_gdf[self.target_col])), 1.0)
+            target_sum = np.sum(np.abs(scale_gdf[self.target_col]))
+            scale = [np.divide(target_sum, target_nz_count) + 1.0]
+
+            if len(self.temporal_known_num_indices) > 0:
+              known_nz_count = np.maximum(np.count_nonzero(np.abs(scale_gdf[self.temporal_known_num_col_list].values), axis=0), 1.0)
+              known_sum = np.sum(np.abs(scale_gdf[self.temporal_known_num_col_list].values), axis=0)
+              known_scale = [np.divide(known_sum, known_nz_count) + 1.0]
+            else:
+              known_scale = [1]
+
+            if len(self.temporal_unknown_num_indices) > 0:
+              unknown_nz_count = np.maximum(np.count_nonzero(np.abs(scale_gdf[self.temporal_unknown_num_col_list].values), axis=0), 1.0)
+              unknown_sum = np.sum(np.abs(scale_gdf[self.temporal_unknown_num_col_list].values), axis=0)
+              unknown_scale = [np.divide(unknown_sum, unknown_nz_count) + 1.0]
+            else:
+              unknown_scale = [1]
+
         elif self.scaling_method == 'standard_scaling':
             scale_mu = scale_gdf[self.target_col].mean()
             scale_std = np.maximum(scale_gdf[self.target_col].std(), 0.0001)
             scale = [scale_mu, scale_std]
-        elif self.scaling_method == 'no_scaling':
+
+            if len(self.temporal_known_num_indices) > 0:
+              known_mean = np.mean(scale_gdf[self.temporal_known_num_col_list].values, axis=0)
+              known_stddev = np.maximum(np.std(scale_gdf[self.temporal_known_num_col_list].values, axis=0), 0.0001)
+              known_scale = [known_mean, known_stddev]
+            else:
+              known_scale = [0, 1]
+
+            if len(self.temporal_unknown_num_indices) > 0:
+              unknown_mean = np.mean(scale_gdf[self.temporal_unknown_num_col_list].values, axis=0)
+              unknown_stddev = np.maximum(np.std(scale_gdf[self.temporal_unknown_num_col_list].values, axis=0), 0.0001)
+              unknown_scale = [unknown_mean, unknown_stddev]
+            else:
+              unknown_scale = [0, 1]
+
+        elif self.scaling_method == 'no_scaling' or self.scaling_method == 'log_scaling':
             scale = [1.0]
-        
+            known_scale = [1.0]
+            unknown_scale = [1.0]
+            
+        # restrict to prediction window_len
+        gdf = gdf[gdf[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
         gdf = gdf.reset_index(drop=True)
+        
         delta = len(gdf) - self.window_len
         if delta<0:
             arr = gdf.loc[:,self.col_list].reset_index(drop=True).values
             pad_len = np.abs(delta)
             arr = np.pad(arr,pad_width=((pad_len,0),(0,0)), mode='constant', constant_values=0)
             date_arr = gdf.loc[:,self.time_index_col].reset_index(drop=True).values
             date_arr = np.pad(date_arr,pad_width=((pad_len,0)), mode='constant', constant_values=0)
@@ -262,34 +335,42 @@
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
             date_arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.time_index_col].reset_index(drop=True).tail(self.fh).values
         else:
             pad_len = 0
             rand_start = random.randrange(delta)
             arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.col_list].reset_index(drop=True).values
             date_arr = gdf.loc[rand_start:rand_start + self.window_len - 1, self.time_index_col].reset_index(drop=True).tail(self.fh).values
-        return (arr, pad_len, date_arr, scale)
+        return (arr, pad_len, date_arr, scale, known_scale, unknown_scale)
     
     def select_all_arrs(self, data):
         """
         Use for inference dataset
         """
+        # filter out ids with insufficient timestamps (at least one datapoint should be before history cutoff period)
+        data = data.groupby(self.id_col).filter(lambda x: x[self.time_index_col].min()<self.history_till)
+
         groups = data.groupby([self.id_col])
         sampled_arr = Parallel(n_jobs=self.PARALLEL_DATA_JOBS, batch_size=self.PARALLEL_DATA_JOBS_BATCHSIZE)(delayed(self.df_infer_sampler)(gdf) for _,gdf in groups)
         arr_list = [tup[0] for tup in sampled_arr]
         pad_list = [tup[1] for tup in sampled_arr]
         date_list = [tup[2] for tup in sampled_arr]
         scale_list = [tup[3] for tup in sampled_arr]
-        
+        known_scale_list = [tup[4] for tup in sampled_arr]
+        unknown_scale_list = [tup[5] for tup in sampled_arr]
+
         arr = np.stack(arr_list, axis=0)
         pad_arr = np.stack(pad_list, axis=0)
         date_arr = np.stack(date_list, axis=0)
         scale_arr = np.stack(scale_list, axis=0)
+        known_scale_arr = np.stack(known_scale_list, axis=0)
+        unknown_scale_arr = np.stack(unknown_scale_list, axis=0)
+
         id_arr = arr[:,-1:,0]
         
-        return arr, pad_arr, id_arr, date_arr, scale_arr
+        return arr, pad_arr, id_arr, date_arr, scale_arr, known_scale_arr, unknown_scale_arr
     
     def sort_dataset(self, data):
         """
         sort pandas dataframe by provided col list & order
         """
         if len(self.sort_col_list) > 0:
             data = data.sort_values(by=self.sort_col_list, ascending=True)
@@ -327,23 +408,26 @@
         
         keys_dict, wts_dict = self.get_keys(data)
         self.train_test_batch_size = int(self.batch*len(keys_dict))
        
         while True:
             sample_id = self.select_ids(keys_dict, wts_dict)
             df = data.query("{}==@sample_id".format(self.id_col))
-            arr, pad_arr, scale_arr = self.select_arrs(df, mode)
+            arr, pad_arr, scale_arr, known_scale_arr, unknown_scale_arr = self.select_arrs(df, mode)
             
             #print("data gen: ", scale_arr.shape)
             # -- done for @tf.function retracing reason. May revisit later
-            #valid_indices = np.where(np.count_nonzero(arr[:,:self.window_len-self.fh,self.target_index].astype(np.float32)>0,axis=1)>=self.min_nz)
-            #arr = arr[valid_indices]
-            #pad_arr = pad_arr[valid_indices]
-            
-            model_in, model_out, scale, weights  = self.preprocess(arr, pad_arr, scale_arr)
+            valid_indices = np.where(np.count_nonzero(arr[:,:self.window_len-self.fh,self.target_index].astype(np.float32)>0,axis=1)>=self.min_nz)
+            arr = arr[valid_indices]
+            pad_arr = pad_arr[valid_indices]
+            scale_arr = scale_arr[valid_indices]
+            known_scale_arr = known_scale_arr[valid_indices]
+            unknown_scale_arr = unknown_scale_arr[valid_indices]
+
+            model_in, model_out, scale, weights  = self.preprocess(arr, pad_arr, scale_arr, known_scale_arr, unknown_scale_arr, mode)
             yield model_in.astype(str), model_out.astype(np.float32), scale.astype(np.float32), weights.astype(np.float32)
             
             
     def vocab_list(self, data):
         """
         Function to generate default embedding dimensions for categorical vars as 3rd root of no. of unique values.
         
@@ -367,99 +451,93 @@
                         emb_dim = max(m.ceil(len(col_unique_vals)**0.33),2)       
                         cols_val_list.append(col_unique_vals)
                         cols_dim_list.append(emb_dim)
                     vocab_dict[k] = [d[0], cols_val_list, cols_dim_list]
                            
         return vocab_dict
     
-    def preprocess(self, sample_arr, pad_arr, scale_arr):
+    def preprocess(self, sample_arr, pad_arr, scale_arr, known_scale_arr, unknown_scale_arr, mode):
         """
         Preprocess_samples Tensorflow Ops & outputs resp.
         """
         sequence_len = int(self.window_len)
         max_input_len = int(self.window_len - self.fh)
         
         sid =  sample_arr[..., [self.id_index]].astype(str)
         target = sample_arr[..., [self.target_index]].astype(float)
         
         # target outlier correction
-        SU = np.maximum(3.0*np.quantile(target[:,:max_input_len,:], q=0.97, axis=1, keepdims=True), 0)
-        SL = np.minimum(np.quantile(target[:,:max_input_len,:], q=0.01, axis=1, keepdims=True), 0)
-        target = np.clip(target, a_min=SL, a_max=SU)
+        #SU = np.maximum(3.0*np.quantile(target[:,:max_input_len,:], q=0.97, axis=1, keepdims=True), 0)
+        #SL = np.minimum(np.quantile(target[:,:max_input_len,:], q=0.01, axis=1, keepdims=True), 0)
+        #target = np.clip(target, a_min=SL, a_max=SU)
         
         # scale target : target/target_mean
         if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
-            #target_nz_count = np.maximum(np.count_nonzero(np.abs(target[:,:max_input_len,:]), axis=1).reshape(-1,1,1), 1.0)
-            #target_sum = np.sum(np.abs(target[:,:max_input_len,:]), axis=1, keepdims=True)
-            #target_nz_mean = np.divide(target_sum, target_nz_count) + 1.0
             target_nz_mean = scale_arr.reshape(-1,1,1)
             target_scaled = np.divide(target, target_nz_mean)
         elif self.scaling_method == 'standard_scaling':
-            #target_mean = np.mean(target[:,:max_input_len,:], axis=1, keepdims=True)
-            #target_stddev = np.maximum(np.std(target[:,:max_input_len,:], axis=1, keepdims=True), 0.001)
             target_mean = scale_arr[:,0].reshape(-1,1,1)
             target_stddev = scale_arr[:,1].reshape(-1,1,1)
             target_scaled = np.divide(np.subtract(target, target_mean), target_stddev)
             target_scaled = np.nan_to_num(target_scaled) # correct where stddev is 0
+        elif self.scaling_method == 'log_scaling':
+            target_nz_mean = scale_arr.reshape(-1,1,1)
+            target_scaled = np.log1p(target)
        
         # build model_in array  
         model_in = np.concatenate((sid, target_scaled), axis=-1)
         model_out = target_scaled[:,-self.fh:,:]
         
+        if mode == 'infer':
+            model_in[:,-self.fh:,1] = 0
+        
         # make model_in target values zero for the fh
         #target_scaled[:,-self.fh:, :] = 0
         #model_in = np.concatenate((sid, target_scaled), axis=-1)
         
         if len(self.static_num_indices) > 0:
             static_num = sample_arr[..., self.static_num_indices].astype(float)
-            # scale
-            #static_nz_count = np.maximum(np.count_nonzero(np.abs(static_num), axis=1).reshape(-1,1,len(self.static_num_indices)), 1.0)
-            #static_sum = np.sum(np.abs(static_num), axis=1, keepdims=True)
-            #static_nz_mean = np.divide(static_sum, static_nz_count) + 1.0
-            #static_num = np.divide(static_num, static_nz_mean)
-            # merge
             model_in = np.concatenate((model_in, static_num), axis=-1)
             
         if len(self.static_cat_indices) > 0:
             static_cat = sample_arr[..., self.static_cat_indices].astype(str)
-            # merge
             model_in = np.concatenate((model_in, static_cat), axis=-1)
 
         if len(self.temporal_known_num_indices) > 0:
             known_num = sample_arr[..., self.temporal_known_num_indices].astype(float)
             # scale
             if self.scaling_method == 'mean_scaling':
-                known_nz_count = np.maximum(np.count_nonzero(np.abs(known_num), axis=1).reshape(-1,1,len(self.temporal_known_num_indices)), 1.0)
-                known_sum = np.sum(np.abs(known_num), axis=1, keepdims=True)
-                known_nz_mean = np.divide(known_sum, known_nz_count) + 1.0
-                known_num = np.divide(known_num, known_nz_mean)
+                known_scale_arr = known_scale_arr.reshape(-1,1,len(self.temporal_known_num_indices))
+                known_num = np.divide(known_num, known_scale_arr)
             elif self.scaling_method == 'standard_scaling':
-                known_mean = np.mean(known_num, axis=1, keepdims=True)
-                known_stddev = np.maximum(np.std(known_num, axis=1, keepdims=True), 0.001)
+                known_mean = known_scale_arr[:,0,:].reshape(-1,1,len(self.temporal_known_num_indices))
+                known_stddev = known_scale_arr[:,1,:].reshape(-1,1,len(self.temporal_known_num_indices))
                 known_num = np.divide(np.subtract(known_num, known_mean), known_stddev)
                 known_num = np.nan_to_num(known_num)
+            elif self.scaling_method == 'log_scaling':
+                known_num = np.log1p(known_num)
             elif self.scaling_method == 'no_scaling':
                 pass
             
             # merge
             model_in = np.concatenate((model_in, known_num), axis=-1)
 
         if len(self.temporal_unknown_num_indices) > 0:
             unknown_num = sample_arr[..., self.temporal_unknown_num_indices].astype(float)
             # scale
             if self.scaling_method == 'mean_scaling':
-                unknown_nz_count = np.maximum(np.count_nonzero(np.abs(unknown_num[:,:max_input_len,:]), axis=1).reshape(-1,1,len(self.temporal_unknown_num_indices)), 1.0)
-                unknown_sum = np.sum(np.abs(unknown_num[:,:max_input_len,:]), axis=1, keepdims=True)
-                unknown_nz_mean = np.divide(unknown_sum, unknown_nz_count) + 1.0
-                unknown_num = np.divide(unknown_num, unknown_nz_mean)
+                unknown_scale_arr = unknown_scale_arr.reshape(-1,1,len(self.temporal_unknown_num_indices))
+                unknown_num = np.divide(unknown_num, unknown_scale_arr)
             elif self.scaling_method == 'standard_scaling':
-                unknown_mean = np.mean(unknown_num[:,:max_input_len,:], axis=1, keepdims=True)
-                unknown_stddev = np.maximum(np.std(unknown_num[:,:max_input_len,:], axis=1, keepdims=True), 0.001)
+                unknown_mean = unknown_scale_arr[:,0,:].reshape(-1,1,len(self.temporal_unknown_num_indices))
+                unknown_stddev = unknown_scale_arr[:,1,:].reshape(-1,1,len(self.temporal_unknown_num_indices))
                 unknown_num = np.divide(np.subtract(unknown_num, unknown_mean), unknown_stddev)
                 unknown_num = np.nan_to_num(unknown_num)
+            elif self.scaling_method == 'log_scaling':
+                unknown_num = np.log1p(unknown_num)
             elif self.scaling_method == 'no_scaling':
                 pass
             
             # merge
             model_in = np.concatenate((model_in, unknown_num), axis=-1)
    
         if len(self.temporal_known_cat_indices) > 0:
@@ -472,24 +550,24 @@
             # merge
             model_in = np.concatenate((model_in, unknown_cat), axis=-1)
             
         rel_age = np.broadcast_to((np.arange(0,sequence_len,1)/sequence_len).reshape(-1,1), target.shape)
         model_in = np.concatenate((model_in, rel_age), axis=-1) 
         
         # scale
-        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling') or (self.scaling_method == 'log_scaling'):
             scale_in = np.broadcast_to(target_nz_mean, target.shape)
         elif self.scaling_method == 'standard_scaling':
             scale_mean = np.broadcast_to(target_mean, target.shape)
             scale_std = np.broadcast_to(target_stddev, target.shape)
             scale_in = np.concatenate((scale_mean, scale_std), axis=-1)
             
         model_in = np.concatenate((model_in, scale_in), axis=-1)
         
-        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling') or (self.scaling_method == 'log_scaling'):
             scale_out = np.broadcast_to(target_nz_mean, model_out.shape)
         elif self.scaling_method == 'standard_scaling':
             scale_mean_out = np.broadcast_to(target_mean, model_out.shape)
             scale_std_out = np.broadcast_to(target_stddev, model_out.shape)
             scale_out = np.concatenate((scale_mean_out, scale_std_out), axis=-1)
             
         mask_list = []
@@ -501,22 +579,20 @@
             mask_list.append(mask)
 
         # mask & relative age
         mask = np.vstack(mask_list).reshape(-1,sequence_len,1)
         model_in = np.concatenate((model_in, mask), axis=-1)
 
         # sample weights
-        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling') or (self.scaling_method == 'log_scaling'):
             weights = np.around(np.log10(np.squeeze(target_nz_mean) + 10),2) #/np.quantile(np.squeeze(target_nz_mean), q=0.8)
         elif self.scaling_method == 'standard_scaling':
             weights = np.around(np.log10(np.squeeze(target_mean) + 10),2)
         weights = np.clip(weights, a_min=1.0, a_max=2.0)
         weights = weights.reshape(-1,1)
-        #weights = np.expand_dims(weights.reshape(-1,1), axis=-1)
-        #weights = np.tile(weights, [1,sequence_len,1])
         
         return model_in, model_out, scale_out, weights
     
     def split_train_test(self, data):
         train_data = data[data[self.time_index_col]<=self.train_till].reset_index(drop=True)
         if self.datetime_format is not None:
             delta = max(self.train_test_timedelta, self.window_len) 
@@ -572,23 +648,23 @@
         null_status, null_cols = self.check_null(data)
         if null_status:
             print("NaN column(s): ", null_cols)
             raise ValueError("Column(s) with NaN detected!")
             
         # sort & filter to recent context
         data = self.sort_dataset(data)
-        data = data[data[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
+        #data = data[data[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
 
-        arr, pad_arr, id_arr, date_arr, scale_arr = self.select_all_arrs(data)
+        arr, pad_arr, id_arr, date_arr, scale_arr, known_scale_arr, unknown_scale_arr = self.select_all_arrs(data)
         
-        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr, scale_arr)
+        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr, scale_arr, known_scale_arr, unknown_scale_arr, mode='infer')
         input_tensor = tf.convert_to_tensor(model_in.astype(str), dtype=tf.string)
         
         # for evaluation
-        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling'):
+        if (self.scaling_method == 'mean_scaling') or (self.scaling_method == 'no_scaling') or (self.scaling_method == 'log_scaling'):
             actuals_arr = model_out*scale
         elif self.scaling_method == 'standard_scaling':
             actuals_arr = model_out*scale[:,:,1:2] + scale[:,:,0:1]
             
         if len(self.static_cat_col_list)>0:
             stat_arr_list = []
             for col, i in zip(self.static_cat_col_list, self.static_cat_indices):
@@ -627,23 +703,23 @@
         null_status, null_cols = self.check_null(data)
         if null_status:
             print("NaN column(s): ", null_cols)
             raise ValueError("Column(s) with NaN detected!")
             
         # sort & filter to recent context
         data = self.sort_dataset(data)
-        data = data[data[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
+        #data = data[data[self.time_index_col]<=self.future_till].groupby(self.id_col).apply(lambda x: x[-self.window_len:]).reset_index(drop=True)
         
         # mask out columns in ignore_cols for baseline forecast
         for col,val in zip(ignore_cols, ignore_pad_values):
             data[col] = np.where(data[self.time_index_col]>self.history_till, val, data[col])
         
         arr, pad_arr, id_arr, date_arr, scale_arr = self.select_all_arrs(data)
      
-        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr, scale_arr)
+        model_in, model_out, scale, _ = self.preprocess(arr, pad_arr, scale_arr, mode='infer')
         input_tensor = tf.convert_to_tensor(model_in.astype(str), dtype=tf.string)
         
         return [input_tensor, scale, id_arr, date_arr]
     
     def acf(self, series):
         # https://stackoverflow.com/questions/43344406/is-there-a-bokeh-version-of-pandas-autocorrelation-plot-method
         n = len(series)
@@ -839,12 +915,9 @@
             layouts.append(layout)
             i += 1
         
         supergrid = gridplot(layouts, ncols=1)
         show(supergrid)
 
 
-# In[ ]:
-
-
```

### Comparing `fmldk-1.1.8/tft/tft_losses.py` & `fmldk-1.1.9/sage/sage_losses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[1]:
-
 
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import pprint
 
 
-# In[2]:
-
-
 # NLL Functions
 
 # Negbin Loss
 @tf.function(experimental_relax_shapes=True)
 def Negbin_loss(actual, mu, alpha):
     '''
     Negative Binomial Sample
@@ -27,15 +22,16 @@
     mu: [batch, fh]
     alpha: [batch, fh]
     maximize log l_{nb} = log Gamma(z + 1/alpha) - log Gamma(z + 1) - log Gamma(1 / alpha)
                           - 1 / alpha * log (1 + alpha * mu) + z * log (alpha * mu / (1 + alpha * mu))
     minimize loss = - log l_{nb}
     Note: torch.lgamma: log Gamma function
     '''
-    likelihood = tf.math.lgamma(actual + 1.0/alpha) - tf.math.lgamma(actual + 1) - tf.math.lgamma(1.0/alpha)                 - 1.0/alpha*tf.math.log(1 + alpha*mu) + actual*tf.math.log(alpha*mu/(1 + alpha * mu))
+    likelihood = tf.math.lgamma(actual + 1.0/alpha) - tf.math.lgamma(actual + 1) - tf.math.lgamma(1.0/alpha) \
+                - 1.0/alpha*tf.math.log(1 + alpha*mu) + actual*tf.math.log(alpha*mu/(1 + alpha * mu))
     nll = -1.0*likelihood
     return tf.reduce_mean(nll)
   
 # Normal Loss
 @tf.function(experimental_relax_shapes=True)
 def Normal_loss(actual, mu, std):
     dist = tfd.Normal(mu,std)
@@ -70,15 +66,15 @@
     b = b
     k = (actual - a)/b
     likelihood = -tf.math.log(b) - k - tf.math.exp(-k)
     nll = -1.0*likelihood
     return tf.reduce_mean(nll)
 
 
-# In[3]:
+# In[ ]:
 
 
 # Keras Custom Loss Subclasses -- Quantile Loss, RMSSE, RMSE, Negbin_NLL_Loss, Normal_NLL_Loss, Poisson_NLL_Loss, Gumbel_NLL_Loss
 
 class QuantileLoss(tf.keras.losses.Loss):
     def __init__(self, quantiles = [0.50,0.60,0.65], ** kwargs): 
         self.quantiles = quantiles 
@@ -92,14 +88,33 @@
             error = tf.subtract(true, pred[:,:,i])
             losses += tf.maximum(q*error, (q-1)*error) 
         return tf.reduce_mean(losses) 
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config, "quantiles": self.quantiles}
+
+class JointQuantileLoss(tf.keras.losses.Loss):
+    def __init__(self, quantiles = [0.1,0.5,0.9], ** kwargs): 
+        self.quantiles = quantiles 
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, predictions):
+        pred = tf.cast(predictions, tf.float32)
+        true = tf.cast(tf.squeeze(actuals), tf.float32)
+        losses = tf.cast(tf.zeros_like(true), tf.float32)
+        for i,q in enumerate(self.quantiles):
+            error1 = tf.subtract(true, pred[:,:,0])
+            error2 = tf.subtract(pred[:,:,0], true)
+            losses += q*(tf.maximum(error1,0)) + (1-q)*(tf.maximum(error2,0)) 
+        return tf.reduce_mean(losses) 
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config, "quantiles": self.quantiles}
       
 class QuantileLoss_Weighted(tf.keras.losses.Loss):
     def __init__(self, quantiles = [0.50,0.60,0.65], ** kwargs): 
         self.quantiles = quantiles 
         super().__init__(** kwargs)
     
     def call(self, actuals, output):
@@ -139,14 +154,17 @@
         y_pred = tf.cast(predictions, tf.float32)
         #y_true = tf.cast(tf.squeeze(actuals), tf.float32)
         y_true = tf.cast(tf.reshape(actuals, [-1,seq_len]), tf.float32)
         
         losses = tf.cast(tf.zeros_like(y_true), tf.float32)
         for i,q in enumerate(self.quantiles):
             losses += self.compute_quantile_loss(y_true, y_pred[:,:,i], q)*self.quantile_weights[i]
+        
+        losses = tf.reduce_sum(losses, axis=-1)
+        
         return tf.reduce_mean(wts*losses)
     
     def compute_quantile_loss(self, y_true, y_pred, q):
         #under_bias = q * tf.maximum(y_true - y_pred, 0)
         #over_bias = (1.0 - q) * tf.maximum(y_pred - y_true, 0)
         #qt_loss = 2 * (under_bias + over_bias)
         error = tf.subtract(y_true, y_pred)
@@ -172,21 +190,20 @@
 class RMSSELoss(tf.keras.losses.Loss):
     def __init__(self, sl, fh, ** kwargs):
         self.sl = sl
         self.fh = fh  
         super().__init__(** kwargs)
     
     def call(self, actuals, predictions):
-        seq_len_pred = tf.shape(predictions)[1]
-        seq_len_act = tf.shape(actuals)[1]
-
-        # pred = tf.cast(tf.squeeze(predictions), tf.float32)
-        pred = tf.cast(tf.reshape(predictions, [-1, seq_len_pred]), tf.float32)
-        # true = tf.cast(tf.squeeze(actuals), tf.float32)
-        true = tf.cast(tf.reshape(actuals, [-1, seq_len_act]), tf.float32)
+        seq_len = tf.shape(predictions)[1]
+        
+        #pred = tf.cast(tf.squeeze(predictions), tf.float32)
+        pred = tf.cast(tf.reshape(predictions, [-1, seq_len]), tf.float32)
+        #true = tf.cast(tf.squeeze(actuals), tf.float32)
+        true = tf.cast(tf.reshape(actuals, [-1,seq_len]), tf.float32)
         
         true_fh = true[:,-self.fh:]
         true_in = true[:,1:self.sl]
         true_in_lag = true[:,0:self.sl-1]
         error = tf.reduce_sum(tf.math.square(tf.abs(true_fh - pred)), axis=1, keepdims=True)/tf.cast(self.fh, tf.float32)
         scale = tf.reduce_sum(tf.math.square(tf.abs(true_in - true_in_lag)), axis=1, keepdims=True)/tf.cast((self.sl-1), tf.float32)
         #weights = tf.reduce_sum(true[:,:self.sl], axis=1, keepdims=True)/tf.reduce_sum(true[:,:self.sl])
@@ -252,14 +269,42 @@
         else:
             loss = self.loss_fn(true, output)
         return loss
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config}
+    
+class SMAPE(tf.keras.losses.Loss):
+    def __init__(self, epsilon=0.1, sample_weights=False, ** kwargs):
+        self.sample_weights = sample_weights
+        self.eps = epsilon
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, pred):
+        if self.sample_weights:
+            output, wts = pred[0], pred[1]
+            wts = tf.reshape(wts, [-1,1]) 
+        else:
+            wts = 1.0
+            output = pred
+        seq_len = tf.shape(output)[1]    
+        
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        true = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+        
+        summ = tf.maximum(tf.abs(true) + tf.abs(output) + self.eps, 0.5 + self.eps)
+        smape = tf.abs(true - output)/summ*2.0
+        wtd_smape = wts*tf.math.reduce_mean(smape, axis=1, keepdims=True)
+        
+        return tf.math.reduce_mean(wtd_smape)
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config}
       
         
 class Negbin_NLL_Loss(tf.keras.losses.Loss):
     def __init__(self, sample_weights=False, ** kwargs):
         self.sample_weights = sample_weights
         super().__init__(** kwargs)
     
@@ -299,15 +344,87 @@
         nll = Normal_loss(true, mu, alpha)
         return nll
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config}
       
-        
+class Tweedie_Loss(tf.keras.losses.Loss):
+    def __init__(self, p=1.5, log_scale=False, sample_weights=False, ** kwargs):
+        self.p = p
+        self.log_scale = log_scale
+        self.sample_weights = sample_weights
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, pred):
+        if self.sample_weights:
+            output, wts = pred[0], pred[1]
+            wts = tf.reshape(wts, [-1,]) 
+        else:
+            wts = 1.0
+            output = pred
+
+        seq_len = tf.shape(output)[1] 
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        actuals = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+
+        if self.log_scale:
+          # unexp outputs & actuals (undo log1p transform)
+          output = tf.math.expm1(output)
+          actuals = tf.math.expm1(actuals)
+
+        # apply min value threshold to o/p to prevent nan
+        eps = 1e-8
+        output = tf.math.maximum(output, eps)
+
+        loss = (-actuals * tf.math.pow(output, (1 - self.p)) / (1 - self.p) + tf.math.pow(output, (2 - self.p)) / (2 - self.p))
+        loss = tf.math.reduce_mean(loss, axis=-1)
+
+        return tf.math.reduce_mean(wts * loss)
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config} 
+
+class Poisson_Loss(tf.keras.losses.Loss):
+    def __init__(self, log_scale=False, sample_weights=False, ** kwargs):
+        self.log_scale = log_scale
+        self.sample_weights = sample_weights
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, pred):
+        if self.sample_weights:
+            output, wts = pred[0], pred[1]
+            wts = tf.reshape(wts, [-1,]) 
+        else:
+            wts = 1.0
+            output = pred
+
+        seq_len = tf.shape(output)[1] 
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        actuals = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+
+        if self.log_scale:
+          # unexp outputs & actuals (undo log1p transform)
+          output = tf.math.expm1(output)
+          actuals = tf.math.expm1(actuals)
+
+        # apply min value threshold to o/p to prevent nan
+        eps = 1e-8
+        output = tf.math.maximum(output, eps)
+        loss = output - actuals * tf.math.log(output)
+        loss = tf.math.reduce_mean(loss, axis=-1)
+
+        return tf.math.reduce_mean(wts * loss)
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config} 
+
+
 class Poisson_NLL_Loss(tf.keras.losses.Loss):
     def __init__(self, sample_weights=False, ** kwargs):
         self.sample_weights = sample_weights
         super().__init__(** kwargs)
     
     def call(self, actuals, pred):
         if self.sample_weights:
@@ -346,28 +463,20 @@
         return nll
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config}      
 
 
-# In[12]:
-
-
 supported_losses = {'RMSE': ['loss_type: Point', 'Usage: RMSE(sample_weights=False)'],
                     'Huber': ['loss_type: Point', 'Usage: Huber(delta=1.0, sample_weights=False)'],
                     'Quantile': ['loss_type: Quantile', 'Usage: QuantileLoss_v2(quantiles=[0.5], sample_weights=False)'], 
                     'Normal': ['loss_type: Normal', 'Usage: Normal_NLL_Loss(sample_weights=False)'], 
-                    'Poisson': ['loss_type: Poisson', 'Usage: Poisson_NLL_Loss(sample_weights=False)'],
-                    'Negbin': ['loss_type: Negbin', 'Usage: Negbin_NLL_Loss(sample_weights=False)']
+                    'Poisson': ['loss_type: Poisson', 'Usage: Poisson_Loss(log_scale=False, sample_weights=False)'],
+                    'Negbin': ['loss_type: Negbin', 'Usage: Negbin_NLL_Loss(sample_weights=False)'],
+                    'Tweedie': ['loss_type: Tweedie', 'Usage: Tweedie_Loss(p=1.5, log_scale=False, sample_weights=False)']
                    }
 
 #print("Supported Loss Functions & Typical Usage:")
 #print("-----------------------------------------")
 #pprint.pprint(supported_losses)
 
-
-# In[ ]:
-
-
-
-
```

### Comparing `fmldk-1.1.8/tft/tft_losses_bkp.py` & `fmldk-1.1.9/tft/tft_losses.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 import numpy as np
 import math as m
 import tensorflow as tf
 import tensorflow_probability as tfp
 tfd = tfp.distributions
 import pprint
 
+
+# NLL Functions
+
 # Negbin Loss
 @tf.function(experimental_relax_shapes=True)
 def Negbin_loss(actual, mu, alpha):
     '''
     Negative Binomial Sample
     Args:
     actual: [batch, fh]
     mu: [batch, fh]
     alpha: [batch, fh]
     maximize log l_{nb} = log Gamma(z + 1/alpha) - log Gamma(z + 1) - log Gamma(1 / alpha)
                           - 1 / alpha * log (1 + alpha * mu) + z * log (alpha * mu / (1 + alpha * mu))
     minimize loss = - log l_{nb}
     Note: torch.lgamma: log Gamma function
     '''
-    likelihood = tf.math.lgamma(actual + 1.0/alpha) - tf.math.lgamma(actual + 1) - tf.math.lgamma(1.0/alpha)                 - 1.0/alpha*tf.math.log(1 + alpha*mu) + actual*tf.math.log(alpha*mu/(1 + alpha * mu))
+    likelihood = tf.math.lgamma(actual + 1.0/alpha) - tf.math.lgamma(actual + 1) - tf.math.lgamma(1.0/alpha) \
+                - 1.0/alpha*tf.math.log(1 + alpha*mu) + actual*tf.math.log(alpha*mu/(1 + alpha * mu))
     nll = -1.0*likelihood
     return tf.reduce_mean(nll)
   
 # Normal Loss
 @tf.function(experimental_relax_shapes=True)
 def Normal_loss(actual, mu, std):
     dist = tfd.Normal(mu,std)
@@ -62,14 +66,17 @@
     b = b
     k = (actual - a)/b
     likelihood = -tf.math.log(b) - k - tf.math.exp(-k)
     nll = -1.0*likelihood
     return tf.reduce_mean(nll)
 
 
+# In[ ]:
+
+
 # Keras Custom Loss Subclasses -- Quantile Loss, RMSSE, RMSE, Negbin_NLL_Loss, Normal_NLL_Loss, Poisson_NLL_Loss, Gumbel_NLL_Loss
 
 class QuantileLoss(tf.keras.losses.Loss):
     def __init__(self, quantiles = [0.50,0.60,0.65], ** kwargs): 
         self.quantiles = quantiles 
         super().__init__(** kwargs)
     
@@ -81,14 +88,33 @@
             error = tf.subtract(true, pred[:,:,i])
             losses += tf.maximum(q*error, (q-1)*error) 
         return tf.reduce_mean(losses) 
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config, "quantiles": self.quantiles}
+
+class JointQuantileLoss(tf.keras.losses.Loss):
+    def __init__(self, quantiles = [0.1,0.5,0.9], ** kwargs): 
+        self.quantiles = quantiles 
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, predictions):
+        pred = tf.cast(predictions, tf.float32)
+        true = tf.cast(tf.squeeze(actuals), tf.float32)
+        losses = tf.cast(tf.zeros_like(true), tf.float32)
+        for i,q in enumerate(self.quantiles):
+            error1 = tf.subtract(true, pred[:,:,0])
+            error2 = tf.subtract(pred[:,:,0], true)
+            losses += q*(tf.maximum(error1,0)) + (1-q)*(tf.maximum(error2,0)) 
+        return tf.reduce_mean(losses) 
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config, "quantiles": self.quantiles}
       
 class QuantileLoss_Weighted(tf.keras.losses.Loss):
     def __init__(self, quantiles = [0.50,0.60,0.65], ** kwargs): 
         self.quantiles = quantiles 
         super().__init__(** kwargs)
     
     def call(self, actuals, output):
@@ -118,19 +144,27 @@
     def call(self, actuals, output):
         if self.sample_weights:
             predictions, wts = output[0], output[1]
             wts = tf.reshape(wts, [-1,1]) 
         else:
             wts = 1.0
             predictions = output
+        
+        seq_len = tf.shape(predictions)[1]
+        
         y_pred = tf.cast(predictions, tf.float32)
-        y_true = tf.cast(tf.squeeze(actuals), tf.float32)
+        #y_true = tf.cast(tf.squeeze(actuals), tf.float32)
+        y_true = tf.cast(tf.reshape(actuals, [-1,seq_len]), tf.float32)
+        
         losses = tf.cast(tf.zeros_like(y_true), tf.float32)
         for i,q in enumerate(self.quantiles):
             losses += self.compute_quantile_loss(y_true, y_pred[:,:,i], q)*self.quantile_weights[i]
+        
+        losses = tf.reduce_sum(losses, axis=-1)
+        
         return tf.reduce_mean(wts*losses)
     
     def compute_quantile_loss(self, y_true, y_pred, q):
         #under_bias = q * tf.maximum(y_true - y_pred, 0)
         #over_bias = (1.0 - q) * tf.maximum(y_pred - y_true, 0)
         #qt_loss = 2 * (under_bias + over_bias)
         error = tf.subtract(y_true, y_pred)
@@ -156,16 +190,21 @@
 class RMSSELoss(tf.keras.losses.Loss):
     def __init__(self, sl, fh, ** kwargs):
         self.sl = sl
         self.fh = fh  
         super().__init__(** kwargs)
     
     def call(self, actuals, predictions):
-        pred = tf.cast(tf.squeeze(predictions), tf.float32)
-        true = tf.cast(tf.squeeze(actuals), tf.float32)
+        seq_len = tf.shape(predictions)[1]
+        
+        #pred = tf.cast(tf.squeeze(predictions), tf.float32)
+        pred = tf.cast(tf.reshape(predictions, [-1, seq_len]), tf.float32)
+        #true = tf.cast(tf.squeeze(actuals), tf.float32)
+        true = tf.cast(tf.reshape(actuals, [-1,seq_len]), tf.float32)
+        
         true_fh = true[:,-self.fh:]
         true_in = true[:,1:self.sl]
         true_in_lag = true[:,0:self.sl-1]
         error = tf.reduce_sum(tf.math.square(tf.abs(true_fh - pred)), axis=1, keepdims=True)/tf.cast(self.fh, tf.float32)
         scale = tf.reduce_sum(tf.math.square(tf.abs(true_in - true_in_lag)), axis=1, keepdims=True)/tf.cast((self.sl-1), tf.float32)
         #weights = tf.reduce_sum(true[:,:self.sl], axis=1, keepdims=True)/tf.reduce_sum(true[:,:self.sl])
         rmsse = tf.math.sqrt(error/scale)
@@ -184,16 +223,21 @@
     def call(self, actuals, pred):
         if self.sample_weights:
             output, wts = pred[0], pred[1]
             wts = tf.reshape(wts, [-1,1]) 
         else:
             wts = 1.0
             output = pred
-        output = tf.cast(tf.squeeze(output), tf.float32)
-        true = tf.cast(tf.squeeze(actuals), tf.float32)
+            
+        seq_len = tf.shape(output)[1]    
+        #output = tf.cast(tf.squeeze(output), tf.float32)
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        #true = tf.cast(tf.squeeze(actuals), tf.float32)
+        true = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+        
         error = wts*tf.reduce_mean(tf.math.square(tf.abs(true - output)), axis=1, keepdims=True)
         rmse = tf.math.sqrt(error)
         return tf.reduce_mean(rmse)
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config}
@@ -209,25 +253,58 @@
     def call(self, actuals, pred):
         if self.sample_weights:
             output, wts = pred[0], pred[1]
             wts = tf.reshape(wts, [-1,1]) 
         else:
             wts = 1.0
             output = pred
-        output = tf.cast(tf.squeeze(output), tf.float32)
-        true = tf.cast(tf.squeeze(actuals), tf.float32)
+        seq_len = tf.shape(output)[1]    
+        
+        #output = tf.cast(tf.squeeze(output), tf.float32)
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        #true = tf.cast(tf.squeeze(actuals), tf.float32)
+        true = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+        
         if self.sample_weights:
             loss = self.loss_fn.__call__(true, output, wts)
         else:
             loss = self.loss_fn(true, output)
         return loss
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config}
+    
+class SMAPE(tf.keras.losses.Loss):
+    def __init__(self, epsilon=0.1, sample_weights=False, ** kwargs):
+        self.sample_weights = sample_weights
+        self.eps = epsilon
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, pred):
+        if self.sample_weights:
+            output, wts = pred[0], pred[1]
+            wts = tf.reshape(wts, [-1,1]) 
+        else:
+            wts = 1.0
+            output = pred
+        seq_len = tf.shape(output)[1]    
+        
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        true = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+        
+        summ = tf.maximum(tf.abs(true) + tf.abs(output) + self.eps, 0.5 + self.eps)
+        smape = tf.abs(true - output)/summ*2.0
+        wtd_smape = wts*tf.math.reduce_mean(smape, axis=1, keepdims=True)
+        
+        return tf.math.reduce_mean(wtd_smape)
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config}
       
         
 class Negbin_NLL_Loss(tf.keras.losses.Loss):
     def __init__(self, sample_weights=False, ** kwargs):
         self.sample_weights = sample_weights
         super().__init__(** kwargs)
     
@@ -267,15 +344,87 @@
         nll = Normal_loss(true, mu, alpha)
         return nll
     
     def get_config( self): 
         base_config = super().get_config() 
         return {** base_config}
       
-        
+class Tweedie_Loss(tf.keras.losses.Loss):
+    def __init__(self, p=1.5, log_scale=False, sample_weights=False, ** kwargs):
+        self.p = p
+        self.log_scale = log_scale
+        self.sample_weights = sample_weights
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, pred):
+        if self.sample_weights:
+            output, wts = pred[0], pred[1]
+            wts = tf.reshape(wts, [-1,]) 
+        else:
+            wts = 1.0
+            output = pred
+
+        seq_len = tf.shape(output)[1] 
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        actuals = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+
+        if self.log_scale:
+          # unexp outputs & actuals (undo log1p transform)
+          output = tf.math.expm1(output)
+          actuals = tf.math.expm1(actuals)
+
+        # apply min value threshold to o/p to prevent nan
+        eps = 1e-8
+        output = tf.math.maximum(output, eps)
+
+        loss = (-actuals * tf.math.pow(output, (1 - self.p)) / (1 - self.p) + tf.math.pow(output, (2 - self.p)) / (2 - self.p))
+        loss = tf.math.reduce_mean(loss, axis=-1)
+
+        return tf.math.reduce_mean(wts * loss)
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config} 
+
+class Poisson_Loss(tf.keras.losses.Loss):
+    def __init__(self, log_scale=False, sample_weights=False, ** kwargs):
+        self.log_scale = log_scale
+        self.sample_weights = sample_weights
+        super().__init__(** kwargs)
+    
+    def call(self, actuals, pred):
+        if self.sample_weights:
+            output, wts = pred[0], pred[1]
+            wts = tf.reshape(wts, [-1,]) 
+        else:
+            wts = 1.0
+            output = pred
+
+        seq_len = tf.shape(output)[1] 
+        output = tf.cast(tf.reshape(output, [-1,seq_len]), tf.float32)
+        actuals = tf.cast(tf.reshape(actuals,[-1,seq_len]), tf.float32)
+
+        if self.log_scale:
+          # unexp outputs & actuals (undo log1p transform)
+          output = tf.math.expm1(output)
+          actuals = tf.math.expm1(actuals)
+
+        # apply min value threshold to o/p to prevent nan
+        eps = 1e-8
+        output = tf.math.maximum(output, eps)
+        loss = output - actuals * tf.math.log(output)
+        loss = tf.math.reduce_mean(loss, axis=-1)
+
+        return tf.math.reduce_mean(wts * loss)
+    
+    def get_config( self): 
+        base_config = super().get_config() 
+        return {** base_config} 
+
+
 class Poisson_NLL_Loss(tf.keras.losses.Loss):
     def __init__(self, sample_weights=False, ** kwargs):
         self.sample_weights = sample_weights
         super().__init__(** kwargs)
     
     def call(self, actuals, pred):
         if self.sample_weights:
@@ -318,18 +467,16 @@
         return {** base_config}      
 
 
 supported_losses = {'RMSE': ['loss_type: Point', 'Usage: RMSE(sample_weights=False)'],
                     'Huber': ['loss_type: Point', 'Usage: Huber(delta=1.0, sample_weights=False)'],
                     'Quantile': ['loss_type: Quantile', 'Usage: QuantileLoss_v2(quantiles=[0.5], sample_weights=False)'], 
                     'Normal': ['loss_type: Normal', 'Usage: Normal_NLL_Loss(sample_weights=False)'], 
-                    'Poisson': ['loss_type: Poisson', 'Usage: Poisson_NLL_Loss(sample_weights=False)'],
-                    'Negbin': ['loss_type: Negbin', 'Usage: Negbin_NLL_Loss(sample_weights=False)']
+                    'Poisson': ['loss_type: Poisson', 'Usage: Poisson_Loss(log_scale=False, sample_weights=False)'],
+                    'Negbin': ['loss_type: Negbin', 'Usage: Negbin_NLL_Loss(sample_weights=False)'],
+                    'Tweedie': ['loss_type: Tweedie', 'Usage: Tweedie_Loss(p=1.5, log_scale=False, sample_weights=False)']
                    }
 
 #print("Supported Loss Functions & Typical Usage:")
 #print("-----------------------------------------")
 #pprint.pprint(supported_losses)
 
-
-
-
```

### Comparing `fmldk-1.1.8/tft/tft_model.py` & `fmldk-1.1.9/tft/tft_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 tfd = tfp.distributions
 import shutil
 import pickle
 import absl.logging
 absl.logging.set_verbosity(absl.logging.ERROR)
 import pandas as pd
 import gc
+import os
 
 # Distribution Sampling functions
 
 # negbin
 def negbin_sample(mu, alpha, n_samples=1):
     tol = 1e-5
     r = 1.0 / alpha
@@ -632,27 +633,28 @@
                                                            context=self.context,
                                                            dropout_rate=dropout_rate)
 
         self.pff_layer = final_gating_layer(hidden_layer_size=hidden_layer_size,
                                             dropout_rate=dropout_rate)
 
         if self.loss_fn == 'Point':
-            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=num_quantiles, activation=None))
+            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='linear'))
+        elif self.loss_fn == 'Tweedie':
+            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='linear'))
         elif self.loss_fn == 'Binary':
             self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='sigmoid'))
         elif self.loss_fn == 'Poisson':
-            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='softplus'))
+            self.final_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='linear'))
         elif self.loss_fn == 'Quantile':
             if self.is_iqf:
                 self.proj_intrcpt = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation=None))
                 if self.num_quantiles > 1:
                     self.proj_incrmnt = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=self.num_quantiles-1, activation='softplus'))
             else:
-                self.quantile_layers = [tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation=None)) 
-                                        for _ in range(num_quantiles)]
+                self.quantile_layers = [tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation=None)) for _ in range(num_quantiles)]
         elif self.loss_fn == 'Normal':
             self.m_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1))
             self.s_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='softplus'))
         elif self.loss_fn == 'Negbin':
             self.m_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='softplus'))
             self.a_layer = tf.keras.layers.TimeDistributed(tf.keras.layers.Dense(units=1, activation='softplus'))
         else:
@@ -736,22 +738,18 @@
         attn_out = attn_out[:,-self.f_len:,:]
 
         # final output
         if self.loss_fn == 'Point':
             out = self.final_layer(attn_out, training=training)
         elif self.loss_fn == 'Binary':
             out = self.final_layer(attn_out, training=training)
+        elif self.loss_fn == 'Tweedie':
+            out = self.final_layer(attn_out, training=training)
         elif self.loss_fn == 'Poisson':
-            if scaler == 'mean_scaler':
-                mean = self.final_layer(attn_out, training=training) * scale
-            elif scaler == 'standard_scaler':
-                mean = self.final_layer(attn_out, training=training) * scale_std + scale_mean
-            #mean = self.final_layer(attn_out, training=training)*scale
-            parameters = mean
-            out = poisson_sample(mu=mean)
+            out = self.final_layer(attn_out, training=training)
         elif self.loss_fn == 'Normal':
             if scaler == 'mean_scaler':
                 mean = self.m_layer(attn_out, training=training) * scale  # (batch, f_len, 1)
                 stddev = self.s_layer(attn_out, training=training) * scale  # (batch, f_len, 1)
             elif scaler == 'standard_scaler':
                 mean = self.m_layer(attn_out, training=training) * scale_std + scale_mean  # (batch, f_len, 1)
                 stddev = self.s_layer(attn_out, training=training) * scale_std  # (batch, f_len, 1)
@@ -779,15 +777,15 @@
             else:
                 output = []
                 for i in range(len(self.quantile_layers)):
                     out = self.quantile_layers[i](attn_out, training=training)
                     output.append(out)
                 out = tf.concat(output, axis=-1)
 
-        if self.loss_fn == 'Point' or self.loss_fn == 'Binary' or self.loss_fn == 'Quantile':
+        if self.loss_fn in ['Point','Quantile','Tweedie','Poisson']:
             return out, scale, stat_weights, past_weights, future_weights
         else:
             return out, parameters, stat_weights, past_weights, future_weights
             
 
 # TFT Wrapper
 
@@ -1128,34 +1126,41 @@
     """
     @tf.function
     def trainstep(model, optimizer, x_train, y_train, scale, wts, training):
         with tf.GradientTape() as tape:
             o, s, f = model(x_train, training=training)
             out_len = s.shape.as_list()[1]  # tf.shape(s)[1]
             s_dim = scale.shape.as_list()[-1]  # tf.shape(scale)[-1]
-            if loss_type in ['Normal','Poisson','Negbin']:
-                '''
-                if weighted_training:
-                    loss = loss_function(y_train*scale[:,-out_len:,:], [s, wts])
-                else:
-                    loss = loss_function(y_train*scale[:,-out_len:,:], s)
-                '''
+            if loss_type in ['Normal', 'Negbin']:
                 if s_dim == 1:
                     if weighted_training:
                         loss = loss_function(y_train * scale[:, -out_len:, :], [s, wts])
                     else:
                         loss = loss_function(y_train * scale[:, -out_len:, :], s)
                 else:
                     s_mean = scale[:, -out_len:, 0:1]
                     s_std = scale[:, -out_len:, 1:2]
                     if weighted_training:
                         loss = loss_function(y_train * s_std + s_mean, [s, wts])
                     else:
                         loss = loss_function(y_train * s_std + s_mean, s)
-            elif loss_type in ['Point','Binary']:
+            elif loss_type in ['Tweedie', 'Poisson']:
+                if s_dim == 1:
+                    if weighted_training:
+                        loss = loss_function(y_train*scale[:, -out_len:, :], [o*scale[:, -out_len:, :], wts])
+                    else:
+                        loss = loss_function(y_train*scale[:, -out_len:, :], o*scale[:, -out_len:, :])
+                else:
+                    s_mean = scale[:, -out_len:, 0:1]
+                    s_std = scale[:, -out_len:, 1:2]
+                    if weighted_training:
+                        loss = loss_function(y_train*s_std + s_mean, [o*s_std + s_mean, wts])
+                    else:
+                        loss = loss_function(y_train*s_std + s_mean, o*s_std + s_mean)
+            elif loss_type in ['Point', 'Binary']:
                 if weighted_training:                               
                     loss = loss_function(y_train, [o, wts])
                 else:
                     loss = loss_function(y_train, o)
             elif loss_type in ['Quantile']:
                 if weighted_training:                               
                     loss = loss_function(y_train, [o, wts])
@@ -1168,38 +1173,48 @@
         return loss, o
     
     @tf.function
     def teststep(model, x_test, y_test, scale, wts, training):
         o, s, f = model(x_test, training=training)
         out_len = s.shape.as_list()[1]  # tf.shape(s)[1]
         s_dim = scale.shape.as_list()[-1]  # tf.shape(scale)[-1]
-        if loss_type in ['Normal','Poisson','Negbin']:
-            '''
-            if weighted_training:
-                loss = loss_function(y_test*scale[:,-out_len:,:], [s, wts])
-            else:
-                loss = loss_function(y_test*scale[:,-out_len:,:], s)    
-            '''
+        if loss_type in ['Normal', 'Negbin']:
             if s_dim == 1:
                 if weighted_training:
                     loss = loss_function(y_test * scale[:, -out_len:, :], [s, wts])
                 else:
                     loss = loss_function(y_test * scale[:, -out_len:, :], s)
             else:
                 s_mean = scale[:, -out_len:, 0:1]
                 s_std = scale[:, -out_len:, 1:2]
                 if weighted_training:
                     loss = loss_function(y_test * s_std + s_mean, [s, wts])
                 else:
                     loss = loss_function(y_test * s_std + s_mean, s)
-        elif loss_type in ['Point','Binary']:
+
+        elif loss_type in ['Tweedie', 'Poisson']:
+            if s_dim == 1:
+                if weighted_training:
+                    loss = loss_function(y_test*scale[:, -out_len:, :], [o*scale[:, -out_len:, :], wts])
+                else:
+                    loss = loss_function(y_test*scale[:, -out_len:, :], o*scale[:, -out_len:, :])
+            else:
+                s_mean = scale[:, -out_len:, 0:1]
+                s_std = scale[:, -out_len:, 1:2]
+                if weighted_training:
+                    loss = loss_function(y_test*s_std + s_mean, [o*s_std + s_mean, wts])
+                else:
+                    loss = loss_function(y_test*s_std + s_mean, o*s_std + s_mean)
+
+        elif loss_type in ['Point', 'Binary']:
             if weighted_training:                               
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)
+
         elif loss_type in ['Quantile']:
             if weighted_training:                               
                 loss = loss_function(y_test, [o, wts])
             else:
                 loss = loss_function(y_test, o)                                   
         else:
             raise ValueError("Invalid loss_type specified!")        
@@ -1340,36 +1355,38 @@
                 x_batch = x_train[i * train_batch_size:(i + 1) * train_batch_size]
                 y_batch = y_train[i * train_batch_size:(i + 1) * train_batch_size]
                 scale = train_scale[i * train_batch_size:(i + 1) * train_batch_size]
                 wts = train_wts[i * train_batch_size:(i + 1) * train_batch_size]
                 train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
                 out_len = tf.shape(train_out)[1]
                 train_loss_avg.update_state(train_loss)
-                if loss_type in ['Normal', 'Poisson', 'Negbin']:
+                if loss_type in ['Normal', 'Negbin']:
                     train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out)
-                elif loss_type in ['Point', 'Quantile']:
-                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :],
-                                              train_out * scale[:, -out_len:, :])
+                elif loss_type in ['Point', 'Poisson', 'Tweedie']:
+                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
+                elif loss_type in ['Quantile']:
+                    train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
                 with train_summary_writer.as_default():
                     tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
                     tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
 
             for i in range(num_test_batches):
                 x_batch = x_test[i * train_batch_size:(i + 1) * train_batch_size]
                 y_batch = y_test[i * train_batch_size:(i + 1) * train_batch_size]
                 scale = test_scale[i * train_batch_size:(i + 1) * train_batch_size]
                 wts = test_wts[i * train_batch_size:(i + 1) * train_batch_size]
                 test_loss, test_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=False)
                 out_len = tf.shape(test_out)[1]
                 test_loss_avg.update_state(test_loss)
-                if loss_type in ['Normal', 'Poisson', 'Negbin']:
+                if loss_type in ['Normal', 'Negbin']:
                     test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out)
-                elif loss_type in ['Point', 'Quantile']:
-                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :],
-                                             test_out * scale[:, -out_len:, :])
+                elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
+                elif loss_type in ['Quantile']:
+                    test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
                 with test_summary_writer.as_default():
                     tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
                     tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
 
             print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
                                                                                                        train_loss_avg.result().numpy(),
                                                                                                        test_loss_avg.result().numpy(),
@@ -1388,21 +1405,24 @@
             test_loss_avg.reset_states()
             test_metric.reset_states()
 
             # Save Model
             model_path = model_prefix + '_' + str(epoch)
             model_list.append(model_path)
 
-            prev_min_loss = np.min(test_loss_results[:-1])
+            if epoch == 0:
+                prev_min_loss = np.min(test_loss_results)
+            else:
+                prev_min_loss = np.min(test_loss_results[:-1])
             current_min_loss = np.min(test_loss_results)
             delta = current_min_loss - prev_min_loss
 
             print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
             # track & save best model
-            if test_loss_results[epoch] == np.min(test_loss_results) and (delta > min_delta):
+            if ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
                 best_model = model_path
                 tf.keras.models.save_model(model, model_path)
                 # reset time_since_improvement
                 time_since_improvement = 0
             else:
                 time_since_improvement += 1
 
@@ -1432,33 +1452,37 @@
             for step, (x_batch, y_batch, scale, wts) in enumerate(train_dataset):
                 if step > train_steps_per_epoch:
                     break
                 else:
                     train_loss, train_out = trainstep(model, optimizer, x_batch, y_batch, scale, wts, training=True)
                     out_len = tf.shape(train_out)[1]
                     train_loss_avg.update_state(train_loss)
-                    if loss_type in ['Normal','Poisson','Negbin']:
+                    if loss_type in ['Normal', 'Negbin']:
                         train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out)
-                    elif loss_type in ['Point','Quantile']:
-                        train_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], train_out*scale[:,-out_len:,:])
+                    elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                        train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out * scale[:, -out_len:, :])
+                    elif loss_type in ['Quantile']:
+                        train_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], train_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
                     with train_summary_writer.as_default():
                         tf.summary.scalar('loss', train_loss_avg.result(), step=epoch)
                         tf.summary.scalar('accuracy', train_metric.result(), step=epoch)
 
             for step, (x_batch, y_batch, scale, wts) in enumerate(test_dataset):
                 if step > train_steps_per_epoch:
                     break
                 else:
                     test_loss, test_out = teststep(model, x_batch, y_batch, scale, wts, training=False)
                     out_len = tf.shape(test_out)[1]
                     test_loss_avg.update_state(test_loss)
-                    if loss_type in ['Normal','Poisson','Negbin']:
+                    if loss_type in ['Normal', 'Negbin']:
                         test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out)
-                    elif loss_type in ['Point','Quantile']:
-                        test_metric.update_state(y_batch[:,-out_len:,:]*scale[:,-out_len:,:], test_out*scale[:,-out_len:,:])
+                    elif loss_type in ['Point', 'Tweedie', 'Poisson']:
+                        test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out * scale[:, -out_len:, :])
+                    elif loss_type in ['Quantile']:
+                        test_metric.update_state(y_batch[:, -out_len:, :] * scale[:, -out_len:, :], test_out[:, -out_len:, 0:1] * scale[:, -out_len:, :])
                     with test_summary_writer.as_default():
                         tf.summary.scalar('loss', test_loss_avg.result(), step=epoch)
                         tf.summary.scalar('accuracy', test_metric.result(), step=epoch)
 
             print("Epoch: {}, train_loss: {}, test_loss: {}, train_metric: {}, test_metric: {}".format(epoch,
                                                                                                         train_loss_avg.result().numpy(),
                                                                                                         test_loss_avg.result().numpy(),
@@ -1477,21 +1501,24 @@
             test_loss_avg.reset_states()
             test_metric.reset_states()
 
             # Save Model
             model_path = model_prefix + '_' + str(epoch)
             model_list.append(model_path)
 
-            prev_min_loss = np.min(test_loss_results[:-1])
+            if epoch == 0:
+                prev_min_loss = np.min(test_loss_results)
+            else:
+                prev_min_loss = np.min(test_loss_results[:-1])
             current_min_loss = np.min(test_loss_results)
             delta = current_min_loss - prev_min_loss
 
             print("Improvement delta (min_delta {}):  {}".format(min_delta, delta))
             # track & save best model
-            if test_loss_results[epoch]==np.min(test_loss_results) and (delta > min_delta):
+            if ((test_loss_results[epoch] == np.min(test_loss_results)) and (-delta > min_delta)) or (epoch == 0):
                 best_model = model_path
                 tf.keras.models.save_model(model, model_path)
                 # reset time_since_improvement
                 time_since_improvement = 0
             else:
                 time_since_improvement += 1
 
@@ -1532,19 +1559,19 @@
     window_len = hist_len + f_len
     stat_wts_df = None 
     encoder_wts_df = None 
     decoder_wts_df = None
         
     out, dist, feature_wts = model(infer_tensor, training=False)
             
-    if loss_type in ['Normal','Poisson','Negbin']:
+    if loss_type in ['Normal','Negbin']:
         dist = dist.numpy()
         output_arr = dist[:,:,0]
         
-    elif loss_type in ['Point','Binary']:
+    elif loss_type in ['Point','Binary','Poisson','Tweedie']:
         out = out.numpy()
         output_arr = out[:,:,0]
     
     elif loss_type in ['Quantile']:
         out = out.numpy()
         output_arr = out[:,:,:]
              
@@ -1570,22 +1597,20 @@
     encoder_wts_df = pd.DataFrame(encoder_wts, columns=encoder_columns_string)   
     decoder_wts_df = pd.DataFrame(decoder_wts, columns=decoder_columns_string)    
     if stat_wts is not None:
         stat_wts = stat_wts.numpy()
         stat_wts_df = pd.DataFrame(stat_wts, columns=stat_columns_string)   
             
     # rescale if necessary
-    if loss_type in ['Normal','Poisson','Negbin']:
+    if loss_type in ['Normal', 'Negbin']:
         output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr), axis=1))
         output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
         output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
         
-    elif loss_type in ['Point','Binary']:
-
-        #output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr*scale.reshape(-1,1)), axis=1))
+    elif loss_type in ['Point', 'Binary', 'Poisson', 'Tweedie']:
         if s_dim == 1:
             output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output_arr * scale.reshape(-1, 1)), axis=1))
         else:
             output_arr = output_arr * scale_std.reshape(-1, 1) + scale_mean.reshape(-1, 1)
             output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output_arr), axis=1))
         output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value':'forecast'})
         output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
@@ -1595,16 +1620,16 @@
         for i in range(num_quantiles):
             if s_dim == 1:
                 output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1,1),output_arr[:,:,i]*scale.reshape(-1,1)), axis=1))
                 output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0:'id','value': f"forecast_{i}"})
                 output_df = output_df.rename_axis('index').sort_values(by=['id','index']).reset_index(drop=True)
                 df_list.append(output_df)
             else:
-                output_arr = output_arr[:,:,i]* scale_std.reshape(-1, 1) + scale_mean.reshape(-1, 1)
-                output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output_arr), axis=1))
+                output = output_arr[:,:,i]* scale_std.reshape(-1, 1) + scale_mean.reshape(-1, 1)
+                output_df = pd.DataFrame(np.concatenate((id_arr.reshape(-1, 1), output), axis=1))
                 output_df = output_df.melt(id_vars=0).sort_values(0).drop(columns=['variable']).rename(columns={0: 'id', 'value': f"forecast_{i}"})
                 output_df = output_df.rename_axis('index').sort_values(by=['id', 'index']).reset_index(drop=True)
                 df_list.append(output_df)
         output_df = pd.concat(df_list, axis=1)
         output_df = output_df.loc[:,~output_df.columns.duplicated()]
         
     # merge date_columns
@@ -1648,31 +1673,48 @@
                  num_heads,
                  d_model,
                  forecast_horizon,
                  max_inp_len,
                  loss_type,
                  num_quantiles=1,
                  decoder_start_tokens=1,
-                 dropout_rate=0.1):
+                 dropout_rate=0.1,
+                 seed=None,
+                 deterministic_ops=False):
         
         self.col_index_dict = col_index_dict
         self.vocab_dict = vocab_dict
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.d_model = d_model
         self.forecast_horizon = forecast_horizon
         self.max_inp_len = max_inp_len
         self.loss_type = loss_type
         self.num_quantiles = num_quantiles
         self.dropout_rate = dropout_rate
         self.decoder_start_tokens = decoder_start_tokens
         self.target_col_name, self.target_index = self.col_index_dict.get('target_index')
-    
+        self.seed = seed
+        self.allow_deterministic_ops = deterministic_ops
+
+    def set_seed(self):
+        tf.keras.utils.set_random_seed(self.seed)
+        if self.allow_deterministic_ops:
+            print("Deterministic Ops enabled.")
+            os.environ["TF_DETERMINISTIC_OPS"] = "True"
+            os.environ["TF_DISABLE_SEGMENT_REDUCTION_OP_DETERMINISM_EXCEPTIONS"] = "True"
+
     def build(self):
         tf.keras.backend.clear_session()
+        if self.seed is None:
+            print("No seed set for deterministic weights initialization")
+        else:
+            print("Using seed {} for weights initialization".format(self.seed))
+            self.set_seed()
+
         self.model = TFT_Model(self.col_index_dict,
                                   self.vocab_dict,
                                   self.num_layers,
                                   self.num_heads,
                                   self.d_model,
                                   self.forecast_horizon,
                                   self.max_inp_len,
```

### Comparing `fmldk-1.1.8/tft/tft_model_v0.1.26.py` & `fmldk-1.1.9/tft/tft_model_v0.1.26.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tft/tft_model_v0.1.31.py` & `fmldk-1.1.9/tft/tft_model_v0.1.31.py`

 * *Files identical despite different names*

### Comparing `fmldk-1.1.8/tft/tft_model_v1.1.3.py` & `fmldk-1.1.9/tft/tft_model_v1.1.3.py`

 * *Files identical despite different names*

