# Comparing `tmp/pytorchgan-0.0.1.tar.gz` & `tmp/pytorchgan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorchgan-0.0.1.tar", last modified: Wed Apr 26 07:31:04 2023, max compression
+gzip compressed data, was "pytorchgan-0.0.2.tar", last modified: Wed Apr 26 08:00:09 2023, max compression
```

## Comparing `pytorchgan-0.0.1.tar` & `pytorchgan-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:04.042410 pytorchgan-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 07:31:00.000000 pytorchgan-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-26 07:31:04.042410 pytorchgan-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-26 07:31:00.000000 pytorchgan-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:04.042410 pytorchgan-0.0.1/pytorchgan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-26 07:31:04.000000 pytorchgan-0.0.1/pytorchgan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 07:31:04.000000 pytorchgan-0.0.1/pytorchgan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:31:04.000000 pytorchgan-0.0.1/pytorchgan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 07:31:04.000000 pytorchgan-0.0.1/pytorchgan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 07:31:04.000000 pytorchgan-0.0.1/pytorchgan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:31:04.042410 pytorchgan-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-26 07:31:02.000000 pytorchgan-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:04.042410 pytorchgan-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 07:31:00.000000 pytorchgan-0.0.1/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:04.042410 pytorchgan-0.0.1/torchgan/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 07:31:00.000000 pytorchgan-0.0.1/torchgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 07:31:00.000000 pytorchgan-0.0.1/torchgan/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:09.005717 pytorchgan-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 07:59:59.000000 pytorchgan-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-26 08:00:09.005717 pytorchgan-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-26 07:59:59.000000 pytorchgan-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:09.005717 pytorchgan-0.0.2/pytorchgan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-26 08:00:08.000000 pytorchgan-0.0.2/pytorchgan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 08:00:09.000000 pytorchgan-0.0.2/pytorchgan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:00:08.000000 pytorchgan-0.0.2/pytorchgan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 08:00:08.000000 pytorchgan-0.0.2/pytorchgan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:00:08.000000 pytorchgan-0.0.2/pytorchgan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:00:09.005717 pytorchgan-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-26 08:00:06.000000 pytorchgan-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:09.005717 pytorchgan-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-26 07:59:59.000000 pytorchgan-0.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:00:09.005717 pytorchgan-0.0.2/torchgan/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 07:59:59.000000 pytorchgan-0.0.2/torchgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-26 07:59:59.000000 pytorchgan-0.0.2/torchgan/models.py
```

### Comparing `pytorchgan-0.0.1/LICENSE` & `pytorchgan-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorchgan-0.0.1/setup.py` & `pytorchgan-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 PACKAGE_NAME = "pytorchgan"
 DESCRIPTION = 'PytorchGAN是一个基于Pytorch框架的生成对抗网络（GAN）实现库。'
 LONG_DESCRIPTION = 'PytorchGAN是一个基于Pytorch框架的生成对抗网络（GAN）实现库。GAN是一种用于生成模型的机器学习算法，其通过训练生成器和鉴别器来生成新的数据样本。PytorchGAN提供了许多经典的GAN模型实现，如DCGAN，WGAN，CGAN，CycleGAN等。PytorchGAN的主要优点之一是其使用Pytorch框架。Pytorch是一种动态图形框架，具有易于使用和调试的优点，同时也具有高度灵活性和可扩展性。因此，使用PytorchGAN可以更轻松地构建和训练GAN模型，并且可以利用Pytorch的自动微分功能来优化模型参数。'
 AUTHOR_NAME = "Xuehang Cang"
 AUTHOR_EMAIL = "xuehangcang@outlook.com"
 PROJECT_URL = "https://github.com/xuehangcang/pytorchgan"
```

