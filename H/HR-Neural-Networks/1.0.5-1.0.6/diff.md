# Comparing `tmp/HR_Neural_Networks-1.0.5.tar.gz` & `tmp/HR_Neural_Networks-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HR_Neural_Networks-1.0.5.tar", last modified: Tue Apr 25 15:35:01 2023, max compression
+gzip compressed data, was "HR_Neural_Networks-1.0.6.tar", last modified: Tue Apr 25 19:00:51 2023, max compression
```

## Comparing `HR_Neural_Networks-1.0.5.tar` & `HR_Neural_Networks-1.0.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.887447 HR_Neural_Networks-1.0.5/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     8196 2023-04-24 21:54:05.000000 HR_Neural_Networks-1.0.5/.DS_Store
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.345386 HR_Neural_Networks-1.0.5/HR_Neural_Networks/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-04-24 21:53:26.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/.DS_Store
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    12317 2023-04-25 15:32:47.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/HR.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.448029 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/.DS_Store
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.538465 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.1/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.1/.DS_Store
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      343 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.1/CIFAR_10_note.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    12540 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.1/mnist_single_param.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.578531 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/.DS_Store
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.595704 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/.DS_Store
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    21968 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/Rice_HR.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.637869 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/.DS_Store
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    21736 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/Rice_TRADES.py
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6099 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/trades.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.656812 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4597 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/preactresnet.cpython-39.pyc
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     5537 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4208 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/preactresnet.py
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4043 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/utils.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.697753 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.3/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    17499 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.3/CIFAR_10_all_error_sources.py
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4538 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.3/resnet.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.726647 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/__pycache__/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1739 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/__pycache__/helper_functions.cpython-39.pyc
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1928 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/helper_functions.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.428776 HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-04-25 15:34:59.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/PKG-INFO
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1787 2023-04-25 15:35:00.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)        1 2023-04-25 15:34:59.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       37 2023-04-25 15:34:59.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/requires.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       19 2023-04-25 15:34:59.000000 HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/top_level.txt
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1094 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/LICENSE.txt
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.876288 HR_Neural_Networks-1.0.5/Misc/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/Misc/.DS_Store
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    27583 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/Misc/Classifiers.png
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)   307785 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/DRO_gif.gif
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    56951 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/HD.png
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    22190 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/HR.png
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1017 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/Misc/Julia.svg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)  1056373 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/Misc/SVP-gif.gif
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     2369 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/colab.svg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      987 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/mosek.lic
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1213 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/pt_badge.svg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4781 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/python.svg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     3601 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.5/Misc/tf.svg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-04-25 15:35:01.887935 HR_Neural_Networks-1.0.5/PKG-INFO
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     7328 2023-04-25 15:32:47.000000 HR_Neural_Networks-1.0.5/README.md
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       54 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.5/__init__.py
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.884518 HR_Neural_Networks-1.0.5/__pycache__/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      206 2023-04-16 13:18:40.000000 HR_Neural_Networks-1.0.5/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 15:35:01.886299 HR_Neural_Networks-1.0.5/dist/
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-04-25 15:34:38.000000 HR_Neural_Networks-1.0.5/dist/.DS_Store
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       79 2023-04-25 15:35:01.890453 HR_Neural_Networks-1.0.5/setup.cfg
--rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1983 2023-04-25 15:34:16.000000 HR_Neural_Networks-1.0.5/setup.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.064304 HR_Neural_Networks-1.0.6/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     8196 2023-04-25 18:58:43.000000 HR_Neural_Networks-1.0.6/.DS_Store
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.014922 HR_Neural_Networks-1.0.6/HR_Neural_Networks/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-04-24 21:53:26.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    12308 2023-04-25 18:57:39.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/HR.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.027780 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/.DS_Store
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.030415 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.1/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.1/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      343 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.1/CIFAR_10_note.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    12540 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.1/mnist_single_param.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.032410 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/.DS_Store
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.034234 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    21968 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/Rice_HR.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.036962 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    21736 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/Rice_TRADES.py
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6099 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/trades.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.038732 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4597 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/preactresnet.cpython-39.pyc
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     5537 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4208 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/preactresnet.py
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4043 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/utils.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.040840 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.3/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    17499 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.3/CIFAR_10_all_error_sources.py
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4538 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.3/resnet.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.041837 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/__pycache__/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1739 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/__pycache__/helper_functions.cpython-39.pyc
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1928 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/helper_functions.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.026245 HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-04-25 19:00:50.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1787 2023-04-25 19:00:50.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)        1 2023-04-25 19:00:50.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       37 2023-04-25 19:00:50.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/requires.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       19 2023-04-25 19:00:50.000000 HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/top_level.txt
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1094 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/LICENSE.txt
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.058803 HR_Neural_Networks-1.0.6/Misc/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/Misc/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    27583 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/Misc/Classifiers.png
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)   307785 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/DRO_gif.gif
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    56951 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/HD.png
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)    22190 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/HR.png
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1017 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/Misc/Julia.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)  1056373 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/Misc/SVP-gif.gif
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     2369 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/colab.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      987 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/mosek.lic
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1213 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/pt_badge.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     4781 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/python.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     3601 2023-03-03 17:19:15.000000 HR_Neural_Networks-1.0.6/Misc/tf.svg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1058 2023-04-25 19:00:51.064631 HR_Neural_Networks-1.0.6/PKG-INFO
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     7328 2023-04-25 15:32:47.000000 HR_Neural_Networks-1.0.6/README.md
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       54 2023-03-03 17:19:16.000000 HR_Neural_Networks-1.0.6/__init__.py
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.059839 HR_Neural_Networks-1.0.6/__pycache__/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)      206 2023-04-16 13:18:40.000000 HR_Neural_Networks-1.0.6/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 ryandeclanlucus   (502) staff       (20)        0 2023-04-25 19:00:51.063711 HR_Neural_Networks-1.0.6/dist/
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     6148 2023-04-25 19:00:48.000000 HR_Neural_Networks-1.0.6/dist/.DS_Store
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)       79 2023-04-25 19:00:51.066266 HR_Neural_Networks-1.0.6/setup.cfg
+-rw-r--r--   0 ryandeclanlucus   (502) staff       (20)     1983 2023-04-25 19:00:47.000000 HR_Neural_Networks-1.0.6/setup.py
```

### Comparing `HR_Neural_Networks-1.0.5/.DS_Store` & `HR_Neural_Networks-1.0.6/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0016  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0018  ................
 00000050: 0000 0001 0000 1000 0069 0074 005f 005f  .........i.t._._
 00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,15 +250,15 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0016 0000 000b  ................
+00001000: 0000 0000 0000 0000 0000 0018 0000 000b  ................
 00001010: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 00001020: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
 00001030: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
 00001040: 0000 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
 00001050: 0061 0063 0068 0065 005f 005f 496c 6f63  .a.c.h.e._._Iloc
 00001060: 626c 6f62 0000 0010 0000 00af 0000 002e  blob............
 00001070: ffff ffff ffff 0000 0000 0004 0064 0069  .............d.i
@@ -269,15 +269,15 @@
 000010c0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 000010d0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 000010e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 000010f0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00001100: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00001110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00001120: 6261 7208 0908 095f 1018 7b7b 3632 392c  bar...._..{{629,
-00001130: 2031 3832 7d2c 207b 3932 302c 2034 3336   182}, {920, 436
+00001130: 2031 3833 7d2c 207b 3932 302c 2034 3336   183}, {920, 436
 00001140: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 00001150: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001160: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001170: 0000 0004 0064 0069 0073 0074 7653 726e  .....d.i.s.tvSrn
 00001180: 6c6f 6e67 0000 0001 0000 0012 0048 0052  long.........H.R
 00001190: 005f 004e 0065 0075 0072 0061 006c 005f  ._.N.e.u.r.a.l._
 000011a0: 004e 0065 0074 0077 006f 0072 006b 0073  .N.e.t.w.o.r.k.s
@@ -296,88 +296,88 @@
 00001270: 1018 7b7b 3632 392c 2031 3832 7d2c 207b  ..{{629, 182}, {
 00001280: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
 00001290: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 000012a0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 000012b0: 0000 0000 0000 008b 0000 0012 0048 0052  .............H.R
 000012c0: 005f 004e 0065 0075 0072 0061 006c 005f  ._.N.e.u.r.a.l._
 000012d0: 004e 0065 0074 0077 006f 0072 006b 0073  .N.e.t.w.o.r.k.s
-000012e0: 7653 726e 6c6f 6e67 0000 0001 0000 001b  vSrnlong........
+000012e0: 7653 726e 6c6f 6e67 0000 0001 0000 0018  vSrnlong........
 000012f0: 0048 0052 005f 004e 0065 0075 0072 0061  .H.R._.N.e.u.r.a
 00001300: 006c 005f 004e 0065 0074 0077 006f 0072  .l._.N.e.t.w.o.r
-00001310: 006b 0073 002e 0065 0067 0067 002d 0069  .k.s...e.g.g.-.i
-00001320: 006e 0066 006f 496c 6f63 626c 6f62 0000  .n.f.oIlocblob..
-00001330: 0010 0000 018b 0000 009e ffff ffff ffff  ................
-00001340: 0000 0000 001b 0048 0052 005f 004e 0065  .......H.R._.N.e
-00001350: 0075 0072 0061 006c 005f 004e 0065 0074  .u.r.a.l._.N.e.t
-00001360: 0077 006f 0072 006b 0073 002e 0065 0067  .w.o.r.k.s...e.g
-00001370: 0067 002d 0069 006e 0066 006f 6277 7370  .g.-.i.n.f.obwsp
-00001380: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
-00001390: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-000013a0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-000013b0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-000013c0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-000013d0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-000013e0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000013f0: 6261 7208 0908 095f 1018 7b7b 3632 392c  bar...._..{{629,
-00001400: 2031 3832 7d2c 207b 3932 302c 2034 3336   182}, {920, 436
-00001410: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
-00001420: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00001430: 0000 0000 0000 0000 0000 0000 0000 008b  ................
-00001440: 0000 001b 0048 0052 005f 004e 0065 0075  .....H.R._.N.e.u
-00001450: 0072 0061 006c 005f 004e 0065 0074 0077  .r.a.l._.N.e.t.w
-00001460: 006f 0072 006b 0073 002e 0065 0067 0067  .o.r.k.s...e.g.g
-00001470: 002d 0069 006e 0066 006f 7653 726e 6c6f  .-.i.n.f.ovSrnlo
-00001480: 6e67 0000 0001 0000 000b 004c 0049 0043  ng.........L.I.C
-00001490: 0045 004e 0053 0045 002e 0074 0078 0074  .E.N.S.E...t.x.t
-000014a0: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
-000014b0: 0000 002e ffff ffff ffff 0000 0000 0004  ................
-000014c0: 004d 0069 0073 0063 496c 6f63 626c 6f62  .M.i.s.cIlocblob
-000014d0: 0000 0010 0000 0267 0000 002e ffff ffff  .......g........
-000014e0: ffff 0000 0000 0004 004d 0069 0073 0063  .........M.i.s.c
-000014f0: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
-00001500: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
-00001510: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001520: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00001530: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00001540: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00001550: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00001560: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
-00001570: 3632 392c 2031 3832 7d2c 207b 3932 302c  629, 182}, {920,
-00001580: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
-00001590: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
-000015a0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
-000015b0: 0000 008b 0000 0004 004d 0069 0073 0063  .........M.i.s.c
-000015c0: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
-000015d0: 0000 0004 004d 0069 0073 0063 6d6f 4444  .....M.i.s.cmoDD
-000015e0: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
-000015f0: 0000 0004 004d 0069 0073 0063 6d6f 6444  .....M.i.s.cmodD
-00001600: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
-00001610: 0000 0004 004d 0069 0073 0063 7068 3153  .....M.i.s.cph1S
-00001620: 636f 6d70 0000 0000 0000 0000 0000 0004  comp............
-00001630: 004d 0069 0073 0063 7653 726e 6c6f 6e67  .M.i.s.cvSrnlong
-00001640: 0000 0001 0000 0009 0052 0045 0041 0044  .........R.E.A.D
-00001650: 004d 0045 002e 006d 0064 496c 6f63 626c  .M.E...m.dIlocbl
-00001660: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
-00001670: ffff ffff 0000 0000 0009 0073 0065 0074  ...........s.e.t
-00001680: 0075 0070 002e 0063 0066 0067 496c 6f63  .u.p...c.f.gIloc
-00001690: 626c 6f62 0000 0010 0000 00af 0000 009e  blob............
-000016a0: ffff ffff ffff 0000 0000 0008 0073 0065  .............s.e
-000016b0: 0074 0075 0070 002e 0070 0079 496c 6f63  .t.u.p...p.yIloc
-000016c0: 626c 6f62 0000 0010 0000 011d 0000 009e  blob............
-000016d0: ffff ffff ffff 0000 0000 0000 0000 0000  ................
-000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001310: 006b 0073 002d 0031 002e 0030 002e 0034  .k.s.-.1...0...4
+00001320: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
+00001330: 0000 009e ffff ffff ffff 0000 0000 0018  ................
+00001340: 0048 0052 005f 004e 0065 0075 0072 0061  .H.R._.N.e.u.r.a
+00001350: 006c 005f 004e 0065 0074 0077 006f 0072  .l._.N.e.t.w.o.r
+00001360: 006b 0073 002d 0031 002e 0030 002e 0035  .k.s.-.1...0...5
+00001370: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
+00001380: 0000 009e ffff ffff ffff 0000 0000 001b  ................
+00001390: 0048 0052 005f 004e 0065 0075 0072 0061  .H.R._.N.e.u.r.a
+000013a0: 006c 005f 004e 0065 0074 0077 006f 0072  .l._.N.e.t.w.o.r
+000013b0: 006b 0073 002e 0065 0067 0067 002d 0069  .k.s...e.g.g.-.i
+000013c0: 006e 0066 006f 496c 6f63 626c 6f62 0000  .n.f.oIlocblob..
+000013d0: 0010 0000 018b 0000 009e ffff ffff ffff  ................
+000013e0: 0000 0000 001b 0048 0052 005f 004e 0065  .......H.R._.N.e
+000013f0: 0075 0072 0061 006c 005f 004e 0065 0074  .u.r.a.l._.N.e.t
+00001400: 0077 006f 0072 006b 0073 002e 0065 0067  .w.o.r.k.s...e.g
+00001410: 0067 002d 0069 006e 0066 006f 6277 7370  .g.-.i.n.f.obwsp
+00001420: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00001430: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00001440: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001450: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00001460: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00001470: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00001480: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00001490: 6261 7208 0908 095f 1018 7b7b 3632 392c  bar...._..{{629,
+000014a0: 2031 3832 7d2c 207b 3932 302c 2034 3336   182}, {920, 436
+000014b0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+000014c0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+000014d0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+000014e0: 0000 001b 0048 0052 005f 004e 0065 0075  .....H.R._.N.e.u
+000014f0: 0072 0061 006c 005f 004e 0065 0074 0077  .r.a.l._.N.e.t.w
+00001500: 006f 0072 006b 0073 002e 0065 0067 0067  .o.r.k.s...e.g.g
+00001510: 002d 0069 006e 0066 006f 7653 726e 6c6f  .-.i.n.f.ovSrnlo
+00001520: 6e67 0000 0001 0000 000b 004c 0049 0043  ng.........L.I.C
+00001530: 0045 004e 0053 0045 002e 0074 0078 0074  .E.N.S.E...t.x.t
+00001540: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
+00001550: 0000 002e ffff ffff ffff 0000 0000 0004  ................
+00001560: 004d 0069 0073 0063 496c 6f63 626c 6f62  .M.i.s.cIlocblob
+00001570: 0000 0010 0000 0267 0000 002e ffff ffff  .......g........
+00001580: ffff 0000 0000 0004 004d 0069 0073 0063  .........M.i.s.c
+00001590: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+000015a0: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+000015b0: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+000015c0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+000015d0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+000015e0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+000015f0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001600: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+00001610: 3632 392c 2031 3832 7d2c 207b 3932 302c  629, 182}, {920,
+00001620: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00001630: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00001640: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00001650: 0000 008b 0000 0004 004d 0069 0073 0063  .........M.i.s.c
+00001660: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
+00001670: 0000 0004 004d 0069 0073 0063 6d6f 4444  .....M.i.s.cmoDD
+00001680: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
+00001690: 0000 0004 004d 0069 0073 0063 6d6f 6444  .....M.i.s.cmodD
+000016a0: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
+000016b0: 0000 0004 004d 0069 0073 0063 7068 3153  .....M.i.s.cph1S
+000016c0: 636f 6d70 0000 0000 0000 0000 0000 0004  comp............
+000016d0: 004d 0069 0073 0063 7653 726e 6c6f 6e67  .M.i.s.cvSrnlong
+000016e0: 0000 0001 0000 0009 0052 0045 0041 0044  .........R.E.A.D
+000016f0: 004d 0045 002e 006d 0064 496c 6f63 626c  .M.E...m.dIlocbl
+00001700: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
+00001710: ffff ffff 0000 0000 0009 0073 0065 0074  ...........s.e.t
+00001720: 0075 0070 002e 0063 0066 0067 496c 6f63  .u.p...c.f.gIloc
+00001730: 626c 6f62 0000 0010 0000 00af 0000 009e  blob............
+00001740: ffff ffff ffff 0000 0000 0008 0073 0065  .............s.e
+00001750: 0074 0075 0070 002e 0070 0079 496c 6f63  .t.u.p...p.yIloc
+00001760: 626c 6f62 0000 0010 0000 011d 0000 009e  blob............
+00001770: ffff ffff ffff 0000 0000 0000 0000 0000  ................
 00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,55 +457,55 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0070 6c69  .....@.......pli
-00001d00: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
-00001d10: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001d20: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00001d30: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00001d40: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00001d50: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00001d60: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
-00001d70: 3632 392c 2031 3832 7d2c 207b 3932 302c  629, 182}, {920,
-00001d80: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
-00001d90: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
-00001da0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0000 008b 0000 0004 004d 0069 0073 0063  .........M.i.s.c
-00001dc0: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
-00001dd0: 0000 0004 004d 0069 0073 0063 6d6f 4444  .....M.i.s.cmoDD
-00001de0: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
-00001df0: 0000 0004 004d 0069 0073 0063 6d6f 6444  .....M.i.s.cmodD
-00001e00: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
-00001e10: 0000 0004 004d 0069 0073 0063 7068 3153  .....M.i.s.cph1S
-00001e20: 636f 6d70 0000 0000 0000 0000 0000 0004  comp............
-00001e30: 004d 0069 0073 0063 7653 726e 6c6f 6e67  .M.i.s.cvSrnlong
-00001e40: 0000 0001 0000 0009 0052 0045 0041 0044  .........R.E.A.D
-00001e50: 004d 0045 002e 006d 0064 496c 6f63 626c  .M.E...m.dIlocbl
-00001e60: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
-00001e70: ffff ffff 0000 0000 0009 0073 0065 0074  ...........s.e.t
-00001e80: 0075 0070 002e 0063 0066 0067 496c 6f63  .u.p...c.f.gIloc
-00001e90: 626c 6f62 0000 0010 0000 00af 0000 009e  blob............
-00001ea0: ffff ffff ffff 0000 0000 0008 0073 0065  .............s.e
-00001eb0: 0074 0075 0070 002e 0070 0079 496c 6f63  .t.u.p...p.yIloc
-00001ec0: 626c 6f62 0000 0010 0000 011d 0000 009e  blob............
-00001ed0: ffff ffff ffff 0000 0000 0000 0000 0000  ................
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 0074 0077  .....@.......t.w
+00001d00: 006f 0072 006b 0073 002e 0065 0067 0067  .o.r.k.s...e.g.g
+00001d10: 002d 0069 006e 0066 006f 7653 726e 6c6f  .-.i.n.f.ovSrnlo
+00001d20: 6e67 0000 0001 0000 000b 004c 0049 0043  ng.........L.I.C
+00001d30: 0045 004e 0053 0045 002e 0074 0078 0074  .E.N.S.E...t.x.t
+00001d40: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
+00001d50: 0000 002e ffff ffff ffff 0000 0000 0004  ................
+00001d60: 004d 0069 0073 0063 496c 6f63 626c 6f62  .M.i.s.cIlocblob
+00001d70: 0000 0010 0000 0267 0000 002e ffff ffff  .......g........
+00001d80: ffff 0000 0000 0004 004d 0069 0073 0063  .........M.i.s.c
+00001d90: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00001da0: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00001db0: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00001dc0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00001dd0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00001de0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00001df0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001e00: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+00001e10: 3632 392c 2031 3832 7d2c 207b 3932 302c  629, 182}, {920,
+00001e20: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00001e30: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00001e40: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00001e50: 0000 008b 0000 0004 004d 0069 0073 0063  .........M.i.s.c
+00001e60: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
+00001e70: 0000 0004 004d 0069 0073 0063 6d6f 4444  .....M.i.s.cmoDD
+00001e80: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
+00001e90: 0000 0004 004d 0069 0073 0063 6d6f 6444  .....M.i.s.cmodD
+00001ea0: 626c 6f62 0000 0008 17b7 b301 de82 c441  blob...........A
+00001eb0: 0000 0004 004d 0069 0073 0063 7068 3153  .....M.i.s.cph1S
+00001ec0: 636f 6d70 0000 0000 0000 0000 0000 0004  comp............
+00001ed0: 004d 0069 0073 0063 7653 726e 6c6f 6e67  .M.i.s.cvSrnlong
+00001ee0: 0000 0001 0000 0009 0052 0045 0041 0044  .........R.E.A.D
+00001ef0: 004d 0045 002e 006d 0064 496c 6f63 626c  .M.E...m.dIlocbl
+00001f00: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
+00001f10: ffff ffff 0000 0000 0009 0073 0065 0074  ...........s.e.t
+00001f20: 0075 0070 002e 0063 0066 0067 496c 6f63  .u.p...c.f.gIloc
+00001f30: 626c 6f62 0000 0010 0000 00af 0000 009e  blob............
+00001f40: ffff ffff ffff 0000 0000 0008 0073 0065  .............s.e
+00001f50: 0074 0075 0070 002e 0070 0079 496c 6f63  .t.u.p...p.yIloc
+00001f60: 626c 6f62 0000 0010 0000 011d 0000 009e  blob............
+00001f70: ffff ffff ffff 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/.DS_Store` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/HR.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/HR.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,16 +296,16 @@
                 
                 except:
                     self.model.solve(solver=cp.SCS)
                     # Last resort. Rarely needed.
  
 
             weights = Variable(torch.from_numpy(self.p.value),
-                               requires_grad=True).to(device).to(torch.float32) # Converting primal weights to tensors
-            
+                               requires_grad=True).to(torch.float32).to(device) # Converting primal weights to tensors
+   
             
             if self.output_return == "pytorch_loss_function":
             
                 return torch.dot(weights[0:batch_size], inf_loss) + torch.max(inf_loss)*weights[batch_size]
             
             elif self.output_return == 'weights':
```

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/.DS_Store` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.1/.DS_Store` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.1/mnist_single_param.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.1/mnist_single_param.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/.DS_Store` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/.DS_Store` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/Rice_HR.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_HR/Rice_HR.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/.DS_Store` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/Rice_TRADES.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/Rice_TRADES.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/trades.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/Rice_TRADES/trades.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/preactresnet.cpython-39.pyc` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/preactresnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/utils.cpython-39.pyc` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/preactresnet.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/preactresnet.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.2/utils.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.2/utils.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.3/CIFAR_10_all_error_sources.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.3/CIFAR_10_all_error_sources.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/Section_6.3/resnet.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/Section_6.3/resnet.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/__pycache__/helper_functions.cpython-39.pyc` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/__pycache__/helper_functions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks/Paper_experiments/helper_functions.py` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks/Paper_experiments/helper_functions.py`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/PKG-INFO` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HR-Neural-Networks
-Version: 1.0.5
+Version: 1.0.6
 Summary: Holistic Robust Neural Networks
 Home-page: https://github.com/RyanLucas3/HR_Neural_Networks
-Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.6.tar.gz
 Author: Amine Bennouna, Bart Van Parys, Ryan Lucas
 Author-email: ryanlu@mit.edu
 License: MIT
 Keywords: Neural Networks,Robustness,Machine Learning,Data Science,Adversarial Attacks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `HR_Neural_Networks-1.0.5/HR_Neural_Networks.egg-info/SOURCES.txt` & `HR_Neural_Networks-1.0.6/HR_Neural_Networks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/LICENSE.txt` & `HR_Neural_Networks-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/.DS_Store` & `HR_Neural_Networks-1.0.6/Misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/Classifiers.png` & `HR_Neural_Networks-1.0.6/Misc/Classifiers.png`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/DRO_gif.gif` & `HR_Neural_Networks-1.0.6/Misc/DRO_gif.gif`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/HD.png` & `HR_Neural_Networks-1.0.6/Misc/HD.png`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/HR.png` & `HR_Neural_Networks-1.0.6/Misc/HR.png`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/Julia.svg` & `HR_Neural_Networks-1.0.6/Misc/Julia.svg`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/SVP-gif.gif` & `HR_Neural_Networks-1.0.6/Misc/SVP-gif.gif`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/colab.svg` & `HR_Neural_Networks-1.0.6/Misc/colab.svg`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/mosek.lic` & `HR_Neural_Networks-1.0.6/Misc/mosek.lic`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/pt_badge.svg` & `HR_Neural_Networks-1.0.6/Misc/pt_badge.svg`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/python.svg` & `HR_Neural_Networks-1.0.6/Misc/python.svg`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/Misc/tf.svg` & `HR_Neural_Networks-1.0.6/Misc/tf.svg`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/PKG-INFO` & `HR_Neural_Networks-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HR_Neural_Networks
-Version: 1.0.5
+Version: 1.0.6
 Summary: Holistic Robust Neural Networks
 Home-page: https://github.com/RyanLucas3/HR_Neural_Networks
-Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.6.tar.gz
 Author: Amine Bennouna, Bart Van Parys, Ryan Lucas
 Author-email: ryanlu@mit.edu
 License: MIT
 Keywords: Neural Networks,Robustness,Machine Learning,Data Science,Adversarial Attacks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `HR_Neural_Networks-1.0.5/README.md` & `HR_Neural_Networks-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/dist/.DS_Store` & `HR_Neural_Networks-1.0.6/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `HR_Neural_Networks-1.0.5/setup.py` & `HR_Neural_Networks-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'HR_Neural_Networks',         # How you named your package folder (MyLib)
   packages = ['HR_Neural_Networks'],   # Chose the same as "name"
-  version = '1.0.5',      # Start with a small number and increase it with every change you make
+  version = '1.0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Holistic Robust Neural Networks',   # Give a short description about your library
   author = 'Amine Bennouna, Bart Van Parys, Ryan Lucas',                   # Type in your name
   author_email = 'ryanlu@mit.edu',      # Type in your E-Mail
   url = 'https://github.com/RyanLucas3/HR_Neural_Networks',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.5.tar.gz',
+  download_url = 'https://github.com/RyanLucas3/HR_Neural_Networks/archive/refs/tags/1.0.6.tar.gz',
   keywords = ['Neural Networks', 'Robustness', 'Machine Learning', "Data Science", "Adversarial Attacks"],   # Keywords that define your package best
   install_requires=[ # I get to this in a second
           'mosek',
           'torchattacks',
           'numpy',
           'cvxpy',
           'torch'
```

