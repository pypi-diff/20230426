# Comparing `tmp/mlagility-2.1.1.tar.gz` & `tmp/mlagility-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlagility-2.1.1.tar", last modified: Wed Mar 29 19:20:33 2023, max compression
+gzip compressed data, was "mlagility-2.1.2.tar", last modified: Wed Apr 26 17:02:32 2023, max compression
```

## Comparing `mlagility-2.1.1.tar` & `mlagility-2.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:20:33.471620 mlagility-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-29 19:20:24.000000 mlagility-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-29 19:20:33.471620 mlagility-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-29 19:20:24.000000 mlagility-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 19:20:33.471620 mlagility-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-29 19:20:24.000000 mlagility-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:20:33.471620 mlagility-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:20:33.471620 mlagility-2.1.1/src/mlagility/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-29 19:20:24.000000 mlagility-2.1.1/src/mlagility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-29 19:20:24.000000 mlagility-2.1.1/src/mlagility/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 19:20:24.000000 mlagility-2.1.1/src/mlagility/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:20:33.471620 mlagility-2.1.1/src/mlagility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-29 19:20:33.000000 mlagility-2.1.1/src/mlagility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-29 19:20:33.000000 mlagility-2.1.1/src/mlagility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 19:20:33.000000 mlagility-2.1.1/src/mlagility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-29 19:20:33.000000 mlagility-2.1.1/src/mlagility.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-29 19:20:33.000000 mlagility-2.1.1/src/mlagility.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-29 19:20:33.000000 mlagility-2.1.1/src/mlagility.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:20:33.471620 mlagility-2.1.1/src/onnxflow/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-29 19:20:24.000000 mlagility-2.1.1/src/onnxflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 19:20:24.000000 mlagility-2.1.1/src/onnxflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:32.198678 mlagility-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 17:02:16.000000 mlagility-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-26 17:02:32.198678 mlagility-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-26 17:02:16.000000 mlagility-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:02:32.198678 mlagility-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-26 17:02:16.000000 mlagility-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:32.194678 mlagility-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:32.194678 mlagility-2.1.2/src/mlagility/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 17:02:16.000000 mlagility-2.1.2/src/mlagility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-26 17:02:16.000000 mlagility-2.1.2/src/mlagility/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 17:02:16.000000 mlagility-2.1.2/src/mlagility/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:32.194678 mlagility-2.1.2/src/mlagility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-26 17:02:32.000000 mlagility-2.1.2/src/mlagility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-26 17:02:32.000000 mlagility-2.1.2/src/mlagility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:02:32.000000 mlagility-2.1.2/src/mlagility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 17:02:32.000000 mlagility-2.1.2/src/mlagility.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-26 17:02:32.000000 mlagility-2.1.2/src/mlagility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 17:02:32.000000 mlagility-2.1.2/src/mlagility.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:32.198678 mlagility-2.1.2/src/onnxflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 17:02:16.000000 mlagility-2.1.2/src/onnxflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 17:02:16.000000 mlagility-2.1.2/src/onnxflow/version.py
```

### Comparing `mlagility-2.1.1/LICENSE` & `mlagility-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlagility-2.1.1/PKG-INFO` & `mlagility-2.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,27 @@
-Metadata-Version: 2.1
-Name: mlagility
-Version: 2.1.1
-Summary: MLAgility Benchmark and Tools
-Home-page: https://github.com/groq/mlagility
-Author: Jeremy Fowers, Daniel Holanda, Ramakrishnan Sivakumar, Victoria Godsoe
-Author-email: jfowers@groq.com, dhnoronha@groq.com, rsivakumar@groq.com, vgodsoe@groq.com
-License: MIT
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: tensorflow
-Provides-Extra: groq
-License-File: LICENSE
-
 # The MLAgility Project
 
 [![MLAgility tests](https://github.com/groq/mlagility/actions/workflows/test_mlagility.yml/badge.svg)](https://github.com/groq/mlagility/tree/main/test "Check out our tests")
 [![onnxflow tests](https://github.com/groq/mlagility/actions/workflows/test_onnxflow.yml/badge.svg)](https://github.com/groq/mlagility/tree/main/test "Check out our tests")
 [![OS - Linux](https://img.shields.io/badge/OS-Linux-blue?logo=linux&logoColor=white)](https://github.com/groq/mlagility/blob/main/docs/install.md "Check out our instructions")
 [![Made with Python](https://img.shields.io/badge/Python-3.8,3.10-blue?logo=python&logoColor=white)](https://github.com/groq/mlagility/blob/main/docs/install.md "Check out our instructions")
 [![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/groq/mlagility/blob/main/LICENSE "Check out our license")
 
 
-
 MLAgility offers a complementary approach to MLPerf by examining the capability of vendors to provide turnkey solutions to a corpus of hundreds of off-the-shelf models. All of the model scripts and benchmarking code are published as open source software. The performance data is available at our [Huggingface Space](https://huggingface.co/spaces/Groq/mlagility).
 
+
 ## Benchmarking Tool
 
-Our _benchit_ CLI allows you to benchmark Pytorch models without changing a single line of code. The demo below shows BERT-Base being benchmarked on both Nvidia A100 and Intel Xeon. For more information checkout out our [Tutorials](https://github.com/groq/mlagility/blob/main/examples/cli/readme.md) and [Tools User Guide](https://github.com/groq/mlagility/blob/main/docs/tools_user_guide.md).
+Our _benchit_ CLI allows you to benchmark Pytorch models without changing a single line of code. The demo below shows BERT-Base being benchmarked on both Nvidia A100 and Intel Xeon. For more information, check out our [Tutorials](https://github.com/groq/mlagility/blob/main/examples/cli/readme.md) and [Tools User Guide](https://github.com/groq/mlagility/blob/main/docs/tools_user_guide.md).
 
 <img src="https://github.com/groq/mlagility/raw/main/docs/img/mlagility.gif"  width="800"/>
 
+You can reproduce this demo by trying out the [Just Benchmark BERT](https://github.com/groq/mlagility/blob/main/examples/cli/readme.md#just-benchmark-bert) tutorial.
+
 ## 1000+ Models
 
 [![Transformers](https://img.shields.io/github/directory-file-count/groq/mlagility/models/transformers?label=transformers)](https://github.com/groq/mlagility/tree/main/models/transformers "Transformer models")
 [![Diffusers](https://img.shields.io/github/directory-file-count/groq/mlagility/models/diffusers?label=diffusers)](https://github.com/groq/mlagility/tree/main/models/diffusers "Diffusion models")
 [![popular_on_huggingface](https://img.shields.io/github/directory-file-count/groq/mlagility/models/popular_on_huggingface?label=popular_on_huggingface)](https://github.com/groq/mlagility/tree/main/models/popular_on_huggingface "Popular Models on Huggingface")
 [![torch_hub](https://img.shields.io/github/directory-file-count/groq/mlagility/models/torch_hub?label=torch_hub)](https://github.com/groq/mlagility/tree/main/models/torch_hub "Models from Torch Hub")
 [![torchvision](https://img.shields.io/github/directory-file-count/groq/mlagility/models/torchvision?label=torchvision)](https://github.com/groq/mlagility/tree/main/models/torchvision "Models from Torch Vision")
@@ -43,14 +31,23 @@
 
 ## Benchmarking results
 
 We are also working on making MLAgility results publicly available at our [Huggingface Space](https://huggingface.co/spaces/Groq/mlagility). Check it out!
 
 <img src="https://github.com/groq/mlagility/raw/main/docs/img/dashboard.gif"  width="800"/>
 
+## How everything fits together
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/block_diagram_light.png">
+  <source media="(prefers-color-scheme: light)" srcset="docs/img/block_diagram_dark.png">
+  <img src="docs/img/block_diagram_dark.png" alt="Architecture block diagram" width="700" height="500" />
+</picture>
+
+The diagram above illustrates the MLAgility repository's structure. Simply put, the MLAgility models are leveraged by our benchmarking tool, benchit, to produce benchmarking outcomes showcased on our Hugging Face Spaces page. 
 ## Installation
 
 Please refer to our [mlagility installation guide](https://github.com/groq/mlagility/blob/main/docs/install.md) to get instructions on how to install mlagility.
 
 ## Contributing
 
 We are actively seeking collaborators from across the industry. If you would like to contribute to this project, please check out our [contribution guide](https://github.com/groq/mlagility/blob/main/docs/contribute.md).
```

### Comparing `mlagility-2.1.1/setup.py` & `mlagility-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `mlagility-2.1.1/src/mlagility.egg-info/PKG-INFO` & `mlagility-2.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlagility
-Version: 2.1.1
+Version: 2.1.2
 Summary: MLAgility Benchmark and Tools
 Home-page: https://github.com/groq/mlagility
 Author: Jeremy Fowers, Daniel Holanda, Ramakrishnan Sivakumar, Victoria Godsoe
 Author-email: jfowers@groq.com, dhnoronha@groq.com, rsivakumar@groq.com, vgodsoe@groq.com
 License: MIT
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
@@ -17,23 +17,25 @@
 [![MLAgility tests](https://github.com/groq/mlagility/actions/workflows/test_mlagility.yml/badge.svg)](https://github.com/groq/mlagility/tree/main/test "Check out our tests")
 [![onnxflow tests](https://github.com/groq/mlagility/actions/workflows/test_onnxflow.yml/badge.svg)](https://github.com/groq/mlagility/tree/main/test "Check out our tests")
 [![OS - Linux](https://img.shields.io/badge/OS-Linux-blue?logo=linux&logoColor=white)](https://github.com/groq/mlagility/blob/main/docs/install.md "Check out our instructions")
 [![Made with Python](https://img.shields.io/badge/Python-3.8,3.10-blue?logo=python&logoColor=white)](https://github.com/groq/mlagility/blob/main/docs/install.md "Check out our instructions")
 [![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/groq/mlagility/blob/main/LICENSE "Check out our license")
 
 
-
 MLAgility offers a complementary approach to MLPerf by examining the capability of vendors to provide turnkey solutions to a corpus of hundreds of off-the-shelf models. All of the model scripts and benchmarking code are published as open source software. The performance data is available at our [Huggingface Space](https://huggingface.co/spaces/Groq/mlagility).
 
+
 ## Benchmarking Tool
 
-Our _benchit_ CLI allows you to benchmark Pytorch models without changing a single line of code. The demo below shows BERT-Base being benchmarked on both Nvidia A100 and Intel Xeon. For more information checkout out our [Tutorials](https://github.com/groq/mlagility/blob/main/examples/cli/readme.md) and [Tools User Guide](https://github.com/groq/mlagility/blob/main/docs/tools_user_guide.md).
+Our _benchit_ CLI allows you to benchmark Pytorch models without changing a single line of code. The demo below shows BERT-Base being benchmarked on both Nvidia A100 and Intel Xeon. For more information, check out our [Tutorials](https://github.com/groq/mlagility/blob/main/examples/cli/readme.md) and [Tools User Guide](https://github.com/groq/mlagility/blob/main/docs/tools_user_guide.md).
 
 <img src="https://github.com/groq/mlagility/raw/main/docs/img/mlagility.gif"  width="800"/>
 
+You can reproduce this demo by trying out the [Just Benchmark BERT](https://github.com/groq/mlagility/blob/main/examples/cli/readme.md#just-benchmark-bert) tutorial.
+
 ## 1000+ Models
 
 [![Transformers](https://img.shields.io/github/directory-file-count/groq/mlagility/models/transformers?label=transformers)](https://github.com/groq/mlagility/tree/main/models/transformers "Transformer models")
 [![Diffusers](https://img.shields.io/github/directory-file-count/groq/mlagility/models/diffusers?label=diffusers)](https://github.com/groq/mlagility/tree/main/models/diffusers "Diffusion models")
 [![popular_on_huggingface](https://img.shields.io/github/directory-file-count/groq/mlagility/models/popular_on_huggingface?label=popular_on_huggingface)](https://github.com/groq/mlagility/tree/main/models/popular_on_huggingface "Popular Models on Huggingface")
 [![torch_hub](https://img.shields.io/github/directory-file-count/groq/mlagility/models/torch_hub?label=torch_hub)](https://github.com/groq/mlagility/tree/main/models/torch_hub "Models from Torch Hub")
 [![torchvision](https://img.shields.io/github/directory-file-count/groq/mlagility/models/torchvision?label=torchvision)](https://github.com/groq/mlagility/tree/main/models/torchvision "Models from Torch Vision")
@@ -43,14 +45,23 @@
 
 ## Benchmarking results
 
 We are also working on making MLAgility results publicly available at our [Huggingface Space](https://huggingface.co/spaces/Groq/mlagility). Check it out!
 
 <img src="https://github.com/groq/mlagility/raw/main/docs/img/dashboard.gif"  width="800"/>
 
+## How everything fits together
+
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/block_diagram_light.png">
+  <source media="(prefers-color-scheme: light)" srcset="docs/img/block_diagram_dark.png">
+  <img src="docs/img/block_diagram_dark.png" alt="Architecture block diagram" width="700" height="500" />
+</picture>
+
+The diagram above illustrates the MLAgility repository's structure. Simply put, the MLAgility models are leveraged by our benchmarking tool, benchit, to produce benchmarking outcomes showcased on our Hugging Face Spaces page. 
 ## Installation
 
 Please refer to our [mlagility installation guide](https://github.com/groq/mlagility/blob/main/docs/install.md) to get instructions on how to install mlagility.
 
 ## Contributing
 
 We are actively seeking collaborators from across the industry. If you would like to contribute to this project, please check out our [contribution guide](https://github.com/groq/mlagility/blob/main/docs/contribute.md).
```

