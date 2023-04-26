# Comparing `tmp/astroNN-1.0.1.tar.gz` & `tmp/astroNN-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\astroNN-1.0.1.tar", last modified: Wed Mar  6 00:24:41 2019, max compression
+gzip compressed data, was "astroNN-1.1.0.tar", last modified: Wed Apr 26 18:36:41 2023, max compression
```

## Comparing `astroNN-1.0.1.tar` & `astroNN-1.1.0.tar`

### file list

```diff
@@ -1,69 +1,97 @@
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:41.000000 astroNN-1.0.1/
--rw-rw-rw-   0        0        0       54 2018-12-25 22:25:29.000000 astroNN-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5534 2019-03-06 00:24:41.000000 astroNN-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3920 2019-03-06 00:05:43.000000 astroNN-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:37.000000 astroNN-1.0.1/astroNN/
--rw-rw-rw-   0        0        0      107 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/__init__.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:38.000000 astroNN-1.0.1/astroNN/apogee/
--rw-rw-rw-   0        0        0      845 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/apogee/__init__.py
--rw-rw-rw-   0        0        0     2505 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/apogee/apogee_shared.py
--rw-rw-rw-   0        0        0    13476 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/apogee/chips.py
--rw-rw-rw-   0        0        0    30961 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/apogee/downloader.py
--rw-rw-rw-   0        0        0    12124 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/apogee/plotting.py
--rw-rw-rw-   0        0        0    10800 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/config.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:38.000000 astroNN-1.0.1/astroNN/data/
--rw-rw-rw-   0        0        0     1345 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/data/__init__.py
--rw-rw-rw-   0        0        0  1028531 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/data/anderson_2017_dr14_parallax.npz
--rw-rw-rw-   0        0        0    30184 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/data/aspcap_l31c_masks.npy
--rw-rw-rw-   0        0        0     7642 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/data/dr13_contmask.npy
--rw-rw-rw-   0        0        0     7642 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/data/dr14_contmask.npy
--rw-rw-rw-   0        0        0  8158919 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/data/gaiadr2_apogeedr14_parallax.npz
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:39.000000 astroNN-1.0.1/astroNN/datasets/
--rw-rw-rw-   0        0        0      320 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/datasets/__init__.py
--rw-rw-rw-   0        0        0     3754 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/datasets/apogee_distances.py
--rw-rw-rw-   0        0        0     2087 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/datasets/apogee_rc.py
--rw-rw-rw-   0        0        0     1366 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/datasets/apokasc.py
--rw-rw-rw-   0        0        0     4743 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/datasets/galaxy10.py
--rw-rw-rw-   0        0        0    36862 2019-01-06 02:59:52.000000 astroNN-1.0.1/astroNN/datasets/h5.py
--rw-rw-rw-   0        0        0     3449 2018-12-25 22:25:29.000000 astroNN-1.0.1/astroNN/datasets/xmatch.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:40.000000 astroNN-1.0.1/astroNN/gaia/
--rw-rw-rw-   0        0        0      527 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/gaia/__init__.py
--rw-rw-rw-   0        0        0    14297 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/gaia/downloader.py
--rw-rw-rw-   0        0        0    21553 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/gaia/gaia_shared.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:40.000000 astroNN-1.0.1/astroNN/lamost/
--rw-rw-rw-   0        0        0      713 2019-03-06 00:05:43.000000 astroNN-1.0.1/astroNN/lamost/__init__.py
--rw-rw-rw-   0        0        0     2669 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/lamost/chips.py
--rw-rw-rw-   0        0        0     1202 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/lamost/lamost_shared.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:40.000000 astroNN-1.0.1/astroNN/models/
--rw-rw-rw-   0        0        0     1737 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/SimpleBayesPolyNN.py
--rw-rw-rw-   0        0        0    12068 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/__init__.py
--rw-rw-rw-   0        0        0    45320 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/apogee_models.py
--rw-rw-rw-   0        0        0    36856 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/base_bayesian_cnn.py
--rw-rw-rw-   0        0        0    20297 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/base_cnn.py
--rw-rw-rw-   0        0        0    38479 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/base_master_nn.py
--rw-rw-rw-   0        0        0    22500 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/base_vae.py
--rw-rw-rw-   0        0        0     9539 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/models/misc_models.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:40.000000 astroNN-1.0.1/astroNN/nn/
--rw-rw-rw-   0        0        0     3000 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/nn/__init__.py
--rw-rw-rw-   0        0        0     3290 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/nn/callbacks.py
--rw-rw-rw-   0        0        0    37315 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/nn/layers.py
--rw-rw-rw-   0        0        0    21838 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/nn/losses.py
--rw-rw-rw-   0        0        0      873 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/nn/metrics.py
--rw-rw-rw-   0        0        0     9160 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/nn/numpy.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:41.000000 astroNN-1.0.1/astroNN/nn/utilities/
--rw-rw-rw-   0        0        0       56 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/nn/utilities/__init__.py
--rw-rw-rw-   0        0        0     2170 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/nn/utilities/generator.py
--rw-rw-rw-   0        0        0     5708 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/nn/utilities/normalizer.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:41.000000 astroNN-1.0.1/astroNN/shared/
--rw-rw-rw-   0        0        0        0 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/shared/__init__.py
--rw-rw-rw-   0        0        0      946 2019-03-06 00:05:44.000000 astroNN-1.0.1/astroNN/shared/custom_warnings.py
--rw-rw-rw-   0        0        0     2563 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/shared/downloader_tools.py
--rw-rw-rw-   0        0        0     3083 2018-12-25 22:25:30.000000 astroNN-1.0.1/astroNN/shared/nn_tools.py
-drwxrwxrwx   0        0        0        0 2019-03-06 00:24:38.000000 astroNN-1.0.1/astroNN.egg-info/
--rw-rw-rw-   0        0        0     5534 2019-03-06 00:24:36.000000 astroNN-1.0.1/astroNN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1544 2019-03-06 00:24:37.000000 astroNN-1.0.1/astroNN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-03-06 00:24:36.000000 astroNN-1.0.1/astroNN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2019-03-06 00:24:36.000000 astroNN-1.0.1/astroNN.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2019-03-06 00:24:37.000000 astroNN-1.0.1/astroNN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-03-06 00:24:41.000000 astroNN-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2350 2019-03-06 00:21:40.000000 astroNN-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.930339 astroNN-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 18:35:07.000000 astroNN-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 18:35:07.000000 astroNN-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-26 18:36:41.930339 astroNN-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-26 18:35:07.000000 astroNN-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.910339 astroNN-1.1.0/astroNN/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.914339 astroNN-1.1.0/astroNN/apogee/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/apogee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/apogee/apogee_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/apogee/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40447 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/apogee/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.922339 astroNN-1.1.0/astroNN/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1028531 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/anderson_2017_dr14_parallax.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    30184 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/aspcap_l31c_masks.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/dr13_contmask.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/dr14_contmask.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/dr16_contmask.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/dr17_contmask.npy
+-rw-r--r--   0 runner    (1001) docker     (123)  8158919 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/gaiadr2_apogeedr14_parallax.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/tf1_12.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/tf1_14.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/data/tf2_5.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/datasets/apogee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/datasets/galaxy10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/datasets/galaxy10sdss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/datasets/h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/datasets/xmatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/gaia/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/gaia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/gaia/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21717 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/gaia/gaia_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/lamost/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/lamost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/lamost/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/lamost/lamost_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/SimpleBayesPolyNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63896 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/apogee_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48462 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/base_bayesian_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26273 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/base_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33552 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/base_master_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38913 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/base_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/models/misc_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/neuralode/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/neuralode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/neuralode/dop853.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/neuralode/odeint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/neuralode/runge_kutta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39087 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32584 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.926339 astroNN-1.1.0/astroNN/nn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/utilities/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/nn/utilities/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.930339 astroNN-1.1.0/astroNN/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/downloader_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/nn_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25778 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-26 18:35:07.000000 astroNN-1.1.0/astroNN/shared/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.914339 astroNN-1.1.0/astroNN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-26 18:36:41.000000 astroNN-1.1.0/astroNN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-26 18:36:41.000000 astroNN-1.1.0/astroNN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:36:41.000000 astroNN-1.1.0/astroNN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-26 18:36:41.000000 astroNN-1.1.0/astroNN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 18:36:41.000000 astroNN-1.1.0/astroNN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:36:41.930339 astroNN-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-26 18:35:07.000000 astroNN-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:36:41.930339 astroNN-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_apogee_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_apogee_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_gaia_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_lamost_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_loss_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_neuralODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_numpy_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_paper_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-04-26 18:35:07.000000 astroNN-1.1.0/tests/travis_tf_1_12.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `astroNN-1.0.1/README.rst` & `astroNN-1.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-.. image:: http://astronn.readthedocs.io/en/latest/_static/astroNN_icon_withname.png
-
-|
-
-.. image:: https://readthedocs.org/projects/astronn/badge/?version=latest
-   :target: http://astronn.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://img.shields.io/github/license/henrysky/astroNN.svg
-   :target: https://github.com/henrysky/astroNN/blob/master/LICENSE
-   :alt: GitHub license
-
-.. image:: https://travis-ci.org/henrysky/astroNN.svg?branch=master
-   :target: https://travis-ci.org/henrysky/astroNN
-   :alt: Build Status
-
-.. image:: https://img.shields.io/coveralls/henrysky/astroNN.svg
-   :target: https://coveralls.io/github/henrysky/astroNN?branch=master
-   :alt: Coverage Status
-
-.. image:: https://badge.fury.io/py/astroNN.svg
-    :target: https://badge.fury.io/py/astroNN
-
-.. image:: http://img.shields.io/badge/DOI-10.1093/mnras/sty3217-blue.svg
-   :target: http://dx.doi.org/10.1093/mnras/sty3217
-
-Getting Started
-=================
-
-astroNN is a python package to do various kinds of neural networks with targeted application in astronomy by using Keras
-as model and training prototyping, but at the same time take advantage of Tensorflow's flexibility.
-
-For non-astronomy applications, astroNN contains custom loss functions and layers which are compatible with Tensorflow
-or Keras with Tensorflow backend. The custom loss functions mostly designed to deal with incomplete labels.
-astroNN contains demo for implementing Bayesian Neural Net with Dropout Variational Inference in which you can get
-reasonable uncertainty estimation and other neural nets.
-
-For astronomy applications, astroNN contains some tools to deal with APOGEE, Gaia and LAMOST data. astroNN is mainly designed
-to apply neural nets on APOGEE spectra analysis and predicting luminosity from spectra using data from Gaia
-parallax with reasonable uncertainty from Bayesian Neural Net. Generally, astroNN can handle 2D and 2D colored images too.
-Currently astroNN is a python package being developed by the main author to facilitate his research
-project on deep learning application in stellar and galactic astronomy using SDSS APOGEE, Gaia and LAMOST data.
-
-For learning purpose, astroNN includes a deep learning toy dataset for astronomer - `Galaxy10 Dataset`_.
-
-
-`astroNN Documentation`_
-
-`Quick Start guide`_
-
-`Uncertainty Analysis of Neural Nets with Variational Methods`_
-
-
-Acknowledging astroNN
------------------------
-
-| Please cite the following paper that describes astroNN if astroNN used in your research as well as consider linking it to https://github.com/henrysky/astroNN
-| **Deep learning of multi-element abundances from high-resolution spectroscopic data** [`arXiv:1804.08622`_][`ADS`_]
-
-.. _arXiv:1804.08622: https://arxiv.org/abs/1808.04428
-.. _ADS: https://ui.adsabs.harvard.edu/#abs/2019MNRAS.483.3255L/
-
-Authors
--------------
--  | **Henry Leung** - *Initial work and developer* - henrysky_
-   | Astronomy Student, University of Toronto
-   | Contact Henry: henrysky.leung [at] mail.utoronto.ca
-
--  | **Jo Bovy** - *Project Supervisor* - jobovy_
-   | Astronomy Professor, University of Toronto
-
-License
--------------
-This project is licensed under the MIT License - see the `LICENSE`_ file for details
-
-.. _LICENSE: LICENSE
-.. _henrysky: https://github.com/henrysky
-.. _jobovy: https://github.com/jobovy
-
-.. _astroNN Documentation: http://astronn.readthedocs.io/
-.. _Quick Start guide: http://astronn.readthedocs.io/en/latest/quick_start.html
-.. _Galaxy10 Dataset: http://astronn.readthedocs.io/en/latest/galaxy10.html
-.. _Galaxy10 Tutorial Notebook: https://github.com/henrysky/astroNN/blob/master/demo_tutorial/galaxy10/Galaxy10_Tutorial.ipynb
-.. _Uncertainty Analysis of Neural Nets with Variational Methods: https://github.com/henrysky/astroNN/tree/master/demo_tutorial/NN_uncertainty_analysis
+.. image:: https://raw.githubusercontent.com/henrysky/astroNN/master/astroNN_icon_withname.png
+   :width: 200px
+   :align: center
+
+|
+
+.. image:: https://readthedocs.org/projects/astronn/badge/?version=latest
+   :target: http://astronn.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+.. image:: https://img.shields.io/github/license/henrysky/astroNN.svg
+   :target: https://github.com/henrysky/astroNN/blob/master/LICENSE
+   :alt: GitHub license
+
+.. image:: https://github.com/henrysky/astroNN/workflows/CI/badge.svg
+   :target: https://github.com/henrysky/astroNN/actions
+   :alt: Build Status
+
+.. image:: https://codecov.io/gh/henrysky/astroNN/branch/master/graph/badge.svg?token=oI3JSmEHvG
+  :target: https://codecov.io/gh/henrysky/astroNN
+
+.. image:: https://badge.fury.io/py/astroNN.svg
+    :target: https://badge.fury.io/py/astroNN
+
+.. image:: http://img.shields.io/badge/DOI-10.1093/mnras/sty3217-blue.svg
+   :target: http://dx.doi.org/10.1093/mnras/sty3217
+
+Getting Started
+=================
+
+astroNN is a python package to do various kinds of neural networks with targeted application in astronomy by using Keras API
+as model and training prototyping, but at the same time take advantage of Tensorflow's flexibility.
+
+For non-astronomy applications, astroNN contains custom loss functions and layers which are compatible with Tensorflow. The custom loss functions mostly designed to deal with incomplete labels.
+astroNN contains demo for implementing Bayesian Neural Net with Dropout Variational Inference in which you can get
+reasonable uncertainty estimation and other neural nets.
+
+For astronomy applications, astroNN contains some tools to deal with APOGEE, Gaia and LAMOST data. astroNN is mainly designed
+to apply neural nets on APOGEE spectra analysis and predicting luminosity from spectra using data from Gaia
+parallax with reasonable uncertainty from Bayesian Neural Net. Generally, astroNN can handle 2D and 2D colored images too.
+Currently astroNN is a python package being developed by the main author to facilitate his research
+project on deep learning application in stellar and galactic astronomy using SDSS APOGEE, Gaia and LAMOST data.
+
+For learning purpose, astroNN includes a deep learning toy dataset for astronomer - `Galaxy10 Dataset`_.
+
+
+`astroNN Documentation`_
+
+`Quick Start guide`_
+
+`Uncertainty Analysis of Neural Nets with Variational Methods`_
+
+
+Acknowledging astroNN
+-----------------------
+
+| Please cite the following paper that describes astroNN if astroNN is used in your research as well as linking it to https://github.com/henrysky/astroNN
+| **Deep learning of multi-element abundances from high-resolution spectroscopic data** [`arXiv:1808.04428`_][`ADS`_]
+
+.. _arXiv:1808.04428: https://arxiv.org/abs/1808.04428
+.. _ADS: https://ui.adsabs.harvard.edu/abs/2019MNRAS.483.3255L/abstract
+
+Authors
+-------------
+-  | **Henry Leung** - *Initial work and developer* - henrysky_
+   | Astronomy Student, University of Toronto
+   | Contact Henry: henrysky.leung [at] utoronto.ca
+
+-  | **Jo Bovy** - *Project Supervisor* - jobovy_
+   | Astronomy Professor, University of Toronto
+
+License
+-------------
+This project is licensed under the MIT License - see the `LICENSE`_ file for details
+
+.. _LICENSE: LICENSE
+.. _henrysky: https://github.com/henrysky
+.. _jobovy: https://github.com/jobovy
+
+.. _astroNN Documentation: http://astronn.readthedocs.io/
+.. _Quick Start guide: http://astronn.readthedocs.io/en/latest/quick_start.html
+.. _Galaxy10 Dataset: http://astronn.readthedocs.io/en/latest/galaxy10.html
+.. _Galaxy10 Tutorial Notebook: https://github.com/henrysky/astroNN/blob/master/demo_tutorial/galaxy10/Galaxy10_Tutorial.ipynb
+.. _Uncertainty Analysis of Neural Nets with Variational Methods: https://github.com/henrysky/astroNN/tree/master/demo_tutorial/NN_uncertainty_analysis
```

### Comparing `astroNN-1.0.1/astroNN/apogee/apogee_shared.py` & `astroNN-1.1.0/astroNN/apogee/apogee_shared.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,93 @@
-# ---------------------------------------------------------#
-#   astroNN.apogee.apogee_shared: shared functions for apogee
-# ---------------------------------------------------------#
-
-import os
-
-
-def apogee_env():
-    """
-    Get APOGEE environment variable
-
-    :return: path to APOGEE local dir
-    :rtype: str
-    :History: 2017-Oct-26 - Written - Henry Leung (University of Toronto)
-    """
-    from astroNN.config import ENVVAR_WARN_FLAG
-    _APOGEE = os.getenv('SDSS_LOCAL_SAS_MIRROR')
-    if _APOGEE is None and ENVVAR_WARN_FLAG is True:
-        print("WARNING! APOGEE environment variable SDSS_LOCAL_SAS_MIRROR not set")
-
-    return _APOGEE
-
-
-def apogee_default_dr(dr=None):
-    """
-    Check if dr argument is provided, if none then use default
-
-    :param dr: APOGEE DR
-    :type dr: int
-    :return: APOGEE DR
-    :rtype: int
-    :History:
-        | 2017-Oct-26 - Written - Henry Leung (University of Toronto)
-        | 2018-Sept-08 - Updated - Henry Leung (University of Toronto)
-    """
-    if dr == 15:
-        print("SDSS APOGEE DR15 is equivalent to DR14, so astroNN is using DR14 even you set DR15")
-        dr = 14
-
-    if dr is None:
-        try:
-            redux_ver = os.environ["RESULTS_VERS"]  # RESULTS_VERS is from Jo Bovy APOGEE Tool
-            if redux_ver is "v402":
-                dr = 11
-            elif redux_ver == "v603":
-                dr = 12
-            elif redux_ver == "l30e.2":
-                dr = 13
-            elif redux_ver == "l31c.2":
-                dr = 14
-        except KeyError:
-            pass
-
-        if dr is None:  # if it is still None
-            dr = 14
-            print(f'dr is not provided, using default dr={dr}')
-    else:
-        pass
-
-    return dr
-
-
-def apogeeid_digit(arr):
-    """
-    NAME:
-        apogeeid_digit
-    PURPOSE:
-        Extract digits from apogeeid because its too painful to deal with APOGEE ID in h5py
-    INPUT:
-        arr (ndarray): apogee_id
-    OUTPUT:
-        apogee_id with digits only (ndarray)
-    HISTORY:
-        2017-Oct-26 - Written - Henry Leung (University of Toronto)
-    """
-    import numpy as np
-    if isinstance(arr, np.ndarray) or isinstance(arr, list):
-        arr_copy = np.array(arr)  # make a copy
-        for i in range(arr_copy.shape[0]):
-            arr_copy[i] = str(''.join(filter(str.isdigit, arr_copy[i])))
-        return arr_copy
-    else:
-        return str(''.join(filter(str.isdigit, arr)))
+# ---------------------------------------------------------#
+#   astroNN.apogee.apogee_shared: shared functions for apogee
+# ---------------------------------------------------------#
+
+import os
+
+
+def apogee_env():
+    """
+    Get APOGEE environment variable
+
+    :return: path to APOGEE local dir
+    :rtype: str
+    :History: 2017-Oct-26 - Written - Henry Leung (University of Toronto)
+    """
+    from astroNN.config import ENVVAR_WARN_FLAG
+
+    _APOGEE = os.getenv("SDSS_LOCAL_SAS_MIRROR")
+    if _APOGEE is None and ENVVAR_WARN_FLAG is True:
+        print("WARNING! APOGEE environment variable SDSS_LOCAL_SAS_MIRROR not set")
+
+    return _APOGEE
+
+
+def apogee_default_dr(dr=None):
+    """
+    Check if dr argument is provided, if none then use default
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :return: APOGEE DR
+    :rtype: int
+    :History:
+        | 2017-Oct-26 - Written - Henry Leung (University of Toronto)
+        | 2018-Sept-08 - Updated - Henry Leung (University of Toronto)
+    """
+    if dr == 15:
+        print(
+            "SDSS APOGEE DR15 is equivalent to DR14, so astroNN is using DR14 even you set DR15"
+        )
+        dr = 14
+
+    if dr is None:
+        try:
+            redux_ver = os.environ[
+                "RESULTS_VERS"
+            ]  # RESULTS_VERS is from Jo Bovy APOGEE Tool
+            if redux_ver == "v402":
+                dr = 11
+            elif redux_ver == "v603":
+                dr = 12
+            elif redux_ver == "l30e.2":
+                dr = 13
+            elif redux_ver == "l31c.2":
+                dr = 14
+            elif redux_ver == "l33":
+                dr = 16
+            elif redux_ver == "dr17":
+                dr = 17
+        except KeyError:
+            pass
+
+        if dr is None:  # if it is still None
+            dr = 17
+            print(f"dr is not provided, using default dr={dr}")
+    else:
+        pass
+
+    return dr
+
+
+def apogeeid_digit(arr):
+    """
+    NAME:
+        apogeeid_digit
+    PURPOSE:
+        Extract digits from apogeeid because its too painful to deal with APOGEE ID in h5py
+    INPUT:
+        arr (ndarray): apogee_id
+    OUTPUT:
+        apogee_id with digits only (ndarray)
+    HISTORY:
+        2017-Oct-26 - Written - Henry Leung (University of Toronto)
+    """
+    import numpy as np
+
+    if isinstance(arr, np.ndarray) or isinstance(arr, list):
+        arr_copy = np.array(arr)  # make a copy
+        for i in range(arr_copy.shape[0]):
+            arr_copy[i] = str("".join(filter(str.isdigit, arr_copy[i])))
+        return arr_copy
+    else:
+        return str("".join(filter(str.isdigit, arr)))
```

### Comparing `astroNN-1.0.1/astroNN/apogee/chips.py` & `astroNN-1.1.0/astroNN/apogee/chips.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,343 +1,420 @@
-# ---------------------------------------------------------#
-#   astroNN.apogee.chips: tools for dealing with apogee camera chips
-# ---------------------------------------------------------#
-
-import os
-
-import numpy as np
-
-import astroNN
-from astroNN.apogee.apogee_shared import apogee_default_dr
-
-
-def chips_pix_info(dr=None):
-    """
-    To return chips info according to dr
-
-    :param dr: data release
-    :type dr: Union(int, NoneType)
-    :return:
-        | The starting and ending pixels location of APOGEE camera chips in the original 8575 pixels spectra
-        |   - list[0] refers to the location where blue chips starts
-        |   - list[1] refers to the location where blue chips ends
-        |   - list[2] refers to the location where green chips starts
-        |   - list[3] refers to the location where blue chips end
-        |   - list[4] refers to the location where red chips starts
-        |   - list[5] refers to the location where red chips ends
-        |   - list[6] refers to the total number of pixels after deleting gap
-    :rtype: list
-    :History:
-        | 2017-Nov-27 - Written - Henry Leung (University of Toronto)
-        | 2017-Dec-16 - Updated - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 11 or dr == 12:
-        blue_start = 322
-        blue_end = 3242
-        green_start = 3648
-        green_end = 6048
-        red_start = 6412
-        red_end = 8306
-        total_pixel = 7214
-    elif dr == 13 or dr == 14 or dr == 15:
-        blue_start = 246
-        blue_end = 3274
-        green_start = 3585
-        green_end = 6080
-        red_start = 6344
-        red_end = 8335
-        total_pixel = 7514
-    else:
-        raise ValueError('Only DR11 to DR15 are supported')
-
-    return [blue_start, blue_end, green_start, green_end, red_start, red_end, total_pixel]
-
-
-def gap_delete(spectra, dr=None):
-    """
-    To delete the gap between APOGEE CCDs from the original 8575 pixels spectra
-
-    :param spectra: The original 8575 pixels spectrum/spectra
-    :type spectra: ndarray
-    :param dr: data release
-    :type dr: Union(int, NoneType)
-    :return: Gap deleted spectrum/spectra
-    :rtype: ndarray
-    :History:
-        | 2017-Oct-26 - Written - Henry Leung (University of Toronto)
-        | 2017-Dec-16 - Updated - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-    spectra = np.atleast_2d(spectra)
-    info = chips_pix_info(dr=dr)
-
-    if spectra.shape[1] != 8575 and spectra.shape[1] != info[6]:
-        raise EnvironmentError('Are you sure you are giving astroNN APOGEE spectra?')
-    if spectra.shape[1] != info[6]:
-        spectra = spectra[:, np.r_[info[0]:info[1], info[2]:info[3], info[4]:info[5]]]
-
-    return spectra
-
-
-def wavelength_solution(dr=None):
-    """
-    To return wavelegnth_solution, apStarWavegrid was provided by Jo Bovy's apogee tools (Toronto)
-
-    :param dr: data release
-    :type dr: Union(int, NoneType)
-    :return:
-        | lambda_blue, lambda_green, lambda_red which are 3 wavelength solution array
-        |   - lambda_blue refers to the wavelength solution for each pixel in blue chips
-        |   - lambda_green refers to the wavelength solution for each pixel in green chips
-        |   - lambda_red refers to the wavelength solution for each pixel in red chips
-    :rtype: ndarray
-    :History:
-        | 2017-Nov-20 - Written - Henry Leung (University of Toronto)
-        | 2017-Dec-16 - Updated - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-    info = chips_pix_info(dr=dr)
-
-    apstar_wavegrid = 10. ** np.arange(4.179, 4.179 + 8575 * 6. * 10. ** -6., 6. * 10. ** -6.)
-
-    lambda_blue = apstar_wavegrid[info[0]:info[1]]
-    lambda_green = apstar_wavegrid[info[2]:info[3]]
-    lambda_red = apstar_wavegrid[info[4]:info[5]]
-
-    return lambda_blue, lambda_green, lambda_red
-
-
-def chips_split(spectra, dr=None):
-    """
-    To split APOGEE spectra into RGB chips, will delete the gap if detected
-
-    :param spectra: APOGEE spectrum/spectra
-    :type spectra: ndarray
-    :param dr: data release
-    :type dr: Union(int, NoneType)
-    :return: 3 ndarrays which are spectra_blue, spectra_green, spectra_red
-    :rtype: ndarray
-    :History:
-        | 2017-Nov-20 - Written - Henry Leung (University of Toronto)
-        | 2017-Dec-17 - Updated - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-    info = chips_pix_info(dr=dr)
-    blue = info[1] - info[0]
-    green = info[3] - info[2]
-    red = info[5] - info[4]
-
-    spectra = np.atleast_2d(spectra)
-
-    if spectra.shape[1] == 8575:
-        spectra = gap_delete(spectra, dr=dr)
-        print("Raw Spectra detected, astroNN has deleted the gap automatically")
-    elif spectra.shape[1] == info[6]:
-        pass
-    else:
-        raise EnvironmentError('Are you sure you are giving astroNN APOGEE spectra?')
-
-    spectra_blue = spectra[:, 0:blue]
-    spectra_green = spectra[:, blue:(blue + green)]
-    spectra_red = spectra[:, (blue + green):(blue + green + red)]
-
-    return spectra_blue, spectra_green, spectra_red
-
-
-def bitmask_boolean(bitmask, target_bit):
-    """
-    Turn bitmask to boolean with provided bitmask array and target bit to mask
-
-    :param bitmask: bitmask
-    :type bitmask: ndarray
-    :param target_bit: target bit to mask
-    :type target_bit: list[int]
-    :return: boolean array, True for clean, False for masked
-    :rtype: ndarray[bool]
-    :History: 2018-Feb-03 - Written - Henry Leung (University of Toronto)
-    """
-    target_bit = np.array(target_bit)
-    target_bit = np.sum(2 ** target_bit)
-    bitmask = np.atleast_2d(bitmask)
-    boolean_output = np.zeros(bitmask.shape, dtype=bool)
-    boolean_output[(bitmask & target_bit) != 0] = True
-    return boolean_output
-
-
-def bitmask_decompositor(bit):
-    """
-    To decompose a bit from bitmask array to individual bit
-
-    :param bit: bitmask
-    :type bit: int
-    :return: boolean array, True for clean, False for masked
-    :rtype: ndarray[bool]
-    :History: 2018-Feb-03 - Written - Henry Leung (University of Toronto)
-    """
-    bitmask_num = int(bit)
-    if bitmask_num < 0:
-        raise ValueError(f"Your number ({bit}) is not valid, this value must not from a bitmask")
-    if bitmask_num == 0:
-        print('0 corresponds to good pixel, thus this bit cannot be decomposed')
-        return None
-    decomposited_bits = [int(np.log2(bitmask_num))]
-    while True:
-        if bitmask_num - 2 ** decomposited_bits[-1] == 0:
-            decomposited_bits.sort()
-            decomposited_bits = np.array(decomposited_bits)
-            break
-        bitmask_num -= 2 ** decomposited_bits[-1]
-        if bitmask_num != 0:
-            decomposited_bits.append(int(np.log2(bitmask_num)))
-
-    return decomposited_bits
-
-
-def continuum(spectra, spectra_err, cont_mask, deg=2):
-    """
-    Fit Chebyshev polynomials to the flux values in the continuum mask by chips.
-    The resulting continuum will have the same shape as `fluxes`.
-
-    :param spectra: spectra
-    :type spectra: ndarray
-    :param spectra_err: spectra uncertainty, same shape as spectra
-    :type spectra_err: ndarray
-    :param cont_mask: continuum mask
-    :type cont_mask: ndarray[bool]
-    :param deg: The degree of Chebyshev polynomial to use in each region, default is 2 which works the best so far
-    :type deg: int
-    :return: normalized spectra, normalized spectra uncertainty
-    :rtype: ndarray, ndarray
-    :History:
-        | 2017-Dec-04 - Written - Henry Leung (University of Toronto)
-        | 2017-Dec-16 - Update - Henry Leung (University of Toronto)
-        | 2018-Mar-21 - Update - Henry Leung (University of Toronto)
-    """
-    spectra = np.atleast_2d(np.array(spectra))
-    spectra_err = np.atleast_2d(np.array(spectra_err))
-    flux_ivars = 1 / (np.square(np.array(spectra_err)) + 1e-8)  # for numerical stability
-
-    pix_element = np.arange(spectra.shape[1])  # Array with size spectra
-
-    for counter, (spectrum, spectrum_err, flux_ivar) in enumerate(zip(spectra, spectra_err, flux_ivars)):
-        fit = np.polynomial.chebyshev.Chebyshev.fit(x=np.arange(spectrum.shape[0])[cont_mask], y=spectrum[cont_mask],
-                                                    w=flux_ivar[cont_mask], deg=deg)
-        spectra[counter] = spectrum / fit(pix_element)
-        spectra_err[counter] = spectrum_err / fit(pix_element)
-
-    return spectra, spectra_err
-
-
-def apogee_continuum(spectra, spectra_err, cont_mask=None, deg=2, dr=None, bitmask=None, target_bit=None,
-                     mask_value=1.):
-    """
-    It is designed only for apogee spectra by fitting Chebyshev polynomials to the flux values in the continuum mask 
-    by chips. The resulting continuum will have the same shape as `fluxes`.
-        
-    :param spectra: spectra
-    :type spectra: ndarray
-    :param spectra_err: spectra uncertainty, same shape as spectra
-    :type spectra_err: ndarray
-    :param cont_mask: continuum mask
-    :type cont_mask: ndarray[bool]
-    :param deg: The degree of Chebyshev polynomial to use in each region, default is 2 which works the best so far
-    :type deg: int
-    :param dr: apogee dr
-    :type dr: int
-    :param bitmask: bitmask array of the spectra, same shape as spectra
-    :type bitmask: ndarray
-    :param target_bit: a list of bit to be masked
-    :type target_bit: Union(int, list[int], ndarray[int])
-    :param mask_value: if a pixel is determined to be a bad pixel, this value will be used to replace that pixel flux
-    :type mask_value: Union(int, float)
-    :return: normalized spectra, normalized spectra uncertainty
-    :rtype: ndarray, ndarray
-    :History: 2018-Mar-21 - Written - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    spectra = gap_delete(spectra, dr=dr)
-    flux_errs = gap_delete(spectra_err, dr=dr)
-
-    spectra_blue, spectra_green, spectra_red = chips_split(spectra, dr=dr)
-    yerrs_blue, yerrs_green, yerrs_red = chips_split(flux_errs, dr=dr)
-
-    if cont_mask is None:
-        maskpath = os.path.join(os.path.dirname(astroNN.__path__[0]), 'astroNN', 'data', f'dr{dr}_contmask.npy')
-        cont_mask = np.load(maskpath)
-
-    con_mask_blue, con_mask_green, con_mask_red = chips_split(cont_mask, dr=dr)
-    con_mask_blue, con_mask_green, con_mask_red = con_mask_blue[0], con_mask_green[0], con_mask_red[0]
-
-    # Continuum chips by chips
-    blue_spectra, blue_spectra_err = continuum(spectra_blue, yerrs_blue, cont_mask=con_mask_blue, deg=deg)
-    green_spectra, green_spectra_err = continuum(spectra_green, yerrs_green, cont_mask=con_mask_green, deg=deg)
-    red_spectra, red_spectra_err = continuum(spectra_red, yerrs_red, cont_mask=con_mask_red, deg=deg)
-
-    normalized_spectra = np.concatenate((blue_spectra, green_spectra, red_spectra), axis=1)
-    normalized_spectra_err = np.concatenate((blue_spectra_err, green_spectra_err, red_spectra_err), axis=1)
-
-    # set negative flux and error as 0
-    normalized_spectra[normalized_spectra < 0.] = 0.
-    normalized_spectra_err[normalized_spectra < 0.] = 0.
-
-    # set inf and nan as 0
-    normalized_spectra[np.isinf(normalized_spectra)] = mask_value
-    normalized_spectra[np.isnan(normalized_spectra)] = mask_value
-    normalized_spectra_err[np.isinf(normalized_spectra)] = 0.
-    normalized_spectra_err[np.isnan(normalized_spectra)] = 0.
-
-    if bitmask is not None:
-        bitmask = gap_delete(bitmask, dr=dr)
-        if target_bit is None:
-            target_bit = [0, 1, 2, 3, 4, 5, 6, 7, 12]
-
-        mask = bitmask_boolean(bitmask, target_bit)
-        normalized_spectra[mask] = mask_value
-        normalized_spectra_err[mask] = mask_value
-
-    return normalized_spectra, normalized_spectra_err
-
-
-def aspcap_mask(elem, dr=None):
-    """
-    | To load ASPCAP elements window masks
-    | DR14 Elements: ``'C', 'CI', 'N', 'O', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'K', 'Ca', 'TI', 'TiII', 'V', 'Cr', 'Mn',
-                     'Fe', 'Co', 'Ni', 'Cu', 'Ge', 'Ce', 'Rb', 'Y', 'Nd'``
-
-    :param elem: element name
-    :type elem: str
-    :param dr: apogee dr
-    :type dr: int
-    :return: mask
-    :rtype: ndarray[bool]
-    :History: 2018-Mar-24 - Written - Henry Leung (University of Toronto)
-    """
-    if elem.lower() == 'c1':
-        elem = 'CI'
-
-    elif elem.lower() == 'ti2':
-        elem = 'TiII'
-
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 14:
-        aspcap_code = 'l31c'
-        elem_list = ['C', 'CI', 'N', 'O', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'K', 'Ca', 'TI', 'TiII', 'V', 'Cr', 'Mn',
-                     'Fe', 'Co', 'Ni', 'Cu', 'Ge', 'Ce', 'Rb', 'Y', 'Nd']
-    else:
-        raise ValueError('Only DR14 is supported currently')
-
-    masks = np.load(
-        os.path.join(os.path.dirname(astroNN.__path__[0]), 'astroNN', 'data', f'aspcap_{aspcap_code}_masks.npy'))
-
-    try:
-        # turn everything to lowercase to avoid case-related issue
-        index = [x.lower() for x in elem_list].index(elem.lower())
-    except ValueError:
-        # nicely handle if element not found
-        print(f'Element not found, the only elements for dr{dr} supported are {elem_list}')
-        return None
-
-    return [(masks & 2 ** index) != 0][0]
+# ---------------------------------------------------------#
+#   astroNN.apogee.chips: tools for dealing with apogee camera chips
+# ---------------------------------------------------------#
+
+import os
+import warnings
+
+import numpy as np
+
+import astroNN
+import astroNN.data
+from astroNN.apogee.apogee_shared import apogee_default_dr
+
+
+def chips_pix_info(dr=None):
+    """
+    To return chips info according to dr
+
+    :param dr: data release
+    :type dr: Union(int, NoneType)
+    :return:
+        | The starting and ending pixels location of APOGEE camera chips in the original 8575 pixels spectra
+        |   - list[0] refers to the location where blue chips starts
+        |   - list[1] refers to the location where blue chips ends
+        |   - list[2] refers to the location where green chips starts
+        |   - list[3] refers to the location where blue chips end
+        |   - list[4] refers to the location where red chips starts
+        |   - list[5] refers to the location where red chips ends
+        |   - list[6] refers to the total number of pixels after deleting gap
+    :rtype: list
+    :History:
+        | 2017-Nov-27 - Written - Henry Leung (University of Toronto)
+        | 2017-Dec-16 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 11 or dr == 12:
+        blue_start = 322
+        blue_end = 3242
+        green_start = 3648
+        green_end = 6048
+        red_start = 6412
+        red_end = 8306
+        total_pixel = 7214
+    elif 13 <= dr <= 17:
+        blue_start = 246
+        blue_end = 3274
+        green_start = 3585
+        green_end = 6080
+        red_start = 6344
+        red_end = 8335
+        total_pixel = 7514
+    else:
+        raise ValueError("Only DR11 to DR16 are supported")
+
+    return [
+        blue_start,
+        blue_end,
+        green_start,
+        green_end,
+        red_start,
+        red_end,
+        total_pixel,
+    ]
+
+
+def gap_delete(spectra, dr=None):
+    """
+    To delete the gap between APOGEE CCDs from the original 8575 pixels spectra
+
+    :param spectra: The original 8575 pixels spectrum/spectra
+    :type spectra: ndarray
+    :param dr: data release
+    :type dr: Union(int, NoneType)
+    :return: Gap deleted spectrum/spectra
+    :rtype: ndarray
+    :History:
+        | 2017-Oct-26 - Written - Henry Leung (University of Toronto)
+        | 2017-Dec-16 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+    spectra = np.atleast_2d(spectra)
+    info = chips_pix_info(dr=dr)
+
+    if spectra.shape[1] != 8575 and spectra.shape[1] != info[6]:
+        raise EnvironmentError("Are you sure you are giving astroNN APOGEE spectra?")
+    if spectra.shape[1] != info[6]:
+        spectra = spectra[
+            :, np.r_[info[0] : info[1], info[2] : info[3], info[4] : info[5]]
+        ]
+
+    return spectra
+
+
+def wavelength_solution(dr=None):
+    """
+    To return wavelegnth_solution, apStarWavegrid was provided by Jo Bovy's apogee tools (Toronto)
+
+    :param dr: data release
+    :type dr: Union(int, NoneType)
+    :return:
+        | lambda_blue, lambda_green, lambda_red which are 3 wavelength solution array
+        |   - lambda_blue refers to the wavelength solution for each pixel in blue chips
+        |   - lambda_green refers to the wavelength solution for each pixel in green chips
+        |   - lambda_red refers to the wavelength solution for each pixel in red chips
+    :rtype: ndarray
+    :History:
+        | 2017-Nov-20 - Written - Henry Leung (University of Toronto)
+        | 2017-Dec-16 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+    info = chips_pix_info(dr=dr)
+
+    apstar_wavegrid = 10.0 ** np.arange(
+        4.179, 4.179 + 8575 * 6.0 * 10.0**-6.0, 6.0 * 10.0**-6.0
+    )
+
+    lambda_blue = apstar_wavegrid[info[0] : info[1]]
+    lambda_green = apstar_wavegrid[info[2] : info[3]]
+    lambda_red = apstar_wavegrid[info[4] : info[5]]
+
+    return lambda_blue, lambda_green, lambda_red
+
+
+def chips_split(spectra, dr=None):
+    """
+    To split APOGEE spectra into RGB chips, will delete the gap if detected
+
+    :param spectra: APOGEE spectrum/spectra
+    :type spectra: ndarray
+    :param dr: data release
+    :type dr: Union(int, NoneType)
+    :return: 3 ndarrays which are spectra_blue, spectra_green, spectra_red
+    :rtype: ndarray
+    :History:
+        | 2017-Nov-20 - Written - Henry Leung (University of Toronto)
+        | 2017-Dec-17 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+    info = chips_pix_info(dr=dr)
+    blue = info[1] - info[0]
+    green = info[3] - info[2]
+    red = info[5] - info[4]
+
+    spectra = np.atleast_2d(spectra)
+
+    if spectra.shape[1] == 8575:
+        spectra = gap_delete(spectra, dr=dr)
+        warnings.warn(
+            "Raw spectra with gaps between detectors, gaps are removed automatically"
+        )
+    elif spectra.shape[1] == info[6]:
+        pass
+    else:
+        raise EnvironmentError("Are you sure you are giving me APOGEE spectra?")
+
+    spectra_blue = spectra[:, 0:blue]
+    spectra_green = spectra[:, blue : (blue + green)]
+    spectra_red = spectra[:, (blue + green) : (blue + green + red)]
+
+    return spectra_blue, spectra_green, spectra_red
+
+
+def bitmask_boolean(bitmask, target_bit):
+    """
+    Turn bitmask to boolean with provided bitmask array and target bit to mask
+
+    :param bitmask: bitmask
+    :type bitmask: ndarray
+    :param target_bit: target bit to mask
+    :type target_bit: list[int]
+    :return: boolean array, True for clean, False for masked
+    :rtype: ndarray[bool]
+    :History: 2018-Feb-03 - Written - Henry Leung (University of Toronto)
+    """
+    target_bit = np.array(target_bit)
+    target_bit = np.sum(2**target_bit)
+    bitmask = np.atleast_2d(bitmask)
+    boolean_output = np.zeros(bitmask.shape, dtype=bool)
+    boolean_output[(bitmask & target_bit) != 0] = True
+    return boolean_output
+
+
+def bitmask_decompositor(bit):
+    """
+    To decompose a bit from bitmask array to individual bit
+
+    :param bit: bitmask
+    :type bit: int
+    :return: boolean array, True for clean, False for masked
+    :rtype: ndarray[bool]
+    :History: 2018-Feb-03 - Written - Henry Leung (University of Toronto)
+    """
+    bitmask_num = int(bit)
+    if bitmask_num < 0:
+        raise ValueError(
+            f"Your number ({bit}) is not valid, this value must not from a bitmask"
+        )
+    if bitmask_num == 0:
+        print("0 corresponds to good pixel, thus this bit cannot be decomposed")
+        return None
+    decomposited_bits = [int(np.log2(bitmask_num))]
+    while True:
+        if bitmask_num - 2 ** decomposited_bits[-1] == 0:
+            decomposited_bits.sort()
+            decomposited_bits = np.array(decomposited_bits)
+            break
+        bitmask_num -= 2 ** decomposited_bits[-1]
+        if bitmask_num != 0:
+            decomposited_bits.append(int(np.log2(bitmask_num)))
+
+    return decomposited_bits
+
+
+def continuum(spectra, spectra_err, cont_mask, deg=2):
+    """
+    Fit Chebyshev polynomials to the flux values in the continuum mask by chips.
+    The resulting continuum will have the same shape as `fluxes`.
+
+    :param spectra: spectra
+    :type spectra: ndarray
+    :param spectra_err: spectra uncertainty, same shape as spectra
+    :type spectra_err: ndarray
+    :param cont_mask: continuum mask
+    :type cont_mask: ndarray[bool]
+    :param deg: The degree of Chebyshev polynomial to use in each region, default is 2 which works the best so far
+    :type deg: int
+    :return: normalized spectra, normalized spectra uncertainty
+    :rtype: ndarray, ndarray
+    :History:
+        | 2017-Dec-04 - Written - Henry Leung (University of Toronto)
+        | 2017-Dec-16 - Update - Henry Leung (University of Toronto)
+        | 2018-Mar-21 - Update - Henry Leung (University of Toronto)
+    """
+    spectra = np.atleast_2d(np.array(spectra))
+    spectra_err = np.atleast_2d(np.array(spectra_err))
+    flux_ivars = 1 / (
+        np.square(np.array(spectra_err)) + 1e-8
+    )  # for numerical stability
+
+    pix_element = np.arange(spectra.shape[1])  # Array with size spectra
+
+    for counter, (spectrum, spectrum_err, flux_ivar) in enumerate(
+        zip(spectra, spectra_err, flux_ivars)
+    ):
+        fit = np.polynomial.chebyshev.Chebyshev.fit(
+            x=np.arange(spectrum.shape[0])[cont_mask],
+            y=spectrum[cont_mask],
+            w=flux_ivar[cont_mask],
+            deg=deg,
+        )
+        spectra[counter] = spectrum / fit(pix_element)
+        spectra_err[counter] = spectrum_err / fit(pix_element)
+
+    return spectra, spectra_err
+
+
+def apogee_continuum(
+    spectra,
+    spectra_err,
+    cont_mask=None,
+    deg=2,
+    dr=None,
+    bitmask=None,
+    target_bit=None,
+    mask_value=1.0,
+):
+    """
+    It is designed only for apogee spectra by fitting Chebyshev polynomials to the flux values in the continuum mask
+    by chips. The resulting continuum will have the same shape as `fluxes`.
+
+    :param spectra: spectra
+    :type spectra: ndarray
+    :param spectra_err: spectra uncertainty, same shape as spectra
+    :type spectra_err: ndarray
+    :param cont_mask: continuum mask
+    :type cont_mask: ndarray[bool]
+    :param deg: The degree of Chebyshev polynomial to use in each region, default is 2 which works the best so far
+    :type deg: int
+    :param dr: apogee dr
+    :type dr: int
+    :param bitmask: bitmask array of the spectra, same shape as spectra
+    :type bitmask: ndarray
+    :param target_bit: a list of bit to be masked
+    :type target_bit: Union(int, list[int], ndarray[int])
+    :param mask_value: if a pixel is determined to be a bad pixel, this value will be used to replace that pixel flux
+    :type mask_value: Union(int, float)
+    :return: normalized spectra, normalized spectra uncertainty
+    :rtype: ndarray, ndarray
+    :History: 2018-Mar-21 - Written - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    spectra = gap_delete(spectra, dr=dr)
+    flux_errs = gap_delete(spectra_err, dr=dr)
+
+    spectra_blue, spectra_green, spectra_red = chips_split(spectra, dr=dr)
+    yerrs_blue, yerrs_green, yerrs_red = chips_split(flux_errs, dr=dr)
+
+    if cont_mask is None:
+        maskpath = os.path.join(astroNN.data.datapath(), f"dr{dr}_contmask.npy")
+        cont_mask = np.load(maskpath)
+
+    con_mask_blue, con_mask_green, con_mask_red = chips_split(cont_mask, dr=dr)
+    con_mask_blue, con_mask_green, con_mask_red = (
+        con_mask_blue[0],
+        con_mask_green[0],
+        con_mask_red[0],
+    )
+
+    # Continuum chips by chips
+    blue_spectra, blue_spectra_err = continuum(
+        spectra_blue, yerrs_blue, cont_mask=con_mask_blue, deg=deg
+    )
+    green_spectra, green_spectra_err = continuum(
+        spectra_green, yerrs_green, cont_mask=con_mask_green, deg=deg
+    )
+    red_spectra, red_spectra_err = continuum(
+        spectra_red, yerrs_red, cont_mask=con_mask_red, deg=deg
+    )
+
+    normalized_spectra = np.concatenate(
+        (blue_spectra, green_spectra, red_spectra), axis=1
+    )
+    normalized_spectra_err = np.concatenate(
+        (blue_spectra_err, green_spectra_err, red_spectra_err), axis=1
+    )
+
+    # set negative flux and error as 0
+    normalized_spectra[normalized_spectra < 0.0] = 0.0
+    normalized_spectra_err[normalized_spectra < 0.0] = 0.0
+
+    # set inf and nan as 0
+    normalized_spectra[np.isinf(normalized_spectra)] = mask_value
+    normalized_spectra[np.isnan(normalized_spectra)] = mask_value
+    normalized_spectra_err[np.isinf(normalized_spectra)] = 0.0
+    normalized_spectra_err[np.isnan(normalized_spectra)] = 0.0
+
+    if bitmask is not None:
+        bitmask = gap_delete(bitmask, dr=dr)
+        if target_bit is None:
+            target_bit = [0, 1, 2, 3, 4, 5, 6, 7, 12]
+
+        mask = bitmask_boolean(bitmask, target_bit)
+        normalized_spectra[mask] = mask_value
+        normalized_spectra_err[mask] = mask_value
+
+    return normalized_spectra, normalized_spectra_err
+
+
+def aspcap_mask(elem, dr=None):
+    """
+    | To load ASPCAP elements window masks
+    | DR14 Elements: ``'C', 'CI', 'N', 'O', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'K', 'Ca', 'TI', 'TiII', 'V', 'Cr', 'Mn',
+                     'Fe', 'Co', 'Ni', 'Cu', 'Ge', 'Ce', 'Rb', 'Y', 'Nd'``
+
+    :param elem: element name
+    :type elem: str
+    :param dr: apogee dr
+    :type dr: int
+    :return: mask
+    :rtype: ndarray[bool]
+    :History: 2018-Mar-24 - Written - Henry Leung (University of Toronto)
+    """
+    if elem.lower() == "c1":
+        elem = "CI"
+
+    elif elem.lower() == "ti2":
+        elem = "TiII"
+
+    dr = apogee_default_dr(dr=dr)
+
+    if 14 <= dr <= 17:
+        aspcap_code = "l31c"
+        elem_list = [
+            "C",
+            "CI",
+            "N",
+            "O",
+            "Na",
+            "Mg",
+            "Al",
+            "Si",
+            "P",
+            "S",
+            "K",
+            "Ca",
+            "TI",
+            "TiII",
+            "V",
+            "Cr",
+            "Mn",
+            "Fe",
+            "Co",
+            "Ni",
+            "Cu",
+            "Ge",
+            "Ce",
+            "Rb",
+            "Y",
+            "Nd",
+        ]
+    else:
+        raise ValueError("Only DR14-DR16 is supported currently")
+
+    masks = np.load(
+        os.path.join(astroNN.data.datapath(), f"aspcap_{aspcap_code}_masks.npy")
+    )
+
+    try:
+        # turn everything to lowercase to avoid case-related issue
+        index = [x.lower() for x in elem_list].index(elem.lower())
+    except ValueError:
+        # nicely handle if element not found
+        print(
+            f"Element not found, the only elements for dr{dr} supported are {elem_list}"
+        )
+        return None
+
+    return [(masks & 2**index) != 0][0]
```

### Comparing `astroNN-1.0.1/astroNN/apogee/downloader.py` & `astroNN-1.1.0/astroNN/apogee/downloader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,688 +1,1028 @@
-# ---------------------------------------------------------#
-#   astroNN.apogee.downloader: download apogee files
-# ---------------------------------------------------------#
-
-import getpass
-import os
-import urllib.request
-
-import numpy as np
-from astropy.io import fits
-
-from astroNN.apogee.apogee_shared import apogee_env, apogee_default_dr
-from astroNN.shared.downloader_tools import TqdmUpTo
-from astroNN.shared.downloader_tools import sha1_checksum
-
-currentdir = os.getcwd()
-
-# global var
-warning_flag = False
-_ALLSTAR_TEMP = {}
-__apogee_credentials_username = None
-__apogee_credentials_pw = None
-
-
-def __apogee_credentials_downloader(url, fullfilename):
-    """
-    Download file at the URL with apogee credentials, this function will prompt for username and password
-
-    :param dr: URL
-    :type dr: str
-    :param fullfilename: Full file name including path in local system
-    :type dr: str
-    :return: None
-    :History: 2018-Aug-31 - Written - Henry Leung (University of Toronto)
-    """
-    passman = urllib.request.HTTPPasswordMgrWithDefaultRealm()
-    global __apogee_credentials_username
-    global __apogee_credentials_pw
-    if __apogee_credentials_username is None:
-        print("You are trying to access APOGEE proprietary data...Please provide username and password...")
-        print("You are trying to access APOGEE proprietary data...Please provide username and password...")
-        __apogee_credentials_username = input('Username: ')
-        __apogee_credentials_pw = getpass.getpass('Password: ')
-    passman.add_password(None, url, __apogee_credentials_username, __apogee_credentials_pw)
-    authhandler = urllib.request.HTTPBasicAuthHandler(passman)
-    opener = urllib.request.build_opener(authhandler)
-    urllib.request.install_opener(opener)
-    try:
-        urllib.request.urlretrieve(url, fullfilename)
-    except urllib.request.HTTPError as emsg:
-        if '401' in str(emsg):
-            raise ConnectionError('Wrong username or password')
-        elif '404' in str(emsg):
-            print(f'{url} cannot be found on server, skipped')
-            fullfilename = warning_flag
-        else:
-            print(f"Unknown error occurred - {emsg}")
-            fullfilename = warning_flag
-
-    return fullfilename
-
-
-def allstar(dr=None, flag=None):
-    """
-    Download the allStar file (catalog of ASPCAP stellar parameters and abundances from combined spectra)
-
-    :param dr: APOGEE DR
-    :type dr: int
-    :param flag: 0: normal, 1: force to re-download
-    :type flag: int
-    :return: full file path and download in background if not found locally, False if cannot be found on server
-    :rtype: str
-    :History: 2017-Oct-09 - Written - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 13:
-        file_hash = '1718723ada3018de94e1022cd57d4d950a74f91f'
-
-        # Check if directory exists
-        fullfoldername = os.path.join(apogee_env(), 'dr13/apogee/spectro/redux/r6/stars/l30e/l30e.2/')
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-        filename = 'allStar-l30e.2.fits'
-        fullfilename = os.path.join(fullfoldername, filename)
-        url = f'https://data.sdss.org/sas/dr13/apogee/spectro/redux/r6/stars/l30e/l30e.2/{filename}'
-    elif dr == 14:
-        file_hash = 'a7e1801924661954da792e377ad54f412219b105'
-
-        fullfoldername = os.path.join(apogee_env(), 'dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/')
-        # Check if directory exists
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-        filename = 'allStar-l31c.2.fits'
-        fullfilename = os.path.join(fullfoldername, filename)
-        url = f'https://data.sdss.org/sas/dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/{filename}'
-    elif dr == 16:
-        file_hash = '4d191dede9048046e31429bc1890ab3f241739f5'
-
-        fullfoldername = os.path.join(apogee_env(), 'apogeework/apogee/spectro/aspcap/r10/l31c/')
-        # Check if directory exists
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-        filename = 'allStar-r10-l31c-58297.fits'
-        fullfilename = os.path.join(fullfoldername, filename)
-        url = f'https://data.sdss.org/sas/apogeework/apogee/spectro/aspcap/r10/l31c/{filename}'
-    else:
-        raise ValueError('allstar() only supports APOGEE DR13-DR16')
-
-    # check file integrity
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash.lower():
-            print('File corruption detected, astroNN attempting to download again')
-            allstar(dr=dr, flag=1)
-        else:
-            print(fullfilename + ' was found!')
-
-    # Check if files exists
-    if not os.path.isfile(os.path.join(fullfoldername, filename)) or flag == 1:
-        with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=url.split('/')[-1]) as t:
-            try:
-                urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
-                print(f'Downloaded DR{dr:d} allStar file catalog successfully to {fullfilename}')
-                checksum = sha1_checksum(fullfilename)
-                if checksum != file_hash.lower():
-                    print('File corruption detected, astroNN attempting to download again')
-                    allstar(dr=dr, flag=1)
-            except urllib.request.HTTPError as emsg:
-                if '401' in str(emsg):
-                    fullfilename = __apogee_credentials_downloader(url, fullfilename)
-                elif '404' in str(emsg):
-                    print(f'{url} cannot be found on server, skipped')
-                    fullfilename = warning_flag
-                else:
-                    print(f"Unknown error occurred - {emsg}")
-                    fullfilename = warning_flag
-
-    return fullfilename
-
-
-def allstarcannon(dr=None, flag=None):
-    """
-    Download the allStarCannon file (catalog of Cannon stellar parameters and abundances from combined spectra)
-
-    :param dr: APOGEE DR
-    :type dr: int
-    :param flag: 0: normal, 1: force to re-download
-    :type flag: int
-    :return: full file path and download in background if not found locally, False if cannot be found on server
-    :rtype: str
-    :History: 2017-Oct-24 - Written - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 14:
-        # Check if directory exists
-        fullfoldername = os.path.join(apogee_env(), 'dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/cannon/')
-        # Check if directory exists
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-        filename = 'allStarCannon-l31c.2.fits'
-        fullfilename = os.path.join(fullfoldername, filename)
-        file_hash = '64d485e95b3504df0b795ab604e21a71d5c7ae45'
-
-        url = f'https://data.sdss.org/sas/dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/cannon/{filename}'
-    else:
-        raise ValueError('allstarcannon() only supports APOGEE DR14-DR15')
-
-    # check file integrity
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash.lower():
-            print('File corruption detected, astroNN attempting to download again')
-            allstarcannon(dr=dr, flag=1)
-        else:
-            print(fullfilename + ' was found!')
-
-    # Check if files exists
-    if not os.path.isfile(os.path.join(fullfoldername, filename)) or flag == 1:
-        with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=url.split('/')[-1]) as t:
-            urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
-            print(f'Downloaded DR{dr:d} allStarCannon file catalog successfully to {fullfilename}')
-            checksum = sha1_checksum(fullfilename)
-            if checksum != file_hash.lower():
-                print('File corruption detected, astroNN attempting to download again')
-                allstarcannon(dr=dr, flag=1)
-
-    return fullfilename
-
-
-def allvisit(dr=None, flag=None):
-    """
-    Download the allVisit file (catalog of properties from individual visit spectra)
-
-    :param dr: APOGEE DR
-    :type dr: int
-    :param flag: 0: normal, 1: force to re-download
-    :type flag: int
-    :return: full file path and download in background if not found locally, False if cannot be found on server
-    :rtype: str
-    :History: 2017-Oct-11 - Written - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 13:
-        file_hash = '2a3b13ccd40a2c8aea8321be9630117922d55b51'
-
-        # Check if directory exists
-        fullfilepath = os.path.join(apogee_env(), 'dr13/apogee/spectro/redux/r6/')
-        if not os.path.exists(fullfilepath):
-            os.makedirs(fullfilepath)
-        filename = 'allVisit-l30e.2.fits'
-        fullfilename = os.path.join(fullfilepath, filename)
-        url = f'https://data.sdss.org/sas/dr13/apogee/spectro/redux/r6/{filename}'
-    elif dr == 14:
-        file_hash = 'abcecbcdc5fe8d00779738702c115633811e6bbd'
-
-        # Check if directory exists
-        fullfilepath = os.path.join(apogee_env(), 'dr14/apogee/spectro/redux/r8/')
-        if not os.path.exists(fullfilepath):
-            os.makedirs(fullfilepath)
-        filename = 'allVisit-l31c.2.fits'
-        fullfilename = os.path.join(fullfilepath, filename)
-        url = f'https://data.sdss.org/sas/dr14/apogee/spectro/redux/r8/{filename}'
-    else:
-        raise ValueError('allvisit() only supports APOGEE DR13-DR15')
-
-    # check file integrity
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash.lower():
-            print('File corruption detected, astroNN attempting to download again')
-            allvisit(dr=dr, flag=1)
-        else:
-            print(fullfilename + ' was found!')
-    elif not os.path.isfile(os.path.join(fullfilepath, filename)) or flag == 1:
-        with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=url.split('/')[-1]) as t:
-            urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
-            print(f'Downloaded DR{dr:d} allVisit file catalog successfully to {fullfilepath}')
-            checksum = sha1_checksum(fullfilename)
-            if checksum != file_hash.lower():
-                print('File corruption detected, astroNN attempting to download again')
-                allstar(dr=dr, flag=1)
-
-    return fullfilename
-
-
-def combined_spectra(dr=None, location=None, apogee=None, telescope=None, verbose=1, flag=None):
-    """
-    Download the required combined spectra file a.k.a aspcapStar
-
-    :param dr: APOGEE DR
-    :type dr: int
-    :param location: Location ID [Optional]
-    :type location: int
-    :param apogee: Apogee ID
-    :type apogee: str
-    :param telescope: Telescope ID, for example 'apo25m' or 'lco25m'
-    :type telescope: str
-    :param flag: 0: normal, 1: force to re-download
-    :type flag: int
-
-    :return: full file path and download in background if not found locally, False if cannot be found on server
-    :rtype: str
-    :History:
-        | 2017-Oct-15 - Written - Henry Leung (University of Toronto)
-        | 2018-Aug-31 - Updated - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if location is None:    # for DR16=<, location is expected to be none because field is used
-        global _ALLSTAR_TEMP
-        if not str(f'dr{dr}') in _ALLSTAR_TEMP:
-            _ALLSTAR_TEMP[f'dr{dr}'] = fits.getdata(allstar(dr=dr))
-        if telescope is None:
-            matched_idx = [np.nonzero(_ALLSTAR_TEMP[f'dr{dr}']['APOGEE_ID'] == apogee)[0]][0]
-        else:
-            matched_idx = [np.nonzero([(_ALLSTAR_TEMP[f'dr{dr}']['APOGEE_ID'] == apogee) &
-                                       (_ALLSTAR_TEMP[f'dr{dr}']['TELESCOPE'] == telescope)])][0][1]
-        if len(matched_idx) == 0:
-            raise ValueError(f"No entry found in allstar DR{dr} met with your requirement!!")
-
-        location = _ALLSTAR_TEMP[f'dr{dr}']['LOCATION_ID'][matched_idx][0]
-        field = _ALLSTAR_TEMP[f'dr{dr}']['FIELD'][matched_idx][0]
-        telescope = _ALLSTAR_TEMP[f'dr{dr}']['TELESCOPE'][matched_idx][0]
-
-    if dr == 13:
-        reduce_prefix = 'r6'
-        aspcap_code = 'l30e'
-        str1 = f'https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/{location}/'
-
-        filename = f'aspcapStar-{reduce_prefix}-{aspcap_code}.2-{apogee}.fits'
-        hash_filename = f'stars_{aspcap_code}_{aspcap_code}.2_{location}.sha1sum'
-        urlstr = str1 + filename
-
-        # check folder existence
-        fullfoldername = os.path.join(apogee_env(),
-                                      f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/',
-                                      str(location))
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-
-        fullfilename = os.path.join(apogee_env(),
-                                    f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/',
-                                    str(location),
-                                    filename)
-    elif dr == 14:
-        reduce_prefix = 'r8'
-        aspcap_code = 'l31c'
-        str1 = f'https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/{location}/'
-
-        filename = f'aspcapStar-{reduce_prefix}-{aspcap_code}.2-{apogee}.fits'
-        hash_filename = f'stars_{aspcap_code}_{aspcap_code}.2_{location}.sha1sum'
-        urlstr = str1 + filename
-
-        # check folder existence
-        fullfoldername = os.path.join(apogee_env(),
-                                      f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/',
-                                      str(location))
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-
-        fullfilename = os.path.join(apogee_env(),
-                                    f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/',
-                                    str(location),
-                                    filename)
-    elif dr == 16:
-        reduce_prefix = 'r10'
-        aspcap_code = 'l31c'
-        str1 = f'https://data.sdss.org/sas/apogeework/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}/{field}/'
-
-        filename = f'aspcapStar-{reduce_prefix}-{apogee}.fits'
-        hash_filename = f'stars_{reduce_prefix}_{reduce_prefix}.2_{location}.sha1sum'
-        urlstr = str1 + filename
-
-        # check folder existence
-        fullfoldername = os.path.join(apogee_env(),
-                                      f'apogeework/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}',
-                                      str(f'{field}'))
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-
-        fullfilename = os.path.join(apogee_env(),
-                                    f'apogeework/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}',
-                                    str(f'{field}'), filename)
-    else:
-        raise ValueError('combined_spectra() only supports DR13-DR16')
-
-    # check hash file
-    if dr != 16:
-        full_hash_filename = os.path.join(fullfoldername, hash_filename)
-        if not os.path.isfile(full_hash_filename):
-            # return warning flag if the location_id cannot even be found
-            try:
-                urllib.request.urlopen(str1)
-            except urllib.request.HTTPError:
-                return warning_flag
-            urllib.request.urlretrieve(str1 + hash_filename, full_hash_filename)
-
-        hash_list = np.loadtxt(full_hash_filename, dtype='str').T
-    else:
-        # just a dummy list
-        hash_list = np.array([np.array(['yyy', 'yyy', 'yyy']), np.array(['zzz', 'zzz', 'zzz'])])
-
-    # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
-    file_hash = hash_list[0][np.argwhere(hash_list[1] == filename)]
-
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash and len(file_hash) != 0:
-            print('File corruption detected, astroNN attempting to download again')
-            combined_spectra(dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1)
-
-        if verbose == 1:
-            print(fullfilename + ' was found!')
-
-    elif not os.path.isfile(fullfilename) or flag == 1:
-        try:
-            urllib.request.urlretrieve(urlstr, fullfilename)
-            print(f'Downloaded DR{dr} combined file successfully to {fullfilename}')
-            checksum = sha1_checksum(fullfilename)
-            if checksum != file_hash and len(file_hash) != 0:
-                print('File corruption detected, astroNN attempting to download again')
-                combined_spectra(dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1)
-        except urllib.request.HTTPError as emsg:
-            if '401' in str(emsg):
-                fullfilename = __apogee_credentials_downloader(urlstr, fullfilename)
-            elif '404' in str(emsg):
-                print(f'{urlstr} cannot be found on server, skipped')
-                fullfilename = warning_flag
-            else:
-                print(f"Unknown error occurred - {emsg}")
-                fullfilename = warning_flag
-
-    return fullfilename
-
-
-def visit_spectra(dr=None, location=None, apogee=None, telescope=None, verbose=1, flag=None, commission=False):
-    """
-    Download the required individual spectra file a.k.a apStar
-
-    :param dr: APOGEE DR
-    :type dr: int
-    :param location: Location ID [Optional]
-    :type location: int
-    :param apogee: Apogee ID
-    :type apogee: str
-    :param telescope: Telescope ID, for example 'apo25m' or 'lco25m'
-    :type telescope: str
-    :param verbose: verbose
-    :type verbose: int
-    :param flag: 0: normal, 1: force to re-download
-    :type flag: int
-    :param commission: whether the spectra is taken during commissioning
-    :type commission: bool
-
-    :return: full file path and download in background if not found locally, False if cannot be found on server
-    :rtype: str
-    :History:
-        | 2017-Nov-11 - Written - Henry Leung (University of Toronto)
-        | 2018-Aug-31 - Updated - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if location is None:  # for DR16=<, location is expected to be none because field is used
-        global _ALLSTAR_TEMP
-        if not str(f'dr{dr}') in _ALLSTAR_TEMP:
-            _ALLSTAR_TEMP[f'dr{dr}'] = fits.getdata(allstar(dr=dr))
-        if telescope is None:
-            matched_idx = [np.nonzero(_ALLSTAR_TEMP[f'dr{dr}']['APOGEE_ID'] == apogee)[0]][0]
-        else:
-            matched_idx = [np.nonzero([(_ALLSTAR_TEMP[f'dr{dr}']['APOGEE_ID'] == apogee) &
-                                       (_ALLSTAR_TEMP[f'dr{dr}']['TELESCOPE'] == telescope)])][0][1]
-        if len(matched_idx) == 0:
-            raise ValueError(f"No entry found in allstar DR{dr} met with your requirement!!")
-
-        location = _ALLSTAR_TEMP[f'dr{dr}']['LOCATION_ID'][matched_idx][0]
-        field = _ALLSTAR_TEMP[f'dr{dr}']['FIELD'][matched_idx][0]
-        telescope = _ALLSTAR_TEMP[f'dr{dr}']['TELESCOPE'][matched_idx][0]
-
-    if dr == 13:
-        reduce_prefix = 'r6'
-        str1 = f'https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/{location}/'
-        if commission:
-            filename = f'apStarC-{reduce_prefix}-{apogee}.fits'
-        else:
-            filename = f'apStar-{reduce_prefix}-{apogee}.fits'
-        urlstr = str1 + filename
-        hash_filename = f'{reduce_prefix}_stars_apo25m_{location}.sha1sum'
-
-        fullfoldername = os.path.join(apogee_env(), f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/',
-                                      str(location))
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-
-        # check hash file
-        full_hash_filename = os.path.join(fullfoldername, hash_filename)
-        if not os.path.isfile(full_hash_filename):
-            # return warning flag if the location_id cannot even be found
-            try:
-                urllib.request.urlopen(str1)
-            except urllib.request.HTTPError:
-                return warning_flag
-            urllib.request.urlretrieve(str1 + hash_filename, full_hash_filename)
-
-        hash_list = np.loadtxt(full_hash_filename, dtype='str').T
-
-        fullfilename = os.path.join(apogee_env(), f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/',
-                                    str(location), filename)
-
-    elif dr == 14:
-        reduce_prefix = 'r8'
-        str1 = f'https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/{location}/'
-        if commission:
-            filename = f'apStarC-{reduce_prefix}-{apogee}.fits'
-        else:
-            filename = f'apStar-{reduce_prefix}-{apogee}.fits'
-        urlstr = str1 + filename
-        hash_filename = f'{reduce_prefix}_stars_apo25m_{location}.sha1sum'
-
-        fullfoldername = os.path.join(apogee_env(), f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/',
-                                      str(location))
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-
-        # check hash file
-        full_hash_filename = os.path.join(fullfoldername, hash_filename)
-        if not os.path.isfile(full_hash_filename):
-            # return warning flag if the location_id cannot even be found
-            try:
-                urllib.request.urlopen(str1)
-            except urllib.request.HTTPError:
-                return warning_flag
-            urllib.request.urlretrieve(str1 + hash_filename, full_hash_filename)
-
-        hash_list = np.loadtxt(full_hash_filename, dtype='str').T
-
-        fullfilename = os.path.join(apogee_env(), f'dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/',
-                                    str(location), filename)
-
-    elif dr == 16:
-        reduce_prefix = 'r10'
-        str1 = f'https://data.sdss.org/sas/apogeework/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/{field}/'
-        if commission:
-            filename = f'apStarC-{reduce_prefix}-{apogee}.fits'
-        else:
-            filename = f'apStar-{reduce_prefix}-{apogee}.fits'
-        urlstr = str1 + filename
-        hash_filename = f'{reduce_prefix}_stars_apo25m_{location}.sha1sum'
-
-        fullfoldername = os.path.join(apogee_env(),
-                                      f'apogeework/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/',
-                                      str(f'{field}'))
-
-        if not os.path.exists(fullfoldername):
-            os.makedirs(fullfoldername)
-
-        # # check hash file
-        # full_hash_filename = os.path.join(fullfoldername, hash_filename)
-        # if not os.path.isfile(full_hash_filename):
-        #     # return warning flag if the location_id cannot even be found
-        #     try:
-        #         urllib.request.urlopen(str1)
-        #     except urllib.request.HTTPError:
-        #         return warning_flag
-        #     urllib.request.urlretrieve(str1 + hash_filename, full_hash_filename)
-        #
-        # hash_list = np.loadtxt(full_hash_filename, dtype='str').T
-        hash_list = np.array([np.array(['yyy', 'yyy', 'yyy']), np.array(['zzz', 'zzz', 'zzz'])])
-
-        fullfilename = os.path.join(apogee_env(),
-                                    f'apogeework/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/',
-                                    str(f'{field}'), filename)
-
-    else:
-        raise ValueError('visit_spectra() only supports DR13-DR16')
-
-    # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
-    # visit spectra has a different filename in checksum
-    # handle the case where apogee_id cannot be found
-    hash_idx = [i for i, item in enumerate(hash_list[1]) if f'apStar-{reduce_prefix}-{apogee}' in item]
-    file_hash = hash_list[0][hash_idx]
-
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash and len(file_hash) != 0:
-            print('File corruption detected, astroNN attempting to download again')
-            visit_spectra(dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1)
-
-        if verbose:
-            print(fullfilename + ' was found!')
-
-    elif not os.path.isfile(fullfilename) or flag == 1:
-        try:
-            urllib.request.urlretrieve(urlstr, fullfilename)
-            print(f'Downloaded DR{dr} individual visit file successfully to {fullfilename}')
-            checksum = sha1_checksum(fullfilename)
-            if checksum != file_hash and len(file_hash) != 0:
-                print('File corruption detected, astroNN attempting to download again')
-                visit_spectra(dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1)
-        except urllib.request.HTTPError as emsg:
-            if '401' in str(emsg):
-                fullfilename = __apogee_credentials_downloader(urlstr, fullfilename)
-            elif '404' in str(emsg):
-                print(f'{urlstr} cannot be found on server, skipped')
-                fullfilename = warning_flag
-            else:
-                print(f"Unknown error occurred - {emsg}")
-                fullfilename = warning_flag
-
-    return fullfilename
-
-
-def apogee_vac_rc(dr=None, flag=None):
-    """
-    Download the red clumps catalogue
-
-    :param dr: Apogee DR
-    :type dr: int
-    :param flag: Force to download if flag=1
-    :type flag: int
-    :return: full file path
-    :rtype: str
-    :History: 2017-Nov-16 - Written - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 13:
-        file_hash = '5e87eb3ba202f9db24216978dafb19d39d382fc6'
-
-        str1 = 'https://data.sdss.org/sas/dr13/apogee/vac/apogee-rc/cat/'
-        filename = f'apogee-rc-DR{dr}.fits'
-        urlstr = str1 + filename
-        fullfilename = os.path.join(apogee_env(), 'dr13/apogee/vac/apogee-rc/cat/')
-        if not os.path.exists(fullfilename):
-            os.makedirs(fullfilename)
-        fullfilename = os.path.join(apogee_env(), 'dr13/apogee/vac/apogee-rc/cat/', filename)
-
-    elif dr == 14:
-        file_hash = '104513070f1c280954f3d1886cac429dbdf2eaf6'
-
-        str1 = 'https://data.sdss.org/sas/dr14/apogee/vac/apogee-rc/cat/'
-        filename = f'apogee-rc-DR{dr}.fits'
-        urlstr = str1 + filename
-        fullfilename = os.path.join(apogee_env(), 'dr14/apogee/vac/apogee-rc/cat/')
-        if not os.path.exists(fullfilename):
-            os.makedirs(fullfilename)
-        fullfilename = os.path.join(apogee_env(), 'dr14/apogee/vac/apogee-rc/cat/', filename)
-
-    else:
-        raise ValueError('apogee_vac_rc() only supports DR13 or DR14')
-
-    # check file integrity
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash.lower():
-            print('File corruption detected, astroNN attempting to download again')
-            apogee_vac_rc(dr=dr, flag=1)
-        else:
-            print(fullfilename + ' was found!')
-
-    elif not os.path.isfile(fullfilename) or flag == 1:
-        try:
-            with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=urlstr.split('/')[-1]) as t:
-                urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
-                print(f'Downloaded DR{dr} Red Clumps Catalog successfully to {fullfilename}')
-                checksum = sha1_checksum(fullfilename)
-                if checksum != file_hash.lower():
-                    print('File corruption detected, astroNN attempting to download again')
-                    apogee_vac_rc(dr=dr, flag=1)
-        except urllib.request.HTTPError:
-            print(f'{urlstr} cannot be found on server, skipped')
-            fullfilename = warning_flag
-
-    return fullfilename
-
-
-def apogee_distances(dr=None, flag=None):
-    """
-    Download the Apogee Distances catalogue
-
-    :param dr: Apogee DR
-    :type dr: int
-    :param flag: Force to download if flag=1
-    :type flag: int
-    :return: full file path
-    :rtype: str
-    :History: 2018-Jan-24 - Written - Henry Leung (University of Toronto)
-    """
-    dr = apogee_default_dr(dr=dr)
-
-    if dr == 14:
-        file_hash = 'b33c8419be784b1be3d14af3ee9696c6ac31830f'
-
-        str1 = 'https://data.sdss.org/sas/dr14/apogee/vac/apogee-distances/'
-        filename = f'apogee_distances-DR{dr}.fits'
-        urlstr = str1 + filename
-        fullfilename = os.path.join(apogee_env(), 'dr14/apogee/vac/apogee-distances/')
-        if not os.path.exists(fullfilename):
-            os.makedirs(fullfilename)
-        fullfilename = os.path.join(apogee_env(), 'dr14/apogee/vac/apogee-distances/', filename)
-    else:
-        raise ValueError('apogee_distances() only supports DR14')
-
-    # check file integrity
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha1_checksum(fullfilename)
-        if checksum != file_hash.lower():
-            print('File corruption detected, astroNN attempting to download again')
-            apogee_distances(dr=dr, flag=1)
-        else:
-            print(fullfilename + ' was found!')
-
-    elif not os.path.isfile(fullfilename) or flag == 1:
-        try:
-            with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=urlstr.split('/')[-1]) as t:
-                urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
-                print(f'Downloaded DR{dr} Distances successfully to {fullfilename}')
-                checksum = sha1_checksum(fullfilename)
-                if checksum != file_hash.lower():
-                    print('File corruption detected, astroNN attempting to download again')
-                    apogee_distances(dr=dr, flag=1)
-        except urllib.request.HTTPError:
-            print(f'{urlstr} cannot be found on server, skipped')
-            fullfilename = warning_flag
-
-    return fullfilename
+# ---------------------------------------------------------#
+#   astroNN.apogee.downloader: download apogee files
+# ---------------------------------------------------------#
+
+import getpass
+import os
+import urllib.request, urllib.error
+import warnings
+
+import numpy as np
+from astroNN.apogee.apogee_shared import apogee_env, apogee_default_dr
+from astroNN.shared.downloader_tools import TqdmUpTo, filehash
+from astropy.io import fits
+from astroNN.shared import logging as logging
+
+currentdir = os.getcwd()
+
+# global var
+warning_flag = False
+_ALLSTAR_TEMP = {}
+__apogee_credentials_username = None
+__apogee_credentials_pw = None
+
+
+def __apogee_credentials_downloader(url, fullfilename):
+    """
+    Download file at the URL with apogee credentials, this function will prompt for username and password
+
+    :param url: URL
+    :type url: str
+    :param fullfilename: Full file name including path in local system
+    :type fullfilename: str
+    :return: None
+    :History: 2018-Aug-31 - Written - Henry Leung (University of Toronto)
+    """
+    passman = urllib.request.HTTPPasswordMgrWithDefaultRealm()
+    global __apogee_credentials_username
+    global __apogee_credentials_pw
+    if __apogee_credentials_username is None:
+        print(
+            "\nYou are trying to access APOGEE proprietary data...Please provide username and password..."
+        )
+        __apogee_credentials_username = input("Username: ")
+        __apogee_credentials_pw = getpass.getpass("Password: ")
+    passman.add_password(
+        None, url, __apogee_credentials_username, __apogee_credentials_pw
+    )
+    authhandler = urllib.request.HTTPBasicAuthHandler(passman)
+    opener = urllib.request.build_opener(authhandler)
+    urllib.request.install_opener(opener)
+    # Check if directory exists
+    if not os.path.exists(os.path.dirname(fullfilename)):
+        os.makedirs(os.path.dirname(fullfilename))
+    try:
+        with TqdmUpTo(
+            unit="B", unit_scale=True, miniters=1, desc=url.split("/")[-1]
+        ) as t:
+            urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
+    except urllib.error.HTTPError as emsg:
+        if "401" in str(emsg):
+            __apogee_credentials_username = None
+            __apogee_credentials_pw = None
+            raise ConnectionError("Wrong username or password")
+        elif "404" in str(emsg):
+            warnings.warn(f"{url} cannot be found on server, skipped")
+            fullfilename = warning_flag
+        else:
+            # don't raise error, so a batch downloading script will keep running despite some files not found
+            warnings.warn(f"Unknown error occurred - {emsg}", RuntimeWarning)
+            fullfilename = warning_flag
+
+    return fullfilename
+
+
+def allstar(dr=None, flag=None):
+    """
+    Download the allStar file (catalog of ASPCAP stellar parameters and abundances from combined spectra)
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param flag: 0: normal, 1: force to re-download
+    :type flag: int
+    :return: full file path and download in background if not found locally, False if cannot be found on server
+    :rtype: str
+    :History: 2017-Oct-09 - Written - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 13:
+        file_hash = "1718723ada3018de94e1022cd57d4d950a74f91f"
+
+        # Check if directory exists
+        fullfoldername = os.path.join(
+            apogee_env(), "dr13/apogee/spectro/redux/r6/stars/l30e/l30e.2/"
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "allStar-l30e.2.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        url = f"https://data.sdss.org/sas/dr13/apogee/spectro/redux/r6/stars/l30e/l30e.2/{filename}"
+    elif dr == 14:
+        file_hash = "a7e1801924661954da792e377ad54f412219b105"
+
+        fullfoldername = os.path.join(
+            apogee_env(), "dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/"
+        )
+        # Check if directory exists
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "allStar-l31c.2.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        url = f"https://data.sdss.org/sas/dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/{filename}"
+    elif dr == 16:
+        file_hash = "66fe854bd000ca1c0a6b50a998877e4a3e41d184"
+
+        fullfoldername = os.path.join(
+            apogee_env(), "dr16/apogee/spectro/aspcap/r12/l33/"
+        )
+        # Check if directory exists
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "allStar-r12-l33.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        url = f"https://data.sdss.org/sas/dr16/apogee/spectro/aspcap/r12/l33/{filename}"
+    elif dr == 17:
+        file_hash = "7aa2f381de0e8e246f9833cc7da540ef45096702"
+
+        fullfoldername = os.path.join(
+            apogee_env(), "dr17/apogee/spectro/aspcap/dr17/synspec_rev1/"
+        )
+        # Check if directory exists
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "allStar-dr17-synspec_rev1.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        url = f"https://data.sdss.org/sas/dr17/apogee/spectro/aspcap/dr17/synspec_rev1/{filename}"
+    else:
+        raise ValueError("allstar() only supports APOGEE DR13-DR17")
+
+    # check file integrity
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash.lower():
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            allstar(dr=dr, flag=1)
+        else:
+            logging.info(fullfilename + " was found!")
+
+    # Check if files exists
+    if not os.path.isfile(os.path.join(fullfoldername, filename)) or flag == 1:
+        with TqdmUpTo(
+            unit="B", unit_scale=True, miniters=1, desc=url.split("/")[-1]
+        ) as t:
+            try:
+                urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
+                logging.info(
+                    f"Downloaded DR{dr:d} allStar file catalog successfully to {fullfilename}"
+                )
+                checksum = filehash(fullfilename, algorithm="sha1")
+                if checksum != file_hash.lower():
+                    warnings.warn(
+                        "File corruption detected, astroNN is attempting to download again"
+                    )
+                    allstar(dr=dr, flag=1)
+            except urllib.error.HTTPError as emsg:
+                if "401" in str(emsg):
+                    fullfilename = __apogee_credentials_downloader(url, fullfilename)
+                elif "404" in str(emsg):
+                    warnings.warn(f"{url} cannot be found on server, skipped")
+                    fullfilename = warning_flag
+                else:
+                    warnings.warn(f"Unknown error occurred - {emsg}")
+                    fullfilename = warning_flag
+
+    return fullfilename
+
+
+def apogee_astronn(dr=None, flag=None):
+    """
+    Download the apogee_astroNN file (catalog of astroNN stellar parameters, abundances, distances and orbital
+     parameters from combined spectra)
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param flag: 0: normal, 1: force to re-download
+    :type flag: int
+    :return: full file path and download in background if not found locally, False if cannot be found on server
+    :rtype: str
+    :History: 2019-Dec-10 - Written - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 16:
+        # Check if directory exists
+        fullfoldername = os.path.join(apogee_env(), "dr16/apogee/vac/apogee-astronn/")
+        # Check if directory exists
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "apogee_astroNN-DR16-v1.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        file_hash = "1b81ed13eef36fe9a327a05f4a622246522199b2"
+
+        url = f"https://data.sdss.org/sas/dr16/apogee/vac/apogee-astronn/{filename}"
+    elif dr == 17:
+        # Check if directory exists
+        fullfoldername = os.path.join(apogee_env(), "dr17/apogee/vac/apogee-astronn/")
+        # Check if directory exists
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "apogee_astroNN-DR17.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        file_hash = "c422b9adba840b3415af2fe6dec6500219f1b68f"
+
+        url = f"https://data.sdss.org/sas/dr17/apogee/vac/apogee-astronn/{filename}"
+    else:
+        raise ValueError("apogee_astroNN() only supports APOGEE DR16-DR17")
+
+    # check file integrity
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash.lower():
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            apogee_astronn(dr=dr, flag=1)
+        else:
+            logging.info(fullfilename + " was found!")
+
+    # Check if files exists
+    if not os.path.isfile(os.path.join(fullfoldername, filename)) or flag == 1:
+        with TqdmUpTo(
+            unit="B", unit_scale=True, miniters=1, desc=url.split("/")[-1]
+        ) as t:
+            try:
+                urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
+                logging.info(
+                    f"Downloaded DR{dr:d} apogee_astroNN file catalog successfully to {fullfilename}"
+                )
+                checksum = filehash(fullfilename, algorithm="sha1")
+                if checksum != file_hash.lower():
+                    warnings.warn(
+                        "File corruption detected, astroNN is attempting to download again"
+                    )
+                    apogee_astronn(dr=dr, flag=1)
+            except urllib.error.HTTPError as emsg:
+                if "401" in str(emsg):
+                    fullfilename = __apogee_credentials_downloader(url, fullfilename)
+                elif "404" in str(emsg):
+                    warnings.warn(f"{url} cannot be found on server, skipped")
+                    fullfilename = warning_flag
+                else:
+                    warnings.warn(f"Unknown error occurred - {emsg}")
+                    fullfilename = warning_flag
+
+    return fullfilename
+
+
+def allstar_cannon(dr=None, flag=None):
+    """
+    Download the allStarCannon file (catalog of Cannon stellar parameters and abundances from combined spectra)
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param flag: 0: normal, 1: force to re-download
+    :type flag: int
+    :return: full file path and download in background if not found locally, False if cannot be found on server
+    :rtype: str
+    :History: 2017-Oct-24 - Written - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 14:
+        # Check if directory exists
+        fullfoldername = os.path.join(
+            apogee_env(), "dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/cannon/"
+        )
+        # Check if directory exists
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        filename = "allStarCannon-l31c.2.fits"
+        fullfilename = os.path.join(fullfoldername, filename)
+        file_hash = "64d485e95b3504df0b795ab604e21a71d5c7ae45"
+
+        url = f"https://data.sdss.org/sas/dr14/apogee/spectro/redux/r8/stars/l31c/l31c.2/cannon/{filename}"
+    else:
+        raise ValueError("allstar_cannon() only supports APOGEE DR14-DR15")
+
+    # check file integrity
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash.lower():
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            allstar_cannon(dr=dr, flag=1)
+        else:
+            logging.info(fullfilename + " was found!")
+
+    # Check if files exists
+    if not os.path.isfile(os.path.join(fullfoldername, filename)) or flag == 1:
+        with TqdmUpTo(
+            unit="B", unit_scale=True, miniters=1, desc=url.split("/")[-1]
+        ) as t:
+            urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
+            logging.info(
+                f"Downloaded DR{dr:d} allStarCannon file catalog successfully to {fullfilename}"
+            )
+            checksum = filehash(fullfilename, algorithm="sha1")
+            if checksum != file_hash.lower():
+                warnings.warn(
+                    "File corruption detected, astroNN is attempting to download again"
+                )
+                allstar_cannon(dr=dr, flag=1)
+
+    return fullfilename
+
+
+def allvisit(dr=None, flag=None):
+    """
+    Download the allVisit file (catalog of properties from individual visit spectra)
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param flag: 0: normal, 1: force to re-download
+    :type flag: int
+    :return: full file path and download in background if not found locally, False if cannot be found on server
+    :rtype: str
+    :History: 2017-Oct-11 - Written - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 13:
+        file_hash = "2a3b13ccd40a2c8aea8321be9630117922d55b51"
+
+        # Check if directory exists
+        fullfilepath = os.path.join(apogee_env(), "dr13/apogee/spectro/redux/r6/")
+        if not os.path.exists(fullfilepath):
+            os.makedirs(fullfilepath)
+        filename = "allVisit-l30e.2.fits"
+        fullfilename = os.path.join(fullfilepath, filename)
+        url = f"https://data.sdss.org/sas/dr13/apogee/spectro/redux/r6/{filename}"
+    elif dr == 14:
+        file_hash = "abcecbcdc5fe8d00779738702c115633811e6bbd"
+
+        # Check if directory exists
+        fullfilepath = os.path.join(apogee_env(), "dr14/apogee/spectro/redux/r8/")
+        if not os.path.exists(fullfilepath):
+            os.makedirs(fullfilepath)
+        filename = "allVisit-l31c.2.fits"
+        fullfilename = os.path.join(fullfilepath, filename)
+        url = f"https://data.sdss.org/sas/dr14/apogee/spectro/redux/r8/{filename}"
+    elif dr == 16:
+        file_hash = "65befb967d8d9d6f4f87711c1fa8d0ac014b62da"
+
+        # Check if directory exists
+        fullfilepath = os.path.join(apogee_env(), "dr16/apogee/spectro/aspcap/r12/l33/")
+        if not os.path.exists(fullfilepath):
+            os.makedirs(fullfilepath)
+        filename = "allVisit-r12-l33.fits"
+        fullfilename = os.path.join(fullfilepath, filename)
+        url = f"https://data.sdss.org/sas/dr16/apogee/spectro/aspcap/r12/l33/{filename}"
+    elif dr == 17:
+        file_hash = "fb2f5ecbabbe156f8ec37b420e095f3ba8323cc6"
+
+        # Check if directory exists
+        fullfilepath = os.path.join(
+            apogee_env(), "dr17/apogee/spectro/aspcap/dr17/synspec_rev1/"
+        )
+        if not os.path.exists(fullfilepath):
+            os.makedirs(fullfilepath)
+        filename = "allVisit-dr17-synspec_rev1.fits"
+        fullfilename = os.path.join(fullfilepath, filename)
+        url = f"https://data.sdss.org/sas/dr17/apogee/spectro/aspcap/dr17/synspec_rev1/{filename}"
+    else:
+        raise ValueError("allvisit() only supports APOGEE DR13-DR17")
+
+    # check file integrity
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash.lower():
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            allvisit(dr=dr, flag=1)
+        else:
+            logging.info(fullfilename + " was found!")
+    elif not os.path.isfile(os.path.join(fullfilepath, filename)) or flag == 1:
+        with TqdmUpTo(
+            unit="B", unit_scale=True, miniters=1, desc=url.split("/")[-1]
+        ) as t:
+            urllib.request.urlretrieve(url, fullfilename, reporthook=t.update_to)
+            logging.info(
+                f"Downloaded DR{dr:d} allVisit file catalog successfully to {fullfilepath}"
+            )
+            checksum = filehash(fullfilename, algorithm="sha1")
+            if checksum != file_hash.lower():
+                warnings.warn(
+                    "File corruption detected, astroNN is attempting to download again"
+                )
+                allvisit(dr=dr, flag=1)
+
+    return fullfilename
+
+
+def combined_spectra(
+    dr=None,
+    location=None,
+    field=None,
+    apogee=None,
+    telescope=None,
+    verbose=1,
+    flag=None,
+):
+    """
+    Download the required combined spectra file a.k.a aspcapStar
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param location: Location ID [Optional]
+    :type location: int
+    :param field: Field [Optional]
+    :type field: str
+    :param apogee: Apogee ID
+    :type apogee: str
+    :param telescope: Telescope ID, for example 'apo25m' or 'lco25m'
+    :type telescope: str
+    :param verbose: verbose, set 0 to silent most logging
+    :type verbose: int
+    :param flag: 0: normal, 1: force to re-download
+    :type flag: int
+
+    :return: full file path and download in background if not found locally, False if cannot be found on server
+    :rtype: str
+    :History:
+        | 2017-Oct-15 - Written - Henry Leung (University of Toronto)
+        | 2018-Aug-31 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    # for DR16=<, location is expected to be none because field is used
+    if (location is None and dr < 16) or (
+        field is None and dr >= 16
+    ):  # try to load info if not enough info
+        global _ALLSTAR_TEMP
+        if not str(f"dr{dr}") in _ALLSTAR_TEMP:
+            _ALLSTAR_TEMP[f"dr{dr}"] = fits.getdata(allstar(dr=dr))
+        if telescope is None:
+            matched_idx = [
+                np.nonzero(_ALLSTAR_TEMP[f"dr{dr}"]["APOGEE_ID"] == apogee)[0]
+            ][0]
+        else:
+            matched_idx = [
+                np.nonzero(
+                    [
+                        (_ALLSTAR_TEMP[f"dr{dr}"]["APOGEE_ID"] == apogee)
+                        & (_ALLSTAR_TEMP[f"dr{dr}"]["TELESCOPE"] == telescope)
+                    ]
+                )
+            ][0][1]
+        if len(matched_idx) == 0:
+            raise ValueError(
+                f"No entry found in allstar DR{dr} met with your requirement!!"
+            )
+
+        location = (
+            _ALLSTAR_TEMP[f"dr{dr}"]["LOCATION_ID"][matched_idx][0]
+            if not location
+            else location
+        )
+        field = (
+            _ALLSTAR_TEMP[f"dr{dr}"]["FIELD"][matched_idx][0] if not field else field
+        )
+        telescope = (
+            _ALLSTAR_TEMP[f"dr{dr}"]["TELESCOPE"][matched_idx][0]
+            if not telescope
+            else telescope
+        )
+
+    if dr == 13:
+        reduce_prefix = "r6"
+        aspcap_code = "l30e"
+        str1 = f"https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/{location}/"
+
+        filename = f"aspcapStar-{reduce_prefix}-{aspcap_code}.2-{apogee}.fits"
+        hash_filename = f"stars_{aspcap_code}_{aspcap_code}.2_{location}.sha1sum"
+        urlstr = str1 + filename
+
+        # check folder existence
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/",
+            str(location),
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+
+        fullfilename = os.path.join(fullfoldername, filename)
+
+    elif dr == 14:
+        reduce_prefix = "r8"
+        aspcap_code = "l31c"
+        str1 = f"https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/{location}/"
+
+        filename = f"aspcapStar-{reduce_prefix}-{aspcap_code}.2-{apogee}.fits"
+        hash_filename = f"stars_{aspcap_code}_{aspcap_code}.2_{location}.sha1sum"
+        urlstr = str1 + filename
+
+        # check folder existence
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{aspcap_code}/{aspcap_code}.2/",
+            str(location),
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+
+        fullfilename = os.path.join(fullfoldername, filename)
+    elif dr == 16:
+        reduce_prefix = "r12"
+        aspcap_code = "l33"
+        str1 = f"https://data.sdss.org/sas/dr16/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}/{field}/"
+
+        filename = f"aspcapStar-{reduce_prefix}-{apogee}.fits"
+        hash_filename = f"{reduce_prefix}_{aspcap_code}_{telescope}_{field}.sha1sum"
+        urlstr = str1 + filename
+
+        # check folder existence
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}",
+            str(f"{field}"),
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+
+        fullfilename = os.path.join(fullfoldername, filename)
+    elif dr == 17:
+        reduce_prefix = "dr17"
+        aspcap_code = "synspec_rev1"
+        str1 = f"https://data.sdss.org/sas/dr17/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}/{field}/"
+
+        filename = f"aspcapStar-{reduce_prefix}-{apogee}.fits"
+        if telescope == "lco25m":  # syncspec_rev1 only affected lco25m
+            hash_filename = f"{reduce_prefix}_{aspcap_code}_{telescope}_{field}.sha1sum"
+        else:
+            hash_filename = (
+                f"{reduce_prefix}_{aspcap_code[:7]}_{telescope}_{field}.sha1sum"
+            )
+        urlstr = str1 + filename
+
+        # check folder existence
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/aspcap/{reduce_prefix}/{aspcap_code}/{telescope}",
+            str(f"{field}"),
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+
+        fullfilename = os.path.join(fullfoldername, filename)
+    else:
+        raise ValueError("combined_spectra() only supports APOGEE DR13-DR17")
+
+    # check hash file
+    full_hash_filename = os.path.join(fullfoldername, hash_filename)
+    if not os.path.isfile(full_hash_filename):
+        # return warning flag if the location_id cannot even be found
+        try:
+            urllib.request.urlopen(str1)
+        except urllib.error.HTTPError:
+            return warning_flag
+        urllib.request.urlretrieve(str1 + hash_filename, full_hash_filename)
+
+    hash_list = np.loadtxt(full_hash_filename, dtype="str").T
+
+    # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
+    file_hash = hash_list[0][np.argwhere(hash_list[1] == filename)]
+
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash and len(file_hash) != 0:
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            combined_spectra(
+                dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1
+            )
+
+        if verbose == 1:
+            logging.info(fullfilename + " was found!")
+
+    elif not os.path.isfile(fullfilename) or flag == 1:
+        try:
+            urllib.request.urlretrieve(urlstr, fullfilename)
+            logging.info(
+                f"Downloaded DR{dr} combined file successfully to {fullfilename}"
+            )
+            checksum = filehash(fullfilename, algorithm="sha1")
+            if checksum != file_hash and len(file_hash) != 0:
+                warnings.warn(
+                    "File corruption detected, astroNN is attempting to download again"
+                )
+                combined_spectra(
+                    dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1
+                )
+        except urllib.error.HTTPError as emsg:
+            if "401" in str(emsg):
+                fullfilename = __apogee_credentials_downloader(urlstr, fullfilename)
+            elif "404" in str(emsg):
+                warnings.warn(f"{urlstr} cannot be found on server, skipped")
+                fullfilename = warning_flag
+            else:
+                warnings.warn(f"Unknown error occurred - {emsg}")
+                fullfilename = warning_flag
+
+    return fullfilename
+
+
+def visit_spectra(
+    dr=None,
+    location=None,
+    field=None,
+    apogee=None,
+    telescope=None,
+    verbose=1,
+    flag=None,
+    commission=False,
+):
+    """
+    Download the required individual spectra file a.k.a apStar or asStar
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param location: Location ID [Optional]
+    :type location: int
+    :param field: Field [Optional]
+    :type field: str
+    :param apogee: Apogee ID
+    :type apogee: str
+    :param telescope: Telescope ID, for example 'apo25m' or 'lco25m'
+    :type telescope: str
+    :param verbose: verbose, set 0 to silent most logging
+    :type verbose: int
+    :param flag: 0: normal, 1: force to re-download
+    :type flag: int
+    :param commission: whether the spectra is taken during commissioning
+    :type commission: bool
+
+    :return: full file path and download in background if not found locally, False if cannot be found on server
+    :rtype: str
+    :History:
+        | 2017-Nov-11 - Written - Henry Leung (University of Toronto)
+        | 2018-Aug-31 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    # for DR16=<, location is expected to be none because field is used
+    if (location is None and dr < 16) or (
+        field is None and dr >= 16
+    ):  # try to load info if not enough info
+        global _ALLSTAR_TEMP
+        if not str(f"dr{dr}") in _ALLSTAR_TEMP:
+            _ALLSTAR_TEMP[f"dr{dr}"] = fits.getdata(allstar(dr=dr))
+        if telescope is None:
+            matched_idx = [
+                np.nonzero(_ALLSTAR_TEMP[f"dr{dr}"]["APOGEE_ID"] == apogee)[0]
+            ][0]
+        else:
+            matched_idx = [
+                np.nonzero(
+                    [
+                        (_ALLSTAR_TEMP[f"dr{dr}"]["APOGEE_ID"] == apogee)
+                        & (_ALLSTAR_TEMP[f"dr{dr}"]["TELESCOPE"] == telescope)
+                    ]
+                )
+            ][0][1]
+        if len(matched_idx) == 0:
+            raise ValueError(
+                f"No entry found in allstar DR{dr} met with your requirement!!"
+            )
+
+        location = (
+            _ALLSTAR_TEMP[f"dr{dr}"]["LOCATION_ID"][matched_idx][0]
+            if not location
+            else location
+        )
+        field = (
+            _ALLSTAR_TEMP[f"dr{dr}"]["FIELD"][matched_idx][0] if not field else field
+        )
+        telescope = (
+            _ALLSTAR_TEMP[f"dr{dr}"]["TELESCOPE"][matched_idx][0]
+            if not telescope
+            else telescope
+        )
+
+    if dr == 13:
+        reduce_prefix = "r6"
+        str1 = f"https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/{location}/"
+        if commission:
+            filename = f"apStarC-{reduce_prefix}-{apogee}.fits"
+        else:
+            filename = f"apStar-{reduce_prefix}-{apogee}.fits"
+        urlstr = str1 + filename
+        hash_filename = f"{reduce_prefix}_stars_apo25m_{location}.sha1sum"
+
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/",
+            str(location),
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+
+    elif dr == 14:
+        reduce_prefix = "r8"
+        str1 = f"https://data.sdss.org/sas/dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/{location}/"
+        if commission:
+            filename = f"apStarC-{reduce_prefix}-{apogee}.fits"
+        else:
+            filename = f"apStar-{reduce_prefix}-{apogee}.fits"
+        urlstr = str1 + filename
+        hash_filename = f"{reduce_prefix}_stars_apo25m_{location}.sha1sum"
+
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/apo25m/",
+            str(location),
+        )
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+
+    elif dr == 16:
+        reduce_prefix = "r12"
+        str1 = f"https://data.sdss.org/sas/dr16/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/{field}/"
+        if telescope == "lco25m":
+            if commission:
+                filename = f"asStarC-{reduce_prefix}-{apogee}.fits"
+            else:
+                filename = f"asStar-{reduce_prefix}-{apogee}.fits"
+        else:
+            if commission:
+                filename = f"apStarC-{reduce_prefix}-{apogee}.fits"
+            else:
+                filename = f"apStar-{reduce_prefix}-{apogee}.fits"
+        urlstr = str1 + filename
+        hash_filename = f"{reduce_prefix}_stars_{telescope}_{field}.sha1sum"
+
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/",
+            str(f"{field}"),
+        )
+
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+    elif dr == 17:
+        reduce_prefix = "dr17"
+        str1 = f"https://data.sdss.org/sas/dr17/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/{field}/"
+        if telescope == "lco25m":
+            if commission:
+                filename = f"asStarC-{reduce_prefix}-{apogee}.fits"
+            else:
+                filename = f"asStar-{reduce_prefix}-{apogee}.fits"
+        else:
+            if commission:
+                filename = f"apStarC-{reduce_prefix}-{apogee}.fits"
+            else:
+                filename = f"apStar-{reduce_prefix}-{apogee}.fits"
+        urlstr = str1 + filename
+        hash_filename = f"{reduce_prefix}_stars_{telescope}_{field}.sha1sum"
+
+        fullfoldername = os.path.join(
+            apogee_env(),
+            f"dr{dr}/apogee/spectro/redux/{reduce_prefix}/stars/{telescope}/",
+            str(f"{field}"),
+        )
+
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+    else:
+        raise ValueError("visit_spectra() only supports APOGEE DR13-DR17")
+
+    # check hash file
+    full_hash_filename = os.path.join(fullfoldername, hash_filename)
+    if not os.path.isfile(full_hash_filename):
+        # return warning flag if the location_id cannot even be found
+        try:
+            urllib.request.urlopen(str1)
+        except urllib.error.HTTPError:
+            return warning_flag
+        urllib.request.urlretrieve(str1 + hash_filename, full_hash_filename)
+
+    hash_list = np.loadtxt(full_hash_filename, dtype="str").T
+
+    fullfilename = os.path.join(fullfoldername, filename)
+
+    # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
+    # visit spectra has a different filename in checksum
+    # handle the case where apogee_id cannot be found
+    hash_idx = [
+        i
+        for i, item in enumerate(hash_list[1])
+        if f"apStar-{reduce_prefix}-{apogee}" in item
+    ]
+    file_hash = hash_list[0][hash_idx]
+
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash and len(file_hash) != 0:
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            visit_spectra(
+                dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1
+            )
+
+        if verbose:
+            logging.info(fullfilename + " was found!")
+
+    elif not os.path.isfile(fullfilename) or flag == 1:
+        try:
+            urllib.request.urlretrieve(urlstr, fullfilename)
+            logging.info(
+                f"Downloaded DR{dr} individual visit file successfully to {fullfilename}"
+            )
+            checksum = filehash(fullfilename, algorithm="sha1")
+            if checksum != file_hash and len(file_hash) != 0:
+                warnings.warn(
+                    "File corruption detected, astroNN is attempting to download again"
+                )
+                visit_spectra(
+                    dr=dr, location=location, apogee=apogee, verbose=verbose, flag=1
+                )
+        except urllib.error.HTTPError as emsg:
+            if "401" in str(emsg):
+                fullfilename = __apogee_credentials_downloader(urlstr, fullfilename)
+            elif "404" in str(emsg):
+                warnings.warn(f"{urlstr} cannot be found on server, skipped")
+                fullfilename = warning_flag
+            else:
+                warnings.warn(f"Unknown error occurred - {emsg}")
+                fullfilename = warning_flag
+
+    return fullfilename
+
+
+def apogee_rc(dr=None, flag=None):
+    """
+    Download the APOGEE red clumps catalogue
+
+    :param dr: Apogee DR
+    :type dr: int
+    :param flag: Force to download if flag=1
+    :type flag: int
+    :return: full file path
+    :rtype: str
+    :History: 2017-Nov-16 - Written - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 13:
+        file_hash = "5e87eb3ba202f9db24216978dafb19d39d382fc6"
+
+        str1 = "https://data.sdss.org/sas/dr13/apogee/vac/apogee-rc/cat/"
+        filename = f"apogee-rc-DR{dr}.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr13/apogee/vac/apogee-rc/cat/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+
+    elif dr == 14:
+        file_hash = "104513070f1c280954f3d1886cac429dbdf2eaf6"
+
+        str1 = "https://data.sdss.org/sas/dr14/apogee/vac/apogee-rc/cat/"
+        filename = f"apogee-rc-DR{dr}.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr14/apogee/vac/apogee-rc/cat/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+
+    elif dr == 16:
+        file_hash = "0bc75a230058f50ed8a5ea3fa8554d803ffc103d"
+
+        str1 = "https://data.sdss.org/sas/dr16/apogee/vac/apogee-rc/cat/"
+        filename = f"apogee-rc-DR{dr}.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr16/apogee/vac/apogee-rc/cat/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+
+    elif dr == 17:
+        file_hash = "491e854d6db6b828554eda2b4b2e31365ccf65aa"
+
+        str1 = "https://data.sdss.org/sas/dr17/apogee/vac/apogee-rc/cat/"
+        filename = f"apogee-rc-DR{dr}.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr17/apogee/vac/apogee-rc/cat/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+
+    else:
+        raise ValueError("apogee_rc() only supports APOGEE DR13-DR17")
+
+    # check file integrity
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash.lower():
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            apogee_rc(dr=dr, flag=1)
+        else:
+            logging.info(fullfilename + " was found!")
+
+    elif not os.path.isfile(fullfilename) or flag == 1:
+        try:
+            with TqdmUpTo(
+                unit="B", unit_scale=True, miniters=1, desc=urlstr.split("/")[-1]
+            ) as t:
+                urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
+                logging.info(
+                    f"Downloaded DR{dr} Red Clumps Catalog successfully to {fullfilename}"
+                )
+                checksum = filehash(fullfilename, algorithm="sha1")
+                if checksum != file_hash.lower():
+                    warnings.warn(
+                        "File corruption detected, astroNN is attempting to download again"
+                    )
+                    apogee_rc(dr=dr, flag=1)
+        except urllib.error.HTTPError as emsg:
+            if "401" in str(emsg):
+                fullfilename = __apogee_credentials_downloader(urlstr, fullfilename)
+            elif "404" in str(emsg):
+                warnings.warn(f"{urlstr} cannot be found on server, skipped")
+                fullfilename = warning_flag
+            else:
+                warnings.warn(f"Unknown error occurred - {emsg}")
+                fullfilename = warning_flag
+
+    return fullfilename
+
+
+def apogee_distances(dr=None, flag=None):
+    """
+    Download the APOGEE Distances VAC catalogue (APOGEE Distances for DR14, APOGEE Starhourse for DR16/17)
+
+    :param dr: APOGEE DR
+    :type dr: int
+    :param flag: Force to download if flag=1
+    :type flag: int
+    :return: full file path
+    :rtype: str
+    :History:
+        | 2018-Jan-24 - Written - Henry Leung (University of Toronto)
+        | 2021-Jan-29 - Updated - Henry Leung (University of Toronto)
+    """
+    dr = apogee_default_dr(dr=dr)
+
+    if dr == 14:
+        file_hash = "b33c8419be784b1be3d14af3ee9696c6ac31830f"
+
+        str1 = "https://data.sdss.org/sas/dr14/apogee/vac/apogee-distances/"
+        filename = f"apogee_distances-DR{dr}.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr14/apogee/vac/apogee-distances/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+    if dr == 16:
+        file_hash = "2502e2f7703046163f81ecc4054dce39b2038e4f"
+
+        str1 = "https://data.sdss.org/sas/dr16/apogee/vac/apogee-starhorse/"
+        filename = f"apogee_starhorse-DR{dr}-v1.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr16/apogee/vac/apogee-starhorse/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+    if dr == 17:
+        file_hash = "2502e2f7703046163f81ecc4054dce39b2038e4f"
+
+        str1 = "https://data.sdss.org/sas/dr17/apogee/vac/apogee-starhorse/"
+        filename = f"APOGEE_DR17_EDR3_STARHORSE_v2.fits"
+        urlstr = str1 + filename
+        fullfoldername = os.path.join(apogee_env(), "dr17/apogee/vac/apogee-starhorse/")
+        if not os.path.exists(fullfoldername):
+            os.makedirs(fullfoldername)
+        fullfilename = os.path.join(fullfoldername, filename)
+    else:
+        raise ValueError("apogee_distances() only supports APOGEE DR14-DR17")
+
+    # check file integrity
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha1")
+        if checksum != file_hash.lower():
+            warnings.warn(
+                "File corruption detected, astroNN is attempting to download again"
+            )
+            apogee_distances(dr=dr, flag=1)
+        else:
+            logging.info(fullfilename + " was found!")
+
+    elif not os.path.isfile(fullfilename) or flag == 1:
+        try:
+            with TqdmUpTo(
+                unit="B", unit_scale=True, miniters=1, desc=urlstr.split("/")[-1]
+            ) as t:
+                urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
+                logging.info(
+                    f"Downloaded DR{dr} Distances successfully to {fullfilename}"
+                )
+                checksum = filehash(fullfilename, algorithm="sha1")
+                if checksum != file_hash.lower():
+                    warnings.warn(
+                        "File corruption detected, astroNN is attempting to download again"
+                    )
+                    apogee_distances(dr=dr, flag=1)
+        except urllib.error.HTTPError:
+            warnings.warn(f"{urlstr} cannot be found on server, skipped")
+            fullfilename = warning_flag
+
+    return fullfilename
```

### Comparing `astroNN-1.0.1/astroNN/config.py` & `astroNN-1.1.0/astroNN/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,330 +1,331 @@
-import configparser
-import os
-import platform
-
-from astroNN.shared.nn_tools import cpu_fallback, gpu_memory_manage
-
-astroNN_CACHE_DIR = os.path.join(os.path.expanduser('~'), '.astroNN')
-_astroNN_MODEL_NAME = 'model_weights.h5'  # default astroNN model filename
-
-
-def config_path(flag=None):
-    """
-    NAME: config_path
-    PURPOSE: get configuration file path
-    INPUT:
-        flag (boolean): 1 to update the config file, 2 to reset the config file
-    OUTPUT:
-        (path)
-    HISTORY:
-        2018-Jan-25 - Written - Henry Leung (University of Toronto)
-    """
-    filename = 'config.ini'
-    fullpath = os.path.join(astroNN_CACHE_DIR, filename)
-
-    if not os.path.isfile(fullpath) or flag == 1 or flag == 2:
-        if not os.path.exists(astroNN_CACHE_DIR):
-            os.makedirs(astroNN_CACHE_DIR)
-
-        # by default initial settings
-        magicnum_init = -9999
-        envvar_warning_flag_init = True
-        tf_keras_flag_init = 'auto'
-        custom_model_init = 'None'
-        cpu_fallback_init = False
-        gpu_memratio_init = True
-
-        # Set flag back to 0 as flag=1 probably just because the file not even exists (example: first time using it)
-        if not os.path.isfile(fullpath):
-            flag = 0
-        # only try to  migrate the old setting to new one if flag is 1 as flag=2 for reset
-        elif flag == 1:  # Try to migrate the old setting to new one
-            config = configparser.ConfigParser()
-            config.sections()
-            config.read(fullpath)
-            # Try to migrate the old setting to new one
-            try:
-                magicnum_init = float(config['Basics']['MagicNumber'])
-            except KeyError:
-                pass
-            try:
-                envvar_warning_flag_init = config['Basics']['EnvironmentVariableWarning']
-            except KeyError:
-                pass
-            try:
-                tf_keras_flag_init = config['Basics']['Tensorflow_Keras']
-            except KeyError:
-                pass
-            try:
-                custom_model_init = config['NeuralNet']['CustomModelPath']
-            except KeyError:
-                pass
-            try:
-                cpu_fallback_init = config['NeuralNet']['CPUFallback']
-            except KeyError:
-                pass
-            try:
-                gpu_memratio_init = config['NeuralNet']['GPU_Mem_ratio']
-            except KeyError:
-                pass
-        elif flag == 2:
-            # pass because flag==2 is resetting the file
-            pass
-        else:
-            raise ValueError('Unknown flag, it can only either be 0 or 1!')
-
-        os_type = platform.system()
-
-        # Windows cannot do multiprocessing, see issue #2
-        if os_type == 'Windows':
-            multiprocessing_flag = False
-        elif os_type == 'Linux' or os_type == 'Darwin':
-            # Deliberately set to False too as recommended by Keras
-            multiprocessing_flag = False
-        else:
-            # other system also set to False too to be safe
-            multiprocessing_flag = False
-
-        config = configparser.ConfigParser()
-        config['Basics'] = {'MagicNumber': magicnum_init,
-                            'Multiprocessing_Generator': multiprocessing_flag,
-                            'EnvironmentVariableWarning': envvar_warning_flag_init,
-                            'Tensorflow_Keras': tf_keras_flag_init}
-        config['NeuralNet'] = {'CustomModelPath': custom_model_init,
-                               'CPUFallback': cpu_fallback_init,
-                               'GPU_Mem_ratio': gpu_memratio_init}
-
-        with open(fullpath, 'w') as configfile:
-            config.write(configfile)
-            configfile.close()
-
-        if flag == 1:
-            print('=================Important=================')
-            print(f'astroNN just migrated the old config.ini to the new one located at {astroNN_CACHE_DIR}, '
-                  f'please check to make sure !!')
-
-    return fullpath
-
-
-def magic_num_reader():
-    """
-    NAME: magic_num_reader
-    PURPOSE: to read magic number from configuration file
-    INPUT:
-    OUTPUT:
-        (float)
-    HISTORY:
-        2018-Jan-25 - Written - Henry Leung (University of Toronto)
-    """
-    cpath = config_path()
-    config = configparser.ConfigParser()
-    config.read(cpath)
-
-    try:
-        return float(config['Basics']['MagicNumber'])
-    except KeyError:
-        config_path(flag=1)
-        return magic_num_reader()
-
-
-def multiprocessing_flag_reader():
-    """
-    NAME: multiprocessing_flag_readertf.keras
-    PURPOSE: to read multiprocessing flag from configuration file
-    INPUT:
-    OUTPUT:
-        (boolean)
-    HISTORY:
-        2018-Jan-25 - Written - Henry Leung (University of Toronto)
-    """
-    cpath = config_path()
-    config = configparser.ConfigParser()
-    config.read(cpath)
-
-    try:
-        string = config['Basics']['Multiprocessing_Generator']
-        return True if string.upper() == 'TRUE' else False
-    except KeyError:
-        config_path(flag=1)
-        return multiprocessing_flag_reader()
-
-
-def envvar_warning_flag_reader():
-    """
-    NAME: envvar_warning_flag_reader
-    PURPOSE: to read environment variable warning flag from configuration file
-    INPUT:
-    OUTPUT:
-        (boolean)
-    HISTORY:
-        2018-Feb-10 - Written - Henry Leung (University of Toronto)
-    """
-    cpath = config_path()
-    config = configparser.ConfigParser()
-    config.read(cpath)
-
-    try:
-        string = config['Basics']['EnvironmentVariableWarning']
-        return True if string.upper() == 'TRUE' else False
-    except KeyError:
-        config_path(flag=1)
-        return envvar_warning_flag_reader()
-
-
-def tf_keras_flag_reader():
-    """
-    NAME: tf_keras_flag_reader
-    PURPOSE: to read flag to decide whether using keras or tensorflow.keras or auto decided by astroNN
-    INPUT:
-    OUTPUT:
-        (string)
-    HISTORY:
-        2018-Feb-10 - Written - Henry Leung (University of Toronto)
-    """
-    cpath = config_path()
-    config = configparser.ConfigParser()
-    config.read(cpath)
-
-    try:
-        string = config['Basics']['Tensorflow_Keras']
-        return string.upper()
-    except KeyError:
-        config_path(flag=1)
-        return tf_keras_flag_reader()
-
-
-def custom_model_path_reader():
-    """
-    NAME: custom_model_path_reader
-    PURPOSE: to read path of custom models
-    INPUT:
-    OUTPUT:
-        (string)
-    HISTORY:
-        2018-Mar-09 - Written - Henry Leung (University of Toronto)
-    """
-    cpath = config_path()
-    config = configparser.ConfigParser()
-    config.read(cpath)
-
-    try:
-        string = config['NeuralNet']['CustomModelPath']
-        if string.upper() != 'NONE':
-            string = string.split(';')
-            i = 0
-            while i < len(string):
-                string[i] = os.path.expanduser(string[i])
-                if not os.path.isfile(string[i]):
-                    print(f'astroNN cannot find "{string[i]}" on your system, deleted from model path reader')
-                    print(f'Please go and check "custommodelpath" in configuration file located at {cpath}')
-                    del string[i]
-                else:
-                    i += 1
-            return string
-        else:
-            return None
-    except KeyError:
-        config_path(flag=1)
-        return custom_model_path_reader()
-
-
-def cpu_gpu_reader():
-    """
-    NAME: cpu_gpu_reader
-    PURPOSE: to read cpu gpu setting in config
-    INPUT:
-    OUTPUT:
-        (boolean)
-    HISTORY:
-        2018-Mar-14 - Written - Henry Leung (University of Toronto)
-    """
-    cpath = config_path()
-    config = configparser.ConfigParser()
-    config.read(cpath)
-
-    try:
-        cpu_string = config['NeuralNet']['CPUFallback']
-        gpu_string = config['NeuralNet']['GPU_Mem_ratio']
-        cpu_string = True if cpu_string.upper() == 'TRUE' else False
-        gpu_string = True if gpu_string.upper() == 'TRUE' else False
-        return cpu_string, gpu_string
-    except KeyError:
-        config_path(flag=1)
-        return cpu_gpu_reader()
-
-
-def keras_import_manager():
-    """
-    NAME: keras_import_manager
-    PURPOSE: to import either keras or tensorflow.keras
-    INPUT:
-    OUTPUT:
-        (module)
-    HISTORY:
-        2018-Mar-04 - Written - Henry Leung (University of Toronto)
-    """
-
-    def try_import_tf():
-        from tensorflow.python import keras
-        return keras
-
-    if TF_KERAS_FLAG == 'AUTO':
-        try:
-            import keras
-            return keras
-        except ImportError or ModuleNotFoundError:
-            try:
-                return try_import_tf()
-            except ImportError or ModuleNotFoundError:
-                raise ModuleNotFoundError('astroNN cannot import neither Keras nor Tensorflow')
-    elif TF_KERAS_FLAG == 'TENSORFLOW':
-        try:
-            return try_import_tf()
-        except ImportError or ModuleNotFoundError:
-            raise ModuleNotFoundError('Tensorflow not found! You must install Tensorflow to use astroNN')
-    elif TF_KERAS_FLAG == 'KERAS':
-        try:
-            import keras
-            return keras
-        except ImportError or ModuleNotFoundError:
-            raise ModuleNotFoundError('You have forced astroNN to use keras, but keras not found!')
-    else:
-        raise ValueError('Unknown option, only available options are auto, tensorflow or keras')
-
-
-def switch_keras(flag=None):
-    """
-    NAME: switch_keras
-    PURPOSE: to switch between keras or tensorflow.keras without changing the config file
-    INPUT:
-        flag (string): either keras or tensorflow
-    OUTPUT:
-        (string)
-    HISTORY:
-        2018-Mar-07 - Written - Henry Leung (University of Toronto)
-    """
-    if flag is None or (flag.upper() != 'TENSORFLOW' and flag.upper() != 'KERAS'):
-        raise ValueError('flag cannot be None, it should either be tensorflow or keras')
-
-    global TF_KERAS_FLAG
-    TF_KERAS_FLAG = flag.upper()
-
-    return None
-
-
-def cpu_gpu_check():
-    fallback_cpu, limit_gpu_mem = cpu_gpu_reader()
-    if fallback_cpu is True:
-        cpu_fallback()
-    if limit_gpu_mem is True:
-        gpu_memory_manage()
-    elif isinstance(limit_gpu_mem, float) is True:
-        gpu_memory_manage(ratio=limit_gpu_mem)
-
-
-# Constant from configuration file
-MAGIC_NUMBER = magic_num_reader()
-MULTIPROCESS_FLAG = multiprocessing_flag_reader()
-ENVVAR_WARN_FLAG = envvar_warning_flag_reader()
-TF_KERAS_FLAG = tf_keras_flag_reader()
-CUSTOM_MODEL_PATH = custom_model_path_reader()
+import configparser
+import os
+import platform
+
+from astroNN.shared.nn_tools import cpu_fallback, gpu_memory_manage
+
+astroNN_CACHE_DIR = os.path.join(os.path.expanduser("~"), ".astroNN")
+_astroNN_MODEL_NAME = "model_weights.h5"  # default astroNN model filename
+
+
+def config_path(flag=None):
+    """
+    NAME: config_path
+    PURPOSE: get configuration file path
+    INPUT:
+        flag (boolean): 1 to update the config file, 2 to reset the config file
+    OUTPUT:
+        (path)
+    HISTORY:
+        2018-Jan-25 - Written - Henry Leung (University of Toronto)
+    """
+    filename = "config.ini"
+    fullpath = os.path.join(astroNN_CACHE_DIR, filename)
+
+    if os.path.isfile(fullpath):
+        config = configparser.ConfigParser()
+        config.sections()
+        config.read(fullpath)
+
+        # tensorflow_keras is deprecated in config on 6 Match 2019
+        if any("tensorflow_keras" in d for d in config.items("Basics")):
+            flag = 1  # set flag 1 to indicate it needs update
+
+    if not os.path.isfile(fullpath) or flag == 1 or flag == 2:
+        if not os.path.exists(astroNN_CACHE_DIR):
+            os.makedirs(astroNN_CACHE_DIR)
+
+        # by default initial settings
+        magicnum_init = -9999
+        envvar_warning_flag_init = True
+        custom_model_init = "None"
+        cpu_fallback_init = False
+        gpu_memratio_init = True
+
+        # Set flag back to 0 as flag=1 probably just because the file not even exists (example: first time using it)
+        if not os.path.isfile(fullpath):
+            flag = 0
+        # only try to  migrate the old setting to new one if flag is 1 as flag=2 for reset
+        elif flag == 1:  # Try to migrate the old setting to new one
+            config = configparser.ConfigParser()
+            config.sections()
+            config.read(fullpath)
+            # Try to migrate the old setting to new one
+            try:
+                magicnum_init = float(config["Basics"]["MagicNumber"])
+            except KeyError:
+                pass
+            try:
+                envvar_warning_flag_init = config["Basics"][
+                    "EnvironmentVariableWarning"
+                ]
+            except KeyError:
+                pass
+            try:
+                custom_model_init = config["NeuralNet"]["CustomModelPath"]
+            except KeyError:
+                pass
+            try:
+                cpu_fallback_init = config["NeuralNet"]["CPUFallback"]
+            except KeyError:
+                pass
+            try:
+                gpu_memratio_init = config["NeuralNet"]["GPU_Mem_ratio"]
+            except KeyError:
+                pass
+        elif flag == 2:
+            # pass because flag==2 is resetting the file
+            pass
+        else:
+            raise ValueError("Unknown flag, it can only either be 0 or 1!")
+
+        os_type = platform.system()
+
+        # Windows cannot do multiprocessing, see issue #2
+        if os_type == "Windows":
+            multiprocessing_flag = False
+        elif os_type == "Linux" or os_type == "Darwin":
+            # Deliberately set to False too as recommended by Keras
+            multiprocessing_flag = False
+        else:
+            # other system also set to False too to be safe
+            multiprocessing_flag = False
+
+        config = configparser.ConfigParser()
+        config["Basics"] = {
+            "MagicNumber": magicnum_init,
+            "Multiprocessing_Generator": multiprocessing_flag,
+            "EnvironmentVariableWarning": envvar_warning_flag_init,
+        }
+        config["NeuralNet"] = {
+            "CustomModelPath": custom_model_init,
+            "CPUFallback": cpu_fallback_init,
+            "GPU_Mem_ratio": gpu_memratio_init,
+        }
+
+        with open(fullpath, "w") as configfile:
+            config.write(configfile)
+            configfile.close()
+
+        if flag == 1:
+            print(
+                f"astroNN just migrated the old config.ini to the new one located at {astroNN_CACHE_DIR}, "
+                f"please check to make sure !!"
+            )
+
+    return fullpath
+
+
+def magic_num_reader():
+    """
+    NAME: magic_num_reader
+    PURPOSE: to read magic number from configuration file
+    INPUT:
+    OUTPUT:
+        (float)
+    HISTORY:
+        2018-Jan-25 - Written - Henry Leung (University of Toronto)
+    """
+    cpath = config_path()
+    config = configparser.ConfigParser()
+    config.read(cpath)
+
+    try:
+        return float(config["Basics"]["MagicNumber"])
+    except KeyError:
+        config_path(flag=1)
+        return magic_num_reader()
+
+
+def multiprocessing_flag_reader():
+    """
+    NAME: multiprocessing_flag_readertf.keras
+    PURPOSE: to read multiprocessing flag from configuration file
+    INPUT:
+    OUTPUT:
+        (boolean)
+    HISTORY:
+        2018-Jan-25 - Written - Henry Leung (University of Toronto)
+    """
+    cpath = config_path()
+    config = configparser.ConfigParser()
+    config.read(cpath)
+
+    try:
+        string = config["Basics"]["Multiprocessing_Generator"]
+        return True if string.upper() == "TRUE" else False
+    except KeyError:
+        config_path(flag=1)
+        return multiprocessing_flag_reader()
+
+
+def envvar_warning_flag_reader():
+    """
+    NAME: envvar_warning_flag_reader
+    PURPOSE: to read environment variable warning flag from configuration file
+    INPUT:
+    OUTPUT:
+        (boolean)
+    HISTORY:
+        2018-Feb-10 - Written - Henry Leung (University of Toronto)
+    """
+    cpath = config_path()
+    config = configparser.ConfigParser()
+    config.read(cpath)
+
+    try:
+        string = config["Basics"]["EnvironmentVariableWarning"]
+        return True if string.upper() == "TRUE" else False
+    except KeyError:
+        config_path(flag=1)
+        return envvar_warning_flag_reader()
+
+
+def custom_model_path_reader():
+    """
+    NAME: custom_model_path_reader
+    PURPOSE: to read path of custom models
+    INPUT:
+    OUTPUT:
+        (string)
+    HISTORY:
+        2018-Mar-09 - Written - Henry Leung (University of Toronto)
+    """
+    cpath = config_path()
+    config = configparser.ConfigParser()
+    config.read(cpath)
+
+    try:
+        string = config["NeuralNet"]["CustomModelPath"]
+        if string.upper() != "NONE":
+            string = string.split(";")
+            i = 0
+            while i < len(string):
+                string[i] = os.path.expanduser(string[i])
+                if not os.path.isfile(string[i]):
+                    print(
+                        f'astroNN cannot find "{string[i]}" on your system, deleted from model path reader'
+                    )
+                    print(
+                        f'Please go and check "custommodelpath" in configuration file located at {cpath}'
+                    )
+                    del string[i]
+                else:
+                    i += 1
+            return string
+        else:
+            return None
+    except KeyError:
+        config_path(flag=1)
+        return custom_model_path_reader()
+
+
+def cpu_gpu_reader():
+    """
+    NAME: cpu_gpu_reader
+    PURPOSE: to read cpu gpu setting in config
+    INPUT:
+    OUTPUT:
+        (boolean)
+    HISTORY:
+        2018-Mar-14 - Written - Henry Leung (University of Toronto)
+    """
+    cpath = config_path()
+    config = configparser.ConfigParser()
+    config.read(cpath)
+
+    try:
+        cpu_string = config["NeuralNet"]["CPUFallback"]
+        gpu_string = config["NeuralNet"]["GPU_Mem_ratio"]
+        cpu_string = True if cpu_string.upper() == "TRUE" else False
+        gpu_string = True if gpu_string.upper() == "TRUE" else False
+        return cpu_string, gpu_string
+    except KeyError:
+        config_path(flag=1)
+        return cpu_gpu_reader()
+
+
+def cpu_gpu_check():
+    fallback_cpu, limit_gpu_mem = cpu_gpu_reader()
+    if fallback_cpu is True:
+        cpu_fallback()
+    if isinstance(limit_gpu_mem, float) is True:
+        gpu_memory_manage(ratio=limit_gpu_mem)
+    else:
+        gpu_memory_manage()
+
+
+# Constant from configuration file
+MAGIC_NUMBER = magic_num_reader()
+MULTIPROCESS_FLAG = multiprocessing_flag_reader()
+ENVVAR_WARN_FLAG = envvar_warning_flag_reader()
+CUSTOM_MODEL_PATH = custom_model_path_reader()
+
+
+def tf_patch():
+    """
+    | Tensorflow patching function
+    | Usually it is just a few lines patch not merged by Tensorflow in a specific version
+    """
+    __tf_patches(method="patch")
+
+
+def tf_unpatch():
+    """
+    | Tensorflow unpatching function
+    | Usually it is just a few lines patch not merged by Tensorflow in a specific version
+    """
+    __tf_patches(method="unpatch")
+
+
+def __tf_patches(method="patch"):
+    """
+    Internal Tensorflow patch/unpatch function
+
+    :param method: either 'patch' or 'unpatch'
+    :type method: str
+
+    :return: None
+    """
+    import astroNN.data
+    from astroNN.shared.patch_util import Patch
+    import tensorflow as tf
+    from tensorflow.python import keras
+    import tensorflow.python as tfpython
+
+    from packaging import version
+
+    def __master_patch(path, diffpatch):
+        # generate patch and patch
+        patch = Patch(diffpatch)
+        if method == "patch":
+            action_name = "Patched"
+            err = patch.apply(path)
+        elif method == "unpatch":
+            action_name = "Unpatched"
+            err = patch.revert(path)
+        else:
+            raise ValueError(f"Unknown method={method}")
+
+        if err == 0:
+            print(f"{action_name} Successfully at {path}!")
+        else:
+            print("Error Occurred!")
+
+    tf_ver = tf.__version__
+
+    if version.parse("1.12.0") <= version.parse(tf_ver) < version.parse("1.13.0"):
+        diff = os.path.join(astroNN.data.datapath(), "tf1_12.patch")
+        patch_file_path = keras.engine.training_generator.__file__
+        __master_patch(patch_file_path, diff)
+    elif version.parse("1.14.0") <= version.parse(tf_ver) < version.parse("1.15.0"):
+        diff = os.path.join(astroNN.data.datapath(), "tf1_14.patch")
+        patch_file_path = keras.engine.network.__file__
+        __master_patch(patch_file_path, diff)
+    # https://github.com/tensorflow/tensorflow/pull/47957
+    elif version.parse("2.5.0") <= version.parse(tf_ver) < version.parse("2.6.0"):
+        diff = os.path.join(astroNN.data.datapath(), "tf2_5.patch")
+        patch_file_path = tfpython.ops.array_ops.__file__
+        __master_patch(patch_file_path, diff)
+    else:
+        print(f"Your version of Tensorflow {tf_ver} has nothing to patch")
```

### Comparing `astroNN-1.0.1/astroNN/data/anderson_2017_dr14_parallax.npz` & `astroNN-1.1.0/astroNN/data/anderson_2017_dr14_parallax.npz`

 * *Files identical despite different names*

### Comparing `astroNN-1.0.1/astroNN/data/aspcap_l31c_masks.npy` & `astroNN-1.1.0/astroNN/data/aspcap_l31c_masks.npy`

 * *Files identical despite different names*

### Comparing `astroNN-1.0.1/astroNN/data/dr13_contmask.npy` & `astroNN-1.1.0/astroNN/data/dr13_contmask.npy`

 * *Files identical despite different names*

### Comparing `astroNN-1.0.1/astroNN/data/dr14_contmask.npy` & `astroNN-1.1.0/astroNN/data/dr14_contmask.npy`

 * *Files identical despite different names*

### Comparing `astroNN-1.0.1/astroNN/data/gaiadr2_apogeedr14_parallax.npz` & `astroNN-1.1.0/astroNN/data/gaiadr2_apogeedr14_parallax.npz`

 * *Files identical despite different names*

### Comparing `astroNN-1.0.1/astroNN/datasets/galaxy10.py` & `astroNN-1.1.0/astroNN/datasets/galaxy10sdss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,159 @@
-# ---------------------------------------------------------#
-#   astroNN.datasets.galaxy10: galaxy10
-# ---------------------------------------------------------#
-
-import os
-import urllib.request
-
-import h5py
-import numpy as np
-
-from astroNN.config import astroNN_CACHE_DIR
-from astroNN.shared.downloader_tools import TqdmUpTo
-from astroNN.shared.downloader_tools import sha256_checksum
-
-Galaxy10Class = {0: "Disk, Face-on, No Spiral",
-                 1: "Smooth, Completely round",
-                 2: "Smooth, in-between round",
-                 3: "Smooth, Cigar shaped",
-                 4: "Disk, Edge-on, Rounded Bulge",
-                 5: "Disk, Edge-on, Boxy Bulge",
-                 6: "Disk, Edge-on, No Bulge",
-                 7: "Disk, Face-on, Tight Spiral",
-                 8: "Disk, Face-on, Medium Spiral",
-                 9: "Disk, Face-on, Loose Spiral"}
-
-_G10_ORIGIN = 'http://astro.utoronto.ca/~bovy/Galaxy10/'
-
-
-def load_data(flag=None):
-    """
-    NAME:
-        load_data
-    PURPOSE:
-        load_data galaxy10 data
-    INPUT:
-        None
-    OUTPUT:
-        x (ndarray): An array of images
-        y (ndarray): An array of answer
-    HISTORY:
-        2018-Jan-22 - Written - Henry Leung (University of Toronto)
-    """
-
-    filename = 'Galaxy10.h5'
-
-    complete_url = _G10_ORIGIN + filename
-
-    datadir = os.path.join(astroNN_CACHE_DIR, 'datasets')
-    file_hash = '969A6B1CEFCC36E09FFFA86FEBD2F699A4AA19B837BA0427F01B0BC6DED458AF'  # SHA256
-
-    # Notice python expect sha256 in lowercase
-
-    if not os.path.exists(datadir):
-        os.makedirs(datadir)
-    fullfilename = os.path.join(datadir, filename)
-
-    # Check if files exists
-    if os.path.isfile(fullfilename) and flag is None:
-        checksum = sha256_checksum(fullfilename)
-        if checksum != file_hash.lower():
-            print('File corruption detected, astroNN attempting to download again')
-            load_data(flag=1)
-        else:
-            print(fullfilename + ' was found!')
-    elif not os.path.isfile(fullfilename) or flag == 1:
-        with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=complete_url.split('/')[-1]) as t:
-            urllib.request.urlretrieve(complete_url, fullfilename, reporthook=t.update_to)
-            print(f'Downloaded Galaxy10 successfully to {fullfilename}')
-            checksum = sha256_checksum(fullfilename)
-            if checksum != file_hash.lower():
-                load_data(flag=1)
-
-    with h5py.File(fullfilename, 'r') as F:
-        x = np.array(F['images'])
-        y = np.array(F['ans'])
-
-    return x, y
-
-
-def galaxy10cls_lookup(class_num):
-    """
-    NAME:
-        galaxy10cls_lookup
-    PURPOSE:
-        look up class name for Galaxy10
-    INPUT:
-        class_num (int): An integer 0-9
-    OUTPUT:
-        (string): Name of the class
-    HISTORY:
-        2018-Feb-07 - Written - Henry Leung (University of Toronto)
-    """
-    if isinstance(class_num, list) or isinstance(class_num, np.ndarray):
-        class_num = np.argmax(class_num)
-    if 0 > class_num or 9 < class_num:
-        raise ValueError(f'Galaxy10 only has 10 classes, you entered {class_num}')
-    return Galaxy10Class[class_num]
-
-
-def galaxy10_confusion(confusion_mat):
-    """
-    NAME:
-        galaxy10_confusion
-    PURPOSE:
-        to plot confusion matrix
-    INPUT:
-        confusion_mat (ndarray): An integer 0-9
-    OUTPUT:
-        (string): Name of the class
-    HISTORY:
-        2018-Feb-11 - Written - Henry Leung (University of Toronto)
-    """
-    import pylab as plt
-
-    conf_arr = confusion_mat.astype(int)
-
-    norm_conf = []
-    a = np.max(conf_arr)
-    for i in conf_arr:
-        tmp_arr = []
-        for j in i:
-            tmp_arr.append(float(j) / float(a))
-        norm_conf.append(tmp_arr)
-
-    fig, ax = plt.subplots(1, figsize=(10, 10.5), dpi=100)
-    fig.suptitle("Confusion Matrix for Galaxy10 trained by astroNN", fontsize=18)
-    ax.set_aspect(1)
-    ax.imshow(np.array(norm_conf), cmap=plt.get_cmap('Blues'), interpolation='nearest')
-
-    width, height = conf_arr.shape
-
-    for x in range(width):
-        for y in range(height):
-            ax.annotate(str(conf_arr[x][y]), xy=(y, x),
-                        horizontalalignment='center',
-                        verticalalignment='center')
-
-    alphabet = '0123456789'
-    plt.xticks(range(width), alphabet[:width], fontsize=20)
-    plt.yticks(range(height), alphabet[:height], fontsize=20)
-    ax.set_ylabel('Prediction class by astroNN', fontsize=18)
-    ax.set_xlabel('True class', fontsize=18)
-    fig.tight_layout(rect=[0, 0.00, 0.8, 0.96])
-    fig.show()
-
-    return None
+# ---------------------------------------------------------#
+#   astroNN.datasets.galaxy10: galaxy10
+# ---------------------------------------------------------#
+
+import os
+import urllib.request
+
+import h5py
+import numpy as np
+
+from astroNN.config import astroNN_CACHE_DIR
+from astroNN.shared.downloader_tools import TqdmUpTo, filehash
+
+Galaxy10Class = {
+    0: "Disk, Face-on, No Spiral",
+    1: "Smooth, Completely round",
+    2: "Smooth, in-between round",
+    3: "Smooth, Cigar shaped",
+    4: "Disk, Edge-on, Rounded Bulge",
+    5: "Disk, Edge-on, Boxy Bulge",
+    6: "Disk, Edge-on, No Bulge",
+    7: "Disk, Face-on, Tight Spiral",
+    8: "Disk, Face-on, Medium Spiral",
+    9: "Disk, Face-on, Loose Spiral",
+}
+
+_G10_ORIGIN = "https://www.astro.utoronto.ca/~bovy/Galaxy10/"
+
+
+def load_data(flag=None):
+    """
+    NAME:
+        load_data
+    PURPOSE:
+        load_data galaxy10 data
+    INPUT:
+        None
+    OUTPUT:
+        x (ndarray): An array of images
+        y (ndarray): An array of answer
+    HISTORY:
+        2018-Jan-22 - Written - Henry Leung (University of Toronto)
+    """
+
+    filename = "Galaxy10.h5"
+
+    complete_url = _G10_ORIGIN + filename
+
+    datadir = os.path.join(astroNN_CACHE_DIR, "datasets")
+    file_hash = (
+        "969A6B1CEFCC36E09FFFA86FEBD2F699A4AA19B837BA0427F01B0BC6DED458AF"  # SHA256
+    )
+
+    # Notice python expect sha256 in lowercase
+
+    if not os.path.exists(datadir):
+        os.makedirs(datadir)
+    fullfilename = os.path.join(datadir, filename)
+
+    # Check if files exists
+    if os.path.isfile(fullfilename) and flag is None:
+        checksum = filehash(fullfilename, algorithm="sha256")
+        if checksum != file_hash.lower():
+            print("File corruption detected, astroNN is attempting to download again")
+            load_data(flag=1)
+        else:
+            print(fullfilename + " was found!")
+    elif not os.path.isfile(fullfilename) or flag == 1:
+        with TqdmUpTo(
+            unit="B", unit_scale=True, miniters=1, desc=complete_url.split("/")[-1]
+        ) as t:
+            urllib.request.urlretrieve(
+                complete_url, fullfilename, reporthook=t.update_to
+            )
+            print(f"Downloaded Galaxy10 successfully to {fullfilename}")
+            checksum = filehash(fullfilename, algorithm="sha256")
+            if checksum != file_hash.lower():
+                load_data(flag=1)
+
+    with h5py.File(fullfilename, "r") as F:
+        x = np.array(F["images"])
+        y = np.array(F["ans"])
+
+    return x, y
+
+
+def galaxy10cls_lookup(class_num):
+    """
+    NAME:
+        galaxy10cls_lookup
+    PURPOSE:
+        look up class name for Galaxy10
+    INPUT:
+        class_num (int): An integer 0-9
+    OUTPUT:
+        (string): Name of the class
+    HISTORY:
+        2018-Feb-07 - Written - Henry Leung (University of Toronto)
+    """
+    if isinstance(class_num, list) or isinstance(class_num, np.ndarray):
+        class_num = np.argmax(class_num)
+    if 0 > class_num or 9 < class_num:
+        raise ValueError(
+            f"Galaxy10 only has 10 classes (class 0 to class 9), you entered class {class_num}"
+        )
+    return Galaxy10Class[class_num]
+
+
+def galaxy10_confusion(confusion_mat):
+    """
+    NAME:
+        galaxy10_confusion
+    PURPOSE:
+        to plot confusion matrix
+    INPUT:
+        confusion_mat (ndarray): An integer 0-9
+    OUTPUT:
+        (string): Name of the class
+    HISTORY:
+        2018-Feb-11 - Written - Henry Leung (University of Toronto)
+    """
+    import pylab as plt
+
+    conf_arr = confusion_mat.astype(int)
+
+    norm_conf = []
+    a = np.max(conf_arr)
+    for i in conf_arr:
+        tmp_arr = []
+        for j in i:
+            tmp_arr.append(float(j) / float(a))
+        norm_conf.append(tmp_arr)
+
+    fig = plt.figure(figsize=(10, 10.5))
+    ax = fig.gca()
+    ax.set_title("Confusion Matrix for Galaxy10", fontsize=20)
+    ax.set_aspect(1)
+    ax.imshow(np.array(norm_conf), cmap=plt.get_cmap("Blues"), interpolation="nearest")
+
+    width, height = conf_arr.shape
+
+    for x in range(width):
+        for y in range(height):
+            ax.annotate(
+                str(conf_arr[x][y]),
+                xy=(y, x),
+                horizontalalignment="center",
+                verticalalignment="center",
+            )
+
+    ax.set_xticks(np.arange(width))
+    ax.set_xticklabels([str(i) for i in range(width)], fontsize=20)
+    ax.set_yticks(np.arange(height))
+    ax.set_yticklabels([str(i) for i in range(width)], fontsize=20)
+    ax.set_ylabel("Prediction", fontsize=20)
+    ax.set_xlabel("Truth", fontsize=20)
+    fig.tight_layout()
+
+    return None
```

### Comparing `astroNN-1.0.1/astroNN/gaia/downloader.py` & `astroNN-1.1.0/astroNN/gaia/downloader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,327 +1,392 @@
-# ---------------------------------------------------------#
-#   astroNN.gaia.downloader: download gaia files
-# ---------------------------------------------------------#
-
-import os
-import urllib.request
-
-import numpy as np
-from astropy.io import fits
-
-import astroNN
-from astroNN.gaia.gaia_shared import gaia_env, gaia_default_dr
-from astroNN.shared.custom_warnings import deprecated
-from astroNN.shared.downloader_tools import TqdmUpTo, md5_checksum
-
-currentdir = os.getcwd()
-
-
-def tgas(flag=None):
-    """
-    Get path to the Gaia TGAS DR1 files, download if files not found
-
-    :return: List of file path
-    :rtype: list
-    :History: 2017-Oct-13 - Written - Henry Leung (University of Toronto)
-    """
-    # Check if dr arguement is provided, if none then use default
-    fulllist = []
-
-    # Check if directory exists
-    folderpath = os.path.join(gaia_env(), 'Gaia/gdr1/tgas_source/fits/')
-    urlbase = 'http://cdn.gea.esac.esa.int/Gaia/gdr1/tgas_source/fits/'
-
-    if not os.path.exists(folderpath):
-        os.makedirs(folderpath)
-
-    hash_filename = 'MD5SUM.txt'
-    full_hash_filename = os.path.join(folderpath, hash_filename)
-    if not os.path.isfile(full_hash_filename):
-        urllib.request.urlretrieve(urlbase + hash_filename, full_hash_filename)
-
-    hash_list = np.loadtxt(full_hash_filename, dtype='str').T
-
-    for i in range(0, 16, 1):
-        filename = f'TgasSource_000-000-0{i:0{2}d}.fits'
-        fullfilename = os.path.join(folderpath, filename)
-        urlstr = urlbase + filename
-        file_hash = (hash_list[0])[np.argwhere(hash_list[1] == filename)]
-
-        # Check if files exists
-        if os.path.isfile(fullfilename) and flag is None:
-            checksum = md5_checksum(fullfilename)
-            # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
-            if checksum != file_hash and len(file_hash) != 0:
-                print(checksum)
-                print(file_hash)
-                print('File corruption detected, astroNN attempting to download again')
-                tgas(flag=1)
-            else:
-                print(fullfilename + ' was found!')
-
-        elif not os.path.isfile(fullfilename) or flag == 1:
-            # progress bar
-            with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=urlstr.split('/')[-1]) as t:
-                # Download
-                urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
-                checksum = md5_checksum(fullfilename)
-                if checksum != file_hash and len(file_hash) != 0:
-                    print('File corruption detected, astroNN attempting to download again')
-                    tgas(flag=1)
-            print(f'Downloaded Gaia DR1 TGAS ({i:d} of 15) file catalog successfully to {fullfilename}')
-        fulllist.extend([fullfilename])
-
-    return fulllist
-
-
-def tgas_load(cuts=True):
-    """
-    To load useful parameters from multiple TGAS DR1 files
-
-    :param cuts: Whether to cut bad data (negative parallax and percentage error more than 20%, or a custom cut percentage)
-    :type cuts: Union[boolean, 0.2]
-    :return: Dictionary of parameters
-    :rtype: dict
-    :History: 2017-Dec-17 - Written - Henry Leung (University of Toronto)
-    """
-    tgas_list = tgas()
-
-    ra = np.array([])
-    dec = np.array([])
-    pmra_gaia = np.array([])
-    pmdec_gaia = np.array([])
-    parallax_gaia = np.array([])
-    parallax_error_gaia = np.array([])
-    g_band_gaia = np.array([])
-
-    for i in tgas_list:
-        gaia = fits.open(i)
-        ra = np.concatenate((ra, gaia[1].data['RA']))
-        dec = np.concatenate((dec, gaia[1].data['DEC']))
-        pmra_gaia = np.concatenate((pmra_gaia, gaia[1].data['PMRA']))
-        pmdec_gaia = np.concatenate((pmdec_gaia, gaia[1].data['PMDEC']))
-        parallax_gaia = np.concatenate((parallax_gaia, gaia[1].data['parallax']))
-        parallax_error_gaia = np.concatenate((parallax_error_gaia, gaia[1].data['parallax_error']))
-        g_band_gaia = np.concatenate((g_band_gaia, gaia[1].data['phot_g_mean_mag']))
-        gaia.close()
-
-    if cuts is True or isinstance(cuts, float):
-        filtered_index = [(parallax_error_gaia / parallax_gaia < (0.2 if isinstance(cuts, bool) else cuts)) &
-                          (parallax_gaia > 0.)]
-
-        ra = ra[filtered_index]
-        dec = dec[filtered_index]
-        pmra_gaia = pmra_gaia[filtered_index]
-        pmdec_gaia = pmdec_gaia[filtered_index]
-        parallax_gaia = parallax_gaia[filtered_index]
-        parallax_error_gaia = parallax_error_gaia[filtered_index]
-        g_band_gaia = g_band_gaia[filtered_index]
-
-    return {'ra': ra, 'dec': dec, 'pmra': pmra_gaia, 'pmdec': pmdec_gaia, 'parallax': parallax_gaia,
-            'parallax_err': parallax_error_gaia, 'gmag': g_band_gaia}
-
-
-@deprecated
-def gaia_source(dr=None, flag=None):
-    """
-    NAME:
-        gaia_source
-    PURPOSE:
-        download the gaia_source files
-    INPUT:
-        dr (int): Gaia DR, example dr=1
-        flag (int): 0: normal, 1: force to re-download
-    OUTPUT:
-        list of file path
-    HISTORY:
-        2017-Oct-13 - Written - Henry Leung (University of Toronto)
-        2017-Nov-26 - Update - Henry Leung (University of Toronto)
-    """
-    dr = gaia_default_dr(dr=dr)
-    fulllist = []
-
-    if dr == 1:
-
-        # Check if directory exists
-        folderpath = os.path.join(gaia_env(), 'Gaia/gdr1/gaia_source/fits/')
-        urlbase = 'http://cdn.gea.esac.esa.int/Gaia/gdr1/gaia_source/fits/'
-
-        if not os.path.exists(folderpath):
-            os.makedirs(folderpath)
-
-        hash_filename = 'MD5SUM.txt'
-        full_hash_filename = os.path.join(folderpath, hash_filename)
-        if not os.path.isfile(full_hash_filename):
-            urllib.request.urlretrieve(urlbase + hash_filename, full_hash_filename)
-
-        hash_list = np.loadtxt(full_hash_filename, dtype='str').T
-
-        for j in range(0, 20, 1):
-            for i in range(0, 256, 1):
-                filename = f'GaiaSource_000-0{j:0{2}d}-{i:0{3}d}.fits'
-                urlstr = urlbase + filename
-
-                fullfilename = os.path.join(folderpath, filename)
-                file_hash = (hash_list[0])[np.argwhere(hash_list[1] == filename)]
-
-                # Check if files exists
-                if os.path.isfile(fullfilename) and flag is None:
-                    checksum = md5_checksum(fullfilename)
-                    # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
-                    if checksum != file_hash and len(file_hash) != 0:
-                        print(checksum)
-                        print(file_hash)
-                        print('File corruption detected, astroNN attempting to download again')
-                        gaia_source(dr=dr, flag=1)
-                    else:
-                        print(fullfilename + ' was found!')
-                elif not os.path.isfile(fullfilename) or flag == 1:
-                    # progress bar
-                    with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=urlstr.split('/')[-1]) as t:
-                        urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
-                        checksum = md5_checksum(fullfilename)
-                        if checksum != file_hash and len(file_hash) != 0:
-                            print('File corruption detected, astroNN attempting to download again')
-                            gaia_source(dr=dr, flag=1)
-                    print(f'Downloaded Gaia DR{dr} Gaia Source ({(j * 256 + i):d} of {(256 * 20 + 112):d}) '
-                          f'file catalog successfully to {fullfilename}')
-                fulllist.extend([fullfilename])
-
-        for i in range(0, 111, 1):
-            filename = f'GaiaSource_000-020-{i:0{3}d}.fits'
-            urlstr = urlbase + filename
-
-            fullfilename = os.path.join(folderpath, filename)
-            file_hash = (hash_list[0])[np.argwhere(hash_list[1] == filename)]
-            # Check if files exists
-            if os.path.isfile(fullfilename) and flag is None:
-                checksum = md5_checksum(fullfilename)
-                # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
-                if checksum != file_hash and len(file_hash) != 0:
-                    print(checksum)
-                    print(file_hash)
-                    print('File corruption detected, astroNN attempting to download again')
-                    gaia_source(dr=dr, flag=1)
-                else:
-                    print(fullfilename + ' was found!')
-            elif not os.path.isfile(fullfilename) or flag == 1:
-                # progress bar
-                with TqdmUpTo(unit='B', unit_scale=True, miniters=1, desc=urlstr.split('/')[-1]) as t:
-                    urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
-                    checksum = md5_checksum(fullfilename)
-                    if checksum != file_hash and len(file_hash) != 0:
-                        print('File corruption detected, astroNN attempting to download again')
-                        gaia_source(dr=dr, flag=1)
-                    print(f'Downloaded Gaia DR{dr} Gaia Source ({(20 * 256 + i):d} of {(256 * 20 + 112):d}) file '
-                          f'catalog successfully to {fullfilename}')
-            fulllist.extend([fullfilename])
-
-    else:
-        raise ValueError('gaia_source() only supports Gaia DR1 Gaia Source')
-
-    return fulllist
-
-
-@deprecated
-def anderson_2017_parallax(cuts=True):
-    """
-    NAME:
-        anderson_2017_parallax
-    PURPOSE:
-        load pre-compiled Anderson et al 2017 improved parallax from data-driven stars model
-    INPUT:
-        cuts (boolean): whether to cut those parallax err larger than 20% or not
-    OUTPUT:
-        ra (ndarray)
-        dec (ndarray)
-        parallax (ndarray): parallax in mas
-        parallax_err (ndarray): 1-standard derivation parallax error in mas
-    HISTORY:
-        2017-Dec-22 - Written - Henry Leung (University of Toronto)
-    """
-    fullfilename = os.path.join(os.path.dirname(astroNN.__path__[0]), 'astroNN', 'data',
-                                'anderson_2017_dr14_parallax.npz')
-    print('\nOriginal dataset at: http://voms.simonsfoundation.org:50013/8kM7XXPCJleK2M02B9E7YIYmvu5l2rh/ServedFiles/')
-    print('Please be advised starting from 26 April 2018, anderson2017 in astroNN was reduced to parallax cross '
-          'matched with APOGEE DR14 only')
-    print('If you see this message, anderson2017 in this astroNN version is reduced. Moreover, anderson2017 will be '
-          'removed in the future\n')
-
-    hdu = np.load(fullfilename)
-    ra = hdu['ra']
-    dec = hdu['dec']
-    parallax = hdu['parallax']
-    parallax_err = hdu['parallax_err']
-
-    if cuts is True:
-        good_index = np.where(parallax_err / parallax < 0.2)[0]
-        ra = ra[good_index]
-        dec = dec[good_index]
-        parallax = parallax[good_index]
-        parallax_err = parallax_err[good_index]
-    return ra, dec, parallax, parallax_err
-
-
-def gaiadr2_parallax(cuts=True, keepdims=False, offset=False):
-    """
-    Load Gaia DR2 - APOGEE DR14 matches, indices corresponds to APOGEE allstar DR14 file
-
-    :param cuts: Whether to cut bad data (negative parallax and percentage error more than 20%), or a float to set the threshold
-    :type cuts: Union[boolean, float]
-    :param keepdims: Whether to preserve indices the same as APOGEE allstar DR14, no effect when cuts=False, set to -9999 for bad indices when cuts=True keepdims=True
-    :type keepdims: boolean
-    :param offset: Whether to correction Gaia DR2 zero point offset
-
-                   - False to assume no offset correction
-                   - True to assume 52.8-4.21(G-12.2)
-                   - "leungbovy2019" for leung & bovy 2019 offset correction
-                   - a float to assume a float offset globally
-    :type offset: Union[boolean, float, str]
-    :return: numpy array of ra, dec, parallax, parallax_error
-    :rtype: ndarrays
-    :History: 2018-Apr-26 - Written - Henry Leung (University of Toronto)
-    """
-    fullfilename = os.path.join(os.path.dirname(astroNN.__path__[0]), 'astroNN', 'data',
-                                'gaiadr2_apogeedr14_parallax.npz')
-    print('This is Gaia DR2 - APOGEE DR14 matched parallax, RA DEC in J2015.5, parallax in mas')
-
-    hdu = np.load(fullfilename)
-    ra = np.array(hdu['RA'])
-    dec = np.array(hdu['DEC'])
-    parallax = np.array(hdu['parallax'])
-    parallax_err = np.array(hdu['parallax_error'])
-    gmag = np.array(hdu['g'])
-
-    if (cuts is True or isinstance(cuts, float)) and keepdims is False:
-        good_idx = ((parallax_err / parallax < (0.2 if cuts is True else cuts)) & (parallax > 0.))
-        ra = ra[good_idx]
-        dec = dec[good_idx]
-        parallax = parallax[good_idx]
-        parallax_err = parallax_err[good_idx]
-        gmag = gmag[good_idx]
-    elif (cuts is True or isinstance(cuts, float)) and keepdims is True:
-        print("Moreover, indices correspond to APOGEE allstar DR14 file")
-        # Not magic_number because this should be apogee style
-        bad_idx = ((parallax_err / parallax > (0.2 if cuts is True else cuts)) | (parallax < 0.))
-        parallax[bad_idx] = -9999.
-        parallax_err[bad_idx] = -9999.
-    else:
-        # no cuts so do nothing
-        pass
-
-    if offset is True:
-        parallax[parallax != -9999.] += (0.0528 - 0.0421 * (gmag[parallax != -9999.] - 12.2))
-    elif offset is False:
-        pass
-    elif isinstance(offset, float):
-        parallax[parallax != -9999.] += offset
-    elif offset == 'leungbovy2019':
-        def bias(x):
-            bias = 0.056 - 0.00574 * x - 0.0096 * x ** 2
-            return bias
-
-        parallax[(parallax != -9999.) & (parallax < 2.)] += bias(parallax[(parallax != -9999.) & (parallax < 2.)])
-    else:
-        raise ValueError("Unknown offset option")
-
-    return ra, dec, parallax, parallax_err
+# ---------------------------------------------------------#
+#   astroNN.gaia.downloader: download gaia files
+# ---------------------------------------------------------#
+
+import os
+import urllib.request
+
+import numpy as np
+from astropy.io import fits
+
+import astroNN
+import astroNN.data
+from astroNN.gaia.gaia_shared import gaia_env, gaia_default_dr
+from astroNN.shared.warnings import deprecated
+from astroNN.shared.downloader_tools import TqdmUpTo, filehash
+
+currentdir = os.getcwd()
+
+
+def tgas(flag=None):
+    """
+    Get path to the Gaia TGAS DR1 files, download if files not found
+
+    :return: List of file path
+    :rtype: list
+    :History: 2017-Oct-13 - Written - Henry Leung (University of Toronto)
+    """
+    # Check if dr arguement is provided, if none then use default
+    fulllist = []
+
+    # Check if directory exists
+    folderpath = os.path.join(gaia_env(), "Gaia/gdr1/tgas_source/fits/")
+    urlbase = "http://cdn.gea.esac.esa.int/Gaia/gdr1/tgas_source/fits/"
+
+    if not os.path.exists(folderpath):
+        os.makedirs(folderpath)
+
+    hash_filename = "MD5SUM.txt"
+    full_hash_filename = os.path.join(folderpath, hash_filename)
+    if not os.path.isfile(full_hash_filename):
+        urllib.request.urlretrieve(urlbase + hash_filename, full_hash_filename)
+
+    hash_list = np.loadtxt(full_hash_filename, dtype="str").T
+
+    for i in range(0, 16, 1):
+        filename = f"TgasSource_000-000-0{i:0{2}d}.fits"
+        fullfilename = os.path.join(folderpath, filename)
+        urlstr = urlbase + filename
+        file_hash = (hash_list[0])[np.argwhere(hash_list[1] == filename)]
+
+        # Check if files exists
+        if os.path.isfile(fullfilename) and flag is None:
+            checksum = filehash(fullfilename, algorithm="md5")
+            # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
+            if checksum != file_hash and len(file_hash) != 0:
+                print(checksum)
+                print(file_hash)
+                print(
+                    "File corruption detected, astroNN is attempting to download again"
+                )
+                tgas(flag=1)
+            else:
+                print(fullfilename + " was found!")
+
+        elif not os.path.isfile(fullfilename) or flag == 1:
+            # progress bar
+            with TqdmUpTo(
+                unit="B", unit_scale=True, miniters=1, desc=urlstr.split("/")[-1]
+            ) as t:
+                # Download
+                urllib.request.urlretrieve(urlstr, fullfilename, reporthook=t.update_to)
+                checksum = filehash(fullfilename, algorithm="md5")
+                if checksum != file_hash and len(file_hash) != 0:
+                    print(
+                        "File corruption detected, astroNN is attempting to download again"
+                    )
+                    tgas(flag=1)
+            print(
+                f"Downloaded Gaia DR1 TGAS ({i:d} of 15) file catalog successfully to {fullfilename}"
+            )
+        fulllist.extend([fullfilename])
+
+    return fulllist
+
+
+def tgas_load(cuts=True):
+    """
+    To load useful parameters from multiple TGAS DR1 files
+
+    :param cuts: Whether to cut bad data (negative parallax and percentage error more than 20%, or a custom cut percentage)
+    :type cuts: Union[boolean, 0.2]
+    :return: Dictionary of parameters
+    :rtype: dict
+    :History: 2017-Dec-17 - Written - Henry Leung (University of Toronto)
+    """
+    tgas_list = tgas()
+
+    ra = np.array([])
+    dec = np.array([])
+    pmra_gaia = np.array([])
+    pmdec_gaia = np.array([])
+    parallax_gaia = np.array([])
+    parallax_error_gaia = np.array([])
+    g_band_gaia = np.array([])
+
+    for i in tgas_list:
+        gaia = fits.open(i)
+        ra = np.concatenate((ra, gaia[1].data["RA"]))
+        dec = np.concatenate((dec, gaia[1].data["DEC"]))
+        pmra_gaia = np.concatenate((pmra_gaia, gaia[1].data["PMRA"]))
+        pmdec_gaia = np.concatenate((pmdec_gaia, gaia[1].data["PMDEC"]))
+        parallax_gaia = np.concatenate((parallax_gaia, gaia[1].data["parallax"]))
+        parallax_error_gaia = np.concatenate(
+            (parallax_error_gaia, gaia[1].data["parallax_error"])
+        )
+        g_band_gaia = np.concatenate((g_band_gaia, gaia[1].data["phot_g_mean_mag"]))
+        gaia.close()
+
+    if cuts is True or isinstance(cuts, float):
+        filtered_index = [
+            (
+                parallax_error_gaia / parallax_gaia
+                < (0.2 if isinstance(cuts, bool) else cuts)
+            )
+            & (parallax_gaia > 0.0)
+        ]
+
+        ra = ra[filtered_index]
+        dec = dec[filtered_index]
+        pmra_gaia = pmra_gaia[filtered_index]
+        pmdec_gaia = pmdec_gaia[filtered_index]
+        parallax_gaia = parallax_gaia[filtered_index]
+        parallax_error_gaia = parallax_error_gaia[filtered_index]
+        g_band_gaia = g_band_gaia[filtered_index]
+
+    return {
+        "ra": ra,
+        "dec": dec,
+        "pmra": pmra_gaia,
+        "pmdec": pmdec_gaia,
+        "parallax": parallax_gaia,
+        "parallax_err": parallax_error_gaia,
+        "gmag": g_band_gaia,
+    }
+
+
+@deprecated
+def gaia_source(dr=None, flag=None):
+    """
+    NAME:
+        gaia_source
+    PURPOSE:
+        download the gaia_source files
+    INPUT:
+        dr (int): Gaia DR, example dr=1
+        flag (int): 0: normal, 1: force to re-download
+    OUTPUT:
+        list of file path
+    HISTORY:
+        2017-Oct-13 - Written - Henry Leung (University of Toronto)
+        2017-Nov-26 - Update - Henry Leung (University of Toronto)
+    """
+    dr = gaia_default_dr(dr=dr)
+    fulllist = []
+
+    if dr == 1:
+        # Check if directory exists
+        folderpath = os.path.join(gaia_env(), "Gaia/gdr1/gaia_source/fits/")
+        urlbase = "http://cdn.gea.esac.esa.int/Gaia/gdr1/gaia_source/fits/"
+
+        if not os.path.exists(folderpath):
+            os.makedirs(folderpath)
+
+        hash_filename = "MD5SUM.txt"
+        full_hash_filename = os.path.join(folderpath, hash_filename)
+        if not os.path.isfile(full_hash_filename):
+            urllib.request.urlretrieve(urlbase + hash_filename, full_hash_filename)
+
+        hash_list = np.loadtxt(full_hash_filename, dtype="str").T
+
+        for j in range(0, 20, 1):
+            for i in range(0, 256, 1):
+                filename = f"GaiaSource_000-0{j:0{2}d}-{i:0{3}d}.fits"
+                urlstr = urlbase + filename
+
+                fullfilename = os.path.join(folderpath, filename)
+                file_hash = (hash_list[0])[np.argwhere(hash_list[1] == filename)]
+
+                # Check if files exists
+                if os.path.isfile(fullfilename) and flag is None:
+                    checksum = filehash(fullfilename, algorithm="md5")
+                    # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
+                    if checksum != file_hash and len(file_hash) != 0:
+                        print(checksum)
+                        print(file_hash)
+                        print(
+                            "File corruption detected, astroNN is attempting to download again"
+                        )
+                        gaia_source(dr=dr, flag=1)
+                    else:
+                        print(fullfilename + " was found!")
+                elif not os.path.isfile(fullfilename) or flag == 1:
+                    # progress bar
+                    with TqdmUpTo(
+                        unit="B",
+                        unit_scale=True,
+                        miniters=1,
+                        desc=urlstr.split("/")[-1],
+                    ) as t:
+                        urllib.request.urlretrieve(
+                            urlstr, fullfilename, reporthook=t.update_to
+                        )
+                        checksum = filehash(fullfilename, algorithm="md5")
+                        if checksum != file_hash and len(file_hash) != 0:
+                            print(
+                                "File corruption detected, astroNN is attempting to download again"
+                            )
+                            gaia_source(dr=dr, flag=1)
+                    print(
+                        f"Downloaded Gaia DR{dr} Gaia Source ({(j * 256 + i):d} of {(256 * 20 + 112):d}) "
+                        f"file catalog successfully to {fullfilename}"
+                    )
+                fulllist.extend([fullfilename])
+
+        for i in range(0, 111, 1):
+            filename = f"GaiaSource_000-020-{i:0{3}d}.fits"
+            urlstr = urlbase + filename
+
+            fullfilename = os.path.join(folderpath, filename)
+            file_hash = (hash_list[0])[np.argwhere(hash_list[1] == filename)]
+            # Check if files exists
+            if os.path.isfile(fullfilename) and flag is None:
+                checksum = filehash(fullfilename, algorithm="md5")
+                # In some rare case, the hash cant be found, so during checking, check len(file_has)!=0 too
+                if checksum != file_hash and len(file_hash) != 0:
+                    print(checksum)
+                    print(file_hash)
+                    print(
+                        "File corruption detected, astroNN is attempting to download again"
+                    )
+                    gaia_source(dr=dr, flag=1)
+                else:
+                    print(fullfilename + " was found!")
+            elif not os.path.isfile(fullfilename) or flag == 1:
+                # progress bar
+                with TqdmUpTo(
+                    unit="B", unit_scale=True, miniters=1, desc=urlstr.split("/")[-1]
+                ) as t:
+                    urllib.request.urlretrieve(
+                        urlstr, fullfilename, reporthook=t.update_to
+                    )
+                    checksum = filehash(fullfilename, algorithm="md5")
+                    if checksum != file_hash and len(file_hash) != 0:
+                        print(
+                            "File corruption detected, astroNN is attempting to download again"
+                        )
+                        gaia_source(dr=dr, flag=1)
+                    print(
+                        f"Downloaded Gaia DR{dr} Gaia Source ({(20 * 256 + i):d} of {(256 * 20 + 112):d}) file "
+                        f"catalog successfully to {fullfilename}"
+                    )
+            fulllist.extend([fullfilename])
+
+    else:
+        raise ValueError("gaia_source() only supports Gaia DR1 Gaia Source")
+
+    return fulllist
+
+
+@deprecated
+def anderson_2017_parallax(cuts=True):
+    """
+    NAME:
+        anderson_2017_parallax
+    PURPOSE:
+        load pre-compiled Anderson et al 2017 improved parallax from data-driven stars model
+    INPUT:
+        cuts (boolean): whether to cut those parallax err larger than 20% or not
+    OUTPUT:
+        ra (ndarray)
+        dec (ndarray)
+        parallax (ndarray): parallax in mas
+        parallax_err (ndarray): 1-standard derivation parallax error in mas
+    HISTORY:
+        2017-Dec-22 - Written - Henry Leung (University of Toronto)
+    """
+    fullfilename = os.path.join(
+        astroNN.data.datapath(), "anderson_2017_dr14_parallax.npz"
+    )
+    print(
+        "\nOriginal dataset at: http://voms.simonsfoundation.org:50013/8kM7XXPCJleK2M02B9E7YIYmvu5l2rh/ServedFiles/"
+    )
+    print(
+        "Please be advised starting from 26 April 2018, anderson2017 in astroNN was reduced to parallax cross "
+        "matched with APOGEE DR14 only"
+    )
+    print(
+        "If you see this message, anderson2017 in this astroNN version is reduced. Moreover, anderson2017 will be "
+        "removed in the future\n"
+    )
+
+    hdu = np.load(fullfilename)
+    ra = hdu["ra"]
+    dec = hdu["dec"]
+    parallax = hdu["parallax"]
+    parallax_err = hdu["parallax_err"]
+
+    if cuts is True:
+        good_index = np.where(parallax_err / parallax < 0.2)[0]
+        ra = ra[good_index]
+        dec = dec[good_index]
+        parallax = parallax[good_index]
+        parallax_err = parallax_err[good_index]
+    return ra, dec, parallax, parallax_err
+
+
+@deprecated
+def gaiadr2_parallax(cuts=True, keepdims=False, offset=False):
+    """
+    Load Gaia DR2 - APOGEE DR14 matches, indices corresponds to APOGEE allstar DR14 file
+
+    :param cuts: Whether to cut bad data (negative parallax and percentage error more than 20%), or a float to set the threshold
+    :type cuts: Union[boolean, float]
+    :param keepdims: Whether to preserve indices the same as APOGEE allstar DR14, no effect when cuts=False, set to -9999 for bad indices when cuts=True keepdims=True
+    :type keepdims: boolean
+    :param offset: Whether to correction Gaia DR2 zero point offset
+
+                   - False to assume no offset correction
+                   - True to assume 52.8-4.21(G-12.2)
+                   - "leungbovy2019" for leung & bovy 2019 offset correction
+                   - a float to assume a float offset globally
+    :type offset: Union[boolean, float, str]
+    :return: numpy array of ra, dec, parallax, parallax_error
+    :rtype: ndarrays
+    :History: 2018-Apr-26 - Written - Henry Leung (University of Toronto)
+    """
+    fullfilename = os.path.join(
+        astroNN.data.datapath(), "gaiadr2_apogeedr14_parallax.npz"
+    )
+    print(
+        "This is Gaia DR2 - APOGEE DR14 matched parallax, RA DEC in J2015.5, parallax in mas"
+    )
+
+    hdu = np.load(fullfilename)
+    ra = np.array(hdu["RA"])
+    dec = np.array(hdu["DEC"])
+    parallax = np.array(hdu["parallax"])
+    parallax_err = np.array(hdu["parallax_error"])
+    gmag = np.array(hdu["g"])
+
+    if (cuts is True or isinstance(cuts, float)) and keepdims is False:
+        good_idx = (parallax_err / parallax < (0.2 if cuts is True else cuts)) & (
+            parallax > 0.0
+        )
+        ra = ra[good_idx]
+        dec = dec[good_idx]
+        parallax = parallax[good_idx]
+        parallax_err = parallax_err[good_idx]
+        gmag = gmag[good_idx]
+    elif (cuts is True or isinstance(cuts, float)) and keepdims is True:
+        print("Moreover, indices correspond to APOGEE allstar DR14 file")
+        # Not magic_number because this should be apogee style
+        bad_idx = (parallax_err / parallax > (0.2 if cuts is True else cuts)) | (
+            parallax < 0.0
+        )
+        parallax[bad_idx] = -9999.0
+        parallax_err[bad_idx] = -9999.0
+    else:
+        # no cuts so do nothing
+        pass
+
+    if offset is True:
+        parallax[parallax != -9999.0] += 0.0528 - 0.0421 * (
+            gmag[parallax != -9999.0] - 12.2
+        )
+    elif offset is False:
+        pass
+    elif isinstance(offset, float):
+        parallax[parallax != -9999.0] += offset
+    elif offset == "leungbovy2019":
+
+        def bias(x):
+            bias = 0.056 - 0.00574 * x - 0.0096 * x**2
+            return bias
+
+        parallax[(parallax != -9999.0) & (parallax < 2.0)] += bias(
+            parallax[(parallax != -9999.0) & (parallax < 2.0)]
+        )
+    else:
+        raise ValueError("Unknown offset option")
+
+    return ra, dec, parallax, parallax_err
```

### Comparing `astroNN-1.0.1/astroNN/gaia/gaia_shared.py` & `astroNN-1.1.0/astroNN/gaia/gaia_shared.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,507 +1,566 @@
-# ---------------------------------------------------------#
-#   astroNN.gaia.gaia_shared: shared functions for apogee
-# ---------------------------------------------------------#
-
-import os
-import warnings
-
-import numpy as np
-from astropy import units as u
-
-from astroNN.config import MAGIC_NUMBER
-
-# noinspection PyUnresolvedReferences
-default_parallax_unit = u.mas
-
-# Sun's absmag in different Johnson/Cousins/2MASS/Sloan bands
-# sun abs mag in pass bands source: https://arxiv.org/pdf/1804.07788.pdf --> Table 3
-solar_absmag_bands = {'U': 5.61,  # Johnson U
-                      'B': 5.44,  # Johnson B
-                      'V': 4.81,  # Johnson V
-                      'R': 4.43,  # Cousins R
-                      'I': 4.10,  # Cousins I
-                      'J': 3.67,  # 2MASS J
-                      'H': 3.32,  # 2MASS H
-                      'K': 3.27,  # 2MASS Ks
-                      'Ks': 3.27,  # 2MASS Ks
-                      'u': 5.49,  # SDSS u
-                      'g': 5.23,  # SDSS g
-                      'r': 4.53,  # SDSS r
-                      'i': 4.19,  # SDSS i
-                      'z': 4.01}  # SDSS z
-
-
-def gaia_env():
-    """
-    Get Gaia environment variable
-
-    :return: Path to Gaia Data
-    :rtype: str
-    :History: 2017-Oct-26 - Written - Henry Leung (University of Toronto)
-    """
-    from astroNN.config import ENVVAR_WARN_FLAG
-    _GAIA = os.getenv('GAIA_TOOLS_DATA')
-    if _GAIA is None and ENVVAR_WARN_FLAG is True:
-        print("WARNING! Gaia environment variable GAIA_TOOLS_DATA not set")
-    return _GAIA
-
-
-def gaia_default_dr(dr=None):
-    """
-    Check if dr argument is provided, if none then use default
-
-    :param dr: Gaia DR
-    :type dr: Union[NoneType, int]
-    :return: Gaia DR
-    :rtype: int
-    :History: 2017-Oct-26 - Written - Henry Leung (University of Toronto)
-    """
-    if dr is None:
-        dr = 1
-        print(f'dr is not provided, using default dr={dr}')
-    else:
-        pass
-    return dr
-
-
-def mag_to_fakemag(mag, parallax, parallax_err=None):
-    """
-    To convert apparent magnitude to astroNN fakemag, Magic Number will be preserved
-
-    :param mag: apparent magnitude
-    :type mag: Union[float, ndarray]
-    :param parallax: parallax (mas) or with astropy(can be distance with units) so astroNN will convert to appropriate units
-    :type parallax: Union[float, ndarray, astropy Quantity]
-    :param parallax_err: parallax_error (mas) or with astropy so astroNN will convert to appropriate units
-    :type parallax_err: Union[NoneType, float, ndarray, astropy Quantity]
-    :return: astroNN fakemag, with addition (with additional return of propagated error if parallax_err is provided)
-    :rtype: Union[float, ndarray]
-    :History: 2017-Oct-14 - Written - Henry Leung (University of Toronto)
-    """
-    # Check unit if available
-    if isinstance(parallax, u.Quantity):
-        original_parallax_unit = parallax.unit
-        parallax = parallax.to(default_parallax_unit, equivalencies=u.parallax())
-        if parallax_err is not None:
-            if not isinstance(parallax_err, u.Quantity):
-                # assume parallax error carry the same original unit as parallax if no units detected
-                parallax_err = (parallax_err * original_parallax_unit).to(default_parallax_unit).value
-            if isinstance(parallax_err, u.Quantity):
-                parallax_err = parallax_err.to(default_parallax_unit).value
-
-    mag = np.array(mag)
-    parallax_unitless = np.array(parallax)  # Take the value as we cant apply pow() to astropy unit
-
-    magic_idx = ((parallax_unitless == MAGIC_NUMBER) | (mag == MAGIC_NUMBER) | (mag < -90.))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        fakemag = parallax_unitless * (10. ** (0.2 * mag))
-    if parallax_unitless.shape != ():  # check if its only 1 element
-        fakemag[magic_idx] = MAGIC_NUMBER
-    else:
-        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
-
-    if parallax_err is None:
-        return fakemag
-    else:
-        fakemag_err = np.abs((parallax_err / parallax_unitless) * fakemag)
-        if parallax_unitless.shape != ():  # check if its only 1 element
-            fakemag_err[magic_idx] = MAGIC_NUMBER
-        else:
-            fakemag_err = MAGIC_NUMBER if magic_idx == [1] else fakemag_err
-        return fakemag, fakemag_err
-
-
-def mag_to_absmag(mag, parallax, parallax_err=None):
-    """
-    To convert apparent magnitude to absolute magnitude, Magic Number will be preserved
-
-    :param mag: apparent magnitude
-    :type mag: Union[float, ndarray]
-    :param parallax: parallax (mas) or with astropy (can be distance with units) so astroNN will convert to appropriate units
-    :type parallax: Union[float, ndarray, astropy Quantity]
-    :param parallax_err: parallax_error (mas) or with astropy so astroNN will convert to appropriate units
-    :type parallax_err: Union[NoneType, float, ndarray, astropy Quantity]
-    :return: absolute magnitude  (with additional return of propagated error if parallax_err is provided)
-    :rtype: Union[float, ndarray]
-    :History: 2017-Oct-14 - Written - Henry Leung (University of Toronto)
-    """
-    # Check unit if available
-    if isinstance(parallax, u.Quantity):
-        original_parallax_unit = parallax.unit
-        parallax = parallax.to(default_parallax_unit, equivalencies=u.parallax())
-        if parallax_err is not None:
-            if not isinstance(parallax_err, u.Quantity):
-                # assume parallax error carry the same original unit as parallax if no units detected
-                parallax_err = (parallax_err * original_parallax_unit).to(default_parallax_unit).value
-            if isinstance(parallax_err, u.Quantity):
-                parallax_err = parallax_err.to(default_parallax_unit).value
-    #     warnings.warn(f'Please be advised that astroNN mag_to_absmag() expects {default_parallax_unit.name}, '
-    #           f'astroNN has corrected the unit according to astropy unit framework')
-    # else:
-    #     warnings.warn(f'Please be advised that astroNN mag_to_absmag expects parallax in {default_parallax_unit.name}')
-
-    mag = np.array(mag)
-    parallax_unitless = np.array(parallax)  # Take the value as we cant apply log10 to astropy unit
-
-    magic_idx = ((parallax_unitless == MAGIC_NUMBER) | (mag == MAGIC_NUMBER) | (mag < -90.))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        absmag = mag + 5. * (np.log10(parallax_unitless) - 2.)
-
-    if parallax_unitless.shape != ():  # check if its only 1 element
-        absmag[magic_idx] = MAGIC_NUMBER
-    else:
-        absmag = MAGIC_NUMBER if magic_idx == [1] else absmag
-    if parallax_err is None:
-        return absmag
-    else:
-        absmag_err = 5. * np.abs(parallax_err / (parallax_unitless * absmag))
-        if parallax_unitless.shape != ():  # check if its only 1 element
-            absmag_err[magic_idx] = MAGIC_NUMBER
-        else:
-            absmag_err = MAGIC_NUMBER if magic_idx == [1] else absmag_err
-        return absmag, absmag_err
-
-
-# noinspection PyUnresolvedReferences
-def absmag_to_pc(absmag, mag):
-    """
-    To convert absolute magnitude to parsec, Magic Number will be preserved
-
-    :param absmag: absolute magnitude
-    :type absmag: Union[float, ndarray]
-    :param mag: apparent magnitude
-    :type mag: Union[float, ndarray]
-    :return: parsec
-    :rtype: astropy Quantity
-    :History: 2017-Nov-16 - Written - Henry Leung (University of Toronto)
-    """
-    absmag = np.array(absmag)
-    mag = np.array(mag)
-    magic_idx = ((absmag == MAGIC_NUMBER) | (mag == MAGIC_NUMBER))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        pc = (10. ** (((mag - absmag) / 5.) + 1.))
-
-    if absmag.shape != ():  # check if its only 1 element
-        pc[magic_idx] = MAGIC_NUMBER
-        return pc * u.parsec
-    else:
-        return (MAGIC_NUMBER if magic_idx == [1] else pc) * u.parsec
-
-
-def fakemag_to_absmag(fakemag):
-    """
-    To convert fakemag to absmag, Magic Number will be preserved
-
-    :param fakemag: eastroNN fakemag
-    :type fakemag: Union[float, ndarray]
-    :return: absolute magnitude
-    :rtype: Union[float, ndarray]
-    :History: 2018-Jan-31 - Written - Henry Leung (University of Toronto)
-    """
-    fakemag = np.array(fakemag)
-    # treat non-negative fakemag as MAGIC_NUMBER
-    magic_idx = ((fakemag == MAGIC_NUMBER) | (fakemag <= 0.))  # check for magic number and negative fakemag
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        absmag = 5. * (np.log10(fakemag) - 2.)
-
-    if absmag.shape != ():  # check if its only 1 element
-        absmag[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        absmag = MAGIC_NUMBER if magic_idx == [1] else absmag
-    return absmag
-
-
-def absmag_to_fakemag(absmag):
-    """
-    To convert absmag to fakemag, Magic Number will be preserved
-
-    :param absmag: absolute magnitude
-    :type absmag: Union[float, ndarray]
-    :return: astroNN fakemag
-    :rtype: Union[float, ndarray]
-    :History: 2018-Jan-31 - Written - Henry Leung (University of Toronto)
-    """
-    absmag = np.array(absmag)
-    magic_idx = (absmag == MAGIC_NUMBER)  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        fakemag = 10. ** (0.2 * absmag + 2.)
-    if fakemag.shape != ():  # check if its only 1 element
-        fakemag[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
-    return fakemag
-
-
-# noinspection PyUnresolvedReferences
-def fakemag_to_pc(fakemag, mag, fakemag_err=None):
-    """
-    To convert fakemag to parsec, Magic Number will be preserved
-
-    :param fakemag: astroNN fakemag
-    :type fakemag: Union[float, ndarray]
-    :param mag: apparent magnitude
-    :type mag: Union[float, ndarray]
-    :param fakemag_err: Optional, fakemag_err
-    :type fakemag_err: Union[NoneType, float, ndarray]
-    :return: array of pc with astropy Quantity (with additional return of propagated error if fakemag_err is provided)
-    :rtype: astropy Quantity
-    :History: 2018-Jan-31 - Written - Henry Leung (University of Toronto)
-    """
-    fakemag = np.array(fakemag)
-    mag = np.array(mag)
-    # treat non-positive fakemag as MAGIC_NUMBER, check for magic number and negative fakemag
-    magic_idx = ((fakemag == MAGIC_NUMBER) | (mag == MAGIC_NUMBER) | (fakemag <= 0.))
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        pc = 1000. * (10. ** (0.2 * mag)) / fakemag
-    if fakemag.shape != ():  # check if its only 1 element
-        pc[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        pc = MAGIC_NUMBER if magic_idx == [1] else pc
-
-    if fakemag_err is None:
-        return pc * u.parsec
-    else:
-        with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-            warnings.simplefilter("ignore")
-            pc_err = (fakemag_err / fakemag) * pc
-        if fakemag.shape != ():  # check if its only 1 element
-            pc_err[magic_idx] = MAGIC_NUMBER
-        else:  # for float
-            pc_err = MAGIC_NUMBER if magic_idx == [1] else pc_err
-        return pc * u.parsec, pc_err * u.parsec
-
-
-# noinspection PyUnresolvedReferences
-def fakemag_to_parallax(fakemag, mag, fakemag_err=None):
-    """
-    To convert fakemag to parallax, Magic Number will be preserved
-
-    :param fakemag: astroNN fakemag
-    :type fakemag: Union[float, ndarray]
-    :param mag: apparent magnitude
-    :type mag: Union[float, ndarray]
-    :param fakemag_err: Optional, fakemag_err
-    :type fakemag_err: Union[NoneType, float, ndarray]
-    :return: array of parallax in mas with astropy Quantity (with additional return of propagated error if fakemag_err is provided)
-    :rtype: astropy Quantity
-    :History: 2018-Aug-11 - Written - Henry Leung (University of Toronto)
-    """
-    fakemag = np.array(fakemag)
-    mag = np.array(mag)
-    # treat non-positive fakemag as MAGIC_NUMBER, check for magic number and negative fakemag
-    magic_idx = ((fakemag == MAGIC_NUMBER) | (mag == MAGIC_NUMBER) | (fakemag <= 0.))
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        parallax = fakemag / (10. ** (0.2 * mag))
-    if fakemag.shape != ():  # check if its only 1 element
-        parallax[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        parallax = MAGIC_NUMBER if magic_idx == [1] else parallax
-
-    if fakemag_err is None:
-        return parallax * u.mas
-    else:
-        with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-            warnings.simplefilter("ignore")
-            parallax_err = (fakemag_err / fakemag) * parallax
-        if fakemag.shape != ():  # check if its only 1 element
-            parallax_err[magic_idx] = MAGIC_NUMBER
-        else:  # for float
-            parallax_err = MAGIC_NUMBER if magic_idx == [1] else parallax_err
-        return parallax * u.mas, parallax_err * u.mas
-
-
-def fakemag_to_logsol(fakemag, band='K'):
-    """
-    | To convert fakemag to log10 solar luminosity, negative fakemag will be converted to MAGIC_NUMBER because of
-    | fakemag cannot be negative in physical world
-
-    :param fakemag: astroNN fakemag
-    :type fakemag: Union[float, ndarray]
-    :param band: band of your fakemag to use with
-    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
-    :return: log solar luminosity
-    :rtype: Union[float, ndarray]
-    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
-    """
-    fakemag = np.array(fakemag)
-    magic_idx = ((fakemag == MAGIC_NUMBER) | (fakemag <= 0.))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        log10sol_lum = np.array(0.4 * (solar_absmag_bands[band] - fakemag_to_absmag(fakemag)))
-
-    if log10sol_lum.shape != ():  # check if its only 1 element
-        log10sol_lum[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        log10sol_lum = MAGIC_NUMBER if magic_idx == [1] else log10sol_lum
-    return log10sol_lum
-
-
-def absmag_to_logsol(absmag, band='K'):
-    """
-    To convert absmag to log10 solar luminosity
-
-    :param absmag: absolute magnitude
-    :type absmag: Union[float, ndarray]
-    :param band: band of your absmag to use with
-    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
-    :return: log solar luminosity
-    :rtype: Union[float, ndarray]
-    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
-    """
-    absmag = np.array(absmag)
-    magic_idx = (absmag == MAGIC_NUMBER)  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        log10sol_lum = np.array(0.4 * (solar_absmag_bands[band] - absmag))
-
-    if log10sol_lum.shape != ():  # check if its only 1 element
-        log10sol_lum[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        log10sol_lum = MAGIC_NUMBER if magic_idx == [1] else log10sol_lum
-    return log10sol_lum
-
-
-def logsol_to_fakemag(logsol, band='K'):
-    """
-    | To convert log solar luminosity to fakemag, negative fakemag will be converted to MAGIC_NUMBER because of fakemag
-    | cannot be negative in physical world
-
-    :param logsol: log solar luminosity
-    :type logsol: Union[float, ndarray]
-    :param band: band of your fakemag to use with
-    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
-    :return: astroNN fakemag
-    :rtype: Union[float, ndarray]
-    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
-    """
-    logsol = np.array(logsol)
-    magic_idx = ((logsol == MAGIC_NUMBER))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        fakemag = absmag_to_fakemag(solar_absmag_bands[band] - logsol / 0.4)
-
-    if fakemag.shape != ():  # check if its only 1 element
-        fakemag[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
-    return fakemag
-
-
-def logsol_to_absmag(logsol, band='K'):
-    """
-    | To convert log solar luminosity to absmag, negative fakemag will be converted to MAGIC_NUMBER because of fakemag
-    | cannot be negative in physical world
-
-    :param logsol: log solar luminosity
-    :type logsol: Union[float, ndarray]
-    :param band: band of your absmag to use with
-    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
-    :return: absmag
-    :rtype: Union[float, ndarray]
-    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
-    """
-    logsol = np.array(logsol)
-    magic_idx = ((logsol == MAGIC_NUMBER))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        absmag = solar_absmag_bands[band] - logsol / 0.4
-
-    if absmag.shape != ():  # check if its only 1 element
-        absmag[magic_idx] = MAGIC_NUMBER
-    else:  # for float
-        absmag = MAGIC_NUMBER if magic_idx == [1] else absmag
-    return absmag
-
-
-# noinspection PyUnresolvedReferences
-def fakemag_to_mag(fakemag, pc, pc_err=None):
-    """
-    To convert apparent magnitude to astroNN fakemag, Magic Number will be preserved
-
-    :param fakemag: fakemag
-    :type fakemag: Union[float, ndarray]
-    :param pc: parsec or with astropy (can be parallax with units) so astroNN will convert to appropriate units
-    :type pc: Union[float, ndarray, astropy Quantity]
-    :param pc_error: parsec uncertainty or with astropy so astroNN will convert to appropriate units
-    :type pc_error: Union[NoneType, float, ndarray, astropy Quantity]
-    :return: astroNN fakemag, with addition (with additional return of propagated error if parallax_err is provided)
-    :rtype: Union[float, ndarray]
-    :History: 2018-Aug-1 - Written - Henry Leung (University of Toronto)
-    """
-    # Check unit if available
-    if isinstance(pc, u.Quantity):
-        original_parallax_unit = pc.unit
-        pc = pc.to(u.parsec, equivalencies=u.parallax())
-        if pc_err is not None:
-            if not isinstance(pc_err, u.Quantity):
-                # assume parallax error carry the same original unit as parallax if no units detected
-                pc_err = (pc_err * original_parallax_unit).to(u.parsec).value
-            if isinstance(pc_err, u.Quantity):
-                pc_err = pc_err.to(u.parsec).value
-
-    fakemag = np.array(fakemag)
-    pc_unitless = np.array(pc)  # Take the value as we cant apply pow() to astropy unit
-
-    magic_idx = ((pc_unitless == MAGIC_NUMBER) | (fakemag == MAGIC_NUMBER) | (fakemag <= 0.))  # check for magic number
-
-    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
-        warnings.simplefilter("ignore")
-        mag = np.log10((pc_unitless / 1000) * fakemag) / 0.2
-    if pc_unitless.shape != ():  # check if its only 1 element
-        mag[magic_idx] = MAGIC_NUMBER
-    else:
-        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
-
-    if pc_err is None:
-        return mag
-    else:
-        mag_err = np.abs((pc_err / pc) * fakemag)
-        if pc_unitless.shape != ():  # check if its only 1 element
-            mag_err[magic_idx] = MAGIC_NUMBER
-        else:
-            mag_err = MAGIC_NUMBER if magic_idx == [1] else mag_err
-        return mag, mag_err
-
-
-def extinction_correction(mag, extinction):
-    """
-    To correct magnitude with extinction, this function assumes extinction is at the same wavelength as the magnitude
-    you have provided
-
-    :param mag: apparent magnitude
-    :type mag: Union[float, ndarray]
-    :param extinction: extinction
-    :type extinction: Union[float, ndarray]
-    :return: corrected magnitude
-    :rtype: Union[float, ndarray]
-    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
-    """
-    mag = np.array(mag)
-    extinction = np.array(extinction)
-    extinction[extinction < -1.] = 0.  # extinction cannot be that negative, if yes then assume no extinction
-    magic_idx = ((mag == MAGIC_NUMBER) | (mag < -90.))  # check for magic number
-
-    mag_ec = mag - extinction
-    if mag_ec.shape != ():  # check if its only 1 element
-        mag_ec[magic_idx] = MAGIC_NUMBER
-        return mag_ec
-    else:
-        return MAGIC_NUMBER if magic_idx == [1] else mag_ec
+# ---------------------------------------------------------#
+#   astroNN.gaia.gaia_shared: shared functions for apogee
+# ---------------------------------------------------------#
+
+import os
+import warnings
+
+import numpy as np
+from astropy import units as u
+
+from astroNN.config import MAGIC_NUMBER
+
+default_parallax_unit = u.mas
+
+# Sun's absmag in different Johnson/Cousins/2MASS/Sloan bands
+# sun abs mag in pass bands source: https://arxiv.org/pdf/1804.07788.pdf --> Table 3
+solar_absmag_bands = {
+    "U": 5.61,  # Johnson U
+    "B": 5.44,  # Johnson B
+    "V": 4.81,  # Johnson V
+    "R": 4.43,  # Cousins R
+    "I": 4.10,  # Cousins I
+    "J": 3.67,  # 2MASS J
+    "H": 3.32,  # 2MASS H
+    "K": 3.27,  # 2MASS Ks
+    "Ks": 3.27,  # 2MASS Ks
+    "u": 5.49,  # SDSS u
+    "g": 5.23,  # SDSS g
+    "r": 4.53,  # SDSS r
+    "i": 4.19,  # SDSS i
+    "z": 4.01,
+}  # SDSS z
+
+
+def gaia_env():
+    """
+    Get Gaia environment variable
+
+    :return: Path to Gaia Data
+    :rtype: str
+    :History: 2017-Oct-26 - Written - Henry Leung (University of Toronto)
+    """
+    from astroNN.config import ENVVAR_WARN_FLAG
+
+    _GAIA = os.getenv("GAIA_TOOLS_DATA")
+    if _GAIA is None and ENVVAR_WARN_FLAG is True:
+        print("WARNING! Gaia environment variable GAIA_TOOLS_DATA not set")
+    return _GAIA
+
+
+def gaia_default_dr(dr=None):
+    """
+    Check if dr argument is provided, if none then use default
+
+    :param dr: Gaia DR
+    :type dr: Union[NoneType, int]
+    :return: Gaia DR
+    :rtype: int
+    :History: 2017-Oct-26 - Written - Henry Leung (University of Toronto)
+    """
+    if dr is None:
+        dr = 2
+        print(f"dr is not provided, using default dr={dr}")
+    else:
+        pass
+    return dr
+
+
+def mag_to_fakemag(mag, parallax, parallax_err=None):
+    """
+    To convert apparent magnitude to astroNN fakemag, Magic Number will be preserved
+
+    :param mag: apparent magnitude
+    :type mag: Union[float, ndarray]
+    :param parallax: parallax (mas) or with astropy(can be distance with units) so astroNN will convert to appropriate units
+    :type parallax: Union[float, ndarray, astropy Quantity]
+    :param parallax_err: parallax_error (mas) or with astropy so astroNN will convert to appropriate units
+    :type parallax_err: Union[NoneType, float, ndarray, astropy Quantity]
+    :return: astroNN fakemag, with addition (with additional return of propagated error if parallax_err is provided)
+    :rtype: Union[float, ndarray]
+    :History: 2017-Oct-14 - Written - Henry Leung (University of Toronto)
+    """
+    # Check unit if available
+    if isinstance(parallax, u.Quantity):
+        original_parallax_unit = parallax.unit
+        parallax = parallax.to(default_parallax_unit, equivalencies=u.parallax())
+        if parallax_err is not None:
+            if not isinstance(parallax_err, u.Quantity):
+                # assume parallax error carry the same original unit as parallax if no units detected
+                parallax_err = (
+                    (parallax_err * original_parallax_unit)
+                    .to(default_parallax_unit)
+                    .value
+                )
+            if isinstance(parallax_err, u.Quantity):
+                parallax_err = parallax_err.to(default_parallax_unit).value
+
+    mag = np.array(mag)
+    parallax_unitless = np.array(
+        parallax
+    )  # Take the value as we cant apply pow() to astropy unit
+
+    magic_idx = (
+        (parallax_unitless == MAGIC_NUMBER)
+        | (mag == MAGIC_NUMBER)
+        | (mag < -90.0)
+        | np.isnan(parallax_unitless)
+        | np.isnan(mag)
+    )  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        fakemag = parallax_unitless * (10.0 ** (0.2 * mag))
+    if parallax_unitless.shape != ():  # check if its only 1 element
+        fakemag[magic_idx] = MAGIC_NUMBER
+    else:
+        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
+
+    if parallax_err is None:
+        return fakemag
+    else:
+        fakemag_err = np.abs((parallax_err / parallax_unitless) * fakemag)
+        if parallax_unitless.shape != ():  # check if its only 1 element
+            fakemag_err[magic_idx] = MAGIC_NUMBER
+        else:
+            fakemag_err = MAGIC_NUMBER if magic_idx == [1] else fakemag_err
+        return fakemag, fakemag_err
+
+
+def mag_to_absmag(mag, parallax, parallax_err=None):
+    """
+    To convert apparent magnitude to absolute magnitude, Magic Number will be preserved
+
+    :param mag: apparent magnitude
+    :type mag: Union[float, ndarray]
+    :param parallax: parallax (mas) or with astropy (can be distance with units) so astroNN will convert to appropriate units
+    :type parallax: Union[float, ndarray, astropy Quantity]
+    :param parallax_err: parallax_error (mas) or with astropy so astroNN will convert to appropriate units
+    :type parallax_err: Union[NoneType, float, ndarray, astropy Quantity]
+    :return: absolute magnitude  (with additional return of propagated error if parallax_err is provided)
+    :rtype: Union[float, ndarray]
+    :History: 2017-Oct-14 - Written - Henry Leung (University of Toronto)
+    """
+    # Check unit if available
+    if isinstance(parallax, u.Quantity):
+        original_parallax_unit = parallax.unit
+        parallax = parallax.to(default_parallax_unit, equivalencies=u.parallax())
+        if parallax_err is not None:
+            if not isinstance(parallax_err, u.Quantity):
+                # assume parallax error carry the same original unit as parallax if no units detected
+                parallax_err = (
+                    (parallax_err * original_parallax_unit)
+                    .to(default_parallax_unit)
+                    .value
+                )
+            if isinstance(parallax_err, u.Quantity):
+                parallax_err = parallax_err.to(default_parallax_unit).value
+    #     warnings.warn(f'Please be advised that astroNN mag_to_absmag() expects {default_parallax_unit.name}, '
+    #           f'astroNN has corrected the unit according to astropy unit framework')
+    # else:
+    #     warnings.warn(f'Please be advised that astroNN mag_to_absmag expects parallax in {default_parallax_unit.name}')
+
+    mag = np.array(mag)
+    parallax_unitless = np.array(
+        parallax
+    )  # Take the value as we cant apply log10 to astropy unit
+
+    magic_idx = (
+        (parallax_unitless == MAGIC_NUMBER)
+        | (mag == MAGIC_NUMBER)
+        | (mag < -90.0)
+        | np.isnan(parallax_unitless)
+        | np.isnan(mag)
+    )  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        absmag = mag + 5.0 * (np.log10(parallax_unitless) - 2.0)
+
+    if parallax_unitless.shape != ():  # check if its only 1 element
+        absmag[magic_idx] = MAGIC_NUMBER
+    else:
+        absmag = MAGIC_NUMBER if magic_idx == [1] else absmag
+    if parallax_err is None:
+        return absmag
+    else:
+        absmag_err = 5.0 * np.abs(parallax_err / (parallax_unitless * absmag))
+        if parallax_unitless.shape != ():  # check if its only 1 element
+            absmag_err[magic_idx] = MAGIC_NUMBER
+        else:
+            absmag_err = MAGIC_NUMBER if magic_idx == [1] else absmag_err
+        return absmag, absmag_err
+
+
+# noinspection PyUnresolvedReferences
+def absmag_to_pc(absmag, mag):
+    """
+    To convert absolute magnitude to parsec, Magic Number will be preserved
+
+    :param absmag: absolute magnitude
+    :type absmag: Union[float, ndarray]
+    :param mag: apparent magnitude
+    :type mag: Union[float, ndarray]
+    :return: parsec
+    :rtype: astropy Quantity
+    :History: 2017-Nov-16 - Written - Henry Leung (University of Toronto)
+    """
+    absmag = np.array(absmag)
+    mag = np.array(mag)
+    magic_idx = (
+        (absmag == MAGIC_NUMBER)
+        | (mag == MAGIC_NUMBER)
+        | np.isnan(absmag)
+        | np.isnan(mag)
+    )  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        pc = 10.0 ** (((mag - absmag) / 5.0) + 1.0)
+
+    if absmag.shape != ():  # check if its only 1 element
+        pc[magic_idx] = MAGIC_NUMBER
+        return pc * u.parsec
+    else:
+        return (MAGIC_NUMBER if magic_idx == [1] else pc) * u.parsec
+
+
+def fakemag_to_absmag(fakemag):
+    """
+    To convert fakemag to absmag, Magic Number will be preserved
+
+    :param fakemag: eastroNN fakemag
+    :type fakemag: Union[float, ndarray]
+    :return: absolute magnitude
+    :rtype: Union[float, ndarray]
+    :History: 2018-Jan-31 - Written - Henry Leung (University of Toronto)
+    """
+    fakemag = np.array(fakemag)
+    # treat non-negative fakemag as MAGIC_NUMBER
+    magic_idx = (
+        (fakemag == MAGIC_NUMBER) | (fakemag <= 0.0) | np.isnan(fakemag)
+    )  # check for magic number and negative fakemag
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        absmag = 5.0 * (np.log10(fakemag) - 2.0)
+
+    if absmag.shape != ():  # check if its only 1 element
+        absmag[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        absmag = MAGIC_NUMBER if magic_idx == [1] else absmag
+    return absmag
+
+
+def absmag_to_fakemag(absmag):
+    """
+    To convert absmag to fakemag, Magic Number will be preserved
+
+    :param absmag: absolute magnitude
+    :type absmag: Union[float, ndarray]
+    :return: astroNN fakemag
+    :rtype: Union[float, ndarray]
+    :History: 2018-Jan-31 - Written - Henry Leung (University of Toronto)
+    """
+    absmag = np.array(absmag)
+    magic_idx = (absmag == MAGIC_NUMBER) | np.isnan(absmag)  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        fakemag = 10.0 ** (0.2 * absmag + 2.0)
+    if fakemag.shape != ():  # check if its only 1 element
+        fakemag[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
+    return fakemag
+
+
+# noinspection PyUnresolvedReferences
+def fakemag_to_pc(fakemag, mag, fakemag_err=None):
+    """
+    To convert fakemag to parsec, Magic Number will be preserved
+
+    :param fakemag: astroNN fakemag
+    :type fakemag: Union[float, ndarray]
+    :param mag: apparent magnitude
+    :type mag: Union[float, ndarray]
+    :param fakemag_err: Optional, fakemag_err
+    :type fakemag_err: Union[NoneType, float, ndarray]
+    :return: array of pc with astropy Quantity (with additional return of propagated error if fakemag_err is provided)
+    :rtype: astropy Quantity
+    :History: 2018-Jan-31 - Written - Henry Leung (University of Toronto)
+    """
+    fakemag = np.array(fakemag)
+    mag = np.array(mag)
+    # treat non-positive fakemag as MAGIC_NUMBER, check for magic number and negative fakemag
+    magic_idx = (
+        (fakemag == MAGIC_NUMBER)
+        | (mag == MAGIC_NUMBER)
+        | (fakemag <= 0.0)
+        | np.isnan(fakemag)
+        | np.isnan(mag)
+    )
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        pc = 1000.0 * (10.0 ** (0.2 * mag)) / fakemag
+    if fakemag.shape != ():  # check if its only 1 element
+        pc[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        pc = MAGIC_NUMBER if magic_idx == [1] else pc
+
+    if fakemag_err is None:
+        return pc * u.parsec
+    else:
+        with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+            warnings.simplefilter("ignore")
+            pc_err = (fakemag_err / fakemag) * pc
+        if fakemag.shape != ():  # check if its only 1 element
+            pc_err[magic_idx] = MAGIC_NUMBER
+        else:  # for float
+            pc_err = MAGIC_NUMBER if magic_idx == [1] else pc_err
+        return pc * u.parsec, pc_err * u.parsec
+
+
+# noinspection PyUnresolvedReferences
+def fakemag_to_parallax(fakemag, mag, fakemag_err=None):
+    """
+    To convert fakemag to parallax, Magic Number will be preserved
+
+    :param fakemag: astroNN fakemag
+    :type fakemag: Union[float, ndarray]
+    :param mag: apparent magnitude
+    :type mag: Union[float, ndarray]
+    :param fakemag_err: Optional, fakemag_err
+    :type fakemag_err: Union[NoneType, float, ndarray]
+    :return: array of parallax in mas with astropy Quantity (with additional return of propagated error if fakemag_err is provided)
+    :rtype: astropy Quantity
+    :History: 2018-Aug-11 - Written - Henry Leung (University of Toronto)
+    """
+    fakemag = np.array(fakemag)
+    mag = np.array(mag)
+    # treat non-positive fakemag as MAGIC_NUMBER, check for magic number and negative fakemag
+    magic_idx = (
+        (fakemag == MAGIC_NUMBER)
+        | (mag == MAGIC_NUMBER)
+        | (fakemag <= 0.0)
+        | np.isnan(fakemag)
+        | np.isnan(mag)
+    )
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        parallax = fakemag / (10.0 ** (0.2 * mag))
+    if fakemag.shape != ():  # check if its only 1 element
+        parallax[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        parallax = MAGIC_NUMBER if magic_idx == [1] else parallax
+
+    if fakemag_err is None:
+        return parallax * u.mas
+    else:
+        with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+            warnings.simplefilter("ignore")
+            parallax_err = (fakemag_err / fakemag) * parallax
+        if fakemag.shape != ():  # check if its only 1 element
+            parallax_err[magic_idx] = MAGIC_NUMBER
+        else:  # for float
+            parallax_err = MAGIC_NUMBER if magic_idx == [1] else parallax_err
+        return parallax * u.mas, parallax_err * u.mas
+
+
+def fakemag_to_logsol(fakemag, band="K"):
+    """
+    | To convert fakemag to log10 solar luminosity, negative fakemag will be converted to MAGIC_NUMBER because of
+    | fakemag cannot be negative in physical world
+
+    :param fakemag: astroNN fakemag
+    :type fakemag: Union[float, ndarray]
+    :param band: band of your fakemag to use with
+    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
+    :return: log solar luminosity
+    :rtype: Union[float, ndarray]
+    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
+    """
+    fakemag = np.array(fakemag)
+    magic_idx = (
+        (fakemag == MAGIC_NUMBER) | (fakemag <= 0.0) | np.isnan(fakemag)
+    )  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        log10sol_lum = np.array(
+            0.4 * (solar_absmag_bands[band] - fakemag_to_absmag(fakemag))
+        )
+
+    if log10sol_lum.shape != ():  # check if its only 1 element
+        log10sol_lum[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        log10sol_lum = MAGIC_NUMBER if magic_idx == [1] else log10sol_lum
+    return log10sol_lum
+
+
+def absmag_to_logsol(absmag, band="K"):
+    """
+    To convert absmag to log10 solar luminosity
+
+    :param absmag: absolute magnitude
+    :type absmag: Union[float, ndarray]
+    :param band: band of your absmag to use with
+    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
+    :return: log solar luminosity
+    :rtype: Union[float, ndarray]
+    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
+    """
+    absmag = np.array(absmag)
+    magic_idx = (absmag == MAGIC_NUMBER) | np.isnan(absmag)  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        log10sol_lum = np.array(0.4 * (solar_absmag_bands[band] - absmag))
+
+    if log10sol_lum.shape != ():  # check if its only 1 element
+        log10sol_lum[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        log10sol_lum = MAGIC_NUMBER if magic_idx == [1] else log10sol_lum
+    return log10sol_lum
+
+
+def logsol_to_fakemag(logsol, band="K"):
+    """
+    | To convert log10 solar luminosity to fakemag, negative fakemag will be converted to MAGIC_NUMBER because of fakemag
+    | cannot be negative in physical world
+
+    :param logsol: log solar luminosity
+    :type logsol: Union[float, ndarray]
+    :param band: band of your fakemag to use with
+    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
+    :return: astroNN fakemag
+    :rtype: Union[float, ndarray]
+    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
+    """
+    logsol = np.array(logsol)
+    magic_idx = (logsol == MAGIC_NUMBER) | np.isnan(logsol)  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        fakemag = absmag_to_fakemag(solar_absmag_bands[band] - logsol / 0.4)
+
+    if fakemag.shape != ():  # check if its only 1 element
+        fakemag[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
+    return fakemag
+
+
+def logsol_to_absmag(logsol, band="K"):
+    """
+    | To convert log10 solar luminosity to absmag, negative fakemag will be converted to MAGIC_NUMBER because of fakemag
+    | cannot be negative in physical world
+
+    :param logsol: log solar luminosity
+    :type logsol: Union[float, ndarray]
+    :param band: band of your absmag to use with
+    :type band: str(['U', 'B', 'V', 'R', 'I', 'J', 'H', 'K','u', 'g', 'r', 'i', 'z'])
+    :return: absmag
+    :rtype: Union[float, ndarray]
+    :History: 2018-May-06 - Written - Henry Leung (University of Toronto)
+    """
+    logsol = np.array(logsol)
+    magic_idx = (logsol == MAGIC_NUMBER) | np.isnan(logsol)  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        absmag = solar_absmag_bands[band] - logsol / 0.4
+
+    if absmag.shape != ():  # check if its only 1 element
+        absmag[magic_idx] = MAGIC_NUMBER
+    else:  # for float
+        absmag = MAGIC_NUMBER if magic_idx == [1] else absmag
+    return absmag
+
+
+# noinspection PyUnresolvedReferences
+def fakemag_to_mag(fakemag, pc, pc_err=None):
+    """
+    To convert apparent magnitude to astroNN fakemag, Magic Number will be preserved
+
+    :param fakemag: fakemag
+    :type fakemag: Union[float, ndarray]
+    :param pc: parsec or with astropy (can be parallax with units) so astroNN will convert to appropriate units
+    :type pc: Union[float, ndarray, astropy Quantity]
+    :param pc_error: parsec uncertainty or with astropy so astroNN will convert to appropriate units
+    :type pc_error: Union[NoneType, float, ndarray, astropy Quantity]
+    :return: astroNN fakemag, with addition (with additional return of propagated error if parallax_err is provided)
+    :rtype: Union[float, ndarray]
+    :History: 2018-Aug-1 - Written - Henry Leung (University of Toronto)
+    """
+    # Check unit if available
+    if isinstance(pc, u.Quantity):
+        original_parallax_unit = pc.unit
+        pc = pc.to(u.parsec, equivalencies=u.parallax())
+        if pc_err is not None:
+            if not isinstance(pc_err, u.Quantity):
+                # assume parallax error carry the same original unit as parallax if no units detected
+                pc_err = (pc_err * original_parallax_unit).to(u.parsec).value
+            if isinstance(pc_err, u.Quantity):
+                pc_err = pc_err.to(u.parsec).value
+
+    fakemag = np.array(fakemag)
+    pc_unitless = np.array(pc)  # Take the value as we cant apply pow() to astropy unit
+
+    magic_idx = (
+        (pc_unitless == MAGIC_NUMBER)
+        | (fakemag == MAGIC_NUMBER)
+        | (fakemag <= 0.0)
+        | np.isnan(pc_unitless)
+        | np.isnan(fakemag)
+    )  # check for magic number
+
+    with warnings.catch_warnings():  # suppress numpy Runtime warning caused by MAGIC_NUMBER
+        warnings.simplefilter("ignore")
+        mag = np.log10((pc_unitless / 1000) * fakemag) / 0.2
+    if pc_unitless.shape != ():  # check if its only 1 element
+        mag[magic_idx] = MAGIC_NUMBER
+    else:
+        fakemag = MAGIC_NUMBER if magic_idx == [1] else fakemag
+
+    if pc_err is None:
+        return mag
+    else:
+        mag_err = np.abs((pc_err / pc) * fakemag)
+        if pc_unitless.shape != ():  # check if its only 1 element
+            mag_err[magic_idx] = MAGIC_NUMBER
+        else:
+            mag_err = MAGIC_NUMBER if magic_idx == [1] else mag_err
+        return mag, mag_err
+
+
+def extinction_correction(mag, extinction):
+    """
+    To correct magnitude with extinction, this function assumes extinction is at the same wavelength as the magnitude
+    you have provided
+
+    :param mag: apparent magnitude
+    :type mag: Union[float, ndarray]
+    :param extinction: extinction
+    :type extinction: Union[float, ndarray]
+    :return: corrected magnitude
+    :rtype: Union[float, ndarray]
+    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
+    """
+    mag = np.array(mag)
+    extinction = np.array(extinction)
+    extinction[
+        extinction < -1.0
+    ] = 0.0  # extinction cannot be that negative, if yes then assume no extinction
+    magic_idx = (
+        (mag == MAGIC_NUMBER) | (mag < -90.0) | np.isnan(mag)
+    )  # check for magic number
+
+    mag_ec = mag - extinction
+    if mag_ec.shape != ():  # check if its only 1 element
+        mag_ec[magic_idx] = MAGIC_NUMBER
+        return mag_ec
+    else:
+        return MAGIC_NUMBER if magic_idx == [1] else mag_ec
```

### Comparing `astroNN-1.0.1/astroNN/lamost/__init__.py` & `astroNN-1.1.0/astroNN/lamost/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from .chips import wavelength_solution, pseudo_continuum
-from .lamost_shared import lamost_default_dr, lamost_env
-
-
-def load_allstar_dr5():
-    """
-    Open LAMOST DR5 allstar
-
-    :return: fits file opened by astropy
-    :rtype: astropy.io.fits.hdu.hdulist.HDUList
-    :History: 2018-Jun-17 - Written - Henry Leung (University of Toronto)
-    """
-    import os
-    from astropy.io import fits
-
-    file_name = "LAMO5_2MS_AP9_SD14_UC4_PS1_AW_Carlin_M.fits"
-    _lamost_dr5_allsta_path = os.path.join(lamost_env(), "DR5", file_name)
-    if not os.path.isfile(_lamost_dr5_allsta_path):
-        raise FileNotFoundError(f'{file_name} file not found')
-    return fits.open(_lamost_dr5_allsta_path)
+from .chips import wavelength_solution, pseudo_continuum
+from .lamost_shared import lamost_default_dr, lamost_env
+
+
+def load_allstar_dr5():
+    """
+    Open LAMOST DR5 allstar
+
+    :return: fits file opened by astropy
+    :rtype: astropy.io.fits.hdu.hdulist.HDUList
+    :History: 2018-Jun-17 - Written - Henry Leung (University of Toronto)
+    """
+    import os
+    from astropy.io import fits
+
+    file_name = "LAMO5_2MS_AP9_SD14_UC4_PS1_AW_Carlin_M.fits"
+    _lamost_dr5_allsta_path = os.path.join(lamost_env(), "DR5", file_name)
+    if not os.path.isfile(_lamost_dr5_allsta_path):
+        raise FileNotFoundError(f"{file_name} file not found")
+    return fits.open(_lamost_dr5_allsta_path)
```

### Comparing `astroNN-1.0.1/astroNN/lamost/chips.py` & `astroNN-1.1.0/astroNN/lamost/chips.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,85 @@
-import numpy as np
-
-from astroNN.lamost.lamost_shared import lamost_default_dr
-
-
-def wavelength_solution(dr=None):
-    """
-    To return wavelegnth_solution
-
-    :param dr: data release
-    :type dr: Union(int, NoneType)
-    :return: wavelength solution array
-    :rtype: ndarray
-    :History: 2018-Mar-15 - Written - Henry Leung (University of Toronto)
-    """
-    lamost_default_dr(dr=dr)
-
-    # delibreately add 1e-5 to prevent numpy to generate an extra element
-    lamost_wavegrid = 10. ** np.arange(3.5682, 3.5682 - 1e-5 + 3909 * 10. ** -4., 10. ** -4.)
-
-    return lamost_wavegrid
-
-
-def smooth_spec(flux, ivar, wavelength, L=50):
-    """
-    Smooth a spectrum with a running Gaussian.
-
-    :param flux: The observed flux array.
-    :type flux: ndarray
-    :param ivar: The inverse variances of the fluxes.
-    :type ivar: ndarray
-    :param wavelength: An array of the wavelengths.
-    :type wavelength: ndarray
-    :param L: The width of the Gaussian in pixels.
-    :type L: int
-    :returns: An array of smoothed fluxes
-    :rtype: ndarray
-    """
-
-    # Partial Credit: https://github.com/chanconrad/slomp/blob/master/lamost.py
-    w = np.exp(-0.5 * (wavelength[:, None] - wavelength[None, :]) ** 2 / L ** 2)
-    denominator = np.dot(ivar, w.T)
-    numerator = np.dot(flux * ivar, w.T)
-    bad_pixel = denominator == 0
-    smoothed = np.zeros(numerator.shape)
-    smoothed[~bad_pixel] = numerator[~bad_pixel] / denominator[~bad_pixel]
-    return smoothed
-
-
-def pseudo_continuum(flux, ivar, wavelength=None, L=50, dr=None):
-    """
-    Pseudo-Continuum normalise a spectrum by dividing by a Gaussian-weighted smoothed spectrum.
-
-    :param flux: The observed flux array.
-    :type flux: ndarray
-    :param ivar: The inverse variances of the fluxes.
-    :type ivar: ndarray
-    :param wavelength: An array of the wavelengths.
-    :type wavelength: ndarray
-    :param L: [optional] The width of the Gaussian in pixels.
-    :type L: int
-    :param dr: [optional] dara release
-    :type dr: int
-    :returns: Continuum normalized flux and flux uncerteinty
-    :rtype: ndarray
-    """
-
-    # Partial Credit: https://github.com/chanconrad/slomp/blob/master/lamost.py
-    if dr is None:
-        dr = lamost_default_dr(dr)
-
-    if wavelength is None:
-        wavelength = wavelength_solution(dr=dr)
-
-    smoothed_spec = smooth_spec(wavelength, flux, ivar, L)
-    norm_flux = flux / smoothed_spec
-    norm_ivar = smoothed_spec * ivar * smoothed_spec
-
-    bad_pixel = ~np.isfinite(norm_flux)
-    norm_flux[bad_pixel] = 1.0
-    norm_ivar[bad_pixel] = 0.0
-
-    return norm_flux, norm_ivar
+import numpy as np
+
+from astroNN.lamost.lamost_shared import lamost_default_dr
+
+
+def wavelength_solution(dr=None):
+    """
+    To return wavelegnth_solution
+
+    :param dr: data release
+    :type dr: Union(int, NoneType)
+    :return: wavelength solution array
+    :rtype: ndarray
+    :History: 2018-Mar-15 - Written - Henry Leung (University of Toronto)
+    """
+    lamost_default_dr(dr=dr)
+
+    # delibreately add 1e-5 to prevent numpy to generate an extra element
+    lamost_wavegrid = 10.0 ** np.arange(
+        3.5682, 3.5682 - 1e-5 + 3909 * 10.0**-4.0, 10.0**-4.0
+    )
+
+    return lamost_wavegrid
+
+
+def smooth_spec(flux, ivar, wavelength, L=50):
+    """
+    Smooth a spectrum with a running Gaussian.
+
+    :param flux: The observed flux array.
+    :type flux: ndarray
+    :param ivar: The inverse variances of the fluxes.
+    :type ivar: ndarray
+    :param wavelength: An array of the wavelengths.
+    :type wavelength: ndarray
+    :param L: The width of the Gaussian in pixels.
+    :type L: int
+    :returns: An array of smoothed fluxes
+    :rtype: ndarray
+    """
+
+    # Partial Credit: https://github.com/chanconrad/slomp/blob/master/lamost.py
+    w = np.exp(-0.5 * (wavelength[:, None] - wavelength[None, :]) ** 2 / L**2)
+    denominator = np.dot(ivar, w.T)
+    numerator = np.dot(flux * ivar, w.T)
+    bad_pixel = denominator == 0
+    smoothed = np.zeros(numerator.shape)
+    smoothed[~bad_pixel] = numerator[~bad_pixel] / denominator[~bad_pixel]
+    return smoothed
+
+
+def pseudo_continuum(flux, ivar, wavelength=None, L=50, dr=None):
+    """
+    Pseudo-Continuum normalise a spectrum by dividing by a Gaussian-weighted smoothed spectrum.
+
+    :param flux: The observed flux array.
+    :type flux: ndarray
+    :param ivar: The inverse variances of the fluxes.
+    :type ivar: ndarray
+    :param wavelength: An array of the wavelengths.
+    :type wavelength: ndarray
+    :param L: [optional] The width of the Gaussian in pixels.
+    :type L: int
+    :param dr: [optional] dara release
+    :type dr: int
+    :returns: Continuum normalized flux and flux uncerteinty
+    :rtype: ndarray
+    """
+
+    # Partial Credit: https://github.com/chanconrad/slomp/blob/master/lamost.py
+    if dr is None:
+        dr = lamost_default_dr(dr)
+
+    if wavelength is None:
+        wavelength = wavelength_solution(dr=dr)
+
+    smoothed_spec = smooth_spec(wavelength, flux, ivar, L)
+    norm_flux = flux / smoothed_spec
+    norm_ivar = smoothed_spec * ivar * smoothed_spec
+
+    bad_pixel = ~np.isfinite(norm_flux)
+    norm_flux[bad_pixel] = 1.0
+    norm_ivar[bad_pixel] = 0.0
+
+    return norm_flux, norm_ivar
```

### Comparing `astroNN-1.0.1/astroNN/lamost/lamost_shared.py` & `astroNN-1.1.0/astroNN/lamost/lamost_shared.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-# ---------------------------------------------------------#
-#   astroNN.lamost.lamost_shared: shared functions for lamost
-# ---------------------------------------------------------#
-import os
-
-
-def lamost_env():
-    """
-    Get LAMOST environment variable
-
-    :return: Path to LAMOST Data
-    :rtype: str
-    :History: 2018-Jun-17 - Written - Henry Leung (University of Toronto)
-    """
-    from astroNN.config import ENVVAR_WARN_FLAG
-    _LAMOST = os.getenv('LASMOT_DR5_DATA')
-    if _LAMOST is None and ENVVAR_WARN_FLAG is True:
-        print("WARNING! LAMOST environment variable LASMOT_DR5_DATA not set")
-    return _LAMOST
-
-
-def lamost_default_dr(dr=None):
-    """
-    Check if dr argument is provided, if none then use default
-
-    :param dr: data release
-    :type dr: Union(int, NoneType)
-    :return: data release
-    :rtype: int
-    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
-    """
-    # enforce dr5 restriction
-    if dr is None:
-        dr = 5
-        print(f'dr is not provided, using default dr={dr}')
-    elif dr == 5:
-        pass
-    else:
-        raise ValueError('Only LAMOST DR5 is supported')
-
-    return dr
+# ---------------------------------------------------------#
+#   astroNN.lamost.lamost_shared: shared functions for lamost
+# ---------------------------------------------------------#
+import os
+
+
+def lamost_env():
+    """
+    Get LAMOST environment variable
+
+    :return: Path to LAMOST Data
+    :rtype: str
+    :History: 2018-Jun-17 - Written - Henry Leung (University of Toronto)
+    """
+    from astroNN.config import ENVVAR_WARN_FLAG
+
+    _LAMOST = os.getenv("LASMOT_DR5_DATA")
+    if _LAMOST is None and ENVVAR_WARN_FLAG is True:
+        print("WARNING! LAMOST environment variable LASMOT_DR5_DATA not set")
+    return _LAMOST
+
+
+def lamost_default_dr(dr=None):
+    """
+    Check if dr argument is provided, if none then use default
+
+    :param dr: data release
+    :type dr: Union(int, NoneType)
+    :return: data release
+    :rtype: int
+    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
+    """
+    # enforce dr5 restriction
+    if dr is None:
+        dr = 5
+        print(f"dr is not provided, using default dr={dr}")
+    elif dr == 5:
+        pass
+    else:
+        raise ValueError("Only LAMOST DR5 is supported")
+
+    return dr
```

### Comparing `astroNN-1.0.1/astroNN/models/base_cnn.py` & `astroNN-1.1.0/astroNN/models/base_cnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,458 +1,710 @@
-import json
-import os
-import time
-from abc import ABC
-
-import numpy as np
-from sklearn.model_selection import train_test_split
-
-from astroNN.config import MULTIPROCESS_FLAG
-from astroNN.config import _astroNN_MODEL_NAME
-from astroNN.config import keras_import_manager
-from astroNN.models.base_master_nn import NeuralNetMaster
-from astroNN.nn.callbacks import VirutalCSVLogger
-from astroNN.nn.losses import categorical_crossentropy, binary_crossentropy
-from astroNN.nn.losses import mean_squared_error, mean_absolute_error, mean_error
-from astroNN.nn.metrics import categorical_accuracy, binary_accuracy
-from astroNN.nn.utilities import Normalizer
-from astroNN.nn.utilities.generator import GeneratorMaster
-
-keras = keras_import_manager()
-regularizers = keras.regularizers
-ReduceLROnPlateau, EarlyStopping = keras.callbacks.ReduceLROnPlateau, keras.callbacks.EarlyStopping
-Adam = keras.optimizers.Adam
-
-
-class CNNDataGenerator(GeneratorMaster):
-    """
-    To generate data to NN
-
-    :param batch_size: batch size
-    :type batch_size: int
-    :param shuffle: Whether to shuffle batches or not
-    :type shuffle: bool
-    :param data: List of data to NN
-    :type data: list
-    :History:
-        | 2017-Dec-02 - Written - Henry Leung (University of Toronto)
-        | 2019-Feb-17 - Updated - Henry Leung (University of Toronto)
-    """
-
-    def __init__(self, batch_size, shuffle, steps_per_epoch, data):
-        super().__init__(batch_size=batch_size, shuffle=shuffle, steps_per_epoch=steps_per_epoch, data=data)
-        self.inputs = self.data[0]
-        self.labels = self.data[1]
-
-        # initial idx
-        self.idx_list = self._get_exploration_order(range(self.inputs.shape[0]))
-        self.current_idx = 0
-
-    def _data_generation(self, inputs, labels, idx_list_temp):
-        x = self.input_d_checking(inputs, idx_list_temp)
-        y = labels[idx_list_temp]
-        return x, y
-
-    def __getitem__(self, index):
-        x, y = self._data_generation(self.inputs,
-                                     self.labels,
-                                     self.idx_list[self.current_idx:self.current_idx + self.batch_size])
-        self.current_idx += self.batch_size
-        return x, y
-
-    def on_epoch_end(self):
-        # shuffle the list when epoch ends for the next epoch
-        self.idx_list = self._get_exploration_order(range(self.inputs.shape[0]))
-        # reset counter
-        self.current_idx = 0
-
-
-class CNNPredDataGenerator(GeneratorMaster):
-    """
-    To generate data to NN for prediction
-
-    :param batch_size: batch size
-    :type batch_size: int
-    :param shuffle: Whether to shuffle batches or not
-    :type shuffle: bool
-    :param data: List of data to NN
-    :type data: list
-    :History:
-        | 2017-Dec-02 - Written - Henry Leung (University of Toronto)
-        | 2019-Feb-17 - Updated - Henry Leung (University of Toronto)
-    """
-
-    def __init__(self, batch_size, shuffle, steps_per_epoch, data):
-        super().__init__(batch_size=batch_size, shuffle=shuffle, steps_per_epoch=steps_per_epoch, data=data)
-        self.inputs = self.data[0]
-
-        # initial idx
-        self.idx_list = self._get_exploration_order(range(self.inputs.shape[0]))
-        self.current_idx = 0
-
-    def _data_generation(self, inputs, idx_list_temp):
-        # Generate data
-        x = self.input_d_checking(inputs, idx_list_temp)
-        return x
-
-    def __getitem__(self, index):
-        x = self._data_generation(self.inputs, self.idx_list[self.current_idx:self.current_idx + self.batch_size])
-        self.current_idx += self.batch_size
-        return x
-
-    def on_epoch_end(self):
-        # shuffle the list when epoch ends for the next epoch
-        self.idx_list = self._get_exploration_order(range(self.inputs.shape[0]))
-        # reset counter
-        self.current_idx = 0
-
-
-class CNNBase(NeuralNetMaster, ABC):
-    """Top-level class for a convolutional neural network"""
-
-    def __init__(self):
-        """
-        NAME:
-            __init__
-        PURPOSE:
-            To define astroNN convolutional neural network
-        HISTORY:
-            2018-Jan-06 - Written - Henry Leung (University of Toronto)
-        """
-        super().__init__()
-        self.name = 'Convolutional Neural Network'
-        self._model_type = 'CNN'
-        self._model_identifier = None
-        self.initializer = None
-        self.activation = None
-        self._last_layer_activation = None
-        self.num_filters = None
-        self.filter_len = None
-        self.pool_length = None
-        self.num_hidden = None
-        self.reduce_lr_epsilon = None
-        self.reduce_lr_min = None
-        self.reduce_lr_patience = None
-        self.l1 = None
-        self.l2 = None
-        self.maxnorm = None
-        self.dropout_rate = 0.0
-        self.val_size = 0.1
-        self.early_stopping_min_delta = 0.0001
-        self.early_stopping_patience = 4
-
-        self.input_norm_mode = 1
-        self.labels_norm_mode = 2
-
-    def compile(self, optimizer=None, loss=None, metrics=None, loss_weights=None, sample_weight_mode=None):
-        if optimizer is not None:
-            self.optimizer = optimizer
-        elif self.optimizer is None or self.optimizer == 'adam':
-            self.optimizer = Adam(lr=self.lr, beta_1=self.beta_1, beta_2=self.beta_2, epsilon=self.optimizer_epsilon,
-                                  decay=0.0)
-
-        if self.task == 'regression':
-            self._last_layer_activation = 'linear'
-            loss_func = mean_squared_error
-            if self.metrics is None:
-                self.metrics = [mean_absolute_error, mean_error]
-        elif self.task == 'classification':
-            self._last_layer_activation = 'softmax'
-            loss_func = categorical_crossentropy
-            if self.metrics is None:
-                self.metrics = [categorical_accuracy]
-        elif self.task == 'binary_classification':
-            self._last_layer_activation = 'sigmoid'
-            loss_func = binary_crossentropy
-            if self.metrics is None:
-                self.metrics = [binary_accuracy(from_logits=False)]
-        else:
-            raise RuntimeError('Only "regression", "classification" and "binary_classification" are supported')
-
-        self.keras_model = self.model()
-
-        self.keras_model.compile(loss=loss_func, optimizer=self.optimizer, metrics=self.metrics, loss_weights=None)
-
-        return None
-
-    def pre_training_checklist_child(self, input_data, labels):
-        self.pre_training_checklist_master(input_data, labels)
-
-        # check if exists (exists mean fine-tuning, so we do not need calculate mean/std again)
-        if self.input_normalizer is None:
-            self.input_normalizer = Normalizer(mode=self.input_norm_mode)
-            self.labels_normalizer = Normalizer(mode=self.labels_norm_mode)
-
-            norm_data = self.input_normalizer.normalize(input_data)
-            self.input_mean, self.input_std = self.input_normalizer.mean_labels, self.input_normalizer.std_labels
-            norm_labels = self.labels_normalizer.normalize(labels)
-            self.labels_mean, self.labels_std = self.labels_normalizer.mean_labels, self.labels_normalizer.std_labels
-        else:
-            norm_data = self.input_normalizer.normalize(input_data, calc=False)
-            norm_labels = self.labels_normalizer.normalize(labels, calc=False)
-
-        if self.keras_model is None:  # only compiler if there is no keras_model, e.g. fine-tuning does not required
-            self.compile()
-
-        self.train_idx, self.val_idx = train_test_split(np.arange(self.num_train + self.val_num),
-                                                        test_size=self.val_size)
-
-        self.training_generator = CNNDataGenerator(
-            batch_size=self.batch_size,
-            shuffle=True,
-            steps_per_epoch=self.num_train // self.batch_size,
-            data=[norm_data[self.train_idx], norm_labels[self.train_idx]])
-        self.validation_generator = CNNDataGenerator(
-            batch_size=self.batch_size if len(self.val_idx) > self.batch_size else len(self.val_idx),
-            shuffle=False,
-            steps_per_epoch=max(self.val_num // self.batch_size, 1),
-            data=[norm_data[self.val_idx], norm_labels[self.val_idx]])
-
-        return input_data, labels
-
-    def train(self, input_data, labels):
-        """
-        Train a Convolutional neural network
-
-        :param input_data: Data to be trained with neural network
-        :type input_data: ndarray
-        :param labels: Labels to be trained with neural network
-        :type labels: ndarray
-        :return: None
-        :rtype: NoneType
-        :History: 2017-Dec-06 - Written - Henry Leung (University of Toronto)
-        """
-        # Call the checklist to create astroNN folder and save parameters
-        self.pre_training_checklist_child(input_data, labels)
-
-        reduce_lr = ReduceLROnPlateau(monitor='val_mean_absolute_error', factor=0.5,
-                                      min_delta=self.reduce_lr_epsilon,
-                                      patience=self.reduce_lr_patience, min_lr=self.reduce_lr_min, mode='min',
-                                      verbose=2)
-
-        early_stopping = EarlyStopping(monitor='val_mean_absolute_error', min_delta=self.early_stopping_min_delta,
-                                       patience=self.early_stopping_patience, verbose=2, mode='min')
-
-        self.virtual_cvslogger = VirutalCSVLogger()
-
-        self.__callbacks = [reduce_lr, self.virtual_cvslogger]  # default must have unchangeable callbacks
-
-        if self.callbacks is not None:
-            if isinstance(self.callbacks, list):
-                self.__callbacks.extend(self.callbacks)
-            else:
-                self.__callbacks.append(self.callbacks)
-
-        start_time = time.time()
-
-        self.history = self.keras_model.fit_generator(generator=self.training_generator,
-                                                      validation_data=self.validation_generator,
-                                                      epochs=self.max_epochs, verbose=self.verbose,
-                                                      workers=os.cpu_count(),
-                                                      callbacks=self.__callbacks,
-                                                      use_multiprocessing=MULTIPROCESS_FLAG)
-
-        print(f'Completed Training, {(time.time() - start_time):.{2}f}s in total')
-
-        if self.autosave is True:
-            # Call the post training checklist to save parameters
-            self.save()
-
-        return None
-
-    def train_on_batch(self, input_data, labels):
-        """
-        Train a neural network by running a single gradient update on all of your data, suitable for fine-tuning
-
-        :param input_data: Data to be trained with neural network
-        :type input_data: ndarray
-        :param labels: Labels to be trained with neural network
-        :type labels: ndarray
-        :return: None
-        :rtype: NoneType
-        :History: 2018-Aug-22 - Written - Henry Leung (University of Toronto)
-        """
-        self.has_model_check()
-        # check if exists (exists mean fine-tuning, so we do not need calculate mean/std again)
-        if self.input_normalizer is None:
-            self.input_normalizer = Normalizer(mode=self.input_norm_mode)
-            self.labels_normalizer = Normalizer(mode=self.labels_norm_mode)
-
-            norm_data = self.input_normalizer.normalize(input_data)
-            self.input_mean, self.input_std = self.input_normalizer.mean_labels, self.input_normalizer.std_labels
-            norm_labels = self.labels_normalizer.normalize(labels)
-            self.labels_mean, self.labels_std = self.labels_normalizer.mean_labels, self.labels_normalizer.std_labels
-        else:
-            norm_data = self.input_normalizer.normalize(input_data, calc=False)
-            norm_labels = self.labels_normalizer.normalize(labels, calc=False)
-
-        start_time = time.time()
-
-        fit_generator = CNNDataGenerator(batch_size=input_data.shape[0],
-                                         shuffle=False,
-                                         steps_per_epoch=1,
-                                         data=[norm_data, norm_labels])
-
-        scores = self.keras_model.fit_generator(generator=fit_generator,
-                                                epochs=1,
-                                                verbose=self.verbose,
-                                                workers=os.cpu_count(),
-                                                use_multiprocessing=MULTIPROCESS_FLAG)
-
-        print(f'Completed Training on Batch, {(time.time() - start_time):.{2}f}s in total')
-
-        return None
-
-    def post_training_checklist_child(self):
-        self.keras_model.save(self.fullfilepath + _astroNN_MODEL_NAME)
-        print(_astroNN_MODEL_NAME + f' saved to {(self.fullfilepath + _astroNN_MODEL_NAME)}')
-
-        self.hyper_txt.write(f"Dropout Rate: {self.dropout_rate} \n")
-        self.hyper_txt.flush()
-        self.hyper_txt.close()
-
-        data = {'id': self.__class__.__name__ if self._model_identifier is None else self._model_identifier,
-                'pool_length': self.pool_length,
-                'filterlen': self.filter_len,
-                'filternum': self.num_filters,
-                'hidden': self.num_hidden,
-                'input': self._input_shape,
-                'labels': self._labels_shape,
-                'task': self.task,
-                'last_layer_activation': self._last_layer_activation,
-                'activation': self.activation,
-                'input_mean': self.input_mean.tolist(),
-                'labels_mean': self.labels_mean.tolist(),
-                'input_std': self.input_std.tolist(),
-                'labels_std': self.labels_std.tolist(),
-                'valsize': self.val_size,
-                'targetname': self.targetname,
-                'dropout_rate': self.dropout_rate,
-                'l1': self.l1,
-                'l2': self.l2,
-                'maxnorm': self.maxnorm,
-                'input_norm_mode': self.input_norm_mode,
-                'labels_norm_mode': self.labels_norm_mode,
-                'batch_size': self.batch_size}
-
-        with open(self.fullfilepath + '/astroNN_model_parameter.json', 'w') as f:
-            json.dump(data, f, indent=4, sort_keys=True)
-
-    def test(self, input_data):
-        """
-        Use the neural network to do inference
-
-        :param input_data: Data to be inferred with neural network
-        :type input_data: ndarray
-        :return: prediction and prediction uncertainty
-        :rtype: ndarry
-        :History: 2017-Dec-06 - Written - Henry Leung (University of Toronto)
-        """
-        self.has_model_check()
-        self.pre_testing_checklist_master()
-
-        input_data = np.atleast_2d(input_data)
-
-        if self.input_normalizer is not None:
-            input_array = self.input_normalizer.normalize(input_data, calc=False)
-        else:
-            # Prevent shallow copy issue
-            input_array = np.array(input_data)
-            input_array -= self.input_mean
-            input_array /= self.input_std
-
-        total_test_num = input_data.shape[0]  # Number of testing data
-
-        # for number of training data smaller than batch_size
-        if input_data.shape[0] < self.batch_size:
-            self.batch_size = input_data.shape[0]
-
-        # Due to the nature of how generator works, no overlapped prediction
-        data_gen_shape = (total_test_num // self.batch_size) * self.batch_size
-        remainder_shape = total_test_num - data_gen_shape  # Remainder from generator
-
-        predictions = np.zeros((total_test_num, self._labels_shape))
-
-        start_time = time.time()
-        print("Starting Inference")
-
-        # Data Generator for prediction
-        prediction_generator = CNNPredDataGenerator(batch_size=self.batch_size,
-                                                    shuffle=False,
-                                                    steps_per_epoch=input_array.shape[0] // self.batch_size,
-                                                    data=[input_array[:data_gen_shape]])
-        predictions[:data_gen_shape] = np.asarray(self.keras_model.predict_generator(prediction_generator))
-
-        if remainder_shape != 0:
-            remainder_data = input_array[data_gen_shape:]
-            # assume its caused by mono images, so need to expand dim by 1
-            if len(input_array[0].shape) != len(self._input_shape):
-                remainder_data = np.expand_dims(remainder_data, axis=-1)
-            result = self.keras_model.predict(remainder_data)
-            predictions[data_gen_shape:] = result.reshape((remainder_shape, self._labels_shape))
-
-        if self.labels_normalizer is not None:
-            predictions = self.labels_normalizer.denormalize(predictions)
-        else:
-            predictions *= self.labels_std
-            predictions += self.labels_mean
-
-        print(f'Completed Inference, {(time.time() - start_time):.{2}f}s elapsed')
-
-        return predictions
-
-    def evaluate(self, input_data, labels):
-        """
-        Evaluate neural network by provided input data and labels and get back a metrics score
-
-        :param input_data: Data to be inferred with neural network
-        :type input_data: ndarray
-        :param labels: labels
-        :type labels: ndarray
-        :return: metrics score dictionary
-        :rtype: dict
-        :History: 2018-May-20 - Written - Henry Leung (University of Toronto)
-        """
-        self.has_model_check()
-        # check if exists (exists mean fine-tuning, so we do not need calculate mean/std again)
-        if self.input_normalizer is None:
-            self.input_normalizer = Normalizer(mode=self.input_norm_mode)
-            self.labels_normalizer = Normalizer(mode=self.labels_norm_mode)
-
-            norm_data = self.input_normalizer.normalize(input_data)
-            self.input_mean, self.input_std = self.input_normalizer.mean_labels, self.input_normalizer.std_labels
-            norm_labels = self.labels_normalizer.normalize(labels)
-            self.labels_mean, self.labels_std = self.labels_normalizer.mean_labels, self.labels_normalizer.std_labels
-        else:
-            norm_data = self.input_normalizer.normalize(input_data, calc=False)
-            norm_labels = self.labels_normalizer.normalize(labels, calc=False)
-
-        eval_batchsize = self.batch_size if input_data.shape[0] > self.batch_size else input_data.shape[0]
-        steps = input_data.shape[0] // self.batch_size if input_data.shape[0] > self.batch_size else 1
-
-        start_time = time.time()
-        print("Starting Evaluation")
-
-        evaluate_generator = CNNDataGenerator(batch_size=eval_batchsize,
-                                              shuffle=False,
-                                              steps_per_epoch=steps,
-                                              data=[norm_data, norm_labels])
-
-        scores = self.keras_model.evaluate_generator(evaluate_generator)
-        outputname = self.keras_model.output_names
-        funcname = []
-        if isinstance(self.keras_model.metrics, dict):
-            func_list = self.keras_model.metrics[outputname[0]]
-        else:
-            func_list = self.keras_model.metrics
-        for func in func_list:
-            if hasattr(func, __name__):
-                funcname.append(func.__name__)
-            else:
-                funcname.append(func.__class__.__name__)
-        # funcname = [func.__name__ for func in self.keras_model.metrics]
-        output_funcname = [outputname[0] + '_' + name for name in funcname]
-        list_names = ['loss', *output_funcname]
-
-        print(f'Completed Evaluation, {(time.time() - start_time):.{2}f}s elapsed')
-
-        return {name: score for name, score in zip(list_names, scores)}
+import json
+import os
+import time
+from abc import ABC
+
+import numpy as np
+from tqdm import tqdm
+from tensorflow import keras as tfk
+from astroNN.config import MULTIPROCESS_FLAG
+from astroNN.config import _astroNN_MODEL_NAME
+from astroNN.models.base_master_nn import NeuralNetMaster
+from astroNN.nn.callbacks import VirutalCSVLogger
+from astroNN.nn.losses import categorical_crossentropy, binary_crossentropy
+from astroNN.nn.losses import mean_squared_error, mean_absolute_error, mean_error
+from astroNN.nn.metrics import categorical_accuracy, binary_accuracy
+from astroNN.nn.utilities import Normalizer
+from astroNN.nn.utilities.generator import GeneratorMaster
+from astroNN.shared.dict_tools import dict_np_to_dict_list, list_to_dict
+from astroNN.shared.warnings import deprecated, deprecated_copy_signature
+from sklearn.model_selection import train_test_split
+
+regularizers = tfk.regularizers
+ReduceLROnPlateau, EarlyStopping = (
+    tfk.callbacks.ReduceLROnPlateau,
+    tfk.callbacks.EarlyStopping,
+)
+Adam = tfk.optimizers.Adam
+
+
+class CNNDataGenerator(GeneratorMaster):
+    """
+    To generate data to NN
+
+    :param batch_size: batch size
+    :type batch_size: int
+    :param shuffle: Whether to shuffle batches or not
+    :type shuffle: bool
+    :param data: List of data to NN
+    :type data: list
+    :param manual_reset: Whether need to reset the generator manually, usually it is handled by tensorflow
+    :type manual_reset: bool
+    :param sample_weight: Sample weights (if any)
+    :type sample_weight: Union([NoneType, ndarray])
+    :History:
+        | 2017-Dec-02 - Written - Henry Leung (University of Toronto)
+        | 2019-Feb-17 - Updated - Henry Leung (University of Toronto)
+    """
+
+    def __init__(
+        self,
+        batch_size,
+        shuffle,
+        steps_per_epoch,
+        data,
+        manual_reset=False,
+        sample_weight=None,
+    ):
+        super().__init__(
+            batch_size=batch_size,
+            shuffle=shuffle,
+            steps_per_epoch=steps_per_epoch,
+            data=data,
+            manual_reset=manual_reset,
+        )
+        self.inputs = self.data[0]
+        self.labels = self.data[1]
+        self.sample_weight = sample_weight
+
+        # initial idx
+        self.idx_list = self._get_exploration_order(
+            range(self.inputs["input"].shape[0])
+        )
+
+    def _data_generation(self, idx_list_temp):
+        x = self.input_d_checking(self.inputs, idx_list_temp)
+        y = {}
+        for name in self.labels.keys():
+            y.update({name: self.labels[name][idx_list_temp]})
+        if self.sample_weight is not None:
+            return x, y, self.sample_weight[idx_list_temp]
+        else:
+            return x, y
+
+    def __getitem__(self, index):
+        return self._data_generation(
+            self.idx_list[index * self.batch_size : (index + 1) * self.batch_size]
+        )
+
+    def on_epoch_end(self):
+        # shuffle the list when epoch ends for the next epoch
+        self.idx_list = self._get_exploration_order(
+            range(self.inputs["input"].shape[0])
+        )
+
+
+class CNNPredDataGenerator(GeneratorMaster):
+    """
+    To generate data to NN for prediction
+
+    :param batch_size: batch size
+    :type batch_size: int
+    :param shuffle: Whether to shuffle batches or not
+    :type shuffle: bool
+    :param data: List of data to NN
+    :type data: list
+    :param manual_reset: Whether need to reset the generator manually, usually it is handled by tensorflow
+    :type manual_reset: bool
+    :param pbar: tqdm progress bar
+    :type pbar: obj
+    :History:
+        | 2017-Dec-02 - Written - Henry Leung (University of Toronto)
+        | 2019-Feb-17 - Updated - Henry Leung (University of Toronto)
+    """
+
+    def __init__(
+        self, batch_size, shuffle, steps_per_epoch, data, manual_reset=False, pbar=None
+    ):
+        super().__init__(
+            batch_size=batch_size,
+            shuffle=shuffle,
+            steps_per_epoch=steps_per_epoch,
+            data=data,
+            manual_reset=manual_reset,
+        )
+        self.inputs = self.data[0]
+        self.pbar = pbar
+
+        # initial idx
+        self.idx_list = self._get_exploration_order(
+            range(self.inputs[list(self.inputs.keys())[0]].shape[0])
+        )
+        self.current_idx = -1
+
+    def _data_generation(self, idx_list_temp):
+        # Generate data
+        x = self.input_d_checking(self.inputs, idx_list_temp)
+        return x
+
+    def __getitem__(self, index):
+        x = self._data_generation(
+            self.idx_list[index * self.batch_size : (index + 1) * self.batch_size]
+        )
+        if self.pbar and index > self.current_idx:
+            self.pbar.update(self.batch_size)
+        self.current_idx = index
+        return x
+
+    def on_epoch_end(self):
+        # shuffle the list when epoch ends for the next epoch
+        self.idx_list = self._get_exploration_order(
+            range(self.inputs[list(self.inputs.keys())[0]].shape[0])
+        )
+        # reset counter
+
+
+class CNNBase(NeuralNetMaster, ABC):
+    """Top-level class for a convolutional neural network"""
+
+    def __init__(self):
+        """
+        NAME:
+            __init__
+        PURPOSE:
+            To define astroNN convolutional neural network
+        HISTORY:
+            2018-Jan-06 - Written - Henry Leung (University of Toronto)
+        """
+        super().__init__()
+        self.name = "Convolutional Neural Network"
+        self._model_type = "CNN"
+        self._model_identifier = None
+        self.initializer = None
+        self.activation = None
+        self._last_layer_activation = None
+        self.num_filters = None
+        self.filter_len = None
+        self.pool_length = None
+        self.num_hidden = None
+        self.reduce_lr_epsilon = None
+        self.reduce_lr_min = None
+        self.reduce_lr_patience = None
+        self.l1 = None
+        self.l2 = None
+        self.maxnorm = None
+        self.dropout_rate = 0.0
+        self.val_size = 0.1
+        self.early_stopping_min_delta = 0.0001
+        self.early_stopping_patience = 4
+
+        self.input_norm_mode = 1
+        self.labels_norm_mode = 2
+
+    def compile(
+        self,
+        optimizer=None,
+        loss=None,
+        metrics=None,
+        weighted_metrics=None,
+        loss_weights=None,
+        sample_weight_mode=None,
+    ):
+        if optimizer is not None:
+            self.optimizer = optimizer
+        elif self.optimizer is None or self.optimizer == "adam":
+            self.optimizer = Adam(
+                learning_rate=self.lr,
+                beta_1=self.beta_1,
+                beta_2=self.beta_2,
+                epsilon=self.optimizer_epsilon,
+            )
+        if metrics is not None:
+            self.metrics = metrics
+
+        if self.task == "regression":
+            self._last_layer_activation = "linear"
+            loss_func = mean_squared_error if not loss else loss
+            self.metrics = (
+                [mean_absolute_error, mean_error] if not self.metrics else self.metrics
+            )
+        elif self.task == "classification":
+            self._last_layer_activation = "softmax"
+            loss_func = categorical_crossentropy if not loss else loss
+            self.metrics = [categorical_accuracy] if not self.metrics else self.metrics
+        elif self.task == "binary_classification":
+            self._last_layer_activation = "sigmoid"
+            loss_func = binary_crossentropy if not loss else loss
+            self.metrics = [binary_accuracy] if not self.metrics else self.metrics
+        else:
+            raise RuntimeError(
+                'Only "regression", "classification" and "binary_classification" are supported'
+            )
+
+        self.keras_model = self.model()
+
+        self.keras_model.compile(
+            loss=loss_func,
+            optimizer=self.optimizer,
+            metrics=self.metrics,
+            weighted_metrics=weighted_metrics,
+            loss_weights=loss_weights,
+            sample_weight_mode=sample_weight_mode,
+        )
+
+        # inject custom training step if needed
+        try:
+            self.custom_train_step()
+        except NotImplementedError:
+            pass
+        except TypeError:
+            self.keras_model.train_step = self.custom_train_step
+        # inject custom testing  step if needed
+        try:
+            self.custom_test_step()
+        except NotImplementedError:
+            pass
+        except TypeError:
+            self.keras_model.test_step = self.custom_test_step
+
+        return None
+
+    def recompile(
+        self,
+        loss=None,
+        weighted_metrics=None,
+        loss_weights=None,
+        sample_weight_mode=None,
+    ):
+        """
+        To be used when you need to recompile a already existing model
+        """
+        if self.task == "regression":
+            self._last_layer_activation = "linear"
+            loss_func = mean_squared_error if not loss else loss
+            self.metrics = (
+                [mean_absolute_error, mean_error] if not self.metrics else self.metrics
+            )
+        elif self.task == "classification":
+            self._last_layer_activation = "softmax"
+            loss_func = categorical_crossentropy if not loss else loss
+            self.metrics = [categorical_accuracy] if not self.metrics else self.metrics
+        elif self.task == "binary_classification":
+            self._last_layer_activation = "sigmoid"
+            loss_func = binary_crossentropy if not loss else loss
+            self.metrics = [binary_accuracy] if not self.metrics else self.metrics
+        else:
+            raise RuntimeError(
+                'Only "regression", "classification" and "binary_classification" are supported'
+            )
+
+    def pre_training_checklist_child(self, input_data, labels, sample_weight):
+        # on top of checklist, convert input_data/labels to dict
+        input_data, labels = self.pre_training_checklist_master(input_data, labels)
+
+        # check if exists (existing means the model has already been trained (e.g. fine-tuning)
+        # so we do not need calculate mean/std again)
+        if self.input_normalizer is None:
+            self.input_normalizer = Normalizer(
+                mode=self.input_norm_mode, verbose=self.verbose
+            )
+            self.labels_normalizer = Normalizer(
+                mode=self.labels_norm_mode, verbose=self.verbose
+            )
+            norm_data = self.input_normalizer.normalize(input_data)
+            self.input_mean, self.input_std = (
+                self.input_normalizer.mean_labels,
+                self.input_normalizer.std_labels,
+            )
+            norm_labels = self.labels_normalizer.normalize(labels)
+            self.labels_mean, self.labels_std = (
+                self.labels_normalizer.mean_labels,
+                self.labels_normalizer.std_labels,
+            )
+        else:
+            norm_data = self.input_normalizer.normalize(input_data, calc=False)
+            norm_labels = self.labels_normalizer.normalize(labels, calc=False)
+        if (
+            self.keras_model is None
+        ):  # only compile if there is no keras_model, e.g. fine-tuning does not required
+            self.compile()
+
+        norm_data = self._tensor_dict_sanitize(norm_data, self.keras_model.input_names)
+        norm_labels = self._tensor_dict_sanitize(
+            norm_labels, self.keras_model.output_names
+        )
+
+        if self.has_val:
+            self.train_idx, self.val_idx = train_test_split(
+                np.arange(self.num_train + self.val_num), test_size=self.val_size
+            )
+        else:
+            self.train_idx = np.arange(self.num_train + self.val_num)
+            # just dummy, to minimize modification needed
+            self.val_idx = np.arange(self.num_train + self.val_num)[:2]
+
+        norm_data_training = {}
+        norm_data_val = {}
+        norm_labels_training = {}
+        norm_labels_val = {}
+        for name in norm_data.keys():
+            norm_data_training.update({name: norm_data[name][self.train_idx]})
+            norm_data_val.update({name: norm_data[name][self.val_idx]})
+        for name in norm_labels.keys():
+            norm_labels_training.update({name: norm_labels[name][self.train_idx]})
+            norm_labels_val.update({name: norm_labels[name][self.val_idx]})
+
+        if sample_weight is not None:
+            sample_weight_training = sample_weight[self.train_idx]
+            sample_weight_val = sample_weight[self.val_idx]
+        else:
+            sample_weight_training = None
+            sample_weight_val = None
+
+        self.training_generator = CNNDataGenerator(
+            batch_size=self.batch_size,
+            shuffle=True,
+            steps_per_epoch=self.num_train // self.batch_size,
+            data=[norm_data_training, norm_labels_training],
+            manual_reset=False,
+            sample_weight=sample_weight_training,
+        )
+
+        if self.has_val:
+            val_batchsize = (
+                self.batch_size
+                if len(self.val_idx) > self.batch_size
+                else len(self.val_idx)
+            )
+            self.validation_generator = CNNDataGenerator(
+                batch_size=val_batchsize,
+                shuffle=False,
+                steps_per_epoch=max(self.val_num // self.batch_size, 1),
+                data=[norm_data_val, norm_labels_val],
+                manual_reset=True,
+                sample_weight=sample_weight_val,
+            )
+
+        return input_data, labels
+
+    def fit(self, input_data, labels, sample_weight=None):
+        """
+        Train a Convolutional neural network
+
+        :param input_data: Data to be trained with neural network
+        :type input_data: ndarray
+        :param labels: Labels to be trained with neural network
+        :type labels: ndarray
+        :param sample_weight: Sample weights (if any)
+        :type sample_weight: Union([NoneType, ndarray])
+        :return: None
+        :rtype: NoneType
+        :History: 2017-Dec-06 - Written - Henry Leung (University of Toronto)
+        """
+        # Call the checklist to create astroNN folder and save parameters
+        self.pre_training_checklist_child(input_data, labels, sample_weight)
+
+        reduce_lr = ReduceLROnPlateau(
+            monitor="val_loss",
+            factor=0.5,
+            min_delta=self.reduce_lr_epsilon,
+            patience=self.reduce_lr_patience,
+            min_lr=self.reduce_lr_min,
+            mode="min",
+            verbose=self.verbose,
+        )
+
+        early_stopping = EarlyStopping(
+            monitor="val_loss",
+            min_delta=self.early_stopping_min_delta,
+            patience=self.early_stopping_patience,
+            verbose=2,
+            mode="min",
+        )
+
+        self.virtual_cvslogger = VirutalCSVLogger()
+
+        self.__callbacks = [
+            reduce_lr,
+            self.virtual_cvslogger,
+        ]  # default must have unchangeable callbacks
+
+        if self.callbacks is not None:
+            if isinstance(self.callbacks, list):
+                self.__callbacks.extend(self.callbacks)
+            else:
+                self.__callbacks.append(self.callbacks)
+
+        start_time = time.time()
+
+        self.history = self.keras_model.fit(
+            x=self.training_generator,
+            validation_data=self.validation_generator,
+            epochs=self.max_epochs,
+            verbose=self.verbose,
+            workers=os.cpu_count(),
+            callbacks=self.__callbacks,
+            use_multiprocessing=MULTIPROCESS_FLAG,
+        )
+
+        print(f"Completed Training, {(time.time() - start_time):.{2}f}s in total")
+
+        if self.autosave is True:
+            # Call the post training checklist to save parameters
+            self.save()
+
+        return None
+
+    def fit_on_batch(self, input_data, labels, sample_weight=None):
+        """
+        Train a neural network by running a single gradient update on all of your data, suitable for fine-tuning
+
+        :param input_data: Data to be trained with neural network
+        :type input_data: ndarray
+        :param labels: Labels to be trained with neural network
+        :type labels: ndarray
+        :param sample_weight: Sample weights (if any)
+        :type sample_weight: Union([NoneType, ndarray])
+        :return: None
+        :rtype: NoneType
+        :History: 2018-Aug-22 - Written - Henry Leung (University of Toronto)
+        """
+
+        input_data, labels = self.pre_training_checklist_master(input_data, labels)
+
+        # check if exists (existing means the model has already been trained (e.g. fine-tuning),
+        # so we do not need calculate mean/std again)
+        if self.input_normalizer is None:
+            self.input_normalizer = Normalizer(
+                mode=self.input_norm_mode, verbose=self.verbose
+            )
+            self.labels_normalizer = Normalizer(
+                mode=self.labels_norm_mode, verbose=self.verbose
+            )
+
+            norm_data = self.input_normalizer.normalize(input_data)
+            self.input_mean, self.input_std = (
+                self.input_normalizer.mean_labels,
+                self.input_normalizer.std_labels,
+            )
+            norm_labels = self.labels_normalizer.normalize(labels)
+            self.labels_mean, self.labels_std = (
+                self.labels_normalizer.mean_labels,
+                self.labels_normalizer.std_labels,
+            )
+        else:
+            norm_data = self.input_normalizer.normalize(input_data, calc=False)
+            norm_labels = self.labels_normalizer.normalize(labels, calc=False)
+
+        start_time = time.time()
+
+        fit_generator = CNNDataGenerator(
+            batch_size=input_data["input"].shape[0],
+            shuffle=False,
+            steps_per_epoch=1,
+            data=[norm_data, norm_labels],
+            sample_weight=sample_weight,
+        )
+
+        scores = self.keras_model.fit(
+            x=fit_generator,
+            epochs=1,
+            verbose=self.verbose,
+            workers=os.cpu_count(),
+            use_multiprocessing=MULTIPROCESS_FLAG,
+        )
+
+        print(
+            f"Completed Training on Batch, {(time.time() - start_time):.{2}f}s in total"
+        )
+
+        return None
+
+    def post_training_checklist_child(self):
+        self.keras_model.save(self.fullfilepath + _astroNN_MODEL_NAME)
+        print(
+            _astroNN_MODEL_NAME
+            + f" saved to {(self.fullfilepath + _astroNN_MODEL_NAME)}"
+        )
+
+        self.hyper_txt.write(f"Dropout Rate: {self.dropout_rate} \n")
+        self.hyper_txt.flush()
+        self.hyper_txt.close()
+
+        data = {
+            "id": self.__class__.__name__
+            if self._model_identifier is None
+            else self._model_identifier,
+            "pool_length": self.pool_length,
+            "filterlen": self.filter_len,
+            "filternum": self.num_filters,
+            "hidden": self.num_hidden,
+            "input": self._input_shape,
+            "labels": self._labels_shape,
+            "task": self.task,
+            "last_layer_activation": self._last_layer_activation,
+            "activation": self.activation,
+            "input_mean": dict_np_to_dict_list(self.input_mean),
+            "labels_mean": dict_np_to_dict_list(self.labels_mean),
+            "input_std": dict_np_to_dict_list(self.input_std),
+            "labels_std": dict_np_to_dict_list(self.labels_std),
+            "valsize": self.val_size,
+            "targetname": self.targetname,
+            "dropout_rate": self.dropout_rate,
+            "l1": self.l1,
+            "l2": self.l2,
+            "maxnorm": self.maxnorm,
+            "input_norm_mode": self.input_normalizer.normalization_mode,
+            "labels_norm_mode": self.labels_normalizer.normalization_mode,
+            "input_names": self.input_names,
+            "output_names": self.output_names,
+            "batch_size": self.batch_size,
+        }
+
+        with open(self.fullfilepath + "/astroNN_model_parameter.json", "w") as f:
+            json.dump(data, f, indent=4, sort_keys=True)
+
+    def predict(self, input_data):
+        """
+        Use the neural network to do inference
+
+        :param input_data: Data to be inferred with neural network
+        :type input_data: ndarray
+        :return: prediction and prediction uncertainty
+        :rtype: ndarry
+        :History: 2017-Dec-06 - Written - Henry Leung (University of Toronto)
+        """
+        self.has_model_check()
+        input_data = self.pre_testing_checklist_master(input_data)
+
+        input_array = self.input_normalizer.normalize(input_data, calc=False)
+        total_test_num = input_data["input"].shape[0]  # Number of testing data
+
+        # for number of training data smaller than batch_size
+        if total_test_num < self.batch_size:
+            self.batch_size = total_test_num
+
+        # Due to the nature of how generator works, no overlapped prediction
+        data_gen_shape = (total_test_num // self.batch_size) * self.batch_size
+        remainder_shape = total_test_num - data_gen_shape  # Remainder from generator
+
+        # TODO: named output????
+        predictions = np.zeros((total_test_num, self._labels_shape["output"]))
+
+        norm_data_main = {}
+        norm_data_remainder = {}
+        for name in input_array.keys():
+            norm_data_main.update({name: input_array[name][:data_gen_shape]})
+            norm_data_remainder.update({name: input_array[name][data_gen_shape:]})
+
+        norm_data_main = self._tensor_dict_sanitize(
+            norm_data_main, self.keras_model.input_names
+        )
+        norm_data_remainder = self._tensor_dict_sanitize(
+            norm_data_remainder, self.keras_model.input_names
+        )
+
+        # Data Generator for prediction
+        with tqdm(total=total_test_num, unit="sample") as pbar:
+            pbar.set_description_str("Prediction progress: ")
+            prediction_generator = CNNPredDataGenerator(
+                batch_size=self.batch_size,
+                shuffle=False,
+                steps_per_epoch=total_test_num // self.batch_size,
+                data=[norm_data_main],
+                pbar=pbar,
+            )
+            predictions[:data_gen_shape] = np.asarray(
+                self.keras_model.predict(prediction_generator, verbose=0)
+            )
+
+            if remainder_shape != 0:
+                remainder_generator = CNNPredDataGenerator(
+                    batch_size=remainder_shape,
+                    shuffle=False,
+                    steps_per_epoch=1,
+                    data=[norm_data_remainder],
+                )
+                pbar.update(remainder_shape)
+                predictions[data_gen_shape:] = np.asarray(
+                    self.keras_model.predict(remainder_generator, verbose=0)
+                )
+
+        if self.labels_normalizer is not None:
+            predictions = self.labels_normalizer.denormalize(
+                list_to_dict(self.keras_model.output_names, predictions)
+            )
+        else:
+            predictions *= self.labels_std
+            predictions += self.labels_mean
+
+        return predictions["output"]
+
+    def evaluate(self, input_data, labels):
+        """
+        Evaluate neural network by provided input data and labels and get back a metrics score
+
+        :param input_data: Data to be inferred with neural network
+        :type input_data: ndarray
+        :param labels: labels
+        :type labels: ndarray
+        :return: metrics score dictionary
+        :rtype: dict
+        :History: 2018-May-20 - Written - Henry Leung (University of Toronto)
+        """
+        self.has_model_check()
+        input_data = list_to_dict(self.keras_model.input_names, input_data)
+        labels = list_to_dict(self.keras_model.output_names, labels)
+
+        # check if exists (existing means the model has already been trained (e.g. fine-tuning), so we do not need calculate mean/std again)
+        if self.input_normalizer is None:
+            self.input_normalizer = Normalizer(
+                mode=self.input_norm_mode, verbose=self.verbose
+            )
+            self.labels_normalizer = Normalizer(
+                mode=self.labels_norm_mode, verbose=self.verbose
+            )
+
+            norm_data = self.input_normalizer.normalize(input_data)
+            self.input_mean, self.input_std = (
+                self.input_normalizer.mean_labels,
+                self.input_normalizer.std_labels,
+            )
+            norm_labels = self.labels_normalizer.normalize(labels)
+            self.labels_mean, self.labels_std = (
+                self.labels_normalizer.mean_labels,
+                self.labels_normalizer.std_labels,
+            )
+        else:
+            norm_data = self.input_normalizer.normalize(input_data, calc=False)
+            norm_labels = self.labels_normalizer.normalize(labels, calc=False)
+
+        norm_data = self._tensor_dict_sanitize(norm_data, self.keras_model.input_names)
+        norm_labels = self._tensor_dict_sanitize(
+            norm_labels, self.keras_model.output_names
+        )
+
+        total_num = input_data["input"].shape[0]
+        eval_batchsize = self.batch_size if total_num > self.batch_size else total_num
+        steps = total_num // self.batch_size if total_num > self.batch_size else 1
+
+        start_time = time.time()
+        print("Starting Evaluation")
+
+        evaluate_generator = CNNDataGenerator(
+            batch_size=eval_batchsize,
+            shuffle=False,
+            steps_per_epoch=steps,
+            data=[norm_data, norm_labels],
+        )
+
+        scores = self.keras_model.evaluate(evaluate_generator)
+        if isinstance(scores, float):  # make sure scores is iterable
+            scores = list(str(scores))
+        outputname = self.keras_model.output_names
+        funcname = self.keras_model.metrics_names
+
+        print(f"Completed Evaluation, {(time.time() - start_time):.{2}f}s elapsed")
+
+        return list_to_dict(funcname, scores)
+
+    @deprecated_copy_signature(fit)
+    def train(self, *args, **kwargs):
+        return self.fit(*args, **kwargs)
+
+    @deprecated_copy_signature(fit_on_batch)
+    def train_on_batch(self, *args, **kwargs):
+        return self.fit_on_batch(*args, **kwargs)
+
+    @deprecated_copy_signature(predict)
+    def test(self, *args, **kwargs):
+        return self.predict(*args, **kwargs)
```

### Comparing `astroNN-1.0.1/astroNN/models/misc_models.py` & `astroNN-1.1.0/astroNN/models/misc_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,221 +1,303 @@
-# ---------------------------------------------------------#
-#   astroNN.models.misc_models: Contain Misc. Models
-# ---------------------------------------------------------#
-from astroNN.config import keras_import_manager
-from astroNN.models.base_bayesian_cnn import BayesianCNNBase
-from astroNN.models.base_cnn import CNNBase
-from astroNN.nn.layers import MCDropout, PolyFit
-from astroNN.nn.losses import bayesian_binary_crossentropy_wrapper, bayesian_binary_crossentropy_var_wrapper
-from astroNN.nn.losses import bayesian_categorical_crossentropy_wrapper, bayesian_categorical_crossentropy_var_wrapper
-
-keras = keras_import_manager()
-regularizers = keras.regularizers
-
-Dense = keras.layers.Dense
-Input = keras.layers.Input
-Conv2D = keras.layers.Conv2D
-Dropout = keras.layers.Dropout
-Flatten = keras.layers.Flatten
-Activation = keras.layers.Activation
-concatenate = keras.layers.concatenate
-MaxPooling2D = keras.layers.MaxPooling2D
-
-Model = keras.models.Model
-max_norm = keras.constraints.max_norm
-
-
-class Cifar10CNN(CNNBase):
-    """
-    NAME:
-        Cifar10CNN
-    PURPOSE:
-        To create Convolutional Neural Network model for Cifar10 for the purpose of demo
-    HISTORY:
-        2018-Jan-11 - Written - Henry Leung (University of Toronto)
-    """
-
-    def __init__(self, lr=0.005):
-        """
-        NAME:
-            model
-        PURPOSE:
-            To create Convolutional Neural Network model
-        INPUT:
-        OUTPUT:
-        HISTORY:
-            2018-Jan-11 - Written - Henry Leung (University of Toronto)
-        """
-        super().__init__()
-
-        self._implementation_version = '1.0'
-        self.initializer = 'he_normal'
-        self.activation = 'relu'
-        self.num_filters = [8, 16]
-        self.filter_len = (3, 3)
-        self.pool_length = (4, 4)
-        self.num_hidden = [256, 128]
-        self.max_epochs = 30
-        self.lr = lr
-        self.reduce_lr_epsilon = 0.00005
-
-        self.reduce_lr_min = 1e-8
-        self.reduce_lr_patience = 1
-        self.l2 = 1e-4
-
-        self.task = 'classification'
-        self.targetname = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
-        self.input_norm_mode = 255
-        self.labels_norm_mode = 0
-
-    def model(self):
-        input_tensor = Input(shape=self._input_shape, name='input')
-        cnn_layer_1 = Conv2D(kernel_initializer=self.initializer, padding="same", filters=self.num_filters[0],
-                             kernel_size=self.filter_len, kernel_regularizer=regularizers.l2(self.l2))(input_tensor)
-        activation_1 = Activation(activation=self.activation)(cnn_layer_1)
-        cnn_layer_2 = Conv2D(kernel_initializer=self.initializer, padding="same", filters=self.num_filters[1],
-                             kernel_size=self.filter_len, kernel_regularizer=regularizers.l2(self.l2))(activation_1)
-        activation_2 = Activation(activation=self.activation)(cnn_layer_2)
-        maxpool_1 = MaxPooling2D(pool_size=self.pool_length)(activation_2)
-        flattener = Flatten()(maxpool_1)
-        dropout_1 = Dropout(0.2)(flattener)
-        layer_3 = Dense(units=self.num_hidden[0], kernel_regularizer=regularizers.l2(self.l2),
-                        kernel_initializer=self.initializer)(dropout_1)
-        activation_3 = Activation(activation=self.activation)(layer_3)
-        dropout_2 = Dropout(0.2)(activation_3)
-        layer_4 = Dense(units=self.num_hidden[1], kernel_regularizer=regularizers.l2(self.l2),
-                        kernel_initializer=self.initializer, kernel_constraint=max_norm(2))(dropout_2)
-        activation_4 = Activation(activation=self.activation)(layer_4)
-        layer_5 = Dense(units=self._labels_shape)(activation_4)
-        output = Activation(activation=self._last_layer_activation, name='output')(layer_5)
-
-        model = Model(inputs=input_tensor, outputs=output)
-
-        return model
-
-
-# noinspection PyCallingNonCallable
-class MNIST_BCNN(BayesianCNNBase):
-    """
-    NAME:
-        MNIST_BCNN
-    PURPOSE:
-        To create Convolutional Neural Network model for Cifar10 for the purpose of demo
-    HISTORY:
-        2018-Jan-11 - Written - Henry Leung (University of Toronto)
-    """
-
-    def __init__(self, lr=0.005):
-        """
-        NAME:
-            model
-        PURPOSE:
-            To create Convolutional Neural Network model
-        INPUT:
-        OUTPUT:
-        HISTORY:
-            2018-Jan-11 - Written - Henry Leung (University of Toronto)
-        """
-        super().__init__()
-
-        self._implementation_version = '1.0'
-        self.initializer = 'he_normal'
-        self.activation = 'relu'
-        self.num_filters = [8, 16]
-        self.filter_len = (3, 3)
-        self.pool_length = (4, 4)
-        self.num_hidden = [256, 128]
-        self.max_epochs = 30
-        self.lr = lr
-        self.reduce_lr_epsilon = 0.00005
-
-        self.reduce_lr_min = 1e-8
-        self.reduce_lr_patience = 1
-        self.l2 = 1e-4
-
-        self.task = 'classification'
-        self.targetname = ['Zero', 'One', 'Two', 'Three', 'Four', 'Five', 'Six', 'Seven', 'Eight', 'Nine']
-        self.input_norm_mode = 255
-        self.labels_norm_mode = 0
-
-    def __call__(self):
-        return self
-
-    def model(self):
-        input_tensor = Input(shape=self._input_shape, name='input')
-        cnn_layer_1 = Conv2D(kernel_initializer=self.initializer, padding="same", filters=self.num_filters[0],
-                             kernel_size=self.filter_len, kernel_regularizer=regularizers.l2(self.l2))(input_tensor)
-        activation_1 = Activation(activation=self.activation)(cnn_layer_1)
-        dropout_1 = MCDropout(self.dropout_rate, disable=self.disable_dropout)(activation_1)
-        cnn_layer_2 = Conv2D(kernel_initializer=self.initializer, padding="same", filters=self.num_filters[1],
-                             kernel_size=self.filter_len, kernel_regularizer=regularizers.l2(self.l2))(dropout_1)
-        activation_2 = Activation(activation=self.activation)(cnn_layer_2)
-        dropout_2 = MCDropout(self.dropout_rate, disable=self.disable_dropout)(activation_2)
-        maxpool_1 = MaxPooling2D(pool_size=self.pool_length)(dropout_2)
-        flattener = Flatten()(maxpool_1)
-        layer_3 = Dense(units=self.num_hidden[0], kernel_regularizer=regularizers.l2(self.l2),
-                        kernel_initializer=self.initializer)(flattener)
-        activation_3 = Activation(activation=self.activation)(layer_3)
-        dropout_4 = MCDropout(self.dropout_rate, disable=self.disable_dropout)(activation_3)
-        layer_4 = Dense(units=self.num_hidden[1], kernel_regularizer=regularizers.l2(self.l2),
-                        kernel_initializer=self.initializer, kernel_constraint=max_norm(2))(dropout_4)
-        activation_4 = Activation(activation=self.activation)(layer_4)
-        output = Dense(units=self._labels_shape, activation='linear', name='output')(activation_4)
-        output_activated = Activation(self._last_layer_activation)(output)
-        variance_output = Dense(units=self._labels_shape, activation='softplus', name='variance_output')(activation_4)
-
-        model = Model(inputs=[input_tensor], outputs=[output, variance_output])
-        # new astroNN high performance dropout variational inference on GPU expects single output
-        model_prediction = Model(inputs=[input_tensor], outputs=concatenate([output_activated, variance_output]))
-
-        if self.task == 'classification':
-            output_loss = bayesian_categorical_crossentropy_wrapper(variance_output)
-            variance_loss = bayesian_categorical_crossentropy_var_wrapper(output)
-        elif self.task == 'binary_classification':
-            output_loss = bayesian_binary_crossentropy_wrapper(variance_output)
-            variance_loss = bayesian_binary_crossentropy_var_wrapper(output)
-        else:
-            raise RuntimeError('Only "regression", "classification" and "binary_classification" are supported')
-
-        return model, model_prediction, output_loss, variance_loss
-
-
-# noinspection PyCallingNonCallable
-class SimplePolyNN(CNNBase):
-    """
-    Class for Neural Network for Gaia Polynomial fitting
-
-    :History: 2018-Jul-23 - Written - Henry Leung (University of Toronto)
-    """
-
-    def __init__(self, lr=0.005, init_w=None, use_xbias=False):
-        super().__init__()
-
-        self._implementation_version = '1.0'
-        self.max_epochs = 40
-        self.lr = lr
-        self.reduce_lr_epsilon = 0.00005
-        self.num_hidden = 3  # equals degree of polynomial to fit
-
-        self.reduce_lr_min = 1e-8
-        self.reduce_lr_patience = 2
-
-        self.input_norm_mode = 0
-        self.labels_norm_mode = 0
-        self.init_w = init_w
-        self.use_xbias = use_xbias
-        self.task = 'regression'
-        self.targetname = ['unbiased_parallax']
-
-    def model(self):
-        input_tensor = Input(shape=self._input_shape, name='input')
-        flattener = Flatten()(input_tensor)
-        output = PolyFit(deg=self.num_hidden,
-                         output_units=self._labels_shape,
-                         use_xbias=self.use_xbias,
-                         name='output',
-                         init_w=self.init_w,
-                         kernel_regularizer=regularizers.l2(self.l2))(flattener)
-
-        model = Model(inputs=input_tensor, outputs=output)
-
-        return model
+# ---------------------------------------------------------#
+#   astroNN.models.misc_models: Contain Misc. Models
+# ---------------------------------------------------------#
+from tensorflow import keras as tfk
+
+from astroNN.models.base_bayesian_cnn import BayesianCNNBase
+from astroNN.models.base_cnn import CNNBase
+from astroNN.nn.layers import MCDropout, PolyFit
+from astroNN.nn.losses import (
+    bayesian_binary_crossentropy_wrapper,
+    bayesian_binary_crossentropy_var_wrapper,
+)
+from astroNN.nn.losses import (
+    bayesian_categorical_crossentropy_wrapper,
+    bayesian_categorical_crossentropy_var_wrapper,
+)
+
+regularizers = tfk.regularizers
+
+Dense = tfk.layers.Dense
+Input = tfk.layers.Input
+Conv2D = tfk.layers.Conv2D
+Dropout = tfk.layers.Dropout
+Flatten = tfk.layers.Flatten
+Activation = tfk.layers.Activation
+concatenate = tfk.layers.concatenate
+MaxPooling2D = tfk.layers.MaxPooling2D
+
+Model = tfk.models.Model
+MaxNorm = tfk.constraints.MaxNorm
+
+
+class Cifar10CNN(CNNBase):
+    """
+    NAME:
+        Cifar10CNN
+    PURPOSE:
+        To create Convolutional Neural Network model for Cifar10 for the purpose of demo
+    HISTORY:
+        2018-Jan-11 - Written - Henry Leung (University of Toronto)
+    """
+
+    def __init__(self, lr=0.005):
+        """
+        NAME:
+            model
+        PURPOSE:
+            To create Convolutional Neural Network model
+        INPUT:
+        OUTPUT:
+        HISTORY:
+            2018-Jan-11 - Written - Henry Leung (University of Toronto)
+        """
+        super().__init__()
+
+        self._implementation_version = "1.0"
+        self.initializer = "he_normal"
+        self.activation = "relu"
+        self.num_filters = [8, 16]
+        self.filter_len = (3, 3)
+        self.pool_length = (4, 4)
+        self.num_hidden = [256, 128]
+        self.max_epochs = 30
+        self.lr = lr
+        self.reduce_lr_epsilon = 0.00005
+
+        self.reduce_lr_min = 1e-8
+        self.reduce_lr_patience = 1
+        self.l2 = 1e-4
+        self.dropout_rate = 0.1
+
+        self.task = "classification"
+        self.targetname = [
+            "airplane",
+            "automobile",
+            "bird",
+            "cat",
+            "deer",
+            "dog",
+            "frog",
+            "horse",
+            "ship",
+            "truck",
+        ]
+        self.input_norm_mode = 255
+        self.labels_norm_mode = 0
+
+    def model(self):
+        input_tensor = Input(shape=self._input_shape["input"], name="input")
+        cnn_layer_1 = Conv2D(
+            kernel_initializer=self.initializer,
+            padding="same",
+            filters=self.num_filters[0],
+            kernel_size=self.filter_len,
+            kernel_regularizer=regularizers.l2(self.l2),
+        )(input_tensor)
+        activation_1 = Activation(activation=self.activation)(cnn_layer_1)
+        cnn_layer_2 = Conv2D(
+            kernel_initializer=self.initializer,
+            padding="same",
+            filters=self.num_filters[1],
+            kernel_size=self.filter_len,
+            kernel_regularizer=regularizers.l2(self.l2),
+        )(activation_1)
+        activation_2 = Activation(activation=self.activation)(cnn_layer_2)
+        maxpool_1 = MaxPooling2D(pool_size=self.pool_length)(activation_2)
+        flattener = Flatten()(maxpool_1)
+        dropout_1 = Dropout(self.dropout_rate)(flattener)
+        layer_3 = Dense(
+            units=self.num_hidden[0],
+            kernel_regularizer=regularizers.l2(self.l2),
+            kernel_initializer=self.initializer,
+        )(dropout_1)
+        activation_3 = Activation(activation=self.activation)(layer_3)
+        dropout_2 = Dropout(self.dropout_rate)(activation_3)
+        layer_4 = Dense(
+            units=self.num_hidden[1],
+            kernel_regularizer=regularizers.l2(self.l2),
+            kernel_initializer=self.initializer,
+            kernel_constraint=MaxNorm(2),
+        )(dropout_2)
+        activation_4 = Activation(activation=self.activation)(layer_4)
+        layer_5 = Dense(units=self._labels_shape["output"])(activation_4)
+        output = Activation(activation=self._last_layer_activation, name="output")(
+            layer_5
+        )
+
+        model = Model(inputs=input_tensor, outputs=output)
+
+        return model
+
+
+# noinspection PyCallingNonCallable
+class MNIST_BCNN(BayesianCNNBase):
+    """
+    NAME:
+        MNIST_BCNN
+    PURPOSE:
+        To create Convolutional Neural Network model for Cifar10 for the purpose of demo
+    HISTORY:
+        2018-Jan-11 - Written - Henry Leung (University of Toronto)
+    """
+
+    def __init__(self, lr=0.005):
+        """
+        NAME:
+            model
+        PURPOSE:
+            To create Convolutional Neural Network model
+        INPUT:
+        OUTPUT:
+        HISTORY:
+            2018-Jan-11 - Written - Henry Leung (University of Toronto)
+        """
+        super().__init__()
+
+        self._implementation_version = "1.0"
+        self.initializer = "he_normal"
+        self.activation = "relu"
+        self.num_filters = [8, 16]
+        self.filter_len = (3, 3)
+        self.pool_length = (4, 4)
+        self.num_hidden = [256, 128]
+        self.max_epochs = 30
+        self.lr = lr
+        self.reduce_lr_epsilon = 0.00005
+
+        self.reduce_lr_min = 1e-8
+        self.reduce_lr_patience = 1
+        self.l2 = 1e-4
+        self.dropout_rate = 0.1
+
+        self.task = "classification"
+        self.targetname = [
+            "Zero",
+            "One",
+            "Two",
+            "Three",
+            "Four",
+            "Five",
+            "Six",
+            "Seven",
+            "Eight",
+            "Nine",
+        ]
+        self.input_norm_mode = 255
+        self.labels_norm_mode = 0
+
+    def model(self):
+        input_tensor = Input(shape=self._input_shape["input"], name="input")
+        cnn_layer_1 = Conv2D(
+            kernel_initializer=self.initializer,
+            padding="same",
+            filters=self.num_filters[0],
+            kernel_size=self.filter_len,
+            kernel_regularizer=regularizers.l2(self.l2),
+        )(input_tensor)
+        activation_1 = Activation(activation=self.activation)(cnn_layer_1)
+        dropout_1 = MCDropout(self.dropout_rate, disable=self.disable_dropout)(
+            activation_1
+        )
+        cnn_layer_2 = Conv2D(
+            kernel_initializer=self.initializer,
+            padding="same",
+            filters=self.num_filters[1],
+            kernel_size=self.filter_len,
+            kernel_regularizer=regularizers.l2(self.l2),
+        )(dropout_1)
+        activation_2 = Activation(activation=self.activation)(cnn_layer_2)
+        dropout_2 = MCDropout(self.dropout_rate, disable=self.disable_dropout)(
+            activation_2
+        )
+        maxpool_1 = MaxPooling2D(pool_size=self.pool_length)(dropout_2)
+        flattener = Flatten()(maxpool_1)
+        layer_3 = Dense(
+            units=self.num_hidden[0],
+            kernel_regularizer=regularizers.l2(self.l2),
+            kernel_initializer=self.initializer,
+        )(flattener)
+        activation_3 = Activation(activation=self.activation)(layer_3)
+        dropout_4 = MCDropout(self.dropout_rate, disable=self.disable_dropout)(
+            activation_3
+        )
+        layer_4 = Dense(
+            units=self.num_hidden[1],
+            kernel_regularizer=regularizers.l2(self.l2),
+            kernel_initializer=self.initializer,
+            kernel_constraint=MaxNorm(2),
+        )(dropout_4)
+        activation_4 = Activation(activation=self.activation)(layer_4)
+        output = Dense(
+            units=self._labels_shape["output"], activation="linear", name="output"
+        )(activation_4)
+        output_activated = Activation(self._last_layer_activation)(output)
+        variance_output = Dense(
+            units=self._labels_shape["output"],
+            activation="softplus",
+            name="variance_output",
+        )(activation_4)
+
+        model = Model(inputs=[input_tensor], outputs=[output, variance_output])
+        # new astroNN high performance dropout variational inference on GPU expects single output
+        model_prediction = Model(
+            inputs=[input_tensor],
+            outputs=concatenate([output_activated, variance_output]),
+        )
+
+        if self.task == "classification":
+            output_loss = bayesian_categorical_crossentropy_wrapper(variance_output)
+            variance_loss = bayesian_categorical_crossentropy_var_wrapper(output)
+        elif self.task == "binary_classification":
+            output_loss = bayesian_binary_crossentropy_wrapper(variance_output)
+            variance_loss = bayesian_binary_crossentropy_var_wrapper(output)
+        else:
+            raise RuntimeError(
+                'Only "regression", "classification" and "binary_classification" are supported'
+            )
+
+        return model, model_prediction, output_loss, variance_loss
+
+
+# noinspection PyCallingNonCallable
+class SimplePolyNN(CNNBase):
+    """
+    Class for Neural Network for Gaia Polynomial fitting
+
+    :History: 2018-Jul-23 - Written - Henry Leung (University of Toronto)
+    """
+
+    def __init__(self, lr=0.005, init_w=None, use_xbias=False):
+        super().__init__()
+
+        self._implementation_version = "1.0"
+        self.max_epochs = 40
+        self.lr = lr
+        self.reduce_lr_epsilon = 0.00005
+        self.num_hidden = 3  # equals degree of polynomial to fit
+
+        self.reduce_lr_min = 1e-8
+        self.reduce_lr_patience = 2
+
+        self.input_norm_mode = 0
+        self.labels_norm_mode = 0
+        self.init_w = init_w
+        self.use_xbias = use_xbias
+        self.task = "regression"
+        self.targetname = ["unbiased_parallax"]
+
+    def model(self):
+        input_tensor = Input(shape=self._input_shape, name="input")
+        flattener = Flatten()(input_tensor)
+        output = PolyFit(
+            deg=self.num_hidden,
+            output_units=self._labels_shape,
+            use_xbias=self.use_xbias,
+            name="output",
+            init_w=self.init_w,
+            kernel_regularizer=regularizers.l2(self.l2),
+        )(flattener)
+
+        model = Model(inputs=input_tensor, outputs=output)
+
+        return model
```

### Comparing `astroNN-1.0.1/astroNN/nn/__init__.py` & `astroNN-1.1.0/astroNN/nn/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,61 @@
-def magic_correction_term(y_true):
-    """
-    Calculate a correction term to prevent the loss being lowered by magic_num
-
-    :param y_true: Ground Truth
-    :type y_true: tf.Tensor
-    :return: Correction Term
-    :rtype: tf.Tensor
-    :History:
-        | 2018-Jan-30 - Written - Henry Leung (University of Toronto)
-        | 2018-Feb-17 - Updated - Henry Leung (University of Toronto)
-    """
-    import tensorflow as tf
-    from astroNN.config import MAGIC_NUMBER
-
-    num_nonmagic = tf.reduce_sum(tf.cast(tf.not_equal(y_true, MAGIC_NUMBER), tf.float32), axis=-1)
-    num_magic = tf.reduce_sum(tf.cast(tf.equal(y_true, MAGIC_NUMBER), tf.float32), axis=-1)
-
-    # If no magic number, then num_zero=0 and whole expression is just 1 and get back our good old loss
-    # If num_nonzero is 0, that means we don't have any information, then set the correction term to ones
-    return (num_nonmagic + num_magic) / num_nonmagic
-
-
-def reduce_var(x, axis=None, keepdims=False):
-    """
-    Calculate variance using Tensorflow (as opposed to tf.nn.moment which return both variance and mean)
-
-    :param x: Data
-    :type x: tf.Tensor
-    :param axis: Axis
-    :type axis: int
-    :param keepdims: Keeping variance dimension as data or not
-    :type keepdims: boolean
-    :return: Variance
-    :rtype: tf.Tensor
-    :History: 2018-Mar-04 - Written - Henry Leung (University of Toronto)
-    """
-    import tensorflow as tf
-
-    m = tf.reduce_mean(x, axis, True)
-    devs_squared = tf.square(x - m)
-    return tf.reduce_mean(devs_squared, axis, keepdims)
-
-
-def intpow_avx2(x, n):
-    """
-    Calculate integer power of float (including negative) even with Tensorflow compiled with AVX2 since --fast-math
-    compiler flag aggressively optimize float operation which is common with AVX2 flag
-
-    :param x: identifier
-    :type x: tf.Tensor
-    :param n: an integer power (a float will be casted to integer!!)
-    :type n: int
-    :return: powered float(s)
-    :rtype: tf.Tensor
-    :History: 2018-Aug-13 - Written - Henry Leung (University of Toronto)
-    """
-    import tensorflow as tf
-
-    # expand inputs to prepare to be tiled
-    expanded_inputs = tf.expand_dims(x, 1)
-    # we want [1, self.n]
-    return tf.reduce_prod(tf.tile(expanded_inputs, [1, n]), axis=-1)
-
-
-def nn_obj_lookup(identifier, module_obj=None, module_name='default_obj'):
-    """
-    Lookup astroNN.nn function by name
-
-    :param identifier: identifier
-    :type identifier: str
-    :param module_obj: globals()
-    :type module_obj: Union([Nonetype, dir])
-    :param module_name: module english name
-    :type module_name: str
-    :return: Looked up function
-    :rtype: function
-    :History: 2018-Apr-28 - Written - Henry Leung (University of Toronto)
-    """
-    function_name = identifier
-    fn = module_obj.get(function_name)
-    if fn is None:
-        raise ValueError('Unknown function: ' + module_name + '.' + function_name)
-    return fn
+def reduce_var(x, axis=None, keepdims=False):
+    """
+    Calculate variance using Tensorflow (as opposed to tf.nn.moment which return both variance and mean)
+
+    :param x: Data
+    :type x: tf.Tensor
+    :param axis: Axis
+    :type axis: int
+    :param keepdims: Keeping variance dimension as data or not
+    :type keepdims: boolean
+    :return: Variance
+    :rtype: tf.Tensor
+    :History: 2018-Mar-04 - Written - Henry Leung (University of Toronto)
+    """
+    import tensorflow as tf
+
+    m = tf.reduce_mean(x, axis, True)
+    devs_squared = tf.square(x - m)
+    return tf.reduce_mean(devs_squared, axis, keepdims)
+
+
+def intpow_avx2(x, n):
+    """
+    Calculate integer power of float (including negative) even with Tensorflow compiled with AVX2 since --fast-math
+    compiler flag aggressively optimize float operation which is common with AVX2 flag
+
+    :param x: identifier
+    :type x: tf.Tensor
+    :param n: an integer power (a float will be casted to integer!!)
+    :type n: int
+    :return: powered float(s)
+    :rtype: tf.Tensor
+    :History: 2018-Aug-13 - Written - Henry Leung (University of Toronto)
+    """
+    import tensorflow as tf
+
+    # expand inputs to prepare to be tiled
+    expanded_inputs = tf.expand_dims(x, 1)
+    # we want [1, self.n]
+    return tf.reduce_prod(tf.tile(expanded_inputs, [1, n]), axis=-1)
+
+
+def nn_obj_lookup(identifier, module_obj=None, module_name="default_obj"):
+    """
+    Lookup astroNN.nn function by name
+
+    :param identifier: identifier
+    :type identifier: str
+    :param module_obj: globals()
+    :type module_obj: Union([Nonetype, dir])
+    :param module_name: module english name
+    :type module_name: str
+    :return: Looked up function
+    :rtype: function
+    :History: 2018-Apr-28 - Written - Henry Leung (University of Toronto)
+    """
+    function_name = identifier
+    fn = module_obj.get(function_name)
+    if fn is None:
+        raise ValueError("Unknown function: " + module_name + "." + function_name)
+    return fn
```

### Comparing `astroNN-1.0.1/astroNN/nn/metrics.py` & `astroNN-1.1.0/astroNN/nn/metrics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-# ---------------------------------------------------------------#
-#   astroNN.nn.metrics: metrics
-# ---------------------------------------------------------------#
-
-from astroNN.nn.losses import binary_accuracy
-from astroNN.nn.losses import categorical_accuracy
-from astroNN.nn.losses import mean_absolute_error
-from astroNN.nn.losses import mean_absolute_percentage_error
-from astroNN.nn.losses import mean_error
-from astroNN.nn.losses import mean_percentage_error
-from astroNN.nn.losses import mean_squared_error
-from astroNN.nn.losses import mean_squared_logarithmic_error
-
-# Just alias functions
-mse = mean_squared_error
-mae = mean_absolute_error
-mape = mean_absolute_percentage_error
-msle = mean_squared_logarithmic_error
-me = mean_error
-mpe = mean_percentage_error
-categorical_accuracy = categorical_accuracy
-binary_accuracy = binary_accuracy
+# ---------------------------------------------------------------#
+#   astroNN.nn.metrics: metrics
+# ---------------------------------------------------------------#
+import tensorflow as tf
+
+from astroNN.nn.losses import binary_accuracy, binary_accuracy_from_logits
+from astroNN.nn.losses import categorical_accuracy
+from astroNN.nn.losses import mean_absolute_error
+from astroNN.nn.losses import mean_absolute_percentage_error
+from astroNN.nn.losses import mean_error
+from astroNN.nn.losses import mean_percentage_error
+from astroNN.nn.losses import mean_squared_error
+from astroNN.nn.losses import mean_squared_logarithmic_error
+from astroNN.nn.losses import median
+from astroNN.nn.losses import median_absolute_deviation
+from astroNN.nn.losses import median_error
+from astroNN.nn.losses import mad_std
+
+# Just alias functions
+mse = mean_squared_error
+mae = mean_absolute_error
+mape = mean_absolute_percentage_error
+msle = mean_squared_logarithmic_error
+me = mean_error
+mpe = mean_percentage_error
+categorical_accuracy = categorical_accuracy
+binary_accuracy = binary_accuracy
+binary_accuracy_from_logits = binary_accuracy_from_logits
+mad = median_absolute_deviation
```

### Comparing `astroNN-1.0.1/astroNN/nn/numpy.py` & `astroNN-1.1.0/astroNN/nn/numpy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,235 +1,257 @@
-# ---------------------------------------------------------------#
-#   astroNN.nn.numpy: tools written with numpy instead of tf
-# ---------------------------------------------------------------#
-import astropy.units as u
-import numpy as np
-
-from astroNN.config import MAGIC_NUMBER
-
-
-def sigmoid(x):
-    """
-    NumPy implementation of tf.sigmoid, mask ``magicnumber``
-
-    :param x: Data to be applied sigmoid activation
-    :type x: Union[ndarray, float]
-    :return: Sigmoid activated data
-    :rtype: Union[ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    x = np.ma.array(x, mask=(x == MAGIC_NUMBER))
-    return np.ma.divide(1, np.ma.add(1, np.divide(1, np.ma.exp(x))))
-
-
-def sigmoid_inv(x):
-    """
-    NumPy implementation of tf.sigmoid inverse, mask ``magicnumber``
-
-    :param x: Data to be applied inverse sigmoid activation
-    :type x: Union[numpy.ndarray, float]
-    :return: Inverse Sigmoid activated data
-    :rtype: Union[numpy.ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    x = np.ma.array(x, mask=(x == MAGIC_NUMBER))
-    return np.ma.log(np.ma.divide(x, np.ma.subtract(1, x)))
-
-
-def l1(x, l1=0.):
-    """
-    NumPy implementation of tf.keras.regularizers.l1
-
-    :param x: Data to have L1 regularization coefficient calculated
-    :type x: Union[ndarray, float]
-    :param l1: L1 regularization parameter
-    :type l1: Union[ndarray, float]
-    :return: L1 regularization coefficient
-    :rtype: Union[ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    l1_x = 0.
-    l1_x += np.sum(l1 * np.abs(x))
-    return l1_x
-
-
-def l2(x, l2=0.):
-    """
-    NumPy implementation of tf.keras.regularizers.l2
-
-    :param x: Data to have L2 regularization coefficient calculated
-    :type x: Union[ndarray, float]
-    :param l2: L2 regularization parameter
-    :type l2: Union[ndarray, float]
-    :return: L2 regularization coefficient
-    :rtype: Union[ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    l2_x = 0.
-    l2_x += np.sum(l2 * np.square(x))
-    return l2_x
-
-
-def relu(x):
-    """
-    NumPy implementation of tf.nn.relu
-
-    :param x: Data to have ReLU activated
-    :type x: Union[ndarray, float]
-    :return: ReLU activated data
-    :rtype: Union[ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    return x * (x > 0)
-
-
-def mape_core(x, y, axis=None, mode=None):
-    if isinstance(x, list):
-        x = np.array(x)
-    if isinstance(y, list):
-        y = np.array(y)
-    if isinstance(x, u.Quantity) and isinstance(y, u.Quantity):
-        percentage = ((x - y) / y).value
-        # still need to take the value for creating mask
-        x = x.value
-        y = y.value
-    elif (isinstance(x, u.Quantity) and not isinstance(y, u.Quantity)) or \
-            (not isinstance(x, u.Quantity) and isinstance(y, u.Quantity)):
-        raise TypeError("Only one of your data provided has astropy units \n"
-                        "Either both x and y are ndarray or both x and y are astropy.Quatity, "
-                        "return without astropy units in all case")
-    else:
-        percentage = (x - y) / y
-    if mode == 'mean':
-        return np.ma.mean(np.ma.array(np.abs(percentage) * 100., mask=((x == MAGIC_NUMBER) | (y == MAGIC_NUMBER))),
-                          axis=axis)
-    elif mode == 'median':
-        return np.ma.median(np.ma.array(np.abs(percentage) * 100., mask=[(x == MAGIC_NUMBER) | (y == MAGIC_NUMBER)]),
-                            axis=axis)
-
-
-def mean_absolute_percentage_error(x, y, axis=None):
-    """
-    | NumPy implementation of tf.keras.metrics.mean_absolute_percentage_error with capability to deal with ``magicnumber``
-      and astropy Quantity
-    | Either both x and y are ndarray or both x and y are astropy.Quatity, return has no astropy units in all case
-
-    :param x: prediction
-    :type x: Union[ndarray, float, astropy.Quatity]
-    :param y: ground truth
-    :type y: Union[ndarray, float, astropy.Quatity]
-    :param axis: NumPy axis
-    :type axis: Union[NoneType, int]
-    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
-    :return: Mean Absolute Percentage Error
-    :rtype: Union[ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    return mape_core(x, y, axis=axis, mode='mean')
-
-
-def median_absolute_percentage_error(x, y, axis=None):
-    """
-    | NumPy implementation of a median version of tf.keras.metrics.mean_absolute_percentage_error with capability to
-    | deal with ``magicnumber`` and astropy Quantity
-    | Either both x and y are ndarray or both x and y are astropy.Quatity, return has no astropy units in all case
-
-    :param x: prediction
-    :type x: Union[ndarray, float, astropy.Quatity]
-    :param y: ground truth
-    :type y: Union[ndarray, float, astropy.Quatity]
-    :param axis: NumPy axis
-    :type axis: Union[NoneType, int]
-    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
-    :return: Median Absolute Percentage Error
-    :rtype: Union[ndarray, float]
-    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
-    """
-    return mape_core(x, y, axis=axis, mode='median')
-
-
-def mae_core(x, y, axis=None, mode=None):
-    if isinstance(x, list):
-        x = np.array(x)
-    if isinstance(y, list):
-        y = np.array(y)
-    if isinstance(x, u.Quantity) and isinstance(y, u.Quantity):
-        diff = (x - y).value
-        # still need to take the value for creating mask
-        x = x.value
-        y = y.value
-    elif (isinstance(x, u.Quantity) and not isinstance(y, u.Quantity)) or \
-            (not isinstance(x, u.Quantity) and isinstance(y, u.Quantity)):
-        raise TypeError("Only one of your data provided has astropy units \n"
-                        "Either both x and y are ndarray or both x and y are astropy.Quatity, "
-                        "return without astropy units in all case")
-    else:
-        diff = (x - y)
-    if mode == 'mean':
-        return np.ma.mean(np.ma.array(np.abs(diff), mask=((x == MAGIC_NUMBER) | (y == MAGIC_NUMBER))), axis=axis)
-    elif mode == 'median':
-        return np.ma.median(np.ma.array(np.abs(diff), mask=[(x == MAGIC_NUMBER) | (y == MAGIC_NUMBER)]), axis=axis)
-
-
-def mean_absolute_error(x, y, axis=None):
-    """
-    NumPy implementation of tf.keras.metrics.mean_absolute_error  with capability to deal with ``magicnumber``
-    and astropy Quantity
-
-    Either both x and y are ndarray or both x and y are astropy.Quatity, return without astropy units in all case
-
-    :param x: prediction
-    :type x: Union[ndarray, float, astropy.Quatity]
-    :param y: ground truth
-    :type y: Union[ndarray, float, astropy.Quatity]
-    :param axis: NumPy axis
-    :type axis: Union[NoneType, int]
-    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
-    :return: Mean Absolute Error
-    :rtype: Union[ndarray, float]
-    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
-    """
-    return mae_core(x, y, axis=axis, mode='mean')
-
-
-def median_absolute_error(x, y, axis=None):
-    """
-    NumPy implementation of a median version of tf.keras.metrics.mean_absolute_error  with capability to deal with
-    ``magicnumber`` and astropy Quantity
-
-    Either both x and y are ndarray or both x and y are astropy.Quatity, return without astropy units in all case
-
-    :param x: prediction
-    :type x: Union[ndarray, float, astropy.Quatity]
-    :param y: ground truth
-    :type y: Union[ndarray, float, astropy.Quatity]
-    :param axis: NumPy axis
-    :type axis: Union[NoneType, int]
-    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
-    :return: Median Absolute Error
-    :rtype: Union[ndarray, float]
-    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
-    """
-    return mae_core(x, y, axis=axis, mode='median')
-
-
-def kl_divergence(x, y):
-    """
-    NumPy implementation of tf.distributions.kl_divergence
-
-    Either both x and y are ndarray or both x and y are astropy.Quatity, return without astropy units in all case
-
-    :param x: prediction
-    :type x: Union[ndarray, float]
-    :param y: ground truth
-    :type y: Union[ndarray, float]
-    :return: KL-divergence
-    :rtype: Union[ndarray, float]
-    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
-    """
-    if isinstance(x, list):
-        x = np.array(x)
-    if isinstance(y, list):
-        y = np.array(y)
-    x = np.clip(x, 1e-10, 1)
-    y = np.clip(y, 1e-10, 1)
-    return np.sum(x * np.log(x / y), axis=-1)
+# ---------------------------------------------------------------#
+#   astroNN.nn.numpy: tools written with numpy instead of tf
+# ---------------------------------------------------------------#
+import astropy.units as u
+import numpy as np
+
+from astroNN.config import MAGIC_NUMBER
+
+
+def sigmoid(x):
+    """
+    NumPy implementation of tf.sigmoid, mask ``magicnumber``
+
+    :param x: Data to be applied sigmoid activation
+    :type x: Union[ndarray, float]
+    :return: Sigmoid activated data
+    :rtype: Union[ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    x = np.ma.array(x, mask=(x == MAGIC_NUMBER))
+    return np.ma.divide(1, np.ma.add(1, np.divide(1, np.ma.exp(x))))
+
+
+def sigmoid_inv(x):
+    """
+    NumPy implementation of tf.sigmoid inverse, mask ``magicnumber``
+
+    :param x: Data to be applied inverse sigmoid activation
+    :type x: Union[numpy.ndarray, float]
+    :return: Inverse Sigmoid activated data
+    :rtype: Union[numpy.ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    x = np.ma.array(x, mask=(x == MAGIC_NUMBER))
+    return np.ma.log(np.ma.divide(x, np.ma.subtract(1, x)))
+
+
+def l1(x, l1=0.0):
+    """
+    NumPy implementation of tf.keras.regularizers.l1
+
+    :param x: Data to have L1 regularization coefficient calculated
+    :type x: Union[ndarray, float]
+    :param l1: L1 regularization parameter
+    :type l1: Union[ndarray, float]
+    :return: L1 regularization coefficient
+    :rtype: Union[ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    l1_x = 0.0
+    l1_x += np.sum(l1 * np.abs(x))
+    return l1_x
+
+
+def l2(x, l2=0.0):
+    """
+    NumPy implementation of tf.keras.regularizers.l2
+
+    :param x: Data to have L2 regularization coefficient calculated
+    :type x: Union[ndarray, float]
+    :param l2: L2 regularization parameter
+    :type l2: Union[ndarray, float]
+    :return: L2 regularization coefficient
+    :rtype: Union[ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    l2_x = 0.0
+    l2_x += np.sum(l2 * np.square(x))
+    return l2_x
+
+
+def relu(x):
+    """
+    NumPy implementation of tf.nn.relu
+
+    :param x: Data to have ReLU activated
+    :type x: Union[ndarray, float]
+    :return: ReLU activated data
+    :rtype: Union[ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    return x * (x > 0)
+
+
+def mape_core(x, y, axis=None, mode=None):
+    if isinstance(x, list):
+        x = np.array(x)
+    if isinstance(y, list):
+        y = np.array(y)
+    if isinstance(x, u.Quantity) and isinstance(y, u.Quantity):
+        percentage = ((x - y) / y).value
+        # still need to take the value for creating mask
+        x = x.value
+        y = y.value
+    elif (isinstance(x, u.Quantity) and not isinstance(y, u.Quantity)) or (
+        not isinstance(x, u.Quantity) and isinstance(y, u.Quantity)
+    ):
+        raise TypeError(
+            "Only one of your data provided has astropy units \n"
+            "Either both x and y are ndarray or both x and y are astropy.Quatity, "
+            "return without astropy units in all case"
+        )
+    else:
+        percentage = (x - y) / y
+    if mode == "mean":
+        return np.ma.mean(
+            np.ma.array(
+                np.abs(percentage) * 100.0,
+                mask=((x == MAGIC_NUMBER) | (y == MAGIC_NUMBER)),
+            ),
+            axis=axis,
+        )
+    elif mode == "median":
+        return np.ma.median(
+            np.ma.array(
+                np.abs(percentage) * 100.0,
+                mask=[(x == MAGIC_NUMBER) | (y == MAGIC_NUMBER)],
+            ),
+            axis=axis,
+        )
+
+
+def mean_absolute_percentage_error(x, y, axis=None):
+    """
+    | NumPy implementation of tf.keras.metrics.mean_absolute_percentage_error with capability to deal with ``magicnumber``
+      and astropy Quantity
+    | Either both x and y are ndarray or both x and y are astropy.Quatity, return has no astropy units in all case
+
+    :param x: prediction
+    :type x: Union[ndarray, float, astropy.Quatity]
+    :param y: ground truth
+    :type y: Union[ndarray, float, astropy.Quatity]
+    :param axis: NumPy axis
+    :type axis: Union[NoneType, int]
+    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
+    :return: Mean Absolute Percentage Error
+    :rtype: Union[ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    return mape_core(x, y, axis=axis, mode="mean")
+
+
+def median_absolute_percentage_error(x, y, axis=None):
+    """
+    | NumPy implementation of a median version of tf.keras.metrics.mean_absolute_percentage_error with capability to
+    | deal with ``magicnumber`` and astropy Quantity
+    | Either both x and y are ndarray or both x and y are astropy.Quatity, return has no astropy units in all case
+
+    :param x: prediction
+    :type x: Union[ndarray, float, astropy.Quatity]
+    :param y: ground truth
+    :type y: Union[ndarray, float, astropy.Quatity]
+    :param axis: NumPy axis
+    :type axis: Union[NoneType, int]
+    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
+    :return: Median Absolute Percentage Error
+    :rtype: Union[ndarray, float]
+    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
+    """
+    return mape_core(x, y, axis=axis, mode="median")
+
+
+def mae_core(x, y, axis=None, mode=None):
+    if isinstance(x, list):
+        x = np.array(x)
+    if isinstance(y, list):
+        y = np.array(y)
+    if isinstance(x, u.Quantity) and isinstance(y, u.Quantity):
+        diff = (x - y).value
+        # still need to take the value for creating mask
+        x = x.value
+        y = y.value
+    elif (isinstance(x, u.Quantity) and not isinstance(y, u.Quantity)) or (
+        not isinstance(x, u.Quantity) and isinstance(y, u.Quantity)
+    ):
+        raise TypeError(
+            "Only one of your data provided has astropy units \n"
+            "Either both x and y are ndarray or both x and y are astropy.Quatity, "
+            "return without astropy units in all case"
+        )
+    else:
+        diff = x - y
+    if mode == "mean":
+        return np.ma.mean(
+            np.ma.array(np.abs(diff), mask=((x == MAGIC_NUMBER) | (y == MAGIC_NUMBER))),
+            axis=axis,
+        )
+    elif mode == "median":
+        return np.ma.median(
+            np.ma.array(np.abs(diff), mask=[(x == MAGIC_NUMBER) | (y == MAGIC_NUMBER)]),
+            axis=axis,
+        )
+
+
+def mean_absolute_error(x, y, axis=None):
+    """
+    NumPy implementation of tf.keras.metrics.mean_absolute_error  with capability to deal with ``magicnumber``
+    and astropy Quantity
+
+    Either both x and y are ndarray or both x and y are astropy.Quatity, return without astropy units in all case
+
+    :param x: prediction
+    :type x: Union[ndarray, float, astropy.Quatity]
+    :param y: ground truth
+    :type y: Union[ndarray, float, astropy.Quatity]
+    :param axis: NumPy axis
+    :type axis: Union[NoneType, int]
+    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
+    :return: Mean Absolute Error
+    :rtype: Union[ndarray, float]
+    :History: 2018-Apr-11 - Written - Henry Leung (University of Toronto)
+    """
+    return mae_core(x, y, axis=axis, mode="mean")
+
+
+def median_absolute_error(x, y, axis=None):
+    """
+    NumPy implementation of a median version of tf.keras.metrics.mean_absolute_error  with capability to deal with
+    ``magicnumber`` and astropy Quantity
+
+    Either both x and y are ndarray or both x and y are astropy.Quatity, return without astropy units in all case
+
+    :param x: prediction
+    :type x: Union[ndarray, float, astropy.Quatity]
+    :param y: ground truth
+    :type y: Union[ndarray, float, astropy.Quatity]
+    :param axis: NumPy axis
+    :type axis: Union[NoneType, int]
+    :raise: TypeError when only either x or y contains astropy units. Both x, y should carry/not carry astropy units at the same time
+    :return: Median Absolute Error
+    :rtype: Union[ndarray, float]
+    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
+    """
+    return mae_core(x, y, axis=axis, mode="median")
+
+
+def kl_divergence(x, y):
+    """
+    NumPy implementation of tf.distributions.kl_divergence
+
+    Either both x and y are ndarray or both x and y are astropy.Quatity, return without astropy units in all case
+
+    :param x: prediction
+    :type x: Union[ndarray, float]
+    :param y: ground truth
+    :type y: Union[ndarray, float]
+    :return: KL-divergence
+    :rtype: Union[ndarray, float]
+    :History: 2018-May-13 - Written - Henry Leung (University of Toronto)
+    """
+    if isinstance(x, list):
+        x = np.array(x)
+    if isinstance(y, list):
+        y = np.array(y)
+    x = np.clip(x, 1e-10, 1)
+    y = np.clip(y, 1e-10, 1)
+    return np.sum(x * np.log(x / y), axis=-1)
```

### Comparing `astroNN-1.0.1/astroNN.egg-info/SOURCES.txt` & `astroNN-1.1.0/astroNN.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.py
 astroNN/__init__.py
 astroNN/config.py
 astroNN.egg-info/PKG-INFO
 astroNN.egg-info/SOURCES.txt
 astroNN.egg-info/dependency_links.txt
 astroNN.egg-info/requires.txt
 astroNN.egg-info/top_level.txt
 astroNN/apogee/__init__.py
 astroNN/apogee/apogee_shared.py
 astroNN/apogee/chips.py
 astroNN/apogee/downloader.py
-astroNN/apogee/plotting.py
 astroNN/data/__init__.py
 astroNN/data/anderson_2017_dr14_parallax.npz
 astroNN/data/aspcap_l31c_masks.npy
 astroNN/data/dr13_contmask.npy
 astroNN/data/dr14_contmask.npy
+astroNN/data/dr16_contmask.npy
+astroNN/data/dr17_contmask.npy
 astroNN/data/gaiadr2_apogeedr14_parallax.npz
+astroNN/data/tf1_12.patch
+astroNN/data/tf1_14.patch
+astroNN/data/tf2_5.patch
 astroNN/datasets/__init__.py
-astroNN/datasets/apogee_distances.py
-astroNN/datasets/apogee_rc.py
-astroNN/datasets/apokasc.py
+astroNN/datasets/apogee.py
 astroNN/datasets/galaxy10.py
+astroNN/datasets/galaxy10sdss.py
 astroNN/datasets/h5.py
 astroNN/datasets/xmatch.py
 astroNN/gaia/__init__.py
 astroNN/gaia/downloader.py
 astroNN/gaia/gaia_shared.py
 astroNN/lamost/__init__.py
 astroNN/lamost/chips.py
@@ -36,20 +40,42 @@
 astroNN/models/__init__.py
 astroNN/models/apogee_models.py
 astroNN/models/base_bayesian_cnn.py
 astroNN/models/base_cnn.py
 astroNN/models/base_master_nn.py
 astroNN/models/base_vae.py
 astroNN/models/misc_models.py
+astroNN/neuralode/__init__.py
+astroNN/neuralode/dop853.py
+astroNN/neuralode/odeint.py
+astroNN/neuralode/runge_kutta.py
 astroNN/nn/__init__.py
 astroNN/nn/callbacks.py
 astroNN/nn/layers.py
 astroNN/nn/losses.py
 astroNN/nn/metrics.py
 astroNN/nn/numpy.py
 astroNN/nn/utilities/__init__.py
 astroNN/nn/utilities/generator.py
 astroNN/nn/utilities/normalizer.py
 astroNN/shared/__init__.py
-astroNN/shared/custom_warnings.py
+astroNN/shared/dict_tools.py
 astroNN/shared/downloader_tools.py
-astroNN/shared/nn_tools.py
+astroNN/shared/logging.py
+astroNN/shared/matplotlib.py
+astroNN/shared/nn_tools.py
+astroNN/shared/patch_util.py
+astroNN/shared/warnings.py
+tests/__init__.py
+tests/test_apogee_model.py
+tests/test_apogee_tools.py
+tests/test_datasets.py
+tests/test_gaia_tools.py
+tests/test_lamost_tools.py
+tests/test_layers.py
+tests/test_loss_func.py
+tests/test_models.py
+tests/test_neuralODE.py
+tests/test_numpy_tools.py
+tests/test_paper_models.py
+tests/test_utilities.py
+tests/travis_tf_1_12.py
```

