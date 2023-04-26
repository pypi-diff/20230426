# Comparing `tmp/nnx-0.0.0.tar.gz` & `tmp/nnx-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.0.tar", max compression
+gzip compressed data, was "nnx-0.0.1.tar", max compression
```

## Comparing `nnx-0.0.0.tar` & `nnx-0.0.1.tar`

### file list

```diff
@@ -1,8 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.0/LICENSE
--rw-r--r--   0        0        0        5 2023-03-18 22:40:31.494888 nnx-0.0.0/README.md
--rw-r--r--   0        0        0      129 2023-03-18 22:43:03.595827 nnx-0.0.0/nnx/__init__.py
--rw-r--r--   0        0        0        0 2023-03-18 22:42:49.114596 nnx-0.0.0/nnx/module.py
--rw-r--r--   0        0        0     1403 2023-03-18 22:42:49.114596 nnx-0.0.0/nnx/refs.py
--rw-r--r--   0        0        0     5077 2023-03-18 22:42:49.114596 nnx-0.0.0/nnx/transforms.py
--rw-r--r--   0        0        0      320 2023-03-18 22:45:06.338269 nnx-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 nnx-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3952 2023-04-22 20:13:31.443728 nnx-0.0.1/README.md
+-rw-r--r--   0        0        0      776 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/__init__.py
+-rw-r--r--   0        0        0     2235 2023-04-08 23:38:12.700869 nnx-0.0.1/nnx/fields.py
+-rw-r--r--   0        0        0     3789 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/filters.py
+-rw-r--r--   0        0        0      140 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2764 2023-04-08 19:11:50.337195 nnx-0.0.1/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     1888 2023-04-08 18:42:49.425089 nnx-0.0.1/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    13270 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/linear.py
+-rw-r--r--   0        0        0     7325 2023-04-24 23:40:16.468746 nnx-0.0.1/nnx/nn/module.py
+-rw-r--r--   0        0        0    10680 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2250 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0     2431 2023-04-10 14:13:14.802122 nnx-0.0.1/nnx/partitioning.py
+-rw-r--r--   0        0        0     2417 2023-03-30 22:50:08.758780 nnx-0.0.1/nnx/rng_stream.py
+-rw-r--r--   0        0        0     5483 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/scope_lib.py
+-rw-r--r--   0        0        0     6838 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/transforms.py
+-rw-r--r--   0        0        0      563 2023-04-22 15:20:28.647804 nnx-0.0.1/nnx/utils.py
+-rw-r--r--   0        0        0      751 2023-04-25 22:29:59.969018 nnx-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 nnx-0.0.1/PKG-INFO
```

### Comparing `nnx-0.0.0/LICENSE` & `nnx-0.0.1/LICENSE`

 * *Files identical despite different names*

