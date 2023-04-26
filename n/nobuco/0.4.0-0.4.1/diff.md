# Comparing `tmp/nobuco-0.4.0.tar.gz` & `tmp/nobuco-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.0.tar", last modified: Fri Apr 21 21:39:49 2023, max compression
+gzip compressed data, was "nobuco-0.4.1.tar", last modified: Tue Apr 25 18:16:07 2023, max compression
```

## Comparing `nobuco-0.4.0.tar` & `nobuco-0.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.4.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    21659 2023-04-21 21:39:49.926740 nobuco-0.4.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    19825 2023-04-21 21:38:56.000000 nobuco-0.4.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.918740 nobuco-0.4.0/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-21 10:22:54.000000 nobuco-0.4.0/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-21 21:36:43.000000 nobuco-0.4.0/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13497 2023-04-21 21:36:43.000000 nobuco-0.4.0/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.4.0/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.4.0/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-19 23:06:10.000000 nobuco-0.4.0/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.4.0/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.4.0/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-21 21:15:19.000000 nobuco-0.4.0/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.4.0/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-20 11:44:40.000000 nobuco-0.4.0/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-21 21:37:11.000000 nobuco-0.4.0/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-20 10:41:07.000000 nobuco-0.4.0/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.4.0/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.4.0/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-21 13:07:22.000000 nobuco-0.4.0/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.4.0/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.4.0/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-21 10:21:12.000000 nobuco-0.4.0/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-21 13:21:40.000000 nobuco-0.4.0/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-21 10:22:11.000000 nobuco-0.4.0/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.4.0/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-21 11:09:43.000000 nobuco-0.4.0/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-21 11:14:16.000000 nobuco-0.4.0/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-19 08:28:44.000000 nobuco-0.4.0/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.4.0/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.4.0/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-21 09:46:48.000000 nobuco-0.4.0/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.4.0/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.4.0/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-21 13:07:22.000000 nobuco-0.4.0/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-21 13:07:21.000000 nobuco-0.4.0/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.918740 nobuco-0.4.0/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    21659 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-21 11:10:10.000000 nobuco-0.4.0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-21 21:39:49.926740 nobuco-0.4.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-04-25 18:16:07.396770 nobuco-0.4.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20054 2023-04-25 18:07:04.000000 nobuco-0.4.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.1/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-25 18:15:04.000000 nobuco-0.4.1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-25 18:16:07.396770 nobuco-0.4.1/setup.cfg
```

### Comparing `nobuco-0.4.0/LICENSE` & `nobuco-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/PKG-INFO` & `nobuco-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -148,14 +148,20 @@
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
+https://user-images.githubusercontent.com/2457934/233740603-cc11acc5-cd6b-48c8-b089-ff3ead772dd0.mp4
+
+<p align="center">
+To ease debugging, Nobuco lets you jump right where the node was [I]nvoked, [D]efined and [C]onverted
+</p>
+
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
 Transposing tensors between the two layouts incurs non-trivial overhead as generally, tensor data must be physically rearranged.
@@ -514,15 +520,15 @@
 
 
 @nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
 def converter_AddByMask(self, x, mask):
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
-    # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
+    # NB: onnx.export is implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
```

### Comparing `nobuco-0.4.0/README.md` & `nobuco-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,20 @@
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
+https://user-images.githubusercontent.com/2457934/233740603-cc11acc5-cd6b-48c8-b089-ff3ead772dd0.mp4
+
+<p align="center">
+To ease debugging, Nobuco lets you jump right where the node was [I]nvoked, [D]efined and [C]onverted
+</p>
+
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
 Transposing tensors between the two layouts incurs non-trivial overhead as generally, tensor data must be physically rearranged.
@@ -478,15 +484,15 @@
 
 
 @nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
 def converter_AddByMask(self, x, mask):
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
-    # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
+    # NB: onnx.export is implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
```

### Comparing `nobuco-0.4.0/nobuco/__init__.py` & `nobuco-0.4.1/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/commons.py` & `nobuco-0.4.1/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/convert.py` & `nobuco-0.4.1/nobuco/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,26 +233,34 @@
     # Ensure outputs order
     processed = [tf.identity(t) for t in processed]
     return processed
 
 
 def pytorch_to_keras(
         module: nn.Module,
-        args=[], kwargs={},
+        args: List[object] = None,
+        kwargs: Dict[str, object] = None,
         input_shapes: Dict[torch.Tensor, Collection[Optional[int]]] = None,
         inputs_channel_order: Union[ChannelOrder, Dict[torch.Tensor, ChannelOrder]] = ChannelOrder.TENSORFLOW,
         outputs_channel_order: Union[ChannelOrder, Dict[int, ChannelOrder]] = None,
         converter_dict=CONVERTER_DICT,
         constants_to_variables: bool = True,
         full_validation: bool = True,
         validation_tolerance=1e-4,
         save_trace_html=False,
         return_outputs_pt=False,
         debug_traces: TraceLevel = TraceLevel.DEFAULT,
 ) -> Union[keras.Model, Tuple[keras.Model, object]]:
+
+    if args is None:
+        args = []
+
+    if kwargs is None:
+        kwargs = {}
+
     start = time.time()
     node_hierarchy = Tracer.trace(module, args, kwargs)
 
     keras_converted_node = convert_hierarchy(node_hierarchy, converter_dict,
                                              reuse_layers=True, full_validation=full_validation, constants_to_variables=constants_to_variables,
                                              tolerance=validation_tolerance,
                                              )
```

### Comparing `nobuco-0.4.0/nobuco/converters/channel_ordering.py` & `nobuco-0.4.1/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/converters/node_converter.py` & `nobuco-0.4.1/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/converters/tensor.py` & `nobuco-0.4.1/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/converters/type_cast.py` & `nobuco-0.4.1/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/converters/validation.py` & `nobuco-0.4.1/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/entity/keras.py` & `nobuco-0.4.1/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/entity/pytorch.py` & `nobuco-0.4.1/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/funcs.py` & `nobuco-0.4.1/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/layers/channel_order.py` & `nobuco-0.4.1/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/layers/container.py` & `nobuco-0.4.1/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/layers/weight.py` & `nobuco-0.4.1/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/locate/link.py` & `nobuco-0.4.1/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/locate/locate.py` & `nobuco-0.4.1/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/activation.py` & `nobuco-0.4.1/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/boolean.py` & `nobuco-0.4.1/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.1/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/comparison.py` & `nobuco-0.4.1/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/convolution.py` & `nobuco-0.4.1/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/dropout.py` & `nobuco-0.4.1/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/interpolation.py` & `nobuco-0.4.1/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/linear.py` & `nobuco-0.4.1/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/math.py` & `nobuco-0.4.1/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/misc.py` & `nobuco-0.4.1/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/normalization.py` & `nobuco-0.4.1/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/padding.py` & `nobuco-0.4.1/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/pooling.py` & `nobuco-0.4.1/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/recurrent.py` & `nobuco-0.4.1/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/slice.py` & `nobuco-0.4.1/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.1/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.1/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.1/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/trace/tensor_storage.py` & `nobuco-0.4.1/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/trace/trace.py` & `nobuco-0.4.1/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/util.py` & `nobuco-0.4.1/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/vis/console_stylizer.py` & `nobuco-0.4.1/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco/vis/html_stylizer.py` & `nobuco-0.4.1/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.1/nobuco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -148,14 +148,20 @@
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
+https://user-images.githubusercontent.com/2457934/233740603-cc11acc5-cd6b-48c8-b089-ff3ead772dd0.mp4
+
+<p align="center">
+To ease debugging, Nobuco lets you jump right where the node was [I]nvoked, [D]efined and [C]onverted
+</p>
+
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
 Transposing tensors between the two layouts incurs non-trivial overhead as generally, tensor data must be physically rearranged.
@@ -514,15 +520,15 @@
 
 
 @nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
 def converter_AddByMask(self, x, mask):
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
-    # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
+    # NB: onnx.export is implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
     tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
```

### Comparing `nobuco-0.4.0/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.1/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.0/pyproject.toml` & `nobuco-0.4.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.0"
+version = "0.4.1"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

