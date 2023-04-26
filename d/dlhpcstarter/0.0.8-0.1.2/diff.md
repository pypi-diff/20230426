# Comparing `tmp/dlhpcstarter-0.0.8.tar.gz` & `tmp/dlhpcstarter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlhpcstarter-0.0.8.tar", last modified: Tue Mar 14 22:49:05 2023, max compression
+gzip compressed data, was "dlhpcstarter-0.1.2.tar", last modified: Wed Apr 26 05:06:12 2023, max compression
```

## Comparing `dlhpcstarter-0.0.8.tar` & `dlhpcstarter-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.988243 dlhpcstarter-0.0.8/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11558 2022-08-31 09:00:26.000000 dlhpcstarter-0.0.8/LICENSE
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25715 2023-03-14 22:49:05.992023 dlhpcstarter-0.0.8/PKG-INFO
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25986 2023-03-13 02:21:59.000000 dlhpcstarter-0.0.8/README.md
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       84 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/pyproject.toml
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      782 2023-03-14 22:49:05.992246 dlhpcstarter-0.0.8/setup.cfg
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       96 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/setup.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.695770 dlhpcstarter-0.0.8/src/
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.839760 dlhpcstarter-0.0.8/src/dlhpcstarter/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     4227 2023-02-17 00:55:24.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/__main__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9739 2022-09-15 03:20:25.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/cluster.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     5394 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/command_line_arguments.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.914570 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/__init__.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.944041 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/ext/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/ext/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     3156 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/ext/collect_env_details.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.968041 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/mods/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/mods/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     8505 2022-09-08 10:09:36.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/tools/mods/logger.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9687 2023-02-12 10:06:04.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/trainer.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11039 2023-03-13 02:05:32.000000 dlhpcstarter-0.0.8/src/dlhpcstarter/utils.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-03-14 22:49:05.913820 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25715 2023-03-14 22:49:05.000000 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/PKG-INFO
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      678 2023-03-14 22:49:05.000000 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/SOURCES.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        1 2023-03-14 22:49:05.000000 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/dependency_links.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       60 2023-03-14 22:49:05.000000 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/entry_points.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      177 2023-03-14 22:49:05.000000 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/requires.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       13 2023-03-14 22:49:05.000000 dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/top_level.txt
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.674746 dlhpcstarter-0.1.2/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11558 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/LICENSE
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25268 2023-04-26 05:06:12.675801 dlhpcstarter-0.1.2/PKG-INFO
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25540 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/README.md
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       84 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/pyproject.toml
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      807 2023-04-26 05:06:12.678741 dlhpcstarter-0.1.2/setup.cfg
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       96 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/setup.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.081478 dlhpcstarter-0.1.2/src/
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.343139 dlhpcstarter-0.1.2/src/dlhpcstarter/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     4612 2023-04-23 22:41:30.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/__main__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9743 2023-04-23 21:42:40.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/cluster.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     5681 2023-04-23 21:40:40.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/command_line_arguments.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.602478 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/__init__.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.640087 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     3215 2023-04-16 23:14:24.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/collect_env_details.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.654293 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     8505 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/logger.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9793 2023-04-26 01:07:26.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/trainer.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11503 2023-04-24 00:26:55.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/utils.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.407275 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25268 2023-04-26 05:06:11.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/PKG-INFO
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      678 2023-04-26 05:06:12.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/SOURCES.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        1 2023-04-26 05:06:11.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/dependency_links.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       60 2023-04-26 05:06:11.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/entry_points.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      201 2023-04-26 05:06:12.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/requires.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       13 2023-04-26 05:06:12.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/top_level.txt
```

### Comparing `dlhpcstarter-0.0.8/LICENSE` & `dlhpcstarter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.0.8/PKG-INFO` & `dlhpcstarter-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: dlhpcstarter
-Version: 0.0.8
+Version: 0.1.2
 Summary: Deep Learning and HPC Starter Pack
 Home-page: https://github.com/csiro-mlai/dl_hpc_starter_pack
 Author: CSIRO
 License: Apache License 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE
 
 ![](/assets/image.png)
 
 ***Aims of this library:***
 
- - To be simple and easy to understand so that the focus is on the data science.
- - To reduce the time taken from implementation to results.
- - To promote rapid innovation of models via configuration files, class composition and/or class inheritance.
- - Reduce boilerplate code (sections of code that are repeated in multiple places with little to no variation).
- - To simplify cluster management and distributed computing with High Performance Computing (HPC).
- - Be able to easily accommodate multiple research avenues simultaneously.
- - To cooperatively improve the functionality and documentation of this repository to make it better!
+- To be simple and easy to understand so that the focus is on the data science.
+- To reduce the time taken from implementation to results.
+- To promote rapid development of models via configuration files, class composition and/or class inheritance.
+- Reduce boilerplate code (sections of code that are repeated in multiple places with little to no variation).
+- To simplify cluster management and distributed computing with High Performance Computing (HPC).
+- Be able to easily accommodate multiple research avenues simultaneously.
+- To cooperatively improve the functionality and documentation of this repository to make it better!
 
 ***Features:***
- - The [PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/latest/) `LightningModule` and `Trainer` are used to implement, train, and test models. It allows for many of the above aims to be accomplished, such as simplified distributed computing and a reduction of boilerplate code. It also allows us to simply use class inheritance and composition, allowing for rapid innovation.
- - The [Compose API](https://hydra.cc/docs/advanced/compose_api/) of [Hydra](https://hydra.cc/) is used to create a hierarchical configuration, allowing for rapid innovation.
- - [Neptune.ai](https://neptune.ai/) is used to track experiments; metric scores are automatically uploaded to [Neptune.ai](https://neptune.ai/), allowing you to easily track your experiments from your browser.
- - Scripts for submission to a cluster manager, such as [SLURM](https://slurm.schedmd.com/documentation.html) are written for you. Also, cluster manager jobs are automatically resubmitted and resumed if they haven't finished before the time-limit.
+- The [Lightning](https://pytorch-lightning.readthedocs.io/en/latest/) `LightningModule` and `Trainer` are used to implement, train, and test models. It allows for many of the above aims to be accomplished, such as simplified distributed computing and a reduction of boilerplate code. It also allows us to simply use class inheritance and composition, allowing for rapid development.
+- The [Compose API](https://hydra.cc/docs/advanced/compose_api/) of [Hydra](https://hydra.cc/) is used to create a hierarchical configuration, allowing for rapid development.
+- [Neptune.ai](https://neptune.ai/) is used to track experiments; metric scores are automatically uploaded to [Neptune.ai](https://neptune.ai/), allowing you to easily track your experiments from your browser.
+- Scripts for submission to a cluster manager, such as [SLURM](https://slurm.schedmd.com/documentation.html) are written for you. Also, cluster manager jobs are automatically resubmitted and resumed if they haven't finished before the time-limit.
 
 # Installation
 
 The Deep Learning and HPC starter pack is available on PyPI:
 ```shell
 pip install dlhpcstarter
 ```
 
 # Table of Contents
 
 [//]: # (- [How to structure your project]&#40;#how-to-structure-your-project&#41;)
 - [Package map](#package-map)
 - [Tasks](#tasks)
 - [Models](#models)
-- [Innovate via Model Composition and Inheritance](#innovate-via-model-composition-and-inheritance)
+- [Development via Model Composition and Inheritance](#development-via-model-composition-and-inheritance)
 - [Configuration YAML files and argparse](#configuration-yaml-files-and-argparse)
-- [Innovate via Configuration Files](#innovate-via-configuration-files)
+- [Development via Configuration Files](#development-via-configuration-files)
 - [Next level: Configuration composition via Hydra](#next-level-configuration-composition-via-hydra)
 - [Stages and Trainer](#stages-and-trainer)
 - [Tying it all together: `main.py`](#tying-it-all-together-mainpy)
 - [Cluster manager and distributed computing](#cluster-manager-and-distributed-computing)
 - [Monitoring using Neptune.ai](#monitoring-using-neptuneai)
 - [Where all the outputs go: `exp_dir`](#where-all-the-outputs-go-exp_dir)
 - [Repository Wish List](#repository-wish-list)
@@ -65,15 +65,15 @@
 
 [//]: # (│    │)
 
 [//]: # (│    └── TASK_NAME     - name of the task, e.g., cifar10.)
 
 [//]: # (│        └── config    - .yaml configuration files for a model.)
 
-[//]: # (│        └── models    - .py modules that contain pytorch_lightning.LightningModule definitions that represent models.)
+[//]: # (│        └── models    - .py modules that contain Lightning LightningModule definitions that represent models.)
 
 [//]: # (│        └── stages.py - training and testing stages for a task.)
 
 [//]: # (```)
 
 # Package map
 
@@ -81,76 +81,77 @@
 
 The package is structured as follows:
 
 ```
 ├──  dlhpcstarter
 │    │
 │    ├── tools                     - for all other modules; tools that are repeadetly used.
-│    ├──  __main__.py - __main__.py does the following:
-│    │               1. Reads command line arguments using argparse.
-│    │               2. Imports the 'stages' function for the task from task/TASK_NAME/stages.py.
-│    │               3. Loads the specified configuration .yaml for the job from task/TASK_NAME/config.
-│    │               4. Submits the job (the configuration + 'stages') to the cluster manager (or runs it locally if 'submit' is false).
+│    ├── __main__.py               - __main__.py does the following:
+│    │                                    1. Reads command line arguments using argparse.
+│    │                                    2. Imports the 'stages' function for the task from task/
+│    │                                    3. Loads the specified configuration .yaml for the job from 
+│    │                                    4. Submits the job (the configuration + 'stages') to the 
+│    │                                       cluster manager (or runs it locally if 'submit' is false).
 │    └── cluster.py                - contains the cluster management object.
 │    └── command_line_arguments.py - argparse for reading command line arguments.
-│    └── trainer.py                - contains a wrapper for pytorch_lightning.Trainer.
+│    └── trainer.py                - contains an optional wrapper for the Lightning Trainer.
 │    └── utils.py                  - small utility definitions.
 
 ```
 
 # Tasks
 
 ---
 
 
-***Tasks are named based on the data and the type of prediction or inference being made***. For example:
- - Two tasks have the same data but require different names due to differing predictions, e.g., **MS-COCO Detection** and **MS-COCO Caption**.
- - Two tasks may have similar predictions but require different names due to differing data, e.g., **MNIST** and **Chinese MNIST**.
+***Tasks can have any name. The name could be based on the data or the type of inference being made***. For example:
+- Two tasks have the same data but require different names due to differing predictions, e.g., **MS-COCO Detection** and **MS-COCO Caption**.
+- Two tasks may have similar predictions but require different names due to differing data, e.g., **MNIST** and **Chinese MNIST**.
 
 ***Some publicly available tasks include***:
-- Image classification tasks, e.g., [MNIST](http://yann.lecun.com/exdb/mnist/), [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet](https://www.image-net.org/). 
+- Image classification tasks, e.g., [MNIST](http://yann.lecun.com/exdb/mnist/), [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet](https://www.image-net.org/).
 - Object detection tasks, e.g., [MS-COCO Detection](https://cocodataset.org/#detection-2020).
 - Image captioning detection tasks, e.g., [MS-COCO Caption](https://cocodataset.org/#captions-2015).
 - Speech recognition tasks, e.g., [LibriSpeech](https://www.openslr.org/12).
 - Chest X-Ray report generation, e.g., [MIMIC-CXR](https://physionet.org/content/mimic-cxr/2.0.0/).
 
-***How to add a task:***
+***What does the name do?***
 
-Adding a task is as simple as creating a directory with the name of the task in `task`. For example, if we choose CIFAR10 as the task, with the task name `cifar10`, then we would create the directory `task/cifar10`. The task directory will then house everything necessary for that task, for example, the models, the configurations for the models, the data pipeline, and the stages of development (training and testing).
+It is used to separate the outputs of the experiment from other tasks.
 
 # Models
 
 ---
 
 
-***Please familiarise yourself with the [`pytorch_lightning.LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#) in order to correctly implement a model:*** https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html
+***Please familiarise yourself with the [`Lightning LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#) in order to correctly implement a model:*** https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html
 
-Once we have created our task directory (e.g., `task/cifar10`), we now want to create a model using a [`pytorch_lightning.LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#). Everything we need for the model can be placed in the `LightningModule`, in including commonly used libraries and objects, for example:
+A model is created using a [`Lightning LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#). Everything we need for the model can be placed in the `LightningModule`, including commonly used libraries and objects, for example:
 
- - [torch.nn.Module](https://pytorch.org/docs/stable/generated/torch.nn.Module.html#torch.nn.Module): base class for all neural networks in `PyTorch`. 
- - [transformers](https://huggingface.co/docs/transformers/index): a library containing pre-trained Transformer models.
- - [torchvision](https://pytorch.org/vision/stable/index.html): a library for image pre-processing and pre-trained computer vision models.
- - [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset): an object that processes each instance of a dataset.
- - [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader): an object that samples mini-batches from a [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset).
+- [torch.nn.Module](https://pytorch.org/docs/stable/generated/torch.nn.Module.html#torch.nn.Module): base class for all neural networks in `PyTorch`.
+- [transformers](https://huggingface.co/docs/transformers/index): a library containing pre-trained Transformer models.
+- [torchvision](https://pytorch.org/vision/stable/index.html): a library for image pre-processing and pre-trained computer vision models.
+- [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset): an object that processes each instance of a dataset.
+- [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader): an object that samples mini-batches from a [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset).
 
-***Note:*** 
+***Note:***
 
-- The data pipeline could be implemented within the `LightningModule` or seperately from a model using a [pytorch_lightning.LightningDataModule](https://pytorch-lightning.readthedocs.io/en/stable/extensions/datamodules.html). The `LightningModule` instance would then have to be given separately to the `pytorch_lightning.Trainer`. 
+- The data pipeline could be implemented within the `LightningModule` or seperately from a model using a [Lightning LightningDataModule](https://pytorch-lightning.readthedocs.io/en/stable/extensions/datamodules.html). The `LightningModule` instance would then have to be given separately to the `Lightning Trainer` instance.
 
 ***Example:***
 
- - An example model for `cifar10` is in [task/cifar10/model/baseline.py](https://github.com/csiro-mlai/dl_hpc_starter_pack/blob/main/task/cifar10/model/baseline.py). 
+- An example model for `cifar10` is in [task/cifar10/model/baseline.py](https://github.com/csiro-mlai/dl_hpc_starter_pack/blob/main/task/cifar10/model/baseline.py).
 
-# Innovate via Model Composition and Inheritance
+# Development via Model Composition and Inheritance
 
 ---
-To promote rapid innovation of models, we recommend using class composition and/or inheritance. ***For example, we may have a baseline that not only includes a basic model, but also the data pipeline:***
+To promote rapid development of models, one solution is to use class composition and/or inheritance. ***For example, we may have a baseline that not only includes a basic model, but also the data pipeline:***
 
 ```python
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 from torch.utils.data import DataLoader, random_split
 import torchvision
 import torch
 
 class Baseline(LightningModule):
     def __init__(self, lr, ..., **kwargs):
         super(Baseline, self).__init__()
@@ -171,15 +172,15 @@
 
     def val_dataloader(self):
         return DataLoader(self.val_set, ...)
 
     def test_dataloader(self):
         return DataLoader(self.test_set, ...)
 
-    def configure_optimizers(self):     
+    def configure_optimizers(self):
         optimiser = {'optimizer': torch.optim.SGD(self.parameters(), lr=self.lr, momentum=0.9)}
         return optimiser
 
     def forward(self, images):
         return self.model(images)
 
     def training_step(self, batch, batch_idx):
@@ -200,18 +201,18 @@
         images, labels = batch
         y_hat = self(images)
         self.test_accuracy(torch.argmax(y_hat['logits'], dim=1), labels)
         self.log_dict({'test_acc': self.test_accuracy}, ...)
 ```
 
 After training and testing the baseline, we may want to improve upon its performance. For example, if we wanted to make the following modifications:
- 
- - Use a DenseNet instead of a ResNet.
- - Use the `AdamW` optimiser.
- - Use a warmup learning rate scheduler. 
+
+- Use a DenseNet instead of a ResNet.
+- Use the `AdamW` optimiser.
+- Use a warmup learning rate scheduler.
 
 ***All we would need to do is inherit the baseline and make our modifications:***
 
 ```python
 from transformers import get_constant_schedule_with_warmup
 
 class Inheritance(Baseline):
@@ -221,24 +222,24 @@
         self.save_hyperparameters()
         self.num_warmup_steps = num_warmup_steps
         self.model = torchvision.models.densenet121(...)
 
     def configure_optimizers(self):
         optimiser = {'optimizer': torch.optim.AdamW(self.parameters(), lr=self.lr)}
         optimiser['scheduler'] = {
-                'scheduler': get_constant_schedule_with_warmup(optimiser['optimizer'], self.num_warmup_steps),
-                'interval': 'step',
-                'frequency': 1,
-            }
+            'scheduler': get_constant_schedule_with_warmup(optimiser['optimizer'], self.num_warmup_steps),
+            'interval': 'step',
+            'frequency': 1,
+        }
         return optimiser
 ```
 We could also construct a model that is the combination of the two via composition. For example, we may want to use everything from `Baseline`, but the optimiser from `Inheritance`:
 
 ```python
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 
 class Composite(LightningModule):
     def __init__(self, **kwargs):
         self.baseline = Baseline(self, **kwargs)
 
     def setup(self, stage=None):
         self.baseline.setup(stage)
@@ -248,15 +249,15 @@
 
     def val_dataloader(self):
         return self.baseline.val_dataloader()
 
     def test_dataloader(self):
         return self.baseline.test_dataloader()
 
-    def configure_optimizers(self):     
+    def configure_optimizers(self):
         return Inheritance.configure_optimizers(self)  # Use configure_optimizers() from Inheritance.
 
     def forward(self, images):
         return self.baseline.forward(images)
 
     def training_step(self, batch, batch_idx):
         return self.baseline.training_step(batch, batch_idx)
@@ -276,15 +277,15 @@
 Currently, there are two methods for giving arguments:
 
 1. **Via command line arguments using the [`argparse` module](https://docs.python.org/3/library/argparse.html)**. `argparse` mainly handles paths, development stage flags (e.g., training and testing flags), and cluster manager arguments.
 2. **Via a configuration file stored in [`YAML` format](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)**. Can handle all the arguments defined by the `argparse` plus more, including hyperparameters for the model.
 
 ***The mandatory arguments include:***
 1. `task`, the name of the task.
-2. `config`, relative or absolute path to the configuration file (can handle with or without extension).
+2. `config`, relative or absolute path to the configuration file (with or without the extension).
 3. `module`, the module that the model definition is housed.
 4. `definition`, the class representing the model.
 5. `exp_dir`, the experiment directory, i.e., where all outputs, including model checkpoints will be saved.
 6. `monitor`, metric to monitor for [ModelCheckpoint](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.ModelCheckpoint.html) and [EarlyStopping](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.EarlyStopping.html?highlight=earlystoppin#earlystopping) (optional), as well as test checkpoint loading (e.g., 'val_loss').
 7. `monitor_mode`, whether the monitored metric is to be maximised or minimised ('max' or 'min').
 
 ***`task` and `config` must be given as command line arguments for `argparse`:***
@@ -293,15 +294,15 @@
 dlhpcstarter --config task/cifar10/config/baseline --task cifar10
 ```
 
 ***`module`, `definition`, and `exp_dir` can be given either as command line arguments, or be placed in the configuration file.***
 
 For each model of a task, we define a configuration. Hyperparameters, paths, as well as the device configuration can be stored in a configuration file. Configurations are in [`YAML` format](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started), e.g., `task/cifar10/config/baseline.yaml`.
 
-# Innovate via Configuration Files
+# Development via Configuration Files
 
 ---
 
 If we have the following configuration file for the aforementioned CIFAR10  `Baseline` model, `task/cifar10/config/baseline.yaml`:
 
 ```yaml
 train: True
@@ -440,80 +441,80 @@
 
 - `task/cifar10/config/cluster/2hr.yaml`:
    ```yaml
    memory: 32GB
    time_limit: '02:00:00'
    venv_path: /path/to/my/venv/bin/activate
    ```
- - `task/cifar10/config/distributed/4gpu.yaml`:
-   ```yaml
-   num_gpus: 2
-   strategy: ddp
-   ```
- - `task/cifar10/config/paths/hpc.yaml`:
-   ```yaml
-   exp_dir: /path/to/my/experiments
-   dataset_dir: /path/to/my/dataset
-   ```
+- `task/cifar10/config/distributed/4gpu.yaml`:
+  ```yaml
+  num_gpus: 2
+  strategy: ddp
+  ```
+- `task/cifar10/config/paths/hpc.yaml`:
+  ```yaml
+  exp_dir: /path/to/my/experiments
+  dataset_dir: /path/to/my/dataset
+  ```
 
 See the following documentation for more information:
- - https://hydra.cc/docs/1.2/tutorials/basic/your_first_app/defaults/
- - https://hydra.cc/docs/1.2/advanced/defaults_list/#composition-order
- - https://hydra.cc/docs/1.2/advanced/overriding_packages/
+- https://hydra.cc/docs/1.2/tutorials/basic/your_first_app/defaults/
+- https://hydra.cc/docs/1.2/advanced/defaults_list/#composition-order
+- https://hydra.cc/docs/1.2/advanced/overriding_packages/
 
 # Stages and Trainer
 
 ---
 
 
-In each task directory is a Python module called `stages.py`, which contains the `stages` definition. This definition takes an object as input that houses the configuration for a job.  
+In each task directory is a Python module called `stages.py`, which contains the `stages` definition. This definition takes an object as input that houses the configuration for a job.
 
 Typically, the following things happen in `stages()`:
 
- - The `LightningModule` model is imported via the `model` argument, e.g.,
-    ```python
-    from src import importer
-   
-    Model = importer(definition=args.definition, module=args.module)
-    model = Model(**vars(args))
-   ```
-    See `src.utils.importer` for a handy function that imports based on strings.
- - A `pytorch_lightning.Trainer` instance is created, e.g., `trainer = pytorch_lightning.Trainer(...)`.
- - The model is trained using trainer: `trainer.fit(model)`.
- - The model is tested using trainer: `trainer.test(model)`.
+- The `LightningModule` model is imported via the `model` argument, e.g.,
+   ```python
+   from src import importer
+  
+   Model = importer(definition=args.definition, module=args.module)
+   model = Model(**vars(args))
+  ```
+  See `src.utils.importer` for a handy function that imports based on strings.
+- A `Lightning Trainer` instance is created, e.g., `trainer = lightning.pytorch.Trainer(...)`.
+- The model is trained using trainer: `trainer.fit(model)`.
+- The model is tested using trainer: `trainer.test(model)`.
 
-It handles the training and testing of a model for a task by using a [`pytorch_lightning.Trainer`](https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html).
+It handles the training and testing of a model for a task by using a [`Lightning Trainer`](https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html).
 
-***A helpful wrapper at `src/trainer.py` exists that passes frequently used and useful `callbacks`, `loggers`, and `plugins` to a `pytorch_lightning.Trainer` instance:***
+***A helpful wrapper at `src/trainer.py` exists that passes frequently used and useful `callbacks`, `loggers`, and `plugins` to a `Lightning Trainer` instance:***
 
 ```python
 from src.dlhpcstarter.trainer import trainer_instance
 
 trainer = trainer_instance(**vars(args))
 ```
-Place any of the parameters for the trainer detailed at 
-https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api in your configuration file, and they will be passed to the `pytorch_lightning.Trainer` instance.
+Place any of the parameters for the trainer detailed at
+https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api in your configuration file, and they will be passed to the `Lightning Trainer` instance.
 
 # Tying it all together: `dlhpcstarter`
 
 ---
 
 ***This is an overview of what occurs when the entrypoint `dlhpcstarter` is executed, this is not necessary to understand to use the package.***
 
 
 
 `dlhpcstarter` does the following:
 
- - Gets the command line arguments using `argparse`, e.g., arguments like this:
-    ```shell
-    dlhpcstarter --config task.cifar10.config.baseline --task cifar10
-    ```
- - Imports the `stages` definition for the task using `src.utils.importer`.
- - Reads the configuration `.yaml` and combines it with the command line arguments.
- - Submits `stages` to the cluster manager if `args.submit = True` or runs `stages` locally. The command line arguments and the configuration arguments are passed to `stages` in both cases.
+- Gets the command line arguments using `argparse`, e.g., arguments like this:
+   ```shell
+   dlhpcstarter --config task.cifar10.config.baseline --task cifar10
+   ```
+- Imports the `stages` definition for the task using `src.utils.importer`.
+- Reads the configuration `.yaml` and combines it with the command line arguments.
+- Submits `stages` to the cluster manager if `args.submit = True` or runs `stages` locally. The command line arguments and the configuration arguments are passed to `stages` in both cases.
 
 # Cluster manager and distributed computing
 
 ---
 
 The following arguments are used for distributed computing:
 
@@ -596,13 +597,13 @@
 
 ***Description to be finished.
 
 
 # Repository Wish List
 
 ---
- - Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
- - Add description about how to use https://neptune.ai/.
- - Use https://hydra.cc/ instead of argparse (or have the option to use either).
- - https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
- - Notebook examples.
+- Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
+- Add description about how to use https://neptune.ai/.
+- Use https://hydra.cc/ instead of argparse (or have the option to use either).
+- https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
+- Notebook examples.
```

### Comparing `dlhpcstarter-0.0.8/README.md` & `dlhpcstarter-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 ![](/assets/image.png)
 
 ***Aims of this library:***
 
- - To be simple and easy to understand so that the focus is on the data science.
- - To reduce the time taken from implementation to results.
- - To promote rapid innovation of models via configuration files, class composition and/or class inheritance.
- - Reduce boilerplate code (sections of code that are repeated in multiple places with little to no variation).
- - To simplify cluster management and distributed computing with High Performance Computing (HPC).
- - Be able to easily accommodate multiple research avenues simultaneously.
- - To cooperatively improve the functionality and documentation of this repository to make it better!
+- To be simple and easy to understand so that the focus is on the data science.
+- To reduce the time taken from implementation to results.
+- To promote rapid development of models via configuration files, class composition and/or class inheritance.
+- Reduce boilerplate code (sections of code that are repeated in multiple places with little to no variation).
+- To simplify cluster management and distributed computing with High Performance Computing (HPC).
+- Be able to easily accommodate multiple research avenues simultaneously.
+- To cooperatively improve the functionality and documentation of this repository to make it better!
 
 ***Features:***
- - The [PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/latest/) `LightningModule` and `Trainer` are used to implement, train, and test models. It allows for many of the above aims to be accomplished, such as simplified distributed computing and a reduction of boilerplate code. It also allows us to simply use class inheritance and composition, allowing for rapid innovation.
- - The [Compose API](https://hydra.cc/docs/advanced/compose_api/) of [Hydra](https://hydra.cc/) is used to create a hierarchical configuration, allowing for rapid innovation.
- - [Neptune.ai](https://neptune.ai/) is used to track experiments; metric scores are automatically uploaded to [Neptune.ai](https://neptune.ai/), allowing you to easily track your experiments from your browser.
- - Scripts for submission to a cluster manager, such as [SLURM](https://slurm.schedmd.com/documentation.html) are written for you. Also, cluster manager jobs are automatically resubmitted and resumed if they haven't finished before the time-limit.
+- The [Lightning](https://pytorch-lightning.readthedocs.io/en/latest/) `LightningModule` and `Trainer` are used to implement, train, and test models. It allows for many of the above aims to be accomplished, such as simplified distributed computing and a reduction of boilerplate code. It also allows us to simply use class inheritance and composition, allowing for rapid development.
+- The [Compose API](https://hydra.cc/docs/advanced/compose_api/) of [Hydra](https://hydra.cc/) is used to create a hierarchical configuration, allowing for rapid development.
+- [Neptune.ai](https://neptune.ai/) is used to track experiments; metric scores are automatically uploaded to [Neptune.ai](https://neptune.ai/), allowing you to easily track your experiments from your browser.
+- Scripts for submission to a cluster manager, such as [SLURM](https://slurm.schedmd.com/documentation.html) are written for you. Also, cluster manager jobs are automatically resubmitted and resumed if they haven't finished before the time-limit.
 
 # Installation
 
 The Deep Learning and HPC starter pack is available on PyPI:
 ```shell
 pip install dlhpcstarter
 ```
 
 # Table of Contents
 
 [//]: # (- [How to structure your project]&#40;#how-to-structure-your-project&#41;)
 - [Package map](#package-map)
 - [Tasks](#tasks)
 - [Models](#models)
-- [Innovate via Model Composition and Inheritance](#innovate-via-model-composition-and-inheritance)
+- [Development via Model Composition and Inheritance](#development-via-model-composition-and-inheritance)
 - [Configuration YAML files and argparse](#configuration-yaml-files-and-argparse)
-- [Innovate via Configuration Files](#innovate-via-configuration-files)
+- [Development via Configuration Files](#development-via-configuration-files)
 - [Next level: Configuration composition via Hydra](#next-level-configuration-composition-via-hydra)
 - [Stages and Trainer](#stages-and-trainer)
 - [Tying it all together: `main.py`](#tying-it-all-together-mainpy)
 - [Cluster manager and distributed computing](#cluster-manager-and-distributed-computing)
 - [Monitoring using Neptune.ai](#monitoring-using-neptuneai)
 - [Where all the outputs go: `exp_dir`](#where-all-the-outputs-go-exp_dir)
 - [Repository Wish List](#repository-wish-list)
@@ -53,15 +53,15 @@
 
 [//]: # (│    │)
 
 [//]: # (│    └── TASK_NAME     - name of the task, e.g., cifar10.)
 
 [//]: # (│        └── config    - .yaml configuration files for a model.)
 
-[//]: # (│        └── models    - .py modules that contain pytorch_lightning.LightningModule definitions that represent models.)
+[//]: # (│        └── models    - .py modules that contain Lightning LightningModule definitions that represent models.)
 
 [//]: # (│        └── stages.py - training and testing stages for a task.)
 
 [//]: # (```)
 
 # Package map
 
@@ -69,76 +69,77 @@
 
 The package is structured as follows:
 
 ```
 ├──  dlhpcstarter
 │    │
 │    ├── tools                     - for all other modules; tools that are repeadetly used.
-│    ├──  __main__.py - __main__.py does the following:
-│    │               1. Reads command line arguments using argparse.
-│    │               2. Imports the 'stages' function for the task from task/TASK_NAME/stages.py.
-│    │               3. Loads the specified configuration .yaml for the job from task/TASK_NAME/config.
-│    │               4. Submits the job (the configuration + 'stages') to the cluster manager (or runs it locally if 'submit' is false).
+│    ├── __main__.py               - __main__.py does the following:
+│    │                                    1. Reads command line arguments using argparse.
+│    │                                    2. Imports the 'stages' function for the task from task/
+│    │                                    3. Loads the specified configuration .yaml for the job from 
+│    │                                    4. Submits the job (the configuration + 'stages') to the 
+│    │                                       cluster manager (or runs it locally if 'submit' is false).
 │    └── cluster.py                - contains the cluster management object.
 │    └── command_line_arguments.py - argparse for reading command line arguments.
-│    └── trainer.py                - contains a wrapper for pytorch_lightning.Trainer.
+│    └── trainer.py                - contains an optional wrapper for the Lightning Trainer.
 │    └── utils.py                  - small utility definitions.
 
 ```
 
 # Tasks
 
 ---
 
 
-***Tasks are named based on the data and the type of prediction or inference being made***. For example:
- - Two tasks have the same data but require different names due to differing predictions, e.g., **MS-COCO Detection** and **MS-COCO Caption**.
- - Two tasks may have similar predictions but require different names due to differing data, e.g., **MNIST** and **Chinese MNIST**.
+***Tasks can have any name. The name could be based on the data or the type of inference being made***. For example:
+- Two tasks have the same data but require different names due to differing predictions, e.g., **MS-COCO Detection** and **MS-COCO Caption**.
+- Two tasks may have similar predictions but require different names due to differing data, e.g., **MNIST** and **Chinese MNIST**.
 
 ***Some publicly available tasks include***:
-- Image classification tasks, e.g., [MNIST](http://yann.lecun.com/exdb/mnist/), [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet](https://www.image-net.org/). 
+- Image classification tasks, e.g., [MNIST](http://yann.lecun.com/exdb/mnist/), [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet](https://www.image-net.org/).
 - Object detection tasks, e.g., [MS-COCO Detection](https://cocodataset.org/#detection-2020).
 - Image captioning detection tasks, e.g., [MS-COCO Caption](https://cocodataset.org/#captions-2015).
 - Speech recognition tasks, e.g., [LibriSpeech](https://www.openslr.org/12).
 - Chest X-Ray report generation, e.g., [MIMIC-CXR](https://physionet.org/content/mimic-cxr/2.0.0/).
 
-***How to add a task:***
+***What does the name do?***
 
-Adding a task is as simple as creating a directory with the name of the task in `task`. For example, if we choose CIFAR10 as the task, with the task name `cifar10`, then we would create the directory `task/cifar10`. The task directory will then house everything necessary for that task, for example, the models, the configurations for the models, the data pipeline, and the stages of development (training and testing).
+It is used to separate the outputs of the experiment from other tasks.
 
 # Models
 
 ---
 
 
-***Please familiarise yourself with the [`pytorch_lightning.LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#) in order to correctly implement a model:*** https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html
+***Please familiarise yourself with the [`Lightning LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#) in order to correctly implement a model:*** https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html
 
-Once we have created our task directory (e.g., `task/cifar10`), we now want to create a model using a [`pytorch_lightning.LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#). Everything we need for the model can be placed in the `LightningModule`, in including commonly used libraries and objects, for example:
+A model is created using a [`Lightning LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#). Everything we need for the model can be placed in the `LightningModule`, including commonly used libraries and objects, for example:
 
- - [torch.nn.Module](https://pytorch.org/docs/stable/generated/torch.nn.Module.html#torch.nn.Module): base class for all neural networks in `PyTorch`. 
- - [transformers](https://huggingface.co/docs/transformers/index): a library containing pre-trained Transformer models.
- - [torchvision](https://pytorch.org/vision/stable/index.html): a library for image pre-processing and pre-trained computer vision models.
- - [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset): an object that processes each instance of a dataset.
- - [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader): an object that samples mini-batches from a [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset).
+- [torch.nn.Module](https://pytorch.org/docs/stable/generated/torch.nn.Module.html#torch.nn.Module): base class for all neural networks in `PyTorch`.
+- [transformers](https://huggingface.co/docs/transformers/index): a library containing pre-trained Transformer models.
+- [torchvision](https://pytorch.org/vision/stable/index.html): a library for image pre-processing and pre-trained computer vision models.
+- [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset): an object that processes each instance of a dataset.
+- [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader): an object that samples mini-batches from a [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset).
 
-***Note:*** 
+***Note:***
 
-- The data pipeline could be implemented within the `LightningModule` or seperately from a model using a [pytorch_lightning.LightningDataModule](https://pytorch-lightning.readthedocs.io/en/stable/extensions/datamodules.html). The `LightningModule` instance would then have to be given separately to the `pytorch_lightning.Trainer`. 
+- The data pipeline could be implemented within the `LightningModule` or seperately from a model using a [Lightning LightningDataModule](https://pytorch-lightning.readthedocs.io/en/stable/extensions/datamodules.html). The `LightningModule` instance would then have to be given separately to the `Lightning Trainer` instance.
 
 ***Example:***
 
- - An example model for `cifar10` is in [task/cifar10/model/baseline.py](https://github.com/csiro-mlai/dl_hpc_starter_pack/blob/main/task/cifar10/model/baseline.py). 
+- An example model for `cifar10` is in [task/cifar10/model/baseline.py](https://github.com/csiro-mlai/dl_hpc_starter_pack/blob/main/task/cifar10/model/baseline.py).
 
-# Innovate via Model Composition and Inheritance
+# Development via Model Composition and Inheritance
 
 ---
-To promote rapid innovation of models, we recommend using class composition and/or inheritance. ***For example, we may have a baseline that not only includes a basic model, but also the data pipeline:***
+To promote rapid development of models, one solution is to use class composition and/or inheritance. ***For example, we may have a baseline that not only includes a basic model, but also the data pipeline:***
 
 ```python
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 from torch.utils.data import DataLoader, random_split
 import torchvision
 import torch
 
 class Baseline(LightningModule):
     def __init__(self, lr, ..., **kwargs):
         super(Baseline, self).__init__()
@@ -159,15 +160,15 @@
 
     def val_dataloader(self):
         return DataLoader(self.val_set, ...)
 
     def test_dataloader(self):
         return DataLoader(self.test_set, ...)
 
-    def configure_optimizers(self):     
+    def configure_optimizers(self):
         optimiser = {'optimizer': torch.optim.SGD(self.parameters(), lr=self.lr, momentum=0.9)}
         return optimiser
 
     def forward(self, images):
         return self.model(images)
 
     def training_step(self, batch, batch_idx):
@@ -188,18 +189,18 @@
         images, labels = batch
         y_hat = self(images)
         self.test_accuracy(torch.argmax(y_hat['logits'], dim=1), labels)
         self.log_dict({'test_acc': self.test_accuracy}, ...)
 ```
 
 After training and testing the baseline, we may want to improve upon its performance. For example, if we wanted to make the following modifications:
- 
- - Use a DenseNet instead of a ResNet.
- - Use the `AdamW` optimiser.
- - Use a warmup learning rate scheduler. 
+
+- Use a DenseNet instead of a ResNet.
+- Use the `AdamW` optimiser.
+- Use a warmup learning rate scheduler.
 
 ***All we would need to do is inherit the baseline and make our modifications:***
 
 ```python
 from transformers import get_constant_schedule_with_warmup
 
 class Inheritance(Baseline):
@@ -209,24 +210,24 @@
         self.save_hyperparameters()
         self.num_warmup_steps = num_warmup_steps
         self.model = torchvision.models.densenet121(...)
 
     def configure_optimizers(self):
         optimiser = {'optimizer': torch.optim.AdamW(self.parameters(), lr=self.lr)}
         optimiser['scheduler'] = {
-                'scheduler': get_constant_schedule_with_warmup(optimiser['optimizer'], self.num_warmup_steps),
-                'interval': 'step',
-                'frequency': 1,
-            }
+            'scheduler': get_constant_schedule_with_warmup(optimiser['optimizer'], self.num_warmup_steps),
+            'interval': 'step',
+            'frequency': 1,
+        }
         return optimiser
 ```
 We could also construct a model that is the combination of the two via composition. For example, we may want to use everything from `Baseline`, but the optimiser from `Inheritance`:
 
 ```python
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 
 class Composite(LightningModule):
     def __init__(self, **kwargs):
         self.baseline = Baseline(self, **kwargs)
 
     def setup(self, stage=None):
         self.baseline.setup(stage)
@@ -236,15 +237,15 @@
 
     def val_dataloader(self):
         return self.baseline.val_dataloader()
 
     def test_dataloader(self):
         return self.baseline.test_dataloader()
 
-    def configure_optimizers(self):     
+    def configure_optimizers(self):
         return Inheritance.configure_optimizers(self)  # Use configure_optimizers() from Inheritance.
 
     def forward(self, images):
         return self.baseline.forward(images)
 
     def training_step(self, batch, batch_idx):
         return self.baseline.training_step(batch, batch_idx)
@@ -264,15 +265,15 @@
 Currently, there are two methods for giving arguments:
 
 1. **Via command line arguments using the [`argparse` module](https://docs.python.org/3/library/argparse.html)**. `argparse` mainly handles paths, development stage flags (e.g., training and testing flags), and cluster manager arguments.
 2. **Via a configuration file stored in [`YAML` format](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)**. Can handle all the arguments defined by the `argparse` plus more, including hyperparameters for the model.
 
 ***The mandatory arguments include:***
 1. `task`, the name of the task.
-2. `config`, relative or absolute path to the configuration file (can handle with or without extension).
+2. `config`, relative or absolute path to the configuration file (with or without the extension).
 3. `module`, the module that the model definition is housed.
 4. `definition`, the class representing the model.
 5. `exp_dir`, the experiment directory, i.e., where all outputs, including model checkpoints will be saved.
 6. `monitor`, metric to monitor for [ModelCheckpoint](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.ModelCheckpoint.html) and [EarlyStopping](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.EarlyStopping.html?highlight=earlystoppin#earlystopping) (optional), as well as test checkpoint loading (e.g., 'val_loss').
 7. `monitor_mode`, whether the monitored metric is to be maximised or minimised ('max' or 'min').
 
 ***`task` and `config` must be given as command line arguments for `argparse`:***
@@ -281,15 +282,15 @@
 dlhpcstarter --config task/cifar10/config/baseline --task cifar10
 ```
 
 ***`module`, `definition`, and `exp_dir` can be given either as command line arguments, or be placed in the configuration file.***
 
 For each model of a task, we define a configuration. Hyperparameters, paths, as well as the device configuration can be stored in a configuration file. Configurations are in [`YAML` format](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started), e.g., `task/cifar10/config/baseline.yaml`.
 
-# Innovate via Configuration Files
+# Development via Configuration Files
 
 ---
 
 If we have the following configuration file for the aforementioned CIFAR10  `Baseline` model, `task/cifar10/config/baseline.yaml`:
 
 ```yaml
 train: True
@@ -428,80 +429,80 @@
 
 - `task/cifar10/config/cluster/2hr.yaml`:
    ```yaml
    memory: 32GB
    time_limit: '02:00:00'
    venv_path: /path/to/my/venv/bin/activate
    ```
- - `task/cifar10/config/distributed/4gpu.yaml`:
-   ```yaml
-   num_gpus: 2
-   strategy: ddp
-   ```
- - `task/cifar10/config/paths/hpc.yaml`:
-   ```yaml
-   exp_dir: /path/to/my/experiments
-   dataset_dir: /path/to/my/dataset
-   ```
+- `task/cifar10/config/distributed/4gpu.yaml`:
+  ```yaml
+  num_gpus: 2
+  strategy: ddp
+  ```
+- `task/cifar10/config/paths/hpc.yaml`:
+  ```yaml
+  exp_dir: /path/to/my/experiments
+  dataset_dir: /path/to/my/dataset
+  ```
 
 See the following documentation for more information:
- - https://hydra.cc/docs/1.2/tutorials/basic/your_first_app/defaults/
- - https://hydra.cc/docs/1.2/advanced/defaults_list/#composition-order
- - https://hydra.cc/docs/1.2/advanced/overriding_packages/
+- https://hydra.cc/docs/1.2/tutorials/basic/your_first_app/defaults/
+- https://hydra.cc/docs/1.2/advanced/defaults_list/#composition-order
+- https://hydra.cc/docs/1.2/advanced/overriding_packages/
 
 # Stages and Trainer
 
 ---
 
 
-In each task directory is a Python module called `stages.py`, which contains the `stages` definition. This definition takes an object as input that houses the configuration for a job.  
+In each task directory is a Python module called `stages.py`, which contains the `stages` definition. This definition takes an object as input that houses the configuration for a job.
 
 Typically, the following things happen in `stages()`:
 
- - The `LightningModule` model is imported via the `model` argument, e.g.,
-    ```python
-    from src import importer
-   
-    Model = importer(definition=args.definition, module=args.module)
-    model = Model(**vars(args))
-   ```
-    See `src.utils.importer` for a handy function that imports based on strings.
- - A `pytorch_lightning.Trainer` instance is created, e.g., `trainer = pytorch_lightning.Trainer(...)`.
- - The model is trained using trainer: `trainer.fit(model)`.
- - The model is tested using trainer: `trainer.test(model)`.
+- The `LightningModule` model is imported via the `model` argument, e.g.,
+   ```python
+   from src import importer
+  
+   Model = importer(definition=args.definition, module=args.module)
+   model = Model(**vars(args))
+  ```
+  See `src.utils.importer` for a handy function that imports based on strings.
+- A `Lightning Trainer` instance is created, e.g., `trainer = lightning.pytorch.Trainer(...)`.
+- The model is trained using trainer: `trainer.fit(model)`.
+- The model is tested using trainer: `trainer.test(model)`.
 
-It handles the training and testing of a model for a task by using a [`pytorch_lightning.Trainer`](https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html).
+It handles the training and testing of a model for a task by using a [`Lightning Trainer`](https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html).
 
-***A helpful wrapper at `src/trainer.py` exists that passes frequently used and useful `callbacks`, `loggers`, and `plugins` to a `pytorch_lightning.Trainer` instance:***
+***A helpful wrapper at `src/trainer.py` exists that passes frequently used and useful `callbacks`, `loggers`, and `plugins` to a `Lightning Trainer` instance:***
 
 ```python
 from src.dlhpcstarter.trainer import trainer_instance
 
 trainer = trainer_instance(**vars(args))
 ```
-Place any of the parameters for the trainer detailed at 
-https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api in your configuration file, and they will be passed to the `pytorch_lightning.Trainer` instance.
+Place any of the parameters for the trainer detailed at
+https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api in your configuration file, and they will be passed to the `Lightning Trainer` instance.
 
 # Tying it all together: `dlhpcstarter`
 
 ---
 
 ***This is an overview of what occurs when the entrypoint `dlhpcstarter` is executed, this is not necessary to understand to use the package.***
 
 
 
 `dlhpcstarter` does the following:
 
- - Gets the command line arguments using `argparse`, e.g., arguments like this:
-    ```shell
-    dlhpcstarter --config task.cifar10.config.baseline --task cifar10
-    ```
- - Imports the `stages` definition for the task using `src.utils.importer`.
- - Reads the configuration `.yaml` and combines it with the command line arguments.
- - Submits `stages` to the cluster manager if `args.submit = True` or runs `stages` locally. The command line arguments and the configuration arguments are passed to `stages` in both cases.
+- Gets the command line arguments using `argparse`, e.g., arguments like this:
+   ```shell
+   dlhpcstarter --config task.cifar10.config.baseline --task cifar10
+   ```
+- Imports the `stages` definition for the task using `src.utils.importer`.
+- Reads the configuration `.yaml` and combines it with the command line arguments.
+- Submits `stages` to the cluster manager if `args.submit = True` or runs `stages` locally. The command line arguments and the configuration arguments are passed to `stages` in both cases.
 
 # Cluster manager and distributed computing
 
 ---
 
 The following arguments are used for distributed computing:
 
@@ -584,13 +585,13 @@
 
 ***Description to be finished.
 
 
 # Repository Wish List
 
 ---
- - Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
- - Add description about how to use https://neptune.ai/.
- - Use https://hydra.cc/ instead of argparse (or have the option to use either).
- - https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
- - Notebook examples.
+- Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
+- Add description about how to use https://neptune.ai/.
+- Use https://hydra.cc/ instead of argparse (or have the option to use either).
+- https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
+- Notebook examples.
```

### Comparing `dlhpcstarter-0.0.8/setup.cfg` & `dlhpcstarter-0.1.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [metadata]
 name = dlhpcstarter
-version = 0.0.8
+version = 0.1.2
 description = Deep Learning and HPC Starter Pack
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/csiro-mlai/dl_hpc_starter_pack
 author = CSIRO
 license = Apache License 2.0
 license_file = LICENSE
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	Bottleneck>=1.3
+	Bottleneck>=1.3.7
 	GPUtil>=1.4
-	hydra-core>=1.2
-	neptune-client>=0.16
-	numpy>=1.21
-	pytorch-lightning>=1.8.6
-	rich>=12.5
-	scipy>=1.7
-	torchmetrics>=0.9
-	torchvision>=0.11.1
+	hydra-core>=1.3.2
+	lightning>=2.0.1
+	neptune-client==0.16.18
+	numpy>=1.24.2
+	protobuf==3.20.3
+	rich>=13.3.2
+	tensorboard>=2.12.0
+	torch>=1.11
+	torchmetrics>=0.11.4
 
 [options.extras_require]
 test = pytest
 
 [options.packages.find]
 where = src
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/__main__.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from argparse import Namespace
 from dlhpcstarter.command_line_arguments import read_command_line_arguments
-from dlhpcstarter.utils import importer, gpu_usage_and_visibility, load_config_and_update_args
+from dlhpcstarter.utils import importer, load_config_and_update_args
 from dlhpcstarter.cluster import ClusterSubmit
 from typing import Callable
 import sys
 
 
 def main() -> None:
     """
@@ -22,21 +22,27 @@
     1. Get command line arguments using argparse for the job:
     """
     args = read_command_line_arguments()
 
     """
     2. Import the 'stages' function for the task:
     
-        Imports the function that handles the training and testing stages for the task. This is the stages() function
-        defined in the task's stages.py. The model is also defined in the stages function based on the configuration.
+        Imports the function that handles the training and testing stages for the task. The default location of the 
+        stages() function is in the task's stages.py. The model is also initialised in the stages function based on the 
+        configuration.
+        
+        The definition and module of the stages function can also be manually set using 'stages_definition' and 
+        'stages_module', respectively.
     
         For example: stages() in task.cifar10.stages 
     
     """
-    stages_fnc = importer(definition='stages', module='.'.join(['task', args.task, 'stages']))
+    args.stages_definition = 'stages' if args.stages_definition is None else args.stages_definition
+    assert args.stages_module, f'"stages_module" must be specified as a command line argument.'
+    stages_fnc = importer(definition=args.stages_definition, module=args.stages_module)
 
     """
     3. Load the configuration for the job and add it to 'args':
     
         This contains the paths, model configuration, the training and test configuration, the device & cluster manager 
         configuration.
     """
@@ -66,24 +72,25 @@
 
         # Cluster object
         cluster = ClusterSubmit(
             fnc_kwargs=args,
             fnc=stages_fnc,
             save_dir=args.exp_dir_trial,
             time_limit=args.time_limit,
-            num_gpus=args.num_gpus,
+            num_gpus=args.devices,
             num_nodes=args.num_nodes,
             num_workers=args.num_workers,
             memory=args.memory,
             python_cmd='python3' if not hasattr(args, 'python_cmd') else args.python_cmd,
             entrypoint='dlhpcstarter' if not hasattr(args, 'entrypoint') else args.entrypoint,
+            resubmit=True,
         )
 
         # Cluster commands
-        cluster.add_manager_cmd(cmd='ntasks-per-node', value=args.num_gpus if args.num_gpus else 1)
+        cluster.add_manager_cmd(cmd='ntasks-per-node', value=args.devices if args.devices else 1)
 
         # Source virtual environment
         cluster.add_command('source ' + args.venv_path)
 
         # Debug flags
         cluster.add_command('export NCCL_DEBUG=INFO')
         cluster.add_command('export PYTHONFAULTHANDLER=1')
@@ -102,15 +109,15 @@
         if args.qos:
             cluster.add_manager_cmd(cmd='qos', value=args.qos)
 
         # Email job status
         cluster.notify_job_status(email=args.email, on_done=True, on_fail=True)
 
         # Submit job to workload manager
-        job_display_name = args.task + '_' + args.config
+        job_display_name = args.task + '_' + args.config_name
 
         if args.trial is not None:
             job_display_name = job_display_name + f'_trial_{args.trial}'
 
         cluster.submit(job_display_name=job_display_name + '_')
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/cluster.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,7 +253,8 @@
                     cmd = '--{} {}'.format(k, v)
                 params.append(cmd)
         return ' '.join(params)
 
     def escape(self, v):
         v = str(v)
         return '[' in v or ';' in v or ' ' in v
+
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/command_line_arguments.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/command_line_arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import argparse
 
-def str_to_bool(s):
-    return s.lower() in ('yes', 'true', 't', '1')
-
 
 def read_command_line_arguments():
     """
     Reads the command line arguments.
 
     Partial parsing is used. This is because the main function is executed twice when using a cluster manager, with the
     second run having extra arguments. If partial parsing is not used, arguments from the configuration file that are
@@ -34,23 +31,26 @@
     directories.add_argument('--work-dir', '--work_dir', type=str, help='Working directory')
     directories.add_argument('--dataset-dir', '--dataset_dir', type=str, help='The dataset directory')
     directories.add_argument('--ckpt-zoo-dir', '--ckpt_zoo_dir', type=str, help='The checkpoint zoo directory')
 
     # Model module and definition
     model = parser.add_argument_group('Model module name and definition')
     model.add_argument('--definition', type=str, help='Class definition of the model')
-    model.add_argument('--module', type=str, help='Name of the module in task/TASK_NAME/model')
+    model.add_argument('--module', type=str, help='Name of the module')
+
+    # Stages module and definition
+    model = parser.add_argument_group('Stages module name and definition')
+    model.add_argument('--stages_definition', type=str, help='Definition of stages')
+    model.add_argument('--stages_module', type=str, help='Name of the module')
 
     # Training arguments
     training_arguments = parser.add_argument_group('Training arguments')
-    training_arguments.add_argument('--train', type=str_to_bool, help='Perform training')
+    training_arguments.add_argument('--train',  default=None, action='store_true', help='Perform training')
     training_arguments.add_argument('--trial', type=int, help='The trial number')
-    training_arguments.add_argument(
-        '--resumable', type=str_to_bool, help='Resumable training. Automatic resubmission to cluster manager',
-    )
+    training_arguments.add_argument('--resume-last', '--resume_last', default=True, action='store_true', help='Resume training from last epoch')
     training_arguments.add_argument('--resume-epoch', '--resume_epoch', type=int, help='Epoch to resume training from')
     training_arguments.add_argument(
         '--resume-ckpt-path', '--resume_ckpt_path', type=str, help='Checkpoint to resume training from',
     )
     training_arguments.add_argument(
         '--warm-start-ckpt-path', '--warm_start_ckpt_path', type=str, help='Checkpoint for warm-starting',
     )
@@ -60,33 +60,33 @@
         '--monitor_mode',
         type=str,
         help='whether the monitored metric is to be maximised or minimised (''max'' or ''min'')',
     )
 
     # Test arguments
     test = parser.add_argument_group('Testing arguments')
-    test.add_argument('--test', type=str_to_bool, help='Evaluate the model on the test set')
+    test.add_argument('--test', default=None, action='store_true', help='Evaluate the model on the test set')
     test.add_argument('--test-epoch', '--test_epoch', type=int, help='Test epoch')
     test.add_argument('--test-ckpt-path', '--test_ckpt_path', type=str, help='Path to checkpoint to be tested')
 
     # PyTorch Lightning Trainer arguments
     trainer = parser.add_argument_group('PyTorch Lightning Trainer arguments')
-    trainer.add_argument('--debug', type=str_to_bool, help='One mini-batch for training, validation, and testing')
+    training_arguments.add_argument('--fast-dev-run', '--fast_dev_run',  default=None, action='store_true', help='https://lightning.ai/docs/pytorch/stable/common/trainer.html#fast-dev-run')
 
     # Distributed computing arguments
     distributed = parser.add_argument_group('Distributed computing arguments')
     distributed.add_argument('--num-workers', '--num_workers', type=int, help='No. of workers per DataLoader & GPU')
-    distributed.add_argument('--num-gpus', '--num_gpus', type=int, help='Number of GPUs per node')
+    distributed.add_argument('--devices', type=int, help='Number of devices per node')
     distributed.add_argument('--num-nodes', '--num_nodes', type=int, help='Number of nodes')
 
     # Cluster manager arguments
     cluster = parser.add_argument_group('Cluster manager arguments')
     cluster.add_argument('--memory', type=str, help='Amount of memory per node')
     cluster.add_argument('--time-limit', '--time_limit', type=str, help='Job time limit')
-    cluster.add_argument('--submit', type=str_to_bool, help='Submit job to the cluster manager')
+    cluster.add_argument('--submit',  default=None, action='store_true', help='Submit job to the cluster manager')
     cluster.add_argument('--qos', type=str, help='Quality of service')
     cluster.add_argument('--begin', type=str, help='When to begin the Slurm job, e.g. now+1hour')
     cluster.add_argument('--slurm-cmd-path', '--slurm_cmd_path', type=str)
     cluster.add_argument('--email', type=str, help='Email for cluster manager notifications')
 
     # System arguments
     system = parser.add_argument_group('System arguments')
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/tools/ext/collect_env_details.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/collect_env_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import re
 import sys
 
 import numpy
 import torch
 import tqdm
 
-import pytorch_lightning  # noqa: E402
+import lightning  # noqa: E402
 
 LEVEL_OFFSET = "\t"
 KEY_PADDING = 20
 
 
 def run_and_parse_first_match(run_lambda, command, regex):
     """Runs command using run_lambda, returns the first regex match if it exists"""
@@ -69,15 +69,15 @@
 
 
 def info_packages():
     return {
         "numpy": numpy.__version__,
         "pyTorch_version": torch.__version__,
         "pyTorch_debug": torch.version.debug,
-        "pytorch-lightning": pytorch_lightning.__version__,
+        "lightning": lightning.__version__,
         "tqdm": tqdm.__version__,
     }
 
 
 def nice_print(details, level=0):
     lines = []
     for k in sorted(details):
@@ -92,14 +92,17 @@
             template = "{:%is} {}" % KEY_PADDING
             key_val = template.format(key, details[k])
             lines += [(level * LEVEL_OFFSET) + key_val]
     return lines
 
 
 def main():
+
+    raise ValueError('collect environment details is currently not working.')
+
     details = {
         "System": info_system(),
         "CUDA": info_cuda(),
         "Packages": info_packages(),
     }
     lines = nice_print(details)
     text = os.linesep.join(lines)
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/tools/mods/logger.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 import logging
 import os
 from argparse import Namespace
 from typing import Any, Dict, Optional, Union
 
 import torch
 
-from pytorch_lightning.core.saving import save_hparams_to_yaml
-from pytorch_lightning.loggers.base import LightningLoggerBase, rank_zero_experiment
-from pytorch_lightning.utilities.logger import _add_prefix, _convert_params
-from pytorch_lightning.utilities.rank_zero import rank_zero_only, rank_zero_warn
+from lightning.pytorch.core.saving import save_hparams_to_yaml
+from lightning.pytorch.loggers.base import LightningLoggerBase, rank_zero_experiment
+from lightning.pytorch.utilities.logger import _add_prefix, _convert_params
+from lightning.pytorch.utilities.rank_zero import rank_zero_only, rank_zero_warn
 
 log = logging.getLogger(__name__)
 
 
 class ExperimentWriter:
     r"""
     Experiment writer for CSVLogger.
@@ -109,16 +109,16 @@
 class CSVLogger(LightningLoggerBase):
     r"""
     Log to local file system in yaml and CSV format.
 
     Logs are saved to ``os.path.join(save_dir, name, version)``.
 
     Example:
-        >>> from pytorch_lightning import Trainer
-        >>> from pytorch_lightning.loggers import CSVLogger
+        >>> from lightning.pytorch import Trainer
+        >>> from lightning.pytorch.loggers import CSVLogger
         >>> logger = CSVLogger("logs", name="my_exp_name")
         >>> trainer = Trainer(logger=logger)
 
     Args:
         save_dir: Save directory
         name: Experiment name. Defaults to ``'default'``.
         version: Experiment version. If version is not specified the logger inspects the save
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/trainer.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,123 +1,116 @@
-from pytorch_lightning import Trainer
-from pytorch_lightning.callbacks import (
-    EarlyStopping,
-    LearningRateMonitor,
-    ModelCheckpoint,
-)
-from pytorch_lightning.loggers import NeptuneLogger
-from pytorch_lightning.loggers.tensorboard import TensorBoardLogger
-from pytorch_lightning.plugins.environments import SLURMEnvironment
-from dlhpcstarter.tools.mods.logger import CSVLogger
-from dlhpcstarter.utils import resume_from_ckpt_path
-from typing import Optional
 import inspect
 import logging
+from typing import Optional
+
+from lightning.pytorch import Trainer
+from lightning.pytorch.callbacks import (EarlyStopping, LearningRateMonitor,
+                                         ModelCheckpoint)
+from lightning.pytorch.loggers import NeptuneLogger
+from lightning.pytorch.loggers.csv_logs import CSVLogger
+from lightning.pytorch.loggers.tensorboard import TensorBoardLogger
+
 logging.getLogger(
     "neptune.new.internal.operation_processors.async_operation_processor",
 ).setLevel(logging.CRITICAL)
+from lightning.pytorch.plugins.environments import SLURMEnvironment
 
 
 def trainer_instance(
-    monitor: str,
-    monitor_mode: str,
     task: str,
-    config: str,
+    config_name: str,
     trial: int,
+    monitor: Optional[str] = None,
+    monitor_mode: str = 'min',
     early_stopping: bool = False,
     patience: int = 0,
     min_delta: float = 0.0,
     divergence_threshold: Optional[float] = None,
     exp_dir_trial: Optional[str] = None,
-    resumable: bool = True,
-    resume_epoch: Optional[int] = None,
-    resume_ckpt_path: Optional[str] = None,
     sched_inter: Optional[str] = None,  # 'step', 'epoch', or None.
     save_top_k: int = 1,
     every_n_epochs: Optional[int] = 1,
     every_n_train_steps: Optional[int] = None,
-    debug: bool = False,
-    submit: bool = False,
     neptune_api_key: Optional[str] = None,
     neptune_username: Optional[str] = None,
     neptune_mode: Optional[str] = 'async',
     num_nodes: int = 1,
-    num_gpus: Optional[int] = None,
+    devices: Optional[int] = 1,
+    submit: bool = False,
     mbatch_size: Optional[int] = None,
     accumulated_mbatch_size: Optional[int] = None,
     deterministic: bool = True,
     num_sanity_val_steps: int = 0,
     loggers: Optional[list] = None,
     callbacks: Optional[list] = None,  # [RichProgressBar()]
     plugins: Optional[list] = None,
     **kwargs,
 ) -> Trainer:
     """
-    Creates an instance of pytorch_lightning.Trainer using key callbacks and loggers. Also changes some
-    defaults for the init of pytorch_lightning.Trainer.
+    Creates an instance of lightning.pytorch.Trainer using key callbacks and loggers. Also changes some
+    defaults for the init of lightning.pytorch.Trainer.
 
-    Parameters for pytorch_lightning.Trainer are described here:
+    Parameters for lightning.pytorch.Trainer are described here:
         https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api
-    These will be captured by kwargs and passed to pytorch_lightning.Trainer
+    These will be captured by kwargs and passed to lightning.pytorch.Trainer
 
     Argument/s:
+        task - name of the task.
+        config_name - name of the configuration.
+        trial - trial identifier.
         monitor - metric to monitor for EarlyStopping and ModelCheckpoint.
         monitor_mode - whether the metric to be monitored is to be maximised or
             minimised.
-        task - name of the task.
-        config - name of the configuration.
-        trial - trial identifier.
         early_stopping - stop training when a monitored metric has stopped
             improving.
         patience - no. of epochs with no improvement after which training will
             be stopped.
         min_delta - minimum change in the monitored quantity to qualify as an
             improvement.
         divergence_threshold - stop training as soon as the monitored quantity becomes worse than this threshold.
         exp_dir_trial - experiment directory for the trial. All outputs are saved to this path.
-        resumable - whether the last completed epoch is saved to enable resumable training.
-        resume_epoch - the epoch to resume training from.
-        resume_ckpt_path - resume training from the specified checkpoint.
         sched_inter - learning rate scheduler interval ('step' or 'epoch').
         save_top_k - best k models saved according to the monitored metric. If
             0, no models are saved. If -1, all models are saved.
         every_n_epochs - save model every n epochs.
         every_n_epochs - save model every n training steps.
-        debug - training, validation, and testing are completed using one mini-batch.
-        submit - submit to cluster manager.
         neptune_api_key - API key, found on neptune.ai, for NeptuneLogger.
         neptune_username - Username for on neptune.ai, for NeptuneLogger.
         neptune_mode - https://docs.neptune.ai/api/connection_modes/.
         num_nodes - number of nodes for the job.
-        num_gpus - number of GPUs per node.
+        devices - number of devices per node.
+        submit - submit to cluster manager.
         mbatch_size - mini-batch size of dataloaders.
         accumulated_mbatch_size - desired accumulated mini-batch size.
         deterministic - ensures that the training is deterministic.
         num_sanity_val_steps - runs n validation batches before starting the training routine.
         loggers - loggers for Trainer.
         callbacks - callbacks for Trainer.
         plugins - plugins for Trainer.
         kwargs - keyword arguments for Trainer.
     """
     accumulate_grad_batches = None
     loggers = [] if loggers is None else loggers
-    """
-    Potential default callbacks to add:
-        - SLURMEnvironment(auto_requeue=True)  # This could be used in place of the auto requeue in transmodal.cluster
-    """
     callbacks = [] if callbacks is None else callbacks
     plugins = [] if plugins is None else plugins
+
     if submit:
+        # Unsure if Lightning's SLURMEnvironment features fault-tolerant training.
         plugins.append(SLURMEnvironment(auto_requeue=False))
 
+    # Deepspeed has its own autocast capabilities:
+    if 'strategy' in kwargs and 'precision' in kwargs:
+        if 'deepspeed' in kwargs['strategy'] and kwargs['precision'] == 16:
+            raise ValueError('DeepSpeed and "precision=16" are incompatible as DeepSpeed has its own autocast functionality.')
+
     # Loggers
-    loggers.append(CSVLogger(exp_dir_trial, name='', version=''))
-    loggers.append(TensorBoardLogger(exp_dir_trial, name='', version='', default_hp_metric=False))
+    loggers.append(CSVLogger(exp_dir_trial))
+    loggers.append(TensorBoardLogger(exp_dir_trial, default_hp_metric=False))
     if neptune_api_key is not None:
-        custom_run_id = f'{config[:16]}_trial_{trial}'
+        custom_run_id = f'{config_name[:21]}_t_{trial}'
         assert len(custom_run_id) <= 32, '"custom_run_id" must be less than or equal to 32 characters'
         assert neptune_username is not None, 'You must specify your neptune.ai username.'
         loggers.append(
             NeptuneLogger(
                 api_key=neptune_api_key,
                 project=f'{neptune_username}/{task.replace("_", "-")}',
                 prefix='log',
@@ -135,85 +128,89 @@
 
     # Model checkpointing
     assert (every_n_epochs is not None) or (every_n_train_steps is not None), 'Neither "every_n_epochs" or ' \
         '"every_n_train_steps" is set. No checkpoints will be saved.'
     assert save_top_k != 0, '"save_top_k" is 0, therefore, no checkpoints will be saved.'
 
     if every_n_epochs:
+        save_top_k = save_top_k if monitor is not None else -1
         callbacks.append(
             ModelCheckpoint(
                 dirpath=exp_dir_trial,
                 monitor=monitor,
                 mode=monitor_mode,
                 save_top_k=save_top_k,
                 every_n_epochs=every_n_epochs,
-                filename='{epoch:d}-{' + monitor + ':f}',
+                filename='{epoch:d}-{step:d}-{' + monitor + ':f}' if monitor else '{epoch:d}-{step:d}',
                 save_last=True,
             )
         )
-
-    if every_n_train_steps:
-        if resumable:
-            raise ValueError('Cannot resume training from a checkpoint that ended before the epoch ended. Fault '
-                             'tolerant training needs to be implemented for this: '
-                             'https://pytorch-lightning.readthedocs.io/en/latest/clouds'
-                             '/fault_tolerant_training_expert.html#enable-fault-tolerant-behavior-on-your-own-cluster')
-        callbacks.append(
-            ModelCheckpoint(
-                dirpath=exp_dir_trial,
-                monitor=monitor,
-                mode=monitor_mode,
-                save_top_k=save_top_k,
-                every_n_train_steps=every_n_train_steps,
-                filename='{step:d}-{' + monitor + ':f}',
-                save_last=False,  # cannot resume from this checkpoint.
-            )
-        )
+        if 'strategy' in kwargs:
+            if 'deepspeed_stage_3' in kwargs['strategy']: 
+                callbacks[-1].FILE_EXTENSION = ""
+
+    # if every_n_train_steps:
+    #     if resumable:
+    #         raise ValueError('Cannot resume training from a checkpoint that ended before the epoch ended. Fault '
+    #                          'tolerant training needs to be implemented for this: '
+    #                          'https://pytorch-lightning.readthedocs.io/en/latest/clouds'
+    #                          '/fault_tolerant_training_expert.html#enable-fault-tolerant-behavior-on-your-own-cluster')
+    #     callbacks.append(
+    #         ModelCheckpoint(
+    #             dirpath=exp_dir_trial,
+    #             monitor=monitor,
+    #             mode=monitor_mode,
+    #             save_top_k=save_top_k,
+    #             every_n_train_steps=every_n_train_steps,
+    #             filename='{step:d}-{' + monitor + ':f}',
+    #             save_last=False,  # cannot resume from this checkpoint.
+    #         )
+    #     )
 
     # Early stopping
     if early_stopping:
+        if 'strategy' in kwargs:
+            assert 'deepspeed' not in kwargs['strategy'], 'DeepSpeed does not work with early stopping currently.'
         callbacks.append(
             EarlyStopping(
                 monitor=monitor,
                 mode=monitor_mode,
                 min_delta=min_delta,
                 patience=patience,
                 divergence_threshold=divergence_threshold,
-                verbose=False,
+                verbose=True,
             )
         )
 
     # Learning rate monitor
     if sched_inter is not None:
         callbacks.append(LearningRateMonitor(logging_interval=sched_inter))
 
     # Accumulate gradient batches
     if accumulated_mbatch_size:
-        devices = num_gpus * num_nodes if num_gpus * num_nodes > 0 else 1
-        accumulate_grad_batches = accumulated_mbatch_size / (mbatch_size * devices)
+        total_devices = devices * num_nodes if devices * num_nodes > 0 else 1
+        accumulate_grad_batches = accumulated_mbatch_size / (mbatch_size * total_devices)
         assert accumulate_grad_batches.is_integer(), f'Desired accumulated_mbatch_size ({accumulated_mbatch_size}) ' \
-                                                     f'can not be attained with mbatch_size={mbatch_size}, num_gpus=' \
-                                                     f'{num_gpus}, and num_nodes={num_nodes}'
+                                                     f'can not be attained with mbatch_size={mbatch_size}, devices=' \
+                                                     f'{devices}, and num_nodes={num_nodes}'
         accumulate_grad_batches = int(accumulate_grad_batches)
+    else:
+        accumulate_grad_batches = 1
 
-    # Resume from checkpoint
-    ckpt_path = resume_from_ckpt_path(exp_dir_trial, resumable, resume_epoch, resume_ckpt_path)
-
-    # Remove keyword arguments not associated with pytorch_lightning.Trainer.
-    # Parameters associated with pytorch_lightning.Trainer:
+    # Remove keyword arguments not associated with lightning.pytorch.Trainer.
+    # Parameters associated with lightning.pytorch.Trainer:
     #   https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api
     kwargs = {k: v for k, v in kwargs.items() if k in inspect.signature(Trainer).parameters}
 
-    # pytorch_lightning.Trainer
+    # lightning.pytorch.Trainer
     return Trainer(
+        default_root_dir=exp_dir_trial, # Needed for hpc_ckpt save path. 
         logger=loggers,
         callbacks=callbacks,
         plugins=plugins,
-        fast_dev_run=debug,
-        gpus=num_gpus,
+        devices=devices,
         num_nodes=num_nodes,
         accumulate_grad_batches=accumulate_grad_batches,
         deterministic=deterministic,
         num_sanity_val_steps=num_sanity_val_steps,
-        resume_from_checkpoint=ckpt_path,
         **kwargs,
     )
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter/utils.py` & `dlhpcstarter-0.1.2/src/dlhpcstarter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from typing import Optional
 import glob
 import GPUtil
 import importlib
 import numpy as np
 import os
 import re
+
+
+import torch
 import warnings
 
 
 def importer(
         definition: str,
         module: str,
         work_dir: Optional[str] = None,
@@ -29,225 +32,243 @@
     """
 
     if work_dir:
 
         absolute_path = os.path.join(work_dir, *module.split('.')) + '.py'
 
         assert os.path.isfile(absolute_path), \
-            f'''{absolute_path} does not exist. The target definition was: {definition}.'''
+            f'''{absolute_path} does not exist. The target definition and modules: {definition} & {module}. The working directory: {work_dir}.'''
 
         module = importlib.machinery.SourceFileLoader(module, absolute_path).load_module()
 
     else:
 
         path = os.path.join(*module.split('.')) + '.py'
 
-        assert os.path.isfile(path), f'{path} does not exist. The target definition was: {definition}.'
+        assert os.path.isfile(path), f'{path} does not exist. The target definition and modules: {definition} & {module}.'
 
         module = importlib.import_module(module)
 
     return getattr(module, definition)
 
 
 def load_config_and_update_args(args: Namespace, print_args: bool = False) -> None:
     """
     Loads the configuration .yaml file and updates the args object.
 
     Argument/s:
         args - object that houses the arguments for the job.
         print_args - print the arguments for the job.
     """
-    # Add the working directory to paths
+    # Add the working directory to paths:
     if not args.work_dir:
         args.work_dir = os.getcwd()
 
-    # Configuration name
+    # Configuration:
     if args.config.endswith('.yaml'):
         args.config_file_name = args.config
         args.config = args.config.replace('.yaml', '')
     else:
         args.config_file_name = args.config + '.yaml'
+    args.config_name = Path(args.config).parts[-1]
 
-    # Load configuration using Hydra's Compose API
+    # Load configuration using Hydra's Compose API:
     args.config_dir = Path(args.config).parent
     if not os.path.isabs(args.config_dir):
         args.config_dir = os.path.join(args.work_dir, args.config_dir)
     with initialize_config_dir(version_base=None, config_dir=args.config_dir):
-        config = compose(config_name=Path(args.config).parts[-1])
+        config = compose(config_name=args.config_name)
 
-    # Update args with config and check for conflicts
+    # Update args with config and check for conflicts:
     args.config_full_path = os.path.join(args.work_dir, args.config_file_name)
     for k, v in config.items():
         if getattr(args, k, None) is None:
             setattr(args, k, v)
         else:
             if getattr(args, k) != v:
                 raise ValueError(f'There is a conflict between command line argument "--{k} {getattr(args, k)}" '
                                  f'({type(getattr(args, k))}) and configuration argument "{k}: {v}" from '
                                  f'{args.config_full_path} ({type(v)}).')
 
-    # The model name must be defined in the configuration or in the command line arguments
+    # The model name must be defined in the configuration or in the command line arguments:
     assert args.module, f'"module" must be specified as a command line argument or in {args.config_full_path}.'
     assert args.definition, f'"definition" must be specified as a command line argument or in {args.config_full_path}.'
     assert args.exp_dir, f'"exp_dir" must be specified as a command line argument or in {args.config_full_path}.'
 
-    # Defaults: There is probably a better place to do this
+    # Defaults: There is probably a better place to do this:
     args.num_workers = args.num_workers if args.num_workers is not None else 1
     args.num_nodes = args.num_nodes if args.num_nodes is not None else 1
     if args.submit:
         args.time_limit = args.time_limit if args.time_limit is not None else '02:00:00'
         args.memory = args.memory if args.memory is not None else '16GB'
 
-    # Add the task, configuration name, and the trial number to the experiment directory
+    # Add the task, configuration name, and the trial number to the experiment directory:
     args.trial = args.trial if args.trial is not None else 0
-    args.exp_dir_trial = os.path.join(args.exp_dir, args.task, args.config, 'trial_' + f'{args.trial}')
+    args.exp_dir_trial = os.path.join(args.exp_dir, args.task, args.config_name, 'trial_' + f'{args.trial}')
     Path(args.exp_dir_trial).mkdir(parents=True, exist_ok=True)
 
+    # Do not resume from last if fast_dev_run is True:
+    args.resume_last = False if args.fast_dev_run else args.resume_last
+
     if print_args:
         print(f'args: {args.__dict__}')
 
-    # Print GPU usage and set GPU visibility
-    if hasattr(args, 'num_gpus'):
-        gpu_usage_and_visibility(args.cuda_visible_devices, args.submit)
+    # Print GPU usage and set GPU visibility:
+    gpu_usage_and_visibility(args.cuda_visible_devices, args.submit)
 
 
-def get_epoch_ckpt_path(exp_dir_trial: str, load_epoch: int) -> str:
+def get_epoch_ckpt_path(exp_dir_trial: str, load_epoch: int, extension: str = ".ckpt") -> str:
     """
     Get the checkpoint path based on the epoch number.
 
     Argument/s:
         exp_dir_trial - Experiment directory for the trial (where the checkpoints are saved).
         load_epoch - epoch to load.
+        extension - checkpoint extension.
 
     Returns:
         Path to the epoch's checkpoint.
     """
     try:
-        ckpt_path = glob.glob(os.path.join(exp_dir_trial, "*epoch=" + str(load_epoch) + "*.ckpt"))
+        ckpt_path = glob.glob(os.path.join(exp_dir_trial, '*epoch=' + str(load_epoch) + f'*{extension}'))
         assert len(ckpt_path) == 1, f'Multiple checkpoints for epoch {load_epoch}: {ckpt_path}.'
 
     except:
         raise ValueError(
-            "Epoch {} is not in the checkpoint directory.".format(str(load_epoch))
+            'Epoch {} is not in the checkpoint directory.'.format(str(load_epoch))
         )
     return ckpt_path[0]
 
 
-def get_best_ckpt_path(exp_dir_trial: str, monitor_mode: str) -> str:
+def get_best_ckpt_path(exp_dir_trial: str, monitor: str, monitor_mode: str, extension: str = '.ckpt') -> str:
     """
     Get the best performing checkpoint from the experiment directory.
 
     Argument/s:
         exp_dir_trial - Experiment directory for the trial (where the checkpoints are saved).
+        monitor - Monitored metric.
         monitor_mode - Metric monitoring mode, either "min" or "max".
+        extension - checkpoint extension.
 
     Returns:
         Path to the epoch's checkpoint.
     """
 
-    ckpt_list = glob.glob(os.path.join(exp_dir_trial, '*=*=*.ckpt'))
+    ckpt_list = glob.glob(os.path.join(exp_dir_trial, f'*=*{monitor}=*{extension}'))
 
     if not ckpt_list:
-        raise ValueError(f'No checkpoints exist in the checkpoint directory: {exp_dir_trial}.')
+        raise ValueError(f'No checkpoints exist for the regex: *=*{monitor}=*{extension} in the checkpoint directory: {exp_dir_trial}.')
 
     scores = [
-        re.findall(r"[-+]?\d*\.\d+|\d+", i.rsplit('=', 1)[1])[0] for i in ckpt_list
+        re.findall(r'[-+]?\d*\.\d+|\d+', i.rsplit('=', 1)[1])[0] for i in ckpt_list
     ]
 
     if monitor_mode == 'max':
         ckpt_path = ckpt_list[np.argmax(scores)]
     elif monitor_mode == 'min':
         ckpt_path = ckpt_list[np.argmin(scores)]
     else:
         raise ValueError("'monitor_mode' must be max or min, not {}.".format(monitor_mode))
     return ckpt_path
 
 
 def get_test_ckpt_path(
-        exp_dir_trial: str, monitor_mode: str, test_epoch: Optional[int] = None, test_ckpt_path: Optional[str] = None,
+        exp_dir_trial: str, 
+        monitor: Optional[str] = None, 
+        monitor_mode: Optional[str] = None, 
+        test_epoch: Optional[int] = None, 
+        test_ckpt_path: Optional[str] = None,
+        extension: Optional[str] = '.ckpt',
 ) -> str:
     """
     Get the test checkpoint.
 
     Argument/s:
         exp_dir_trial - Experiment directory for the trial (where the checkpoints are saved).
-        monitor_mode - Metric motitoring mode, either "min" or "max".
+        monitor - Monitored metric.
+        monitor_mode - Metric monitoring mode, either "min" or "max".
         test_epoch - epoch to test.
         test_ckpt_path - path to checkpoint to be tested.
+        extension - checkpoint extension.
 
     Returns:
         Path to the epoch's checkpoint.
     """
 
     set_options_bool = list(map(bool, [test_epoch is not None, test_ckpt_path]))
     assert set_options_bool.count(True) <= 1, f'Both "test_epoch" and "test_ckpt_path" cannot be set.'
 
     if test_ckpt_path:
         assert os.path.isfile(test_ckpt_path), f'File does not exist: {test_ckpt_path}.'
         ckpt_path = test_ckpt_path
     elif test_epoch is not None:
-        ckpt_path = get_epoch_ckpt_path(exp_dir_trial, load_epoch=test_epoch)
+        ckpt_path = get_epoch_ckpt_path(exp_dir_trial, test_epoch, extension)
     else:
-        ckpt_path = get_best_ckpt_path(exp_dir_trial, monitor_mode)
+        ckpt_path = get_best_ckpt_path(exp_dir_trial, monitor, monitor_mode, extension)
 
     return ckpt_path
 
 
 def write_test_ckpt_path(ckpt_path: str, exp_dir_trial: str):
     """
     Write ckpt_path used for testing to a text file.
 
     Argument/s:
         ckpt_path - path to the checkpoint of the epoch that scored
             highest for the given validation metric.
         exp_dir_trial - Experiment directory for the trial.
     """
     with open(os.path.join(exp_dir_trial, 'test_ckpt_path.txt'), 'a') as f:
-        f.write(ckpt_path + "\n")
+        f.write(ckpt_path + '\n')
 
 
 def resume_from_ckpt_path(
         exp_dir_trial: str,
-        resumable: bool = False,
+        resume_last: bool = False,
         resume_epoch: int = None,
         resume_ckpt_path: str = None,
+        extension: str = '.ckpt',
 ):
     """
     Resume training from the specified checkpoint.
 
     Argument/s:
         exp_dir_trial - Experiment directory for the trial (where the checkpoints are saved).
-        resumable - if training is automatically resumable (i.e., provide last.ckpt as the path).
+        resume_last - resume from last epoch.
         resume_epoch - get the path of the checkpoint for a given epoch.
         resume_ckpt_path - outright provide the checkpoint path.
+        extension - checkpoint extension.
 
     Returns:
           ckpt_path - path to a checkpoint.
     """
 
     ckpt_path = None
 
-    options = ['resumable', 'resume_epoch', 'resume_ckpt_path']
-    set_options_bool = list(map(bool, [resumable, resume_epoch is not None, resume_ckpt_path]))
+    options = ['resume_last', 'resume_epoch', 'resume_ckpt_path']
+    set_options_bool = list(map(bool, [resume_last, resume_epoch is not None, resume_ckpt_path]))
     set_options = [j for i, j in enumerate(options) if set_options_bool[i]]
     assert set_options_bool.count(True) in [0, 1], \
         f'A maximum of one of these options can be set: {options}. The following are set: {set_options}.'
 
-    if resumable:
-        last_ckpt_path = os.path.join(exp_dir_trial, 'last.ckpt')
+    if resume_last:
+        last_ckpt_path = os.path.join(exp_dir_trial, f'last{extension}')
 
         # last.ckpt will be a directory with deepspeed:
         if os.path.isfile(last_ckpt_path) or os.path.isdir(last_ckpt_path):
-            ckpt_path = os.path.join(exp_dir_trial, 'last.ckpt')
+            ckpt_path = os.path.join(exp_dir_trial, f'last{extension}')
         else:
             warnings.warn('last.ckpt does not exist, starting training from epoch 0.')
     elif resume_epoch is not None:
-        ckpt_path = get_epoch_ckpt_path(exp_dir_trial, load_epoch=resume_epoch)
+        ckpt_path = get_epoch_ckpt_path(exp_dir_trial, resume_epoch, extension)
+        raise ValueError('"resume_epoch" is never used and will be removed in the future as it interferes with the resume from resume_from_ckpt_path logic.')
+    
     elif resume_ckpt_path:
         ckpt_path = resume_ckpt_path
+        raise ValueError('"resume_ckpt_path" is never used and will be removed in the future as it interferes with the resume from resume_from_ckpt_path logic.')
 
     if ckpt_path is not None:
         print('Resuming training from {}.'.format(ckpt_path))
 
     return ckpt_path
 
 
@@ -256,42 +277,20 @@
     Prints out GPU utilisation and sets the visibility of the GPUs to the job.
 
     Argument/s:
         cuda_visible_devices - which GPUs are visible to the job.
         submit - if the job is being submitted to a cluster manager, ignore GPU visibility requirements.
     """
 
-    # Print GPU usage
-    for gpu in GPUtil.getGPUs():
-        print(f'Initial utilisation on GPU:{gpu.id} is {gpu.memoryUtil:0.3f}.')
+    # Print GPU usage:
+    # if torch.cuda.is_available():
+    #     try:
+    #         for gpu in GPUtil.getGPUs():
+    #             print(f'Initial utilisation on GPU:{gpu.id} is {gpu.memoryUtil:0.3f}.')
+    #     except Exception as e:
+    #         print(f'NVIDIA-SMI is not working: {e}.')
 
-    # Determine the visibility of devices
+    # Determine the visibility of devices:
     if cuda_visible_devices and (not submit):
         os.environ['CUDA_VISIBLE_DEVICES'] = cuda_visible_devices
         print(f'CUDA_VISIBLE_DEVICES: {cuda_visible_devices}')
-
-
-class suppress_stdout_stderr(object):
-    """
-    Suppress STDOUT and STDERR.
-    """
-
-    def __init__(self):
-        # Open a pair of null files
-        self.null_fds = [os.open(os.devnull, os.O_RDWR) for x in range(2)]
-
-        # Save the actual stdout (1) and stderr (2) file descriptors.
-        self.save_fds = [os.dup(1), os.dup(2)]
-
-    def __enter__(self):
-        # Assign the null pointers to stdout and stderr.
-        os.dup2(self.null_fds[0], 1)
-        os.dup2(self.null_fds[1], 2)
-
-    def __exit__(self, *_):
-        # Re-assign the real stdout/stderr back to (1) and (2)
-        os.dup2(self.save_fds[0], 1)
-        os.dup2(self.save_fds[1], 2)
-
-        # Close all file descriptors
-        for fd in self.null_fds + self.save_fds:
-            os.close(fd)
+
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/PKG-INFO` & `dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: dlhpcstarter
-Version: 0.0.8
+Version: 0.1.2
 Summary: Deep Learning and HPC Starter Pack
 Home-page: https://github.com/csiro-mlai/dl_hpc_starter_pack
 Author: CSIRO
 License: Apache License 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE
 
 ![](/assets/image.png)
 
 ***Aims of this library:***
 
- - To be simple and easy to understand so that the focus is on the data science.
- - To reduce the time taken from implementation to results.
- - To promote rapid innovation of models via configuration files, class composition and/or class inheritance.
- - Reduce boilerplate code (sections of code that are repeated in multiple places with little to no variation).
- - To simplify cluster management and distributed computing with High Performance Computing (HPC).
- - Be able to easily accommodate multiple research avenues simultaneously.
- - To cooperatively improve the functionality and documentation of this repository to make it better!
+- To be simple and easy to understand so that the focus is on the data science.
+- To reduce the time taken from implementation to results.
+- To promote rapid development of models via configuration files, class composition and/or class inheritance.
+- Reduce boilerplate code (sections of code that are repeated in multiple places with little to no variation).
+- To simplify cluster management and distributed computing with High Performance Computing (HPC).
+- Be able to easily accommodate multiple research avenues simultaneously.
+- To cooperatively improve the functionality and documentation of this repository to make it better!
 
 ***Features:***
- - The [PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/latest/) `LightningModule` and `Trainer` are used to implement, train, and test models. It allows for many of the above aims to be accomplished, such as simplified distributed computing and a reduction of boilerplate code. It also allows us to simply use class inheritance and composition, allowing for rapid innovation.
- - The [Compose API](https://hydra.cc/docs/advanced/compose_api/) of [Hydra](https://hydra.cc/) is used to create a hierarchical configuration, allowing for rapid innovation.
- - [Neptune.ai](https://neptune.ai/) is used to track experiments; metric scores are automatically uploaded to [Neptune.ai](https://neptune.ai/), allowing you to easily track your experiments from your browser.
- - Scripts for submission to a cluster manager, such as [SLURM](https://slurm.schedmd.com/documentation.html) are written for you. Also, cluster manager jobs are automatically resubmitted and resumed if they haven't finished before the time-limit.
+- The [Lightning](https://pytorch-lightning.readthedocs.io/en/latest/) `LightningModule` and `Trainer` are used to implement, train, and test models. It allows for many of the above aims to be accomplished, such as simplified distributed computing and a reduction of boilerplate code. It also allows us to simply use class inheritance and composition, allowing for rapid development.
+- The [Compose API](https://hydra.cc/docs/advanced/compose_api/) of [Hydra](https://hydra.cc/) is used to create a hierarchical configuration, allowing for rapid development.
+- [Neptune.ai](https://neptune.ai/) is used to track experiments; metric scores are automatically uploaded to [Neptune.ai](https://neptune.ai/), allowing you to easily track your experiments from your browser.
+- Scripts for submission to a cluster manager, such as [SLURM](https://slurm.schedmd.com/documentation.html) are written for you. Also, cluster manager jobs are automatically resubmitted and resumed if they haven't finished before the time-limit.
 
 # Installation
 
 The Deep Learning and HPC starter pack is available on PyPI:
 ```shell
 pip install dlhpcstarter
 ```
 
 # Table of Contents
 
 [//]: # (- [How to structure your project]&#40;#how-to-structure-your-project&#41;)
 - [Package map](#package-map)
 - [Tasks](#tasks)
 - [Models](#models)
-- [Innovate via Model Composition and Inheritance](#innovate-via-model-composition-and-inheritance)
+- [Development via Model Composition and Inheritance](#development-via-model-composition-and-inheritance)
 - [Configuration YAML files and argparse](#configuration-yaml-files-and-argparse)
-- [Innovate via Configuration Files](#innovate-via-configuration-files)
+- [Development via Configuration Files](#development-via-configuration-files)
 - [Next level: Configuration composition via Hydra](#next-level-configuration-composition-via-hydra)
 - [Stages and Trainer](#stages-and-trainer)
 - [Tying it all together: `main.py`](#tying-it-all-together-mainpy)
 - [Cluster manager and distributed computing](#cluster-manager-and-distributed-computing)
 - [Monitoring using Neptune.ai](#monitoring-using-neptuneai)
 - [Where all the outputs go: `exp_dir`](#where-all-the-outputs-go-exp_dir)
 - [Repository Wish List](#repository-wish-list)
@@ -65,15 +65,15 @@
 
 [//]: # (│    │)
 
 [//]: # (│    └── TASK_NAME     - name of the task, e.g., cifar10.)
 
 [//]: # (│        └── config    - .yaml configuration files for a model.)
 
-[//]: # (│        └── models    - .py modules that contain pytorch_lightning.LightningModule definitions that represent models.)
+[//]: # (│        └── models    - .py modules that contain Lightning LightningModule definitions that represent models.)
 
 [//]: # (│        └── stages.py - training and testing stages for a task.)
 
 [//]: # (```)
 
 # Package map
 
@@ -81,76 +81,77 @@
 
 The package is structured as follows:
 
 ```
 ├──  dlhpcstarter
 │    │
 │    ├── tools                     - for all other modules; tools that are repeadetly used.
-│    ├──  __main__.py - __main__.py does the following:
-│    │               1. Reads command line arguments using argparse.
-│    │               2. Imports the 'stages' function for the task from task/TASK_NAME/stages.py.
-│    │               3. Loads the specified configuration .yaml for the job from task/TASK_NAME/config.
-│    │               4. Submits the job (the configuration + 'stages') to the cluster manager (or runs it locally if 'submit' is false).
+│    ├── __main__.py               - __main__.py does the following:
+│    │                                    1. Reads command line arguments using argparse.
+│    │                                    2. Imports the 'stages' function for the task from task/
+│    │                                    3. Loads the specified configuration .yaml for the job from 
+│    │                                    4. Submits the job (the configuration + 'stages') to the 
+│    │                                       cluster manager (or runs it locally if 'submit' is false).
 │    └── cluster.py                - contains the cluster management object.
 │    └── command_line_arguments.py - argparse for reading command line arguments.
-│    └── trainer.py                - contains a wrapper for pytorch_lightning.Trainer.
+│    └── trainer.py                - contains an optional wrapper for the Lightning Trainer.
 │    └── utils.py                  - small utility definitions.
 
 ```
 
 # Tasks
 
 ---
 
 
-***Tasks are named based on the data and the type of prediction or inference being made***. For example:
- - Two tasks have the same data but require different names due to differing predictions, e.g., **MS-COCO Detection** and **MS-COCO Caption**.
- - Two tasks may have similar predictions but require different names due to differing data, e.g., **MNIST** and **Chinese MNIST**.
+***Tasks can have any name. The name could be based on the data or the type of inference being made***. For example:
+- Two tasks have the same data but require different names due to differing predictions, e.g., **MS-COCO Detection** and **MS-COCO Caption**.
+- Two tasks may have similar predictions but require different names due to differing data, e.g., **MNIST** and **Chinese MNIST**.
 
 ***Some publicly available tasks include***:
-- Image classification tasks, e.g., [MNIST](http://yann.lecun.com/exdb/mnist/), [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet](https://www.image-net.org/). 
+- Image classification tasks, e.g., [MNIST](http://yann.lecun.com/exdb/mnist/), [CIFAR10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet](https://www.image-net.org/).
 - Object detection tasks, e.g., [MS-COCO Detection](https://cocodataset.org/#detection-2020).
 - Image captioning detection tasks, e.g., [MS-COCO Caption](https://cocodataset.org/#captions-2015).
 - Speech recognition tasks, e.g., [LibriSpeech](https://www.openslr.org/12).
 - Chest X-Ray report generation, e.g., [MIMIC-CXR](https://physionet.org/content/mimic-cxr/2.0.0/).
 
-***How to add a task:***
+***What does the name do?***
 
-Adding a task is as simple as creating a directory with the name of the task in `task`. For example, if we choose CIFAR10 as the task, with the task name `cifar10`, then we would create the directory `task/cifar10`. The task directory will then house everything necessary for that task, for example, the models, the configurations for the models, the data pipeline, and the stages of development (training and testing).
+It is used to separate the outputs of the experiment from other tasks.
 
 # Models
 
 ---
 
 
-***Please familiarise yourself with the [`pytorch_lightning.LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#) in order to correctly implement a model:*** https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html
+***Please familiarise yourself with the [`Lightning LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#) in order to correctly implement a model:*** https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html
 
-Once we have created our task directory (e.g., `task/cifar10`), we now want to create a model using a [`pytorch_lightning.LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#). Everything we need for the model can be placed in the `LightningModule`, in including commonly used libraries and objects, for example:
+A model is created using a [`Lightning LightningModule`](https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#). Everything we need for the model can be placed in the `LightningModule`, including commonly used libraries and objects, for example:
 
- - [torch.nn.Module](https://pytorch.org/docs/stable/generated/torch.nn.Module.html#torch.nn.Module): base class for all neural networks in `PyTorch`. 
- - [transformers](https://huggingface.co/docs/transformers/index): a library containing pre-trained Transformer models.
- - [torchvision](https://pytorch.org/vision/stable/index.html): a library for image pre-processing and pre-trained computer vision models.
- - [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset): an object that processes each instance of a dataset.
- - [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader): an object that samples mini-batches from a [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset).
+- [torch.nn.Module](https://pytorch.org/docs/stable/generated/torch.nn.Module.html#torch.nn.Module): base class for all neural networks in `PyTorch`.
+- [transformers](https://huggingface.co/docs/transformers/index): a library containing pre-trained Transformer models.
+- [torchvision](https://pytorch.org/vision/stable/index.html): a library for image pre-processing and pre-trained computer vision models.
+- [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset): an object that processes each instance of a dataset.
+- [torch.utils.data.DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader): an object that samples mini-batches from a [torch.utils.data.Dataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.Dataset).
 
-***Note:*** 
+***Note:***
 
-- The data pipeline could be implemented within the `LightningModule` or seperately from a model using a [pytorch_lightning.LightningDataModule](https://pytorch-lightning.readthedocs.io/en/stable/extensions/datamodules.html). The `LightningModule` instance would then have to be given separately to the `pytorch_lightning.Trainer`. 
+- The data pipeline could be implemented within the `LightningModule` or seperately from a model using a [Lightning LightningDataModule](https://pytorch-lightning.readthedocs.io/en/stable/extensions/datamodules.html). The `LightningModule` instance would then have to be given separately to the `Lightning Trainer` instance.
 
 ***Example:***
 
- - An example model for `cifar10` is in [task/cifar10/model/baseline.py](https://github.com/csiro-mlai/dl_hpc_starter_pack/blob/main/task/cifar10/model/baseline.py). 
+- An example model for `cifar10` is in [task/cifar10/model/baseline.py](https://github.com/csiro-mlai/dl_hpc_starter_pack/blob/main/task/cifar10/model/baseline.py).
 
-# Innovate via Model Composition and Inheritance
+# Development via Model Composition and Inheritance
 
 ---
-To promote rapid innovation of models, we recommend using class composition and/or inheritance. ***For example, we may have a baseline that not only includes a basic model, but also the data pipeline:***
+To promote rapid development of models, one solution is to use class composition and/or inheritance. ***For example, we may have a baseline that not only includes a basic model, but also the data pipeline:***
 
 ```python
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 from torch.utils.data import DataLoader, random_split
 import torchvision
 import torch
 
 class Baseline(LightningModule):
     def __init__(self, lr, ..., **kwargs):
         super(Baseline, self).__init__()
@@ -171,15 +172,15 @@
 
     def val_dataloader(self):
         return DataLoader(self.val_set, ...)
 
     def test_dataloader(self):
         return DataLoader(self.test_set, ...)
 
-    def configure_optimizers(self):     
+    def configure_optimizers(self):
         optimiser = {'optimizer': torch.optim.SGD(self.parameters(), lr=self.lr, momentum=0.9)}
         return optimiser
 
     def forward(self, images):
         return self.model(images)
 
     def training_step(self, batch, batch_idx):
@@ -200,18 +201,18 @@
         images, labels = batch
         y_hat = self(images)
         self.test_accuracy(torch.argmax(y_hat['logits'], dim=1), labels)
         self.log_dict({'test_acc': self.test_accuracy}, ...)
 ```
 
 After training and testing the baseline, we may want to improve upon its performance. For example, if we wanted to make the following modifications:
- 
- - Use a DenseNet instead of a ResNet.
- - Use the `AdamW` optimiser.
- - Use a warmup learning rate scheduler. 
+
+- Use a DenseNet instead of a ResNet.
+- Use the `AdamW` optimiser.
+- Use a warmup learning rate scheduler.
 
 ***All we would need to do is inherit the baseline and make our modifications:***
 
 ```python
 from transformers import get_constant_schedule_with_warmup
 
 class Inheritance(Baseline):
@@ -221,24 +222,24 @@
         self.save_hyperparameters()
         self.num_warmup_steps = num_warmup_steps
         self.model = torchvision.models.densenet121(...)
 
     def configure_optimizers(self):
         optimiser = {'optimizer': torch.optim.AdamW(self.parameters(), lr=self.lr)}
         optimiser['scheduler'] = {
-                'scheduler': get_constant_schedule_with_warmup(optimiser['optimizer'], self.num_warmup_steps),
-                'interval': 'step',
-                'frequency': 1,
-            }
+            'scheduler': get_constant_schedule_with_warmup(optimiser['optimizer'], self.num_warmup_steps),
+            'interval': 'step',
+            'frequency': 1,
+        }
         return optimiser
 ```
 We could also construct a model that is the combination of the two via composition. For example, we may want to use everything from `Baseline`, but the optimiser from `Inheritance`:
 
 ```python
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
 
 class Composite(LightningModule):
     def __init__(self, **kwargs):
         self.baseline = Baseline(self, **kwargs)
 
     def setup(self, stage=None):
         self.baseline.setup(stage)
@@ -248,15 +249,15 @@
 
     def val_dataloader(self):
         return self.baseline.val_dataloader()
 
     def test_dataloader(self):
         return self.baseline.test_dataloader()
 
-    def configure_optimizers(self):     
+    def configure_optimizers(self):
         return Inheritance.configure_optimizers(self)  # Use configure_optimizers() from Inheritance.
 
     def forward(self, images):
         return self.baseline.forward(images)
 
     def training_step(self, batch, batch_idx):
         return self.baseline.training_step(batch, batch_idx)
@@ -276,15 +277,15 @@
 Currently, there are two methods for giving arguments:
 
 1. **Via command line arguments using the [`argparse` module](https://docs.python.org/3/library/argparse.html)**. `argparse` mainly handles paths, development stage flags (e.g., training and testing flags), and cluster manager arguments.
 2. **Via a configuration file stored in [`YAML` format](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)**. Can handle all the arguments defined by the `argparse` plus more, including hyperparameters for the model.
 
 ***The mandatory arguments include:***
 1. `task`, the name of the task.
-2. `config`, relative or absolute path to the configuration file (can handle with or without extension).
+2. `config`, relative or absolute path to the configuration file (with or without the extension).
 3. `module`, the module that the model definition is housed.
 4. `definition`, the class representing the model.
 5. `exp_dir`, the experiment directory, i.e., where all outputs, including model checkpoints will be saved.
 6. `monitor`, metric to monitor for [ModelCheckpoint](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.ModelCheckpoint.html) and [EarlyStopping](https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.EarlyStopping.html?highlight=earlystoppin#earlystopping) (optional), as well as test checkpoint loading (e.g., 'val_loss').
 7. `monitor_mode`, whether the monitored metric is to be maximised or minimised ('max' or 'min').
 
 ***`task` and `config` must be given as command line arguments for `argparse`:***
@@ -293,15 +294,15 @@
 dlhpcstarter --config task/cifar10/config/baseline --task cifar10
 ```
 
 ***`module`, `definition`, and `exp_dir` can be given either as command line arguments, or be placed in the configuration file.***
 
 For each model of a task, we define a configuration. Hyperparameters, paths, as well as the device configuration can be stored in a configuration file. Configurations are in [`YAML` format](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started), e.g., `task/cifar10/config/baseline.yaml`.
 
-# Innovate via Configuration Files
+# Development via Configuration Files
 
 ---
 
 If we have the following configuration file for the aforementioned CIFAR10  `Baseline` model, `task/cifar10/config/baseline.yaml`:
 
 ```yaml
 train: True
@@ -440,80 +441,80 @@
 
 - `task/cifar10/config/cluster/2hr.yaml`:
    ```yaml
    memory: 32GB
    time_limit: '02:00:00'
    venv_path: /path/to/my/venv/bin/activate
    ```
- - `task/cifar10/config/distributed/4gpu.yaml`:
-   ```yaml
-   num_gpus: 2
-   strategy: ddp
-   ```
- - `task/cifar10/config/paths/hpc.yaml`:
-   ```yaml
-   exp_dir: /path/to/my/experiments
-   dataset_dir: /path/to/my/dataset
-   ```
+- `task/cifar10/config/distributed/4gpu.yaml`:
+  ```yaml
+  num_gpus: 2
+  strategy: ddp
+  ```
+- `task/cifar10/config/paths/hpc.yaml`:
+  ```yaml
+  exp_dir: /path/to/my/experiments
+  dataset_dir: /path/to/my/dataset
+  ```
 
 See the following documentation for more information:
- - https://hydra.cc/docs/1.2/tutorials/basic/your_first_app/defaults/
- - https://hydra.cc/docs/1.2/advanced/defaults_list/#composition-order
- - https://hydra.cc/docs/1.2/advanced/overriding_packages/
+- https://hydra.cc/docs/1.2/tutorials/basic/your_first_app/defaults/
+- https://hydra.cc/docs/1.2/advanced/defaults_list/#composition-order
+- https://hydra.cc/docs/1.2/advanced/overriding_packages/
 
 # Stages and Trainer
 
 ---
 
 
-In each task directory is a Python module called `stages.py`, which contains the `stages` definition. This definition takes an object as input that houses the configuration for a job.  
+In each task directory is a Python module called `stages.py`, which contains the `stages` definition. This definition takes an object as input that houses the configuration for a job.
 
 Typically, the following things happen in `stages()`:
 
- - The `LightningModule` model is imported via the `model` argument, e.g.,
-    ```python
-    from src import importer
-   
-    Model = importer(definition=args.definition, module=args.module)
-    model = Model(**vars(args))
-   ```
-    See `src.utils.importer` for a handy function that imports based on strings.
- - A `pytorch_lightning.Trainer` instance is created, e.g., `trainer = pytorch_lightning.Trainer(...)`.
- - The model is trained using trainer: `trainer.fit(model)`.
- - The model is tested using trainer: `trainer.test(model)`.
+- The `LightningModule` model is imported via the `model` argument, e.g.,
+   ```python
+   from src import importer
+  
+   Model = importer(definition=args.definition, module=args.module)
+   model = Model(**vars(args))
+  ```
+  See `src.utils.importer` for a handy function that imports based on strings.
+- A `Lightning Trainer` instance is created, e.g., `trainer = lightning.pytorch.Trainer(...)`.
+- The model is trained using trainer: `trainer.fit(model)`.
+- The model is tested using trainer: `trainer.test(model)`.
 
-It handles the training and testing of a model for a task by using a [`pytorch_lightning.Trainer`](https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html).
+It handles the training and testing of a model for a task by using a [`Lightning Trainer`](https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html).
 
-***A helpful wrapper at `src/trainer.py` exists that passes frequently used and useful `callbacks`, `loggers`, and `plugins` to a `pytorch_lightning.Trainer` instance:***
+***A helpful wrapper at `src/trainer.py` exists that passes frequently used and useful `callbacks`, `loggers`, and `plugins` to a `Lightning Trainer` instance:***
 
 ```python
 from src.dlhpcstarter.trainer import trainer_instance
 
 trainer = trainer_instance(**vars(args))
 ```
-Place any of the parameters for the trainer detailed at 
-https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api in your configuration file, and they will be passed to the `pytorch_lightning.Trainer` instance.
+Place any of the parameters for the trainer detailed at
+https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api in your configuration file, and they will be passed to the `Lightning Trainer` instance.
 
 # Tying it all together: `dlhpcstarter`
 
 ---
 
 ***This is an overview of what occurs when the entrypoint `dlhpcstarter` is executed, this is not necessary to understand to use the package.***
 
 
 
 `dlhpcstarter` does the following:
 
- - Gets the command line arguments using `argparse`, e.g., arguments like this:
-    ```shell
-    dlhpcstarter --config task.cifar10.config.baseline --task cifar10
-    ```
- - Imports the `stages` definition for the task using `src.utils.importer`.
- - Reads the configuration `.yaml` and combines it with the command line arguments.
- - Submits `stages` to the cluster manager if `args.submit = True` or runs `stages` locally. The command line arguments and the configuration arguments are passed to `stages` in both cases.
+- Gets the command line arguments using `argparse`, e.g., arguments like this:
+   ```shell
+   dlhpcstarter --config task.cifar10.config.baseline --task cifar10
+   ```
+- Imports the `stages` definition for the task using `src.utils.importer`.
+- Reads the configuration `.yaml` and combines it with the command line arguments.
+- Submits `stages` to the cluster manager if `args.submit = True` or runs `stages` locally. The command line arguments and the configuration arguments are passed to `stages` in both cases.
 
 # Cluster manager and distributed computing
 
 ---
 
 The following arguments are used for distributed computing:
 
@@ -596,13 +597,13 @@
 
 ***Description to be finished.
 
 
 # Repository Wish List
 
 ---
- - Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
- - Add description about how to use https://neptune.ai/.
- - Use https://hydra.cc/ instead of argparse (or have the option to use either).
- - https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
- - Notebook examples.
+- Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
+- Add description about how to use https://neptune.ai/.
+- Use https://hydra.cc/ instead of argparse (or have the option to use either).
+- https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
+- Notebook examples.
```

### Comparing `dlhpcstarter-0.0.8/src/dlhpcstarter.egg-info/SOURCES.txt` & `dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

