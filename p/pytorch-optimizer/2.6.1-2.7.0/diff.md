# Comparing `tmp/pytorch_optimizer-2.6.1.tar.gz` & `tmp/pytorch_optimizer-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.6.1.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.7.0.tar", max compression
```

## Comparing `pytorch_optimizer-2.6.1.tar` & `pytorch_optimizer-2.7.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-04-22 12:14:33.011546 pytorch_optimizer-2.6.1/LICENSE
--rw-r--r--   0        0        0    28771 2023-04-22 12:14:33.011546 pytorch_optimizer-2.6.1/README.rst
--rw-r--r--   0        0        0     3649 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     6062 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     4183 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0        0 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0      131 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0     1255 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     7108 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5460 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     7237 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     5941 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     5223 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     5004 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     5828 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5053 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0      781 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3857 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5428 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0    18352 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     4165 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0     5540 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffrgrad.py
--rw-r--r--   0        0        0    10702 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0      474 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     7601 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     5563 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3954 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     2920 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4178 2023-04-22 12:14:33.015546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6550 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3639 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4149 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4314 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     3702 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     5242 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6827 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ralamb.py
--rw-r--r--   0        0        0     6224 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12516 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0     4718 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0     3907 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    15773 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    20180 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     5691 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sm3.py
--rw-r--r--   0        0        0     7895 2023-04-22 12:14:33.019546 pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0    30887 1970-01-01 00:00:00.000000 pytorch_optimizer-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 06:31:20.902848 pytorch_optimizer-2.7.0/LICENSE
+-rw-r--r--   0        0        0    30085 2023-04-26 06:31:20.902848 pytorch_optimizer-2.7.0/README.rst
+-rw-r--r--   0        0        0     3698 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6133 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     4183 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0        0 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0      131 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0     1255 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     7547 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5515 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     8416 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     6037 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     6169 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     6089 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     6544 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5424 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adanorm.py
+-rw-r--r--   0        0        0     6142 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0      781 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3873 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5498 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0    24966 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     7250 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0    10702 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0      474 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     7601 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     8607 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3923 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     2972 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4178 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6550 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3639 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4188 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4314 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     3615 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     5748 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6969 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12435 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0    15565 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/rotograd.py
+-rw-r--r--   0        0        0     4718 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0     3907 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    15801 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20180 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5123 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     8880 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0    32201 1970-01-01 00:00:00.000000 pytorch_optimizer-2.7.0/PKG-INFO
```

### Comparing `pytorch_optimizer-2.6.1/LICENSE` & `pytorch_optimizer-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/README.rst` & `pytorch_optimizer-2.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Lion         | *Symbolic Discovery of Optimization Algorithms*                                                 | `github <https://github.com/google/automl/tree/master/lion>`__                    | `https://arxiv.org/abs/2302.06675 <https://arxiv.org/abs/2302.06675>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Ali-G        | *Adaptive Learning Rates for Interpolation with Gradients*                                      | `github <https://github.com/oval-group/ali-g>`__                                  | `https://arxiv.org/abs/1906.05661 <https://arxiv.org/abs/1906.05661>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | SM3          | *Memory-Efficient Adaptive Optimization*                                                        | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AdaNorm      | *Adaptive Gradient Norm Correction based Optimizer for CNNs*                                    | `github <https://github.com/shivram1987/AdaNorm>`__                               | `https://arxiv.org/abs/2210.06364 <https://arxiv.org/abs/2210.06364>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| RotoGrad     | *Gradient Homogenization in Multitask Learning*                                                 | `github <https://github.com/adrianjav/rotograd>`__                                | `https://openreview.net/pdf?id=T8wHz4rnuGL <https://openreview.net/pdf?id=T8wHz4rnuGL>`__     |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 
 Useful Resources
 ----------------
 
 Several optimization ideas to regularize & stabilize the training. Most
 of the ideas are applied in ``Ranger21`` optimizer.
 
@@ -343,14 +347,18 @@
 
 `Lion <https://github.com/google/automl/tree/master/lion#citation>`__
 
 `Ali-G <https://github.com/oval-group/ali-g#adaptive-learning-rates-for-interpolation-with-gradients>`__
 
 `SM3 <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__
 
+`AdaNorm <https://github.com/shivram1987/AdaNorm/tree/main#citation>`__
+
+`RotoGrad <https://github.com/adrianjav/rotograd#citing>`__
+
 Citation
 --------
 
 Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
 Or you can get from "cite this repository" button.
 
 ::
```

### Comparing `pytorch_optimizer-2.6.1/pyproject.toml` & `pytorch_optimizer-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.6.1"
+version = "2.7.0"
 description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
@@ -99,12 +99,13 @@
 "./pytorch_optimizer/__init__.py" = ["F401"]
 "./pytorch_optimizer/lr_scheduler/__init__.py" = ["F401"]
 
 [tool.coverage.run]
 omit = [
     "./pytorch_optimizer/optimizer/gsam.py",
     "./pytorch_optimizer/optimizer/fp16.py",
+    "./pytorch_optimizer/optimizer/rotograd.py",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,37 +19,37 @@
 from pytorch_optimizer.optimizer.adabelief import AdaBelief
 from pytorch_optimizer.optimizer.adabound import AdaBound
 from pytorch_optimizer.optimizer.adafactor import AdaFactor
 from pytorch_optimizer.optimizer.adai import Adai
 from pytorch_optimizer.optimizer.adamp import AdamP
 from pytorch_optimizer.optimizer.adams import AdamS
 from pytorch_optimizer.optimizer.adan import Adan
+from pytorch_optimizer.optimizer.adanorm import AdaNorm
 from pytorch_optimizer.optimizer.adapnm import AdaPNM
 from pytorch_optimizer.optimizer.agc import agc
 from pytorch_optimizer.optimizer.alig import AliG
 from pytorch_optimizer.optimizer.apollo import Apollo
-from pytorch_optimizer.optimizer.dadapt import DAdaptAdaGrad, DAdaptAdam, DAdaptSGD
+from pytorch_optimizer.optimizer.dadapt import DAdaptAdaGrad, DAdaptAdam, DAdaptAdan, DAdaptSGD
 from pytorch_optimizer.optimizer.diffgrad import DiffGrad
-from pytorch_optimizer.optimizer.diffrgrad import DiffRGrad
 from pytorch_optimizer.optimizer.fp16 import DynamicLossScaler, SafeFP16Optimizer
 from pytorch_optimizer.optimizer.gc import centralize_gradient
 from pytorch_optimizer.optimizer.gsam import GSAM
 from pytorch_optimizer.optimizer.lamb import Lamb
 from pytorch_optimizer.optimizer.lars import LARS
 from pytorch_optimizer.optimizer.lion import Lion
 from pytorch_optimizer.optimizer.lookahead import Lookahead
 from pytorch_optimizer.optimizer.madgrad import MADGRAD
 from pytorch_optimizer.optimizer.nero import Nero
 from pytorch_optimizer.optimizer.novograd import NovoGrad
 from pytorch_optimizer.optimizer.pcgrad import PCGrad
 from pytorch_optimizer.optimizer.pnm import PNM
 from pytorch_optimizer.optimizer.radam import RAdam
-from pytorch_optimizer.optimizer.ralamb import RaLamb
 from pytorch_optimizer.optimizer.ranger import Ranger
 from pytorch_optimizer.optimizer.ranger21 import Ranger21
+from pytorch_optimizer.optimizer.rotograd import RotoGrad
 from pytorch_optimizer.optimizer.sam import SAM
 from pytorch_optimizer.optimizer.sgdp import SGDP
 from pytorch_optimizer.optimizer.shampoo import ScalableShampoo, Shampoo
 from pytorch_optimizer.optimizer.shampoo_utils import (
     AdaGradGraft,
     BlockPartitioner,
     Graft,
@@ -65,50 +65,52 @@
     power_iteration,
 )
 from pytorch_optimizer.optimizer.sm3 import SM3
 from pytorch_optimizer.optimizer.utils import (
     clip_grad_norm,
     disable_running_stats,
     enable_running_stats,
+    get_global_gradient_norm,
     get_optimizer_parameters,
     normalize_gradient,
+    reduce_max_except_dim,
     unit_norm,
 )
 
 OPTIMIZER_LIST: List[OPTIMIZER] = [
     AdaBelief,
     AdaBound,
     AdamP,
     Adai,
     Adan,
     AdaPNM,
     DiffGrad,
-    DiffRGrad,
     Lamb,
     LARS,
     MADGRAD,
     Nero,
     PNM,
     RAdam,
-    RaLamb,
     Ranger,
     Ranger21,
     SGDP,
     Shampoo,
     ScalableShampoo,
     DAdaptAdaGrad,
     DAdaptAdam,
     DAdaptSGD,
+    DAdaptAdan,
     AdamS,
     AdaFactor,
     Apollo,
     NovoGrad,
     Lion,
     AliG,
     SM3,
+    AdaNorm,
 ]
 OPTIMIZERS: Dict[str, OPTIMIZER] = {str(optimizer.__name__).lower(): optimizer for optimizer in OPTIMIZER_LIST}
 
 LR_SCHEDULER_LIST: List[SCHEDULER] = [
     CosineAnnealingWarmupRestarts,
     ConstantLR,
     CosineAnnealingLR,
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/base/exception.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/base/optimizer.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/base/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabelief.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     :param weight_decay: float. weight decay (L2 penalty).
     :param n_sma_threshold: number of SMA threshold (recommended is 5).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
     :param fixed_decay: bool. fix weight decay.
     :param rectify: bool. perform the rectified update similar to RAdam.
     :param degenerated_to_sgd: bool. perform SGD update when variance of gradient is high.
     :param amsgrad: bool. whether to use the AMSBound variant.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
@@ -33,148 +35,162 @@
         weight_decay: float = 0.0,
         n_sma_threshold: int = 5,
         weight_decouple: bool = True,
         fixed_decay: bool = False,
         rectify: bool = True,
         degenerated_to_sgd: bool = True,
         amsgrad: bool = False,
-        adamd_debias_term: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
         eps: float = 1e-16,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
         self.n_sma_threshold = n_sma_threshold
-        self.weight_decouple = weight_decouple
-        self.fixed_decay = fixed_decay
-        self.rectify = rectify
         self.degenerated_to_sgd = degenerated_to_sgd
-        self.adamd_debias_term = adamd_debias_term
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
-            'eps': eps,
             'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'rectify': rectify,
             'amsgrad': amsgrad,
-            'adamd_debias_term': adamd_debias_term,
-            'buffer': [[None, None, None] for _ in range(10)],
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
+            'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
         return 'AdaBelief'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_var'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
                 if group['amsgrad']:
                     state['max_exp_avg_var'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
-            weight_decay: float = group['weight_decay']
+            weight_decay = group['weight_decay']
 
-            if self.rectify:
+            bias_correction1 = 1.0 - beta1 ** group['step']
+            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+
+            if group['rectify']:
                 n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
+                beta2_t: float = beta2 ** group['step']
+                n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_var'] = torch.zeros_like(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
                     if group['amsgrad']:
                         state['max_exp_avg_var'] = torch.zeros_like(p)
 
-                if self.weight_decouple:
-                    p.mul_(1.0 - (group['lr'] * weight_decay if not self.fixed_decay else weight_decay))
+                if group['weight_decouple']:
+                    p.mul_(1.0 - group['weight_decay'] * (1.0 if group['fixed_decay'] else group['lr']))
                 elif weight_decay > 0.0:
                     grad.add_(p, alpha=weight_decay)
 
-                state['step'] += 1
                 exp_avg, exp_avg_var = state['exp_avg'], state['exp_avg_var']
 
-                bias_correction1 = 1.0 - beta1 ** state['step']
-                bias_correction2_sq = math.sqrt(1.0 - beta2 ** state['step'])
-
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
-                grad_residual = grad - exp_avg
-                exp_avg_var.mul_(beta2).addcmul_(grad_residual, grad_residual, value=1.0 - beta2).add_(group['eps'])
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
+
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
+
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
+                grad_residual = s_grad - exp_avg
+                exp_avg_var.mul_(beta2).addcmul_(grad_residual, grad_residual, value=1.0 - beta2).add_(self.eps)
 
                 if group['amsgrad']:
                     max_exp_avg_var = state['max_exp_avg_var']
                     torch.max(max_exp_avg_var, exp_avg_var, out=max_exp_avg_var)
-                    de_nom = max_exp_avg_var.sqrt()
+                    de_nom = max_exp_avg_var.add(self.eps).sqrt()
                 else:
-                    de_nom = exp_avg_var.sqrt()
-                de_nom.div_(bias_correction2_sq).add_(group['eps'])
+                    de_nom = exp_avg_var.add(self.eps).sqrt()
 
-                if not self.rectify:
-                    step_size: float = group['lr'] if group['adamd_debias_term'] else group['lr'] / bias_correction1
+                de_nom.div_(bias_correction2_sq).add_(self.eps)
+
+                if not group['rectify']:
+                    step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
                     p.addcdiv_(exp_avg, de_nom, value=-step_size)
                     continue
 
-                buffered = group['buffer'][state['step'] % 10]
-                if state['step'] == buffered[0]:
-                    n_sma, step_size = buffered[1], buffered[2]
+                if n_sma >= self.n_sma_threshold:
+                    step_size = math.sqrt(
+                        (1 - beta2_t)
+                        * (n_sma - 4)
+                        / (n_sma_max - 4)
+                        * (n_sma - 2)
+                        / n_sma
+                        * n_sma_max
+                        / (n_sma_max - 2)
+                    )
+                elif self.degenerated_to_sgd:
+                    step_size = 1.0
                 else:
-                    buffered[0] = state['step']
-                    beta2_t = beta2 ** state['step']
-                    n_sma = n_sma_max - 2 * state['step'] * beta2_t / (1 - beta2_t)
-                    buffered[1] = n_sma
-
-                    if n_sma >= self.n_sma_threshold:
-                        step_size = math.sqrt(
-                            (1 - beta2_t)
-                            * (n_sma - 4)
-                            / (n_sma_max - 4)
-                            * (n_sma - 2)
-                            / n_sma
-                            * n_sma_max
-                            / (n_sma_max - 2)
-                        )
-                        if not group['adamd_debias_term']:
-                            step_size /= bias_correction1
-                    elif self.degenerated_to_sgd:
-                        step_size = 1.0 / bias_correction1
-                    else:
-                        step_size = -1
+                    step_size = -1
 
-                    buffered[2] = step_size
+                if not group['adam_debias']:
+                    step_size /= bias_correction1
 
                 if n_sma >= self.n_sma_threshold:
-                    de_nom = exp_avg_var.sqrt().add_(group['eps'])
+                    de_nom = exp_avg_var.sqrt().add_(self.eps)
                     p.addcdiv_(exp_avg, de_nom, value=-step_size * group['lr'])
                 elif step_size > 0:
                     p.add_(exp_avg, alpha=-step_size * group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,169 @@
 import math
-from typing import List
 
 import torch
 from torch.optim.optimizer import Optimizer
 
-from pytorch_optimizer.base.exception import NoSparseGradientError
+from pytorch_optimizer.base.exception import NoSparseGradientError, ZeroParameterSizeError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.gc import centralize_gradient
 
 
-class AdaBound(Optimizer, BaseOptimizer):
-    r"""Adaptive Gradient Methods with Dynamic Bound of Learning Rate.
+class Adai(Optimizer, BaseOptimizer):
+    r"""Disentangling the Effects of Adaptive Learning Rate and Momentum.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
-    :param final_lr: float. final learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-    :param gamma: float. convergence speed of the bound functions.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
-    :param fixed_decay: bool. fix weight decay.
-    :param amsbound: bool. whether to use the AMSBound variant.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param stable_weight_decay: bool. perform stable weight decay.
+    :param dampening: float. dampening for momentum. where dampening < 1, it will show some adaptive-moment behavior.
+    :param use_gc: bool. use gradient centralization.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        final_lr: float = 1e-1,
-        betas: BETAS = (0.9, 0.999),
-        gamma: float = 1e-3,
+        betas: BETAS = (0.1, 0.99),
         weight_decay: float = 0.0,
-        weight_decouple: bool = True,
-        fixed_decay: bool = False,
-        amsbound: bool = False,
-        adamd_debias_term: bool = False,
-        eps: float = 1e-8,
+        weight_decouple: bool = False,
+        stable_weight_decay: bool = False,
+        dampening: float = 1.0,
+        use_gc: bool = False,
+        eps: float = 1e-3,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
         self.weight_decouple = weight_decouple
-        self.fixed_decay = fixed_decay
+        self.stable_weight_decay = stable_weight_decay
+        self.dampening = dampening
+        self.use_gc = use_gc
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
-            'final_lr': final_lr,
-            'gamma': gamma,
             'weight_decay': weight_decay,
-            'amsbound': amsbound,
-            'adamd_debias_term': adamd_debias_term,
+            'weight_decouple': weight_decouple,
+            'stable_weight_decay': stable_weight_decay,
+            'dampening': dampening,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-        self.base_lrs: List[float] = [group['lr'] for group in self.param_groups]
-
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'AdaBound'
+        return 'Adai'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
                 state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                if group['amsbound']:
-                    state['max_exp_avg_sq'] = torch.zeros_like(p)
+                state['beta1_prod'] = torch.ones_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        for group, base_lr in zip(self.param_groups, self.base_lrs):
-            beta1, beta2 = group['betas']
+        param_size: int = 0
+        exp_avg_sq_hat_sum: float = 0.0
+
+        for group in self.param_groups:
+            _, beta2 = group['betas']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
+                param_size += p.numel()
+
                 state = self.state[p]
 
                 if len(state) == 0:
                     state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    if group['amsbound']:
-                        state['max_exp_avg_sq'] = torch.zeros_like(p)
+                    state['beta1_prod'] = torch.ones_like(p)
 
                 state['step'] += 1
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                if group['weight_decay'] > 0.0:
-                    if self.weight_decouple:
-                        p.mul_(
-                            1.0 - (group['weight_decay'] if self.fixed_decay else group['lr'] * group['weight_decay'])
-                        )
+                if self.use_gc:
+                    grad = centralize_gradient(grad, gc_conv_only=False)
+
+                bias_correction2 = 1.0 - beta2 ** state['step']
+
+                if not group['stable_weight_decay'] and group['weight_decay'] > 0.0:
+                    if group['weight_decouple']:
+                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
                     else:
                         grad.add_(p, alpha=group['weight_decay'])
 
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+                exp_avg_sq = state['exp_avg_sq']
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
-                if group['amsbound']:
-                    torch.max(state['max_exp_avg_sq'], exp_avg_sq, out=exp_avg_sq)
 
-                de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                exp_avg_sq_hat_sum += exp_avg_sq.sum() / bias_correction2
+
+        if param_size == 0:
+            raise ZeroParameterSizeError()
+
+        exp_avg_sq_hat_mean = exp_avg_sq_hat_sum / param_size
+
+        for group in self.param_groups:
+            beta0, beta2 = group['betas']
+            beta0_dp = math.pow(beta0, 1.0 - group['dampening'])
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                grad = p.grad
+                state = self.state[p]
+
+                if group['stable_weight_decay'] and group['weight_decay'] > 0.0:
+                    if group['weight_decouple']:
+                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
+                    else:
+                        grad.add_(p, alpha=group['weight_decay'])
+
+                bias_correction2 = 1.0 - beta2 ** state['step']
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                bias_correction1 = 1.0 - beta1 ** state['step']
-                bias_correction2_sq = math.sqrt(1.0 - beta2 ** state['step'])
+                exp_avg_sq_hat = exp_avg_sq / bias_correction2
+                beta1 = (
+                    1.0 - (exp_avg_sq_hat / exp_avg_sq_hat_mean).pow(1.0 / (3.0 - 2.0 * group['dampening'])).mul(beta0)
+                ).clamp(0.0, 1.0 - group['eps'])
+                beta3 = (1.0 - beta1).pow(group['dampening'])
 
-                step_size = group['lr'] * bias_correction2_sq
-                if not group['adamd_debias_term']:
-                    step_size /= bias_correction1
+                beta1_prod = state['beta1_prod']
+                beta1_prod.mul_(beta1)
 
-                final_lr = group['final_lr'] * group['lr'] / base_lr
-                lower_bound = final_lr * (1 - 1 / (group['gamma'] * state['step'] + 1))
-                upper_bound = final_lr * (1 + 1 / (group['gamma'] * state['step']))
+                bias_correction1 = 1.0 - beta1_prod
 
-                step_size = torch.full_like(de_nom, step_size)
-                step_size.div_(de_nom).clamp_(lower_bound, upper_bound).mul_(exp_avg)
+                exp_avg.mul_(beta1).addcmul_(beta3, grad)
+                exp_avg_hat = exp_avg.div(bias_correction1).mul(beta0_dp)
 
-                p.add_(-step_size)
+                p.add_(exp_avg_hat, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adafactor.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,50 +14,60 @@
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param decay_rate: float. coefficient used to compute running averages of square gradient.
     :param weight_decay: float. weight decay (L2 penalty).
     :param clip_threshold: float. threshold of root-mean-square of final gradient update.
+    :param amsgrad: bool. whether to use the AMSBound variant.
     :param scale_parameter: bool. if true, learning rate is scaled by root-mean-square of parameter.
     :param relative_step: bool. if true, time-dependent learning rate is computed instead of external learning rate.
-    :param warmup_init: bool. time-dependent learning rate computation depends on
-        whether warm-up initialization is being used.
+    :param warmup_init: bool. time-dependent learning rate computation depends on whether warm-up initialization
+        is being used.
     :param eps1: float. term added to the denominator to improve numerical stability.
     :param eps2: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: Optional[float] = 1e-3,
         betas: BETAS = (0.9, 0.999),
         decay_rate: float = -0.8,
         weight_decay: float = 0.0,
         clip_threshold: float = 1.0,
+        amsgrad: bool = False,
         scale_parameter: bool = True,
         relative_step: bool = True,
         warmup_init: bool = False,
         eps1: float = 1e-30,
         eps2: float = 1e-3,
     ):
         self.lr = lr
         self.betas = betas
         self.decay_rate = decay_rate
         self.weight_decay = weight_decay
         self.clip_threshold = clip_threshold
-        self.scale_parameter = scale_parameter
+        self.amsgrad = amsgrad
         self.relative_step = relative_step
-        self.warmup_init = warmup_init
         self.eps1 = eps1
         self.eps2 = eps2
 
         self.validate_parameters()
 
-        defaults: DEFAULTS = {'lr': lr, 'weight_decay': weight_decay}
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'weight_decay': weight_decay,
+            'amsgrad': amsgrad,
+            'scale_parameter': scale_parameter,
+            'relative_step': relative_step,
+            'warmup_init': warmup_init,
+            'eps1': eps1,
+            'eps2': eps2,
+        }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps1)
@@ -65,40 +75,48 @@
 
     def __str__(self) -> str:
         return 'AdaFactor'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 grad = p.grad
 
                 grad_shape: Tuple[int, ...] = grad.shape
                 factored: bool = self.get_options(grad_shape)
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
 
                 if factored:
-                    state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1]).to(grad)
-                    state['exp_avg_sq_col'] = torch.zeros(grad_shape[:-2] + grad_shape[-1:]).to(grad)
+                    state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype, device=grad.device)
+                    state['exp_avg_sq_col'] = torch.zeros(
+                        grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype, device=grad.device
+                    )
                 else:
                     state['exp_avg_sq'] = torch.zeros_like(grad)
 
+                if group['amsgrad']:
+                    state['exp_avg_sq_hat'] = torch.zeros_like(grad)
+
                 state['RMS'] = 0.0
 
-    def get_lr(self, lr: float, step: int, rms: float) -> float:
+    def get_lr(
+        self, lr: float, step: int, rms: float, relative_step: bool, warmup_init: bool, scale_parameter: bool
+    ) -> float:
+        r"""Get AdaFactor learning rate."""
         relative_step_size: float = lr
-        if self.relative_step:
-            min_step: float = 1e-6 * step if self.warmup_init else 1e-2
+        if relative_step:
+            min_step: float = 1e-6 * step if warmup_init else 1e-2
             relative_step_size = min(min_step, 1.0 / math.sqrt(step))
 
-        param_scale: float = 1.0 if self.scale_parameter else max(self.eps2, rms)
+        param_scale: float = 1.0 if scale_parameter else max(self.eps2, rms)
 
         return param_scale * relative_step_size
 
     @staticmethod
     def get_options(shape: Tuple[int, ...]) -> bool:
         r"""Get `factored`."""
         return len(shape) >= 2
@@ -123,71 +141,86 @@
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
+            beta2_t: float = 1.0 - math.pow(group['step'], self.decay_rate)
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 grad_shape: Tuple[int, ...] = grad.shape
                 factored: bool = self.get_options(grad_shape)
 
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
 
                     if factored:
                         state['exp_avg_sq_row'] = torch.zeros(grad_shape[:-1], dtype=grad.dtype, device=grad.device)
                         state['exp_avg_sq_col'] = torch.zeros(
                             grad_shape[:-2] + grad_shape[-1:], dtype=grad.dtype, device=grad.device
                         )
                     else:
                         state['exp_avg_sq'] = torch.zeros_like(grad)
 
-                    state['RMS'] = 0.0
+                    if group['amsgrad']:
+                        state['exp_avg_sq_hat'] = torch.zeros_like(grad)
 
-                state['step'] += 1
+                    state['RMS'] = 0.0
 
                 state['RMS'] = self.get_rms(p)
-                lr = self.get_lr(group['lr'], state['step'], state['RMS'])
 
-                beta2_t: float = 1.0 - math.pow(state['step'], self.decay_rate)
+                lr = self.get_lr(
+                    group['lr'],
+                    group['step'],
+                    state['RMS'],
+                    relative_step=group['relative_step'],
+                    warmup_init=group['warmup_init'],
+                    scale_parameter=group['scale_parameter'],
+                )
+
                 update = torch.mul(grad, grad).add_(self.eps1)
 
                 if factored:
                     exp_avg_sq_row, exp_avg_sq_col = state['exp_avg_sq_row'], state['exp_avg_sq_col']
 
                     exp_avg_sq_row.mul_(beta2_t).add_(update.mean(dim=-1), alpha=1.0 - beta2_t)
                     exp_avg_sq_col.mul_(beta2_t).add_(update.mean(dim=-2), alpha=1.0 - beta2_t)
 
-                    self.approximate_sq_grad(exp_avg_sq_row, exp_avg_sq_col, output=update)
+                    self.approximate_sq_grad(exp_avg_sq_row, exp_avg_sq_col, update)
                 else:
                     exp_avg_sq = state['exp_avg_sq']
                     exp_avg_sq.mul_(beta2_t).add_(update, alpha=1.0 - beta2_t)
                     torch.rsqrt(exp_avg_sq, out=update)
 
-                update.mul_(grad)
+                if group['amsgrad']:
+                    exp_avg_sq_hat = state['exp_avg_sq_hat']
+                    torch.max(exp_avg_sq_hat, 1 / update, out=exp_avg_sq_hat)
+                    torch.rsqrt(exp_avg_sq_hat / beta2_t, out=update)
 
-                # TODO: implement AMSGrad
+                update.mul_(grad)
 
                 update.div_((self.get_rms(update) / self.clip_threshold).clamp_(min=1.0)).mul_(lr)
 
                 exp_avg = state['exp_avg']
                 exp_avg.mul_(self.betas[0]).add_(update, alpha=1.0 - self.betas[0])
 
-                update = exp_avg
-
                 if group['weight_decay'] > 0.0:
                     p.add_(p, alpha=-lr * group['weight_decay'])
 
-                p.add_(-update)
+                p.add_(-exp_avg)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/apollo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,157 @@
-import math
+from typing import Optional
 
+import numpy as np
 import torch
 from torch.optim.optimizer import Optimizer
 
-from pytorch_optimizer.base.exception import NoSparseGradientError, ZeroParameterSizeError
+from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
-from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
-from pytorch_optimizer.optimizer.gc import centralize_gradient
+from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class Adai(Optimizer, BaseOptimizer):
-    r"""Disentangling the Effects of Adaptive Learning Rate and Momentum.
+class Apollo(Optimizer, BaseOptimizer):
+    r"""An Adaptive Parameter-wise Diagonal Quasi-Newton Method for Nonconvex Stochastic Optimization.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
-    :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
+    :param init_lr: Optional[float]. initial learning rate (default lr / 1000).
+    :param beta: float. coefficient used for computing running averages of gradient.
+    :param rebound: str. rectified bound for diagonal hessian. (constant, belief).
     :param weight_decay: float. weight decay (L2 penalty).
-    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
-    :param use_stable_weight_decay: bool. perform stable weight decay.
-    :param dampening: float. dampening for momentum. where dampening < 1, it will show some adaptive-moment behavior.
-    :param use_gc: bool. use gradient centralization.
+    :param weight_decay_type: str. type of weight decay. (l2, decoupled, stable).
+    :param warmup_steps: int. number of warmup steps.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.1, 0.99),
+        init_lr: Optional[float] = None,
+        beta: float = 0.9,
+        rebound: str = 'constant',
         weight_decay: float = 0.0,
-        weight_decouple: bool = False,
-        use_stable_weight_decay: bool = False,
-        dampening: float = 1.0,
-        use_gc: bool = False,
-        eps: float = 1e-3,
+        weight_decay_type: str = 'l2',
+        warmup_steps: int = 500,
+        eps: float = 1e-4,
     ):
         self.lr = lr
-        self.betas = betas
+        self.beta = beta
+        self.rebound = rebound
         self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
-        self.use_stable_weight_decay = use_stable_weight_decay
-        self.dampening = dampening
-        self.use_gc = use_gc
+        self.weight_decay_type = weight_decay_type
+        self.warmup_steps = warmup_steps
         self.eps = eps
 
         self.validate_parameters()
 
+        self.init_lr: float = init_lr if init_lr is not None else lr / 1000.0
+
         defaults: DEFAULTS = {
             'lr': lr,
-            'betas': betas,
+            'init_lr': self.init_lr,
+            'beta': beta,
+            'rebound': rebound,
             'weight_decay': weight_decay,
-            'dampening': dampening,
+            'weight_decay_type': weight_decay_type,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
-        self.validate_betas(self.betas)
+        self.validate_beta(self.beta)
+        self.validate_rebound(self.rebound)
         self.validate_weight_decay(self.weight_decay)
+        self.validate_weight_decay_type(self.weight_decay_type)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'Adai'
+        return 'Apollo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
-                state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_sq'] = torch.zeros_like(p)
-                state['beta1_prod'] = torch.ones_like(p)
+                state['exp_avg_grad'] = torch.zeros_like(p)
+                state['approx_hessian'] = torch.zeros_like(p)
+                state['update'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        param_size: int = 0
-        exp_avg_sq_hat_sum: float = 0.0
-
         for group in self.param_groups:
-            _, beta2 = group['betas']
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
+            current_lr: float = (
+                group['lr']
+                if group['step'] >= self.warmup_steps
+                else (self.lr - group['init_lr']) * group['step'] / self.warmup_steps + group['init_lr']
+            )
+
+            weight_decay, eps = group['weight_decay'], group['eps']
+
+            bias_correction: float = 1.0 - group['beta'] ** group['step']
+            alpha: float = (1.0 - group['beta']) / bias_correction
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                param_size += p.numel()
-
                 state = self.state[p]
-
                 if len(state) == 0:
-                    state['step'] = 0
-                    state['exp_avg'] = torch.zeros_like(p)
-                    state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['beta1_prod'] = torch.ones_like(p)
-
-                state['step'] += 1
-
-                if self.use_gc:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
-
-                bias_correction2 = 1.0 - beta2 ** state['step']
+                    state['exp_avg_grad'] = torch.zeros_like(p)
+                    state['approx_hessian'] = torch.zeros_like(p)
+                    state['update'] = torch.zeros_like(p)
 
-                if not self.use_stable_weight_decay and group['weight_decay'] > 0.0:
-                    if self.weight_decouple:
-                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    else:
-                        grad.add_(p, alpha=group['weight_decay'])
+                if weight_decay > 0.0 and group['weight_decay_type'] == 'l2':
+                    grad.add_(p, alpha=weight_decay)
 
-                exp_avg_sq = state['exp_avg_sq']
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+                exp_avg_grad, b, d_p = state['exp_avg_grad'], state['approx_hessian'], state['update']
 
-                exp_avg_sq_hat_sum += exp_avg_sq.sum() / bias_correction2
+                delta_grad = grad - exp_avg_grad
+                if group['rebound'] == 'belief':
+                    rebound = delta_grad.norm(p=np.inf)
+                else:
+                    rebound = 1e-2
+                    eps /= rebound
 
-        if param_size == 0:
-            raise ZeroParameterSizeError()
-
-        exp_avg_sq_hat_mean = exp_avg_sq_hat_sum / param_size
-
-        for group in self.param_groups:
-            beta0, beta2 = group['betas']
-            beta0_dp = math.pow(beta0, 1.0 - group['dampening'])
-            for p in group['params']:
-                if p.grad is None:
-                    continue
-
-                grad = p.grad
-                state = self.state[p]
+                exp_avg_grad.add_(delta_grad, alpha=alpha)
 
-                if self.use_stable_weight_decay and group['weight_decay'] > 0.0:
-                    if self.weight_decouple:
-                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    else:
-                        grad.add_(p, alpha=group['weight_decay'])
+                de_nom = d_p.norm(p=4).add(eps)
+                d_p.div_(de_nom)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                v_sq = d_p.mul(d_p)
+                delta = delta_grad.div_(de_nom).mul_(d_p).sum().mul(-alpha) - b.mul(v_sq).sum()
 
-                bias_correction2 = 1.0 - beta2 ** state['step']
+                b.addcmul_(v_sq, delta)
 
-                exp_avg_sq_hat = exp_avg_sq / bias_correction2
-                beta1 = (
-                    1.0 - (exp_avg_sq_hat / exp_avg_sq_hat_mean).pow(1.0 / (3.0 - 2.0 * group['dampening'])).mul(beta0)
-                ).clamp(0.0, 1.0 - group['eps'])
-                beta3 = (1.0 - beta1).pow(group['dampening'])
+                de_nom = b.abs().clamp_(min=rebound)
+                if group['rebound'] == 'belief':
+                    de_nom.add_(eps / alpha)
 
-                beta1_prod = state['beta1_prod']
-                beta1_prod.mul_(beta1)
+                d_p.copy_(exp_avg_grad.div(de_nom))
 
-                bias_correction1 = 1.0 - beta1_prod
+                if weight_decay > 0.0 and group['weight_decay_type'] != 'l2':
+                    if group['weight_decay_type'] == 'stable':
+                        weight_decay /= de_nom.mean().item()
 
-                exp_avg.mul_(beta1).addcmul_(beta3, grad)
-                exp_avg_hat = exp_avg.div(bias_correction1).mul(beta0_dp)
+                    d_p.add_(p, alpha=weight_decay)
 
-                p.add_(exp_avg_hat, alpha=-group['lr'])
+                p.add_(d_p, alpha=-current_lr)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adamp.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,29 +18,33 @@
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param delta: float. threshold that determines whether a set of parameters is scale invariant or not.
     :param wd_ratio: float. relative weight decay applied on scale-invariant parameters compared to that applied
         on scale-variant parameters.
     :param use_gc: bool. use gradient centralization.
     :param nesterov: bool. enables Nesterov momentum.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
         delta: float = 0.1,
         wd_ratio: float = 0.1,
         use_gc: bool = False,
         nesterov: bool = False,
-        adamd_debias_term: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
         eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
         self.eps = eps
         self.wd_ratio = wd_ratio
@@ -51,17 +55,21 @@
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'delta': delta,
             'wd_ratio': wd_ratio,
             'nesterov': nesterov,
-            'adamd_debias_term': adamd_debias_term,
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_weight_decay_ratio(self.wd_ratio)
@@ -69,54 +77,71 @@
 
     def __str__(self) -> str:
         return 'AdamP'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
+            bias_correction1 = 1.0 - beta1 ** group['step']
+            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
-                state['step'] += 1
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                bias_correction1 = 1.0 - beta1 ** state['step']
-                bias_correction2_sq = math.sqrt(1.0 - beta2 ** state['step'])
-
                 if self.use_gc:
                     grad = centralize_gradient(grad, gc_conv_only=False)
 
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
+
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
+
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
                 inv_de_nom = 1.0 / (exp_avg_sq.sqrt() / bias_correction2_sq).add_(group['eps'])
 
                 perturb = exp_avg.clone()
                 if group['nesterov']:
                     perturb.mul_(beta1).addcmul_(grad, inv_de_nom, value=1.0 - beta1)
@@ -133,11 +158,11 @@
                         group['wd_ratio'],
                         group['eps'],
                     )
 
                 if group['weight_decay'] > 0.0:
                     p.mul_(1.0 - group['lr'] * group['weight_decay'] * wd_ratio)
 
-                step_size: float = group['lr'] if group['adamd_debias_term'] else group['lr'] / bias_correction1
+                step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
                 p.add_(perturb, alpha=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adan.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,58 +4,66 @@
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 from pytorch_optimizer.optimizer.gc import centralize_gradient
+from pytorch_optimizer.optimizer.utils import get_global_gradient_norm
 
 
 class Adan(Optimizer, BaseOptimizer):
     r"""Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. decoupled weight decay.
     :param max_grad_norm: float. max gradient norm to clip.
     :param use_gc: bool. use gradient centralization.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.98, 0.92, 0.99),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
         max_grad_norm: float = 0.0,
         use_gc: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
         eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
         self.max_grad_norm = max_grad_norm
         self.use_gc = use_gc
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'max_grad_norm': max_grad_norm,
+            'adanorm': adanorm,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
@@ -68,36 +76,29 @@
     def reset(self):
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['exp_avg'] = torch.zeros_like(p)
+                state['exp_avg_sq'] = torch.zeros_like(p)
                 state['exp_avg_diff'] = torch.zeros_like(p)
-                state['exp_avg_nest'] = torch.zeros_like(p)
                 state['previous_grad'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def get_global_gradient_norm(self) -> Union[torch.Tensor, float]:
         if self.defaults['max_grad_norm'] == 0.0:
             return 1.0
 
-        device = self.param_groups[0]['params'][0].device
-
-        global_grad_norm = torch.zeros(1, device=device)
-        max_grad_norm = torch.tensor(self.defaults['max_grad_norm'], device=device)
+        global_grad_norm = get_global_gradient_norm(self.param_groups, self.param_groups[0]['params'][0].device)
+        global_grad_norm.sqrt_().add_(self.eps)
 
-        for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is not None:
-                    global_grad_norm.add_(torch.linalg.norm(p.grad).pow(2))
-
-        global_grad_norm = torch.sqrt(global_grad_norm)
-
-        return torch.clamp(max_grad_norm / (global_grad_norm + self.eps), max=1.0)
+        return torch.clamp(self.defaults['max_grad_norm'] / global_grad_norm, max=1.0)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -122,39 +123,54 @@
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
+                    state['exp_avg_sq'] = torch.zeros_like(p)
                     state['exp_avg_diff'] = torch.zeros_like(p)
-                    state['exp_avg_nest'] = torch.zeros_like(p)
-                    state['previous_grad'] = grad.clone()
-
-                exp_avg, exp_avg_diff, exp_avg_nest = state['exp_avg'], state['exp_avg_diff'], state['exp_avg_nest']
+                    state['previous_grad'] = grad.clone().mul_(-clip_global_grad_norm)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 grad.mul_(clip_global_grad_norm)
 
                 if self.use_gc:
                     grad = centralize_gradient(grad, gc_conv_only=False)
 
-                grad_diff = -state['previous_grad']
+                grad_diff = state['previous_grad']
                 grad_diff.add_(grad)
-                state['previous_grad'].copy_(grad)
 
-                update = grad + beta2 * grad_diff
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
 
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
+
+                exp_avg, exp_avg_sq, exp_avg_diff = state['exp_avg'], state['exp_avg_sq'], state['exp_avg_diff']
+
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_diff.mul_(beta2).add_(grad_diff, alpha=1.0 - beta2)
-                exp_avg_nest.mul_(beta3).addcmul_(update, update, value=1.0 - beta3)
 
-                de_nom = (exp_avg_nest.sqrt_() / bias_correction3_sq).add_(self.eps)
-                perturb = (exp_avg / bias_correction1 + beta2 * exp_avg_diff / bias_correction2).div_(de_nom)
+                grad_diff.mul_(beta2).add_(grad)
+                exp_avg_sq.mul_(beta3).addcmul_(grad_diff, grad_diff, value=1.0 - beta3)
+
+                de_nom = exp_avg_sq.sqrt()
+                de_nom.div_(bias_correction3_sq).add_(group['eps'])
 
                 if group['weight_decouple']:
                     p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    p.add_(perturb, alpha=-group['lr'])
-                else:
-                    p.add_(perturb, alpha=-group['lr'])
+
+                p.addcdiv_(exp_avg, de_nom, value=-group['lr'] / bias_correction1)
+                p.addcdiv_(exp_avg_diff, de_nom, value=-group['lr'] * beta2 / bias_correction2)
+
+                if not group['weight_decouple']:
                     p.div_(1.0 + group['lr'] * group['weight_decay'])
 
+                state['previous_grad'].copy_(-grad)
+
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabound.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,132 +1,150 @@
 import math
+from typing import List
 
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class AdaPNM(Optimizer, BaseOptimizer):
-    r"""Adam + Positive-Negative Momentum Optimizers.
+class AdaBound(Optimizer, BaseOptimizer):
+    r"""Adaptive Gradient Methods with Dynamic Bound of Learning Rate.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
+    :param final_lr: float. final learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
+    :param gamma: float. convergence speed of the bound functions.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param weight_decouple: bool. use weight_decouple.
-    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
+    :param amsbound: bool. whether to use the AMSBound variant.
+    :param adam_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.999, 1.0),
+        final_lr: float = 1e-1,
+        betas: BETAS = (0.9, 0.999),
+        gamma: float = 1e-3,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
-        amsgrad: bool = True,
-        adamd_debias_term: bool = False,
+        fixed_decay: bool = False,
+        amsbound: bool = False,
+        adam_debias: bool = False,
         eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
-        self.amsgrad = amsgrad
-        self.adamd_debias_term = adamd_debias_term
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
+            'final_lr': final_lr,
+            'gamma': gamma,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'amsgrad': amsgrad,
-            'adamd_debias_term': adamd_debias_term,
+            'fixed_decay': fixed_decay,
+            'amsbound': amsbound,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
+        self.base_lrs: List[float] = [group['lr'] for group in self.param_groups]
+
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'AdaPNM'
+        return 'AdaBound'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
                 state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                state['neg_exp_avg'] = torch.zeros_like(p)
-                if group['amsgrad']:
+                if group['amsbound']:
                     state['max_exp_avg_sq'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        for group in self.param_groups:
-            beta1, beta2, beta3 = group['betas']
-            noise_norm = math.sqrt((1 + beta3) ** 2 + beta3 ** 2)  # fmt: skip
+        for group, base_lr in zip(self.param_groups, self.base_lrs):
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
+            beta1, beta2 = group['betas']
+
+            bias_correction1 = 1.0 - beta1 ** group['step']
+            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+
+            final_lr = group['final_lr'] * group['lr'] / base_lr
+            lower_bound = final_lr * (1 - 1 / (group['gamma'] * group['step'] + 1))
+            upper_bound = final_lr * (1 + 1 / (group['gamma'] * group['step']))
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if group['weight_decouple']:
-                    p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                else:
-                    grad.add_(p, alpha=group['weight_decay'])
-
                 state = self.state[p]
+
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['neg_exp_avg'] = torch.zeros_like(p)
-                    if group['amsgrad']:
+                    if group['amsbound']:
                         state['max_exp_avg_sq'] = torch.zeros_like(p)
 
-                state['step'] += 1
+                if group['weight_decouple']:
+                    p.mul_(1.0 - group['weight_decay'] * (1.0 if group['fixed_decay'] else group['lr']))
+                elif group['weight_decay'] > 0.0:
+                    grad.add_(p, alpha=group['weight_decay'])
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                bias_correction1 = 1 - beta1 ** state['step']
-                bias_correction2_sq = math.sqrt(1 - beta2 ** state['step'])
+                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                exp_avg_sq = state['exp_avg_sq']
-                if state['step'] % 2 == 1:
-                    exp_avg, neg_exp_avg = state['exp_avg'], state['neg_exp_avg']
+                if group['amsbound']:
+                    max_exp_avg_sq = state['max_exp_avg_sq']
+                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
+                    de_nom = max_exp_avg_sq.add(group['eps']).sqrt()
                 else:
-                    exp_avg, neg_exp_avg = state['neg_exp_avg'], state['exp_avg']
+                    de_nom = exp_avg_sq.add(group['eps']).sqrt()
 
-                exp_avg.mul_(beta1 ** 2).add_(grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
-                if group['amsgrad']:
-                    torch.max(state['max_exp_avg_sq'], exp_avg_sq, out=exp_avg_sq)
+                step_size = group['lr'] * bias_correction2_sq
+                if not group['adam_debias']:
+                    step_size /= bias_correction1
 
-                de_nom = (exp_avg_sq.sqrt() / bias_correction2_sq).add_(group['eps'])
+                step_size = torch.full_like(de_nom, step_size)
+                step_size.div_(de_nom).clamp_(lower_bound, upper_bound).mul_(exp_avg)
 
-                step_size: float = group['lr'] if group['adamd_debias_term'] else group['lr'] / bias_correction1
-                pn_momentum = exp_avg.mul(1.0 + beta3).add(neg_exp_avg, alpha=-beta3).mul(1.0 / noise_norm)
-                p.addcdiv_(pn_momentum, de_nom, value=-step_size)
+                p.add_(-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/agc.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/alig.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoClosureError, NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.utils import get_global_gradient_norm
 
 
 class AliG(Optimizer, BaseOptimizer):
     r"""Adaptive Learning Rates for Interpolation with Gradients.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param max_lr: Optional[float]. max learning rate.
@@ -27,20 +28,19 @@
         momentum: float = 0.0,
         adjusted_momentum: bool = False,
         eps: float = 1e-5,
     ):
         self.max_lr = max_lr
         self.projection_fn = projection_fn
         self.momentum = momentum
-        self.adjusted_momentum = adjusted_momentum
         self.eps = eps
 
         self.validate_parameters()
 
-        defaults: DEFAULTS = {'max_lr': max_lr, 'momentum': momentum}
+        defaults: DEFAULTS = {'max_lr': max_lr, 'adjusted_momentum': adjusted_momentum, 'momentum': momentum}
         super().__init__(params, defaults)
 
         if self.projection_fn is not None:
             self.projection_fn()
 
     def validate_parameters(self):
         self.validate_momentum(self.momentum)
@@ -51,27 +51,24 @@
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
-                state['momentum_buffer'] = torch.zeros_like(p)
+                if group['momentum'] > 0.0:
+                    state['momentum_buffer'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def compute_step_size(self, loss: float) -> float:
         r"""Compute step_size."""
-        global_grad_norm: float = 0
-
-        for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is not None:
-                    global_grad_norm += p.grad.norm().pow(2).item()
+        global_grad_norm = get_global_gradient_norm(self.param_groups, torch.device('cpu'))
+        global_grad_norm.add_(self.eps)
 
-        return loss / (global_grad_norm + self.eps)
+        return loss / global_grad_norm.item()
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         if closure is None:
             raise NoClosureError('AliG', '(e.g. `optimizer.step(lambda: float(loss))`).')
 
         loss = closure()
@@ -97,15 +94,15 @@
                     state['momentum_buffer'] = torch.zeros_like(p)
 
                 p.add_(grad, alpha=-step_size)
 
                 if momentum > 0.0:
                     buffer = state['momentum_buffer']
 
-                    if self.adjusted_momentum:
+                    if group['adjusted_momentum']:
                         buffer.mul_(momentum).sub_(grad)
                         p.add_(buffer, alpha=step_size * momentum)
                     else:
                         buffer.mul_(momentum).add_(grad, alpha=-step_size)
                         p.add_(buffer, alpha=momentum)
 
             if self.projection_fn is not None:
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/radam.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,156 +1,162 @@
-from typing import Optional
+import math
 
-import numpy as np
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
-from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class Apollo(Optimizer, BaseOptimizer):
-    r"""An Adaptive Parameter-wise Diagonal Quasi-Newton Method for Nonconvex Stochastic Optimization.
+class RAdam(Optimizer, BaseOptimizer):
+    r"""Rectified Adam.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
-    :param init_lr: Optional[float]. initial learning rate (default lr / 1000).
-    :param beta: float. coefficient used for computing running averages of gradient.
-    :param rebound: str. rectified bound for diagonal hessian. (constant, belief).
+    :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param weight_decay_type: str. type of weight decay. (l2, decoupled, stable).
-    :param warmup_steps: int. number of warmup steps.
+    :param n_sma_threshold: int. (recommended is 5).
+    :param degenerated_to_sgd: float. degenerated to SGD.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        init_lr: Optional[float] = None,
-        beta: float = 0.9,
-        rebound: str = 'constant',
+        betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
-        weight_decay_type: str = 'l2',
-        warmup_steps: int = 500,
-        eps: float = 1e-4,
+        n_sma_threshold: int = 5,
+        degenerated_to_sgd: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
+        eps: float = 1e-8,
     ):
         self.lr = lr
-        self.beta = beta
-        self.rebound = rebound
+        self.betas = betas
         self.weight_decay = weight_decay
-        self.weight_decay_type = weight_decay_type
-        self.warmup_steps = warmup_steps
+        self.n_sma_threshold = n_sma_threshold
+        self.degenerated_to_sgd = degenerated_to_sgd
         self.eps = eps
 
         self.validate_parameters()
 
-        self.init_lr: float = init_lr if init_lr is not None else lr / 1000.0
-
         defaults: DEFAULTS = {
             'lr': lr,
-            'init_lr': self.init_lr,
-            'beta': beta,
+            'betas': betas,
             'weight_decay': weight_decay,
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
-        self.validate_beta(self.beta)
-        self.validate_rebound(self.rebound)
+        self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
-        self.validate_weight_decay_type(self.weight_decay_type)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'Apollo'
+        return 'RAdam'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
-            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['step'] = 0
-                state['exp_avg_grad'] = torch.zeros_like(p)
-                state['approx_hessian'] = torch.zeros_like(p)
-                state['update'] = torch.zeros_like(p)
+                state['exp_avg'] = torch.zeros_like(p)
+                state['exp_avg_sq'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
-            current_lr: float = (
-                group['lr']
-                if group['step'] >= self.warmup_steps
-                else (self.lr - group['init_lr']) * group['step'] / self.warmup_steps + group['init_lr']
-            )
+            beta1, beta2 = group['betas']
 
-            weight_decay, eps = group['weight_decay'], group['eps']
+            bias_correction1 = 1.0 - beta1 ** group['step']
 
-            bias_correction: float = 1.0 - group['beta'] ** group['step']
-            alpha: float = (1.0 - group['beta']) / bias_correction
+            n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
+            beta2_t: float = beta2 ** group['step']
+            n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
+
                 if len(state) == 0:
-                    state['exp_avg_grad'] = torch.zeros_like(p)
-                    state['approx_hessian'] = torch.zeros_like(p)
-                    state['update'] = torch.zeros_like(p)
-
-                exp_avg_grad, b, d_p = state['exp_avg_grad'], state['approx_hessian'], state['update']
-
-                if weight_decay > 0.0 and self.weight_decay_type == 'l2':
-                    grad.add_(p, alpha=weight_decay)
-
-                delta_grad = grad - exp_avg_grad
-                if self.rebound == 'belief':
-                    rebound = delta_grad.norm(p=np.inf)
+                    state['step'] = 0
+                    state['exp_avg'] = torch.zeros_like(p)
+                    state['exp_avg_sq'] = torch.zeros_like(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
+
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
+
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+
+                if n_sma >= self.n_sma_threshold:
+                    step_size = math.sqrt(
+                        (1 - beta2_t)
+                        * (n_sma - 4)
+                        / (n_sma_max - 4)
+                        * (n_sma - 2)
+                        / n_sma
+                        * n_sma_max
+                        / (n_sma_max - 2)
+                    )
+                elif self.degenerated_to_sgd:
+                    step_size = 1.0
                 else:
-                    rebound = 1e-2
-                    eps /= rebound
-
-                exp_avg_grad.add_(delta_grad, alpha=alpha)
-
-                de_nom = d_p.norm(p=4).add(eps)
-                d_p.div_(de_nom)
-
-                v_sq = d_p.mul(d_p)
-                delta = delta_grad.div_(de_nom).mul_(d_p).sum().mul(-alpha) - b.mul(v_sq).sum()
-
-                b.addcmul_(v_sq, delta)
-
-                de_nom = b.abs().clamp_(min=rebound)
-                if self.rebound == 'belief':
-                    de_nom.add_(eps / alpha)
-
-                d_p.copy_(exp_avg_grad.div(de_nom))
+                    step_size = -1
 
-                if weight_decay > 0.0 and self.weight_decay_type != 'l2':
-                    if self.weight_decay_type == 'stable':
-                        weight_decay /= de_nom.mean().item()
+                if not group['adam_debias']:
+                    step_size /= bias_correction1
 
-                    d_p.add_(p, alpha=weight_decay)
+                if group['weight_decay'] > 0.0 and (n_sma >= self.n_sma_threshold or step_size > 0):
+                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
 
-                p.add_(d_p, alpha=-current_lr)
+                if n_sma >= self.n_sma_threshold:
+                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                    p.addcdiv_(exp_avg, de_nom, value=-step_size * group['lr'])
+                elif step_size > 0:
+                    p.add_(exp_avg, alpha=-step_size * group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/dadapt.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,17 +47,14 @@
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
             'd': d0,
             'growth_rate': growth_rate,
             'weight_decay': weight_decay,
-            'gsq_weighted': 0.0,
-            'sk_sq_weighted': 0.0,
-            'sk_l1': 0.0,
             'k': 0,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
@@ -88,26 +85,32 @@
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         group = self.param_groups[0]
 
-        lr, momentum = group['lr'], group['momentum']
-
-        growth_rate = group['growth_rate']
-        gsq_weighted, sk_sq_weighted = group['gsq_weighted'], group['sk_sq_weighted']
-        sk_l1 = group['sk_l1']
+        lr, momentum, growth_rate = group['lr'], group['momentum'], group['growth_rate']
 
         d = group['d']
         d_lr = float(d * lr)
 
         g_sq = torch.tensor([0.0], device=group['params'][0].device)
         sk_sq_weighted_change = torch.tensor([0.0], device=group['params'][0].device)
         sk_l1_change = torch.tensor([0.0], device=group['params'][0].device)
+        if 'gsq_weighted' not in group:
+            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+        if 'sk_sq_weighted' not in group:
+            group['sk_sq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+        if 'sk_l1' not in group:
+            group['sk_l1'] = torch.tensor([0.0], device=group['params'][0].device)
+
+        gsq_weighted = group['gsq_weighted']
+        sk_sq_weighted = group['sk_sq_weighted']
+        sk_l1 = group['sk_l1']
 
         for group in self.param_groups:
             weight_decay, eps = group['weight_decay'], group['eps']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
@@ -178,17 +181,20 @@
 
                     sk_sq_weighted_param = sk.pow(2).div(torch.sqrt(alpha_k) + eps).sum()
                     sk_l1_param = sk.abs().sum()
 
                     sk_sq_weighted_change.add_(sk_sq_weighted_param - old_sk_sq_weighted_param)
                     sk_l1_change.add_(sk_l1_param - old_sk_l1_param)
 
-        sk_sq_weighted += sk_sq_weighted_change
-        gsq_weighted += d_lr * d_lr * g_sq
-        sk_l1 += sk_l1_change
+        sk_sq_weighted.add_(sk_sq_weighted_change)
+        gsq_weighted.add_(g_sq, alpha=d_lr ** 2)  # fmt: skip
+        sk_l1.add_(sk_l1_change)
+
+        if sk_l1 == 0:
+            return loss
 
         if lr > 0.0:
             d_hat = (sk_sq_weighted - gsq_weighted) / sk_l1
             d = self.d0 = max(d, min(d_hat, d * growth_rate))
 
         for group in self.param_groups:
             group['gsq_weighted'] = gsq_weighted
@@ -271,15 +277,14 @@
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'd': d0,
             'growth_rate': growth_rate,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
-            'gsq_weighted': 0.0,
             'k': 0,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
@@ -310,22 +315,25 @@
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         group = self.param_groups[0]
 
         beta1, beta2 = group['betas']
-        gsq_weighted, growth_rate = group['gsq_weighted'], group['growth_rate']
+        growth_rate = group['growth_rate']
 
         d, lr = group['d'], group['lr']
         d_lr = float(d * lr)
 
         g_sq = torch.tensor([0.0], device=group['params'][0].device)
         sk_sq_weighted = torch.tensor([0.0], device=group['params'][0].device)
         sk_l1 = torch.tensor([0.0], device=group['params'][0].device)
+        if 'gsq_weighted' not in group:
+            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+        gsq_weighted = group['gsq_weighted']
 
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
@@ -352,15 +360,19 @@
 
                 s = state['s']
                 s.mul_(beta2).add_(grad, alpha=d_lr * (1.0 - beta2))
 
                 sk_sq_weighted.add_(to_real(s * s.conj()).div_(de_nom).sum())
                 sk_l1.add_(s.abs().sum())
 
-        gsq_weighted = beta2 * gsq_weighted + g_sq * (d_lr**2) * (1 - beta2)
+        if sk_l1 == 0:
+            return loss
+
+        gsq_weighted.mul_(beta2).add_(g_sq, alpha=(d_lr ** 2) * (1.0 - beta2))  # fmt: skip
+
         if lr > 0.0:
             d_hat = (sk_sq_weighted / (1.0 - beta2) - gsq_weighted) / sk_l1
             d = max(d, min(d_hat, d * growth_rate))
 
         for group in self.param_groups:
             group['gsq_weighted'] = gsq_weighted
             group['d'] = d
@@ -416,15 +428,14 @@
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
             'd': d0,
             'growth_rate': growth_rate,
             'weight_decay': weight_decay,
-            'gsq_weighted': 0.0,
             'k': 0,
         }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_momentum(self.momentum)
@@ -452,18 +463,21 @@
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         group = self.param_groups[0]
 
-        gsq_weighted, growth_rate = group['gsq_weighted'], group['growth_rate']
+        growth_rate = group['growth_rate']
 
         g_sq = torch.tensor([0.0], device=group['params'][0].device)
         sk_sq = torch.tensor([0.0], device=group['params'][0].device)
+        if 'gsq_weighted' not in group:
+            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+        gsq_weighted = group['gsq_weighted']
 
         for group in self.param_groups:
             weight_decay = group['weight_decay']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
@@ -478,21 +492,22 @@
                 if 'z' not in state:
                     state['z'] = torch.clone(p)
                     state['s'] = torch.zeros_like(p)
                     state['x0'] = torch.clone(p)
 
                 g_sq.add_(grad.pow(2).sum())
 
+        if g_sq == 0:
+            return loss
+
         group = self.param_groups[0]
+
         if group['k'] == 0:
             group['g0_norm'] = g_sq.sqrt().item()
-
         g0_norm = group['g0_norm']
-        if g0_norm == 0:
-            g0_norm = 1.0
 
         d, lr = group['d'], group['lr']
         d_lr = float(d * lr) / g0_norm
 
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
@@ -501,36 +516,206 @@
                 state = self.state[p]
 
                 s = state['s']
                 s.add_(p.grad, alpha=d_lr)
 
                 sk_sq.add_(s.pow(2).sum())
 
-        group['gsq_weighted'] = gsq_weighted + d_lr * d_lr * g_sq
-        gsq_weighted = group['gsq_weighted']
+        gsq_weighted.add_(g_sq, alpha=d_lr ** 2)  # fmt: skip
 
         if lr > 0.0:
-            d_hat = (sk_sq - group['gsq_weighted']) / sk_sq.sqrt()
+            d_hat = (sk_sq - gsq_weighted) / sk_sq.sqrt()
             d = max(d, min(d_hat, d * growth_rate))
-            group['d'] = d
 
         for group in self.param_groups:
             group['gsq_weighted'] = gsq_weighted
             group['d'] = d
             group['g0_norm'] = g0_norm
 
-            momentum = group['momentum']
-
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 state = self.state[p]
 
                 z = state['z']
                 z.copy_(state['x0'] - state['s'])
 
-                p.mul_(momentum).add_(z, alpha=1.0 - momentum)
+                p.mul_(group['momentum']).add_(z, alpha=1.0 - group['momentum'])
+
+            group['k'] += 1
+
+        return loss
+
+
+class DAdaptAdan(Optimizer, BaseOptimizer):
+    r"""Adan with D-Adaptation. Leave LR set to 1 unless you encounter instability.
+
+    :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
+    :param lr: float. learning rate.
+    :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
+    :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. decoupled weight decay.
+    :param d0: float. initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
+    :param growth_rate: float. prevent the D estimate from growing faster than this multiplicative rate.
+        Default is inf, for unrestricted.
+    :param eps: float. term added to the denominator to improve numerical stability.
+    """
+
+    def __init__(
+        self,
+        params: PARAMETERS,
+        lr: float = 1.0,
+        betas: BETAS = (0.98, 0.92, 0.99),
+        weight_decay: float = 0.0,
+        weight_decouple: bool = False,
+        d0: float = 1e-6,
+        growth_rate: float = float('inf'),
+        eps: float = 1e-8,
+    ):
+        self.lr = lr
+        self.betas = betas
+        self.weight_decay = weight_decay
+        self.d0 = d0
+        self.growth_rate = growth_rate
+        self.eps = eps
+
+        self.validate_parameters()
+
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'betas': betas,
+            'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'd': d0,
+            'growth_rate': growth_rate,
+            'k': 0,
+            'eps': eps,
+        }
+        super().__init__(params, defaults)
+
+    def validate_parameters(self):
+        self.validate_learning_rate(self.lr)
+        self.validate_betas(self.betas)
+        self.validate_weight_decay(self.weight_decay)
+        self.validate_epsilon(self.eps)
+
+    def __str__(self) -> str:
+        return 'DAdaptAdan'
+
+    @torch.no_grad()
+    def reset(self):
+        for group in self.param_groups:
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                state = self.state[p]
+
+                state['step'] = 0
+                state['s'] = torch.zeros_like(p)
+                state['exp_avg'] = torch.zeros_like(p)
+                state['exp_avg_sq'] = torch.zeros_like(p)
+                state['exp_avg_diff'] = torch.zeros_like(p)
+
+    @torch.no_grad()
+    def step(self, closure: CLOSURE = None) -> LOSS:
+        loss: LOSS = None
+        if closure is not None:
+            with torch.enable_grad():
+                loss = closure()
+
+        group = self.param_groups[0]
+
+        beta1, beta2, beta3 = group['betas']
+        growth_rate = group['growth_rate']
+
+        d, lr = group['d'], group['lr']
+        d_lr = float(d * lr)
+
+        g_sq = torch.tensor([0.0], device=group['params'][0].device)
+        sk_sq_weighted = torch.tensor([0.0], device=group['params'][0].device)
+        sk_l1 = torch.tensor([0.0], device=group['params'][0].device)
+        if 'gsq_weighted' not in group:
+            group['gsq_weighted'] = torch.tensor([0.0], device=group['params'][0].device)
+        gsq_weighted = group['gsq_weighted']
+
+        for group in self.param_groups:
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                grad = p.grad
+                if grad.is_sparse:
+                    raise NoSparseGradientError(str(self))
+
+                state = self.state[p]
+                if 'step' not in state:
+                    state['step'] = 0
+
+                    state['s'] = torch.zeros_like(p)
+                    state['exp_avg'] = torch.zeros_like(p)
+                    state['exp_avg_sq'] = torch.zeros_like(p)
+                    state['exp_avg_diff'] = torch.zeros_like(p)
+                    state['previous_grad'] = -grad.clone()
+
+                grad_diff = state['previous_grad']
+                grad_diff.add_(grad)
+
+                exp_avg, exp_avg_sq, exp_avg_diff = state['exp_avg'], state['exp_avg_sq'], state['exp_avg_diff']
+
+                exp_avg.mul_(beta1).add_(grad, alpha=d_lr * (1.0 - beta1))
+                exp_avg_diff.mul_(beta2).add_(grad_diff, alpha=d_lr * (1.0 - beta2))
+
+                grad_diff.mul_(beta2).add_(grad)
+                grad_diff = to_real(grad_diff * grad_diff.conj())
+                exp_avg_sq.mul_(beta3).addcmul_(grad_diff, grad_diff, value=1.0 - beta3)
+
+                grad_power = to_real(grad * grad.conj())
+                de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+
+                g_sq.add_(grad_power.div_(de_nom).sum())
+
+                s = state['s']
+                s.mul_(beta3).add_(grad, alpha=d_lr * (1.0 - beta3))
+
+                sk_sq_weighted.add_(to_real(s * s.conj()).div_(de_nom).sum())
+                sk_l1.add_(s.abs().sum())
+
+                state['previous_grad'].copy_(-grad)
+
+        if sk_l1 == 0:
+            return loss
+
+        gsq_weighted.mul_(beta3).add_(g_sq, alpha=(d_lr ** 2) * (1.0 - beta3))  # fmt: skip
+
+        if lr > 0.0:
+            d_hat = (sk_sq_weighted / (1.0 - beta3) - gsq_weighted) / sk_l1
+            d = max(d, min(d_hat, d * growth_rate))
+
+        for group in self.param_groups:
+            group['gsq_weighted'] = gsq_weighted
+            group['d'] = d
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                state = self.state[p]
+
+                state['step'] += 1
+
+                exp_avg, exp_avg_sq, exp_avg_diff = state['exp_avg'], state['exp_avg_sq'], state['exp_avg_diff']
+
+                de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+
+                if group['weight_decouple']:
+                    p.mul_(1.0 - d_lr * group['weight_decay'])
+
+                p.addcdiv_(exp_avg, de_nom, value=-1.0)
+                p.addcdiv_(exp_avg_diff, de_nom, value=-beta2)
+
+                if not group['weight_decouple']:
+                    p.div_(1.0 + d_lr * group['weight_decay'])
 
             group['k'] += 1
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/novograd.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,115 +4,125 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class DiffGrad(Optimizer, BaseOptimizer):
-    r"""An Optimization Method for Convolutional Neural Networks.
+class NovoGrad(Optimizer, BaseOptimizer):
+    r"""Stochastic Gradient Methods with Layer-wise Adaptive Moments for Training of Deep Networks.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-    :param eps: float. term added to the denominator to improve numerical stability.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param grad_averaging: bool. multiply ck (1 - momentum).
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.999),
-        eps: float = 1e-8,
+        betas: BETAS = (0.95, 0.98),
         weight_decay: float = 0.0,
-        adamd_debias_term: bool = False,
+        grad_averaging: bool = False,
+        adam_debias: bool = False,
+        eps: float = 1e-8,
     ):
         self.lr = lr
-        self.eps = eps
         self.betas = betas
         self.weight_decay = weight_decay
+        self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
-            'adamd_debias_term': adamd_debias_term,
+            'grad_averaging': grad_averaging,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'diffGrad'
+        return 'NovoGrad'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
+                grad = p.grad
+                g_2 = grad ** 2  # fmt: skip
+
                 state['step'] = 0
-                state['exp_avg'] = torch.zeros_like(p)
-                state['exp_avg_sq'] = torch.zeros_like(p)
-                state['previous_grad'] = torch.zeros_like(p)
+                state['moments'] = grad.div(g_2.sqrt() + group['eps']) + group['weight_decay'] * p
+                state['grads_ema'] = g_2
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
+            weight_decay = group['weight_decay']
+
+            bias_correction1 = 1.0 - beta1 ** group['step']
+            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])
+
+            step_size: float = group['lr'] * bias_correction2_sq
+            if not group['adam_debias']:
+                step_size /= bias_correction1
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
-                if len(state) == 0:
-                    state['step'] = 0
-                    state['exp_avg'] = torch.zeros_like(p)
-                    state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['previous_grad'] = torch.zeros_like(p)
+                g_2 = grad ** 2  # fmt: skip
 
-                state['step'] += 1
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                if len(state) == 0:
+                    state['moments'] = grad.div(g_2.sqrt() + group['eps']) + weight_decay * p
+                    state['grads_ema'] = g_2
 
-                if group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                moments, grads_ema = state['moments'], state['grads_ema']
 
-                # Decay the first and second moment running average coefficient
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+                grads_ema.mul_(beta2).add_(g_2, alpha=1.0 - beta2)
 
-                de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                de_nom = grads_ema.sqrt().add_(group['eps'])
+                grad.div_(de_nom)
 
-                bias_correction1 = 1.0 - beta1 ** state['step']
-                bias_correction2_sq = math.sqrt(1.0 - beta2 ** state['step'])
+                if weight_decay > 0.0:
+                    grad.add_(p, alpha=weight_decay)
 
-                # compute diffGrad coefficient (dfc)
-                dfc = state['previous_grad'].clone()
-                dfc.sub_(grad).abs_().sigmoid_().mul_(exp_avg)
-                state['previous_grad'].copy_(grad)
+                if group['grad_averaging']:
+                    grad.mul_(1.0 - beta1)
 
-                step_size = group['lr'] * bias_correction2_sq
-                if not group['adamd_debias_term']:
-                    step_size /= bias_correction1
+                moments.mul_(beta1).add_(grad)
 
-                # update momentum with dfc
-                p.addcdiv_(dfc, de_nom, value=-step_size)
+                p.add_(moments, alpha=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/diffrgrad.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adams.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,149 +1,170 @@
 import math
 
 import torch
 from torch.optim.optimizer import Optimizer
 
-from pytorch_optimizer.base.exception import NoSparseGradientError
+from pytorch_optimizer.base.exception import NoSparseGradientError, ZeroParameterSizeError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class DiffRGrad(Optimizer, BaseOptimizer):
-    r"""RAdam + DiffGrad.
+class AdamS(Optimizer, BaseOptimizer):
+    r"""Adam with stable weight decay.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param n_sma_threshold: int. (recommended is 5).
-    :param degenerated_to_sgd: bool. degenerated to SGD.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
-        weight_decay: float = 0.0,
-        n_sma_threshold: int = 5,
-        degenerated_to_sgd: bool = True,
-        adamd_debias_term: bool = False,
+        weight_decay: float = 1e-4,
+        amsgrad: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
         eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.n_sma_threshold = n_sma_threshold
-        self.degenerated_to_sgd = degenerated_to_sgd
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
-            'adamd_debias_term': adamd_debias_term,
-            'buffer': [[None, None, None] for _ in range(10)],
+            'amsgrad': amsgrad,
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'diffRGrad'
+        return 'AdamS'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
                 state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-                state['previous_grad'] = torch.zeros_like(p)
+                if group['amsgrad']:
+                    state['max_exp_avg_sq'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
+        param_size: int = 0
+        exp_avg_sq_hat_sum: float = 0.0
+
         for group in self.param_groups:
             beta1, beta2 = group['betas']
-            n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
+                param_size += p.numel()
+
                 state = self.state[p]
+
                 if len(state) == 0:
                     state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
-                    state['previous_grad'] = torch.zeros_like(p)
+                    if group['amsgrad']:
+                        state['max_exp_avg_sq'] = torch.zeros_like(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
                 state['step'] += 1
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                bias_correction1 = 1.0 - beta1 ** state['step']
+                bias_correction2 = 1.0 - beta2 ** state['step']
+
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
 
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
+
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
+
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                # compute diffGrad coefficient (dfc)
-                dfc = state['previous_grad'].clone()
-                dfc.sub_(grad).abs_().sigmoid_().mul_(exp_avg)
-                state['previous_grad'].copy_(grad)
-
-                buffered = group['buffer'][state['step'] % 10]
-                if state['step'] == buffered[0]:
-                    n_sma, step_size = buffered[1], buffered[2]
+                if group['amsgrad']:
+                    max_exp_avg_sq = state['max_exp_avg_sq']
+                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
+                    exp_avg_sq_hat = max_exp_avg_sq
                 else:
-                    buffered[0] = state['step']
-                    beta2_t = beta2 ** state['step']
-                    n_sma = n_sma_max - 2.0 * state['step'] * beta2_t / (1.0 - beta2_t)
-                    buffered[1] = n_sma
-
-                    if n_sma >= self.n_sma_threshold:
-                        step_size = math.sqrt(
-                            (1 - beta2_t)
-                            * (n_sma - 4)
-                            / (n_sma_max - 4)
-                            * (n_sma - 2)
-                            / n_sma
-                            * n_sma_max
-                            / (n_sma_max - 2)
-                        )
-                        if not group['adamd_debias_term']:
-                            step_size /= bias_correction1
-                    elif self.degenerated_to_sgd:
-                        step_size = 1.0 / bias_correction1
-                    else:
-                        step_size = -1
+                    exp_avg_sq_hat = exp_avg_sq
+
+                exp_avg_sq_hat_sum += exp_avg_sq_hat.sum() / bias_correction2
+
+        if param_size == 0:
+            raise ZeroParameterSizeError()
+
+        exp_avg_sq_hat_mean = math.sqrt(exp_avg_sq_hat_sum / param_size) + self.eps
+
+        for group in self.param_groups:
+            beta1, beta2 = group['betas']
+            for p in group['params']:
+                if p.grad is None:
+                    continue
 
-                    buffered[2] = step_size
+                state = self.state[p]
 
                 if group['weight_decay'] > 0.0:
-                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
+                    p.mul_(1.0 - group['lr'] * group['weight_decay'] / exp_avg_sq_hat_mean)
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+
+                bias_correction1 = 1.0 - beta1 ** state['step']
+                bias_correction2 = 1.0 - beta2 ** state['step']
+
+                exp_avg_sq_hat = state['max_exp_avg_sq'] if group['amsgrad'] else exp_avg_sq
+                exp_avg_sq_hat.div_(bias_correction2)
+
+                de_nom = exp_avg_sq_hat.sqrt().add(group['eps'])
 
-                if n_sma >= self.n_sma_threshold:
-                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                    p.addcdiv_(dfc, de_nom, value=-step_size * group['lr'])
-                elif step_size > 0:
-                    p.add_(exp_avg, alpha=-step_size * group['lr'])
+                step_size = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
+                p.addcdiv_(exp_avg, de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/gsam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adapnm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,160 @@
-from typing import Union
+import math
 
 import torch
-from torch.optim import Optimizer
+from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class Lamb(Optimizer, BaseOptimizer):
-    r"""Large Batch Optimization for Deep Learning.
-
-        This Lamb implementation is based on the paper v3, which does not use de-biasing.
+class AdaPNM(Optimizer, BaseOptimizer):
+    r"""Adam + Positive-Negative Momentum Optimizers.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param grad_averaging: bool. whether apply (1 - beta2) to gradient when calculating running averages of gradient.
-    :param max_grad_norm: float. max gradient norm to clip.
-    :param adam: bool. always use trust ratio = 1, which turns this into Adam. Useful for comparison purposes.
-    :param pre_norm: bool. perform pre-normalization of all gradients.
+    :param weight_decouple: bool. use weight_decouple.
+    :param amsgrad: bool. whether to use the AMSGrad variant of this algorithm from the paper.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
-    clamp: float = 10.0
-
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.999),
+        betas: BETAS = (0.9, 0.999, 1.0),
         weight_decay: float = 0.0,
-        grad_averaging: bool = True,
-        max_grad_norm: float = 1.0,
-        adam: bool = False,
-        pre_norm: bool = False,
-        eps: float = 1e-6,
+        weight_decouple: bool = True,
+        amsgrad: bool = True,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
+        eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.grad_averaging = grad_averaging
-        self.max_grad_norm = max_grad_norm
-        self.adam = adam
-        self.pre_norm = pre_norm
+        self.weight_decouple = weight_decouple
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
-            'grad_averaging': grad_averaging,
-            'max_grad_norm': max_grad_norm,
+            'weight_decouple': weight_decouple,
+            'amsgrad': amsgrad,
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
-        self.validate_norm(self.max_grad_norm)
 
     def __str__(self) -> str:
-        return 'Lamb'
+        return 'AdaPNM'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 state = self.state[p]
 
                 state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-
-    @torch.no_grad()
-    def get_global_gradient_norm(self) -> Union[torch.Tensor, float]:
-        if self.defaults['max_grad_norm'] == 0.0:
-            return 1.0
-
-        device = self.param_groups[0]['params'][0].device
-
-        global_grad_norm = torch.zeros(1, device=device)
-        max_grad_norm = torch.tensor(self.defaults['max_grad_norm'], device=device)
-
-        for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is not None:
-                    global_grad_norm.add_(torch.linalg.norm(p.grad).pow(2))
-
-        global_grad_norm = torch.sqrt(global_grad_norm)
-
-        return torch.clamp(max_grad_norm / (global_grad_norm + self.eps), max=1.0)
+                state['neg_exp_avg'] = torch.zeros_like(p)
+                if group['amsgrad']:
+                    state['max_exp_avg_sq'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        grad_norm = 1.0
-        if self.pre_norm:
-            grad_norm = self.get_global_gradient_norm()
-
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
-            beta1, beta2 = group['betas']
-            beta3 = 1.0 - beta1 if group['grad_averaging'] else 1.0
+            beta1, beta2, beta3 = group['betas']
+            noise_norm = math.sqrt((1 + beta3) ** 2 + beta3 ** 2)  # fmt: skip
+
+            bias_correction1 = 1 - beta1 ** group['step']
+            bias_correction2_sq = math.sqrt(1 - beta2 ** group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if self.pre_norm:
-                    grad.div_(grad_norm)
+                if group['weight_decouple']:
+                    p.mul_(1.0 - group['lr'] * group['weight_decay'])
+                else:
+                    grad.add_(p, alpha=group['weight_decay'])
 
                 state = self.state[p]
-
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
+                    state['neg_exp_avg'] = torch.zeros_like(p)
+                    if group['amsgrad']:
+                        state['max_exp_avg_sq'] = torch.zeros_like(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
+
+                if group['step'] % 2 == 1:
+                    exp_avg, neg_exp_avg = state['exp_avg'], state['neg_exp_avg']
+                else:
+                    exp_avg, neg_exp_avg = state['neg_exp_avg'], state['exp_avg']
+
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                exp_avg.mul_(beta1).add_(grad, alpha=beta3)
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
 
-                adam_step = exp_avg / exp_avg_sq.sqrt().add(group['eps'])
-                if group['weight_decay'] > 0.0:
-                    adam_step.add_(p, alpha=group['weight_decay'])
-
-                weight_norm = p.norm(2).clamp(0, self.clamp)
-                adam_norm = adam_step.norm(2)
-                trust_ratio: float = (
-                    1.0 if weight_norm == 0 or adam_norm == 0 else weight_norm / (adam_norm + self.eps)
-                )
-
-                state['weight_norm'] = weight_norm
-                state['adam_norm'] = adam_norm
-                state['trust_ratio'] = trust_ratio
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
 
-                if self.adam:
-                    trust_ratio = 1.0
+                exp_avg_sq = state['exp_avg_sq']
+                exp_avg.mul_(beta1 ** 2).add_(s_grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                p.add_(adam_step, alpha=-group['lr'] * trust_ratio)
+                if group['amsgrad']:
+                    max_exp_avg_sq = state['max_exp_avg_sq']
+                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
+                    exp_avg_sq_hat = max_exp_avg_sq.add_(group['eps'])
+                else:
+                    exp_avg_sq_hat = exp_avg_sq.add_(group['eps'])
+
+                de_nom = (exp_avg_sq_hat.sqrt() / bias_correction2_sq).add_(group['eps'])
+
+                step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
+                pn_momentum = exp_avg.mul(1.0 + beta3).add(neg_exp_avg, alpha=-beta3).mul(1.0 / noise_norm)
+                p.addcdiv_(pn_momentum, de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lars.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,33 +81,34 @@
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 if p.ndim > 1:  # if not normalization gamma/beta or bias
-                    param_norm = p.norm(2.0)
-                    update_norm = grad.norm(2.0)
-                    one = torch.ones_like(param_norm, device=param_norm.device)
+                    param_norm = torch.linalg.norm(p)
+                    update_norm = torch.linalg.norm(grad)
+
+                    one = torch.ones_like(param_norm)
 
                     trust_ratio = torch.where(
                         param_norm > 0.0,
                         torch.where(update_norm > 0.0, (group['trust_coefficient'] * param_norm / update_norm), one),
                         one,
                     )
 
                     grad.add_(p, alpha=group['weight_decay'])
                     grad.mul_(trust_ratio)
 
                 if group['momentum'] > 0.0:
-                    param_state = self.state[p]
-                    if 'momentum_buffer' not in param_state:
-                        param_state['momentum_buffer'] = grad.clone().detach()
+                    state = self.state[p]
+                    if 'momentum_buffer' not in state:
+                        state['momentum_buffer'] = grad.clone().detach()
 
-                    mb = param_state['momentum_buffer']
+                    mb = state['momentum_buffer']
                     mb.mul_(group['momentum']).add_(grad, alpha=1.0 - group['dampening'])
 
                     if group['nesterov']:
                         grad.add_(mb, alpha=group['momentum'])
                     else:
                         grad.copy_(mb)
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lion.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,23 @@
         betas: BETAS = (0.9, 0.99),
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
 
         self.validate_parameters()
 
-        defaults: DEFAULTS = {'lr': lr, 'betas': betas, 'weight_decay': weight_decay}
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'betas': betas,
+            'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+        }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
 
@@ -72,15 +76,15 @@
 
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
 
                 update = exp_avg = state['exp_avg']
 
                 if weight_decay > 0.0:
-                    if self.weight_decouple:
+                    if group['weight_decouple']:
                         p.mul_(1.0 - group['lr'] * weight_decay)
                     else:
                         grad.add_(p, alpha=weight_decay)
 
                 update.mul_(beta1).add_(grad, alpha=1.0 - beta1)
                 exp_avg.mul_(beta2).add_(grad, alpha=1.0 - beta2)
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/nero.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pnm.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
         eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.weight_decouple = weight_decouple
         self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
@@ -91,19 +90,17 @@
                     state['step'] = 0
                     state['pos_momentum'] = torch.zeros_like(p)
                     state['neg_momentum'] = torch.zeros_like(p)
 
                 state['step'] += 1
 
                 if state['step'] % 2 == 1:
-                    pos_momentum = state['pos_momentum']
-                    neg_momentum = state['neg_momentum']
+                    pos_momentum, neg_momentum = state['pos_momentum'], state['neg_momentum']
                 else:
-                    neg_momentum = state['pos_momentum']
-                    pos_momentum = state['neg_momentum']
+                    neg_momentum, pos_momentum = state['pos_momentum'], state['neg_momentum']
 
                 pos_momentum.mul_(beta1 ** 2).add_(grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
                 delta_p = pos_momentum.mul(1 + beta2).add(neg_momentum, alpha=-beta2).mul(1.0 / noise_norm)
 
                 p.add_(delta_p, alpha=-group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,141 +2,188 @@
 
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.gc import centralize_gradient
 
 
-class RAdam(Optimizer, BaseOptimizer):
-    r"""Rectified Adam.
+class Ranger(Optimizer, BaseOptimizer):
+    r"""a synergistic optimizer combining RAdam and LookAhead, and now GC in one optimizer.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param n_sma_threshold: int. (recommended is 5).
-    :param degenerated_to_sgd: float. degenerated to SGD.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param degenerated_to_sgd: bool. perform SGD update when variance of gradient is high.
+    :param use_gc: bool. use Gradient Centralization (both convolution & fc layers).
+    :param gc_conv_only: bool. use Gradient Centralization (only convolution layer).
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
-        betas: BETAS = (0.9, 0.999),
-        weight_decay: float = 0.0,
+        alpha: float = 0.5,
+        k: int = 6,
         n_sma_threshold: int = 5,
         degenerated_to_sgd: bool = False,
-        adamd_debias_term: bool = False,
-        eps: float = 1e-8,
+        betas: BETAS = (0.95, 0.999),
+        eps: float = 1e-5,
+        weight_decay: float = 0.0,
+        use_gc: bool = True,
+        gc_conv_only: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
     ):
         self.lr = lr
-        self.betas = betas
-        self.weight_decay = weight_decay
+        self.alpha = alpha
+        self.k = k
         self.n_sma_threshold = n_sma_threshold
         self.degenerated_to_sgd = degenerated_to_sgd
+        self.betas = betas
+        self.weight_decay = weight_decay
+        self.use_gc = use_gc
         self.eps = eps
 
+        self.gc_gradient_threshold: int = 3 if gc_conv_only else 1
+
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
+            'alpha': alpha,
+            'k': k,
+            'step_counter': 0,
+            'n_sma_threshold': n_sma_threshold,
             'weight_decay': weight_decay,
-            'adamd_debias_term': adamd_debias_term,
-            'buffer': [[None, None, None] for _ in range(10)],
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
+        self.validate_lookahead_k(self.k)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'RAdam'
+        return 'Ranger'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
+                state['slow_buffer'] = torch.empty_like(p)
+                state['slow_buffer'].copy_(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
+
+            bias_correction1 = 1.0 - beta1 ** group['step']
+
             n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
+            beta2_t: float = beta2 ** group['step']
+            n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
-
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
+                    state['slow_buffer'] = torch.empty_like(p)
+                    state['slow_buffer'].copy_(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                state['step'] += 1
-                bias_correction1 = 1.0 - beta1 ** state['step']
+                if self.use_gc and grad.dim() > self.gc_gradient_threshold:
+                    grad = centralize_gradient(grad, gc_conv_only=False)
+
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
+
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
 
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
+
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                buffered = group['buffer'][state['step'] % 10]
-                if state['step'] == buffered[0]:
-                    n_sma, step_size = buffered[1], buffered[2]
+                if n_sma >= self.n_sma_threshold:
+                    step_size = math.sqrt(
+                        (1 - beta2_t)
+                        * (n_sma - 4)
+                        / (n_sma_max - 4)
+                        * (n_sma - 2)
+                        / n_sma
+                        * n_sma_max
+                        / (n_sma_max - 2)
+                    )
+                elif self.degenerated_to_sgd:
+                    step_size = 1.0
                 else:
-                    buffered[0] = state['step']
-                    beta2_t = beta2 ** state['step']
-                    n_sma = n_sma_max - 2.0 * state['step'] * beta2_t / (1.0 - beta2_t)
-                    buffered[1] = n_sma
-
-                    if n_sma >= self.n_sma_threshold:
-                        step_size = math.sqrt(
-                            (1 - beta2_t)
-                            * (n_sma - 4)
-                            / (n_sma_max - 4)
-                            * (n_sma - 2)
-                            / n_sma
-                            * n_sma_max
-                            / (n_sma_max - 2)
-                        )
-                        if not group['adamd_debias_term']:
-                            step_size /= bias_correction1
-                    elif self.degenerated_to_sgd:
-                        step_size = 1.0 / bias_correction1
-                    else:
-                        step_size = -1
-                    buffered[2] = step_size
+                    step_size = -1
+
+                if not group['adam_debias']:
+                    step_size /= bias_correction1
 
-                if group['weight_decay'] > 0.0 and (n_sma >= self.n_sma_threshold or step_size > 0):
+                if group['weight_decay'] > 0.0:
                     p.add_(p, alpha=-group['weight_decay'] * group['lr'])
 
                 if n_sma >= self.n_sma_threshold:
                     de_nom = exp_avg_sq.sqrt().add_(group['eps'])
                     p.addcdiv_(exp_avg, de_nom, value=-step_size * group['lr'])
-                elif step_size > 0:
+                else:
                     p.add_(exp_avg, alpha=-step_size * group['lr'])
 
+                if group['step'] % group['k'] == 0:
+                    slow_p = state['slow_buffer']
+                    slow_p.add_(p - slow_p, alpha=self.alpha)
+                    p.copy_(slow_p)
+
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ralamb.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,193 @@
 import math
 
 import torch
-from torch.optim import Optimizer
+from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class RaLamb(Optimizer, BaseOptimizer):
-    r"""RAdam + LAMB. Large Batch Optimization for Deep Learning.
+class DiffGrad(Optimizer, BaseOptimizer):
+    r"""An Optimization Method for Convolutional Neural Networks.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
-    :param eps: float. term added to the denominator to improve numerical stability.
     :param weight_decay: float. weight decay (L2 penalty).
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
-    :param pre_norm: bool. perform pre-normalization of all gradients.
+    :param rectify: bool. perform the rectified update similar to RAdam.
     :param n_sma_threshold: int. (recommended is 5).
-    :param degenerated_to_sgd: float. degenerated to SGD.
+    :param degenerated_to_sgd: bool. degenerated to SGD.
+    :param amsgrad: bool. whether to use the AMSBound variant.
+    :param r: float. EMA factor. between 0.9 ~ 0.99 is preferred.
+    :param adanorm: bool. whether to use the AdaNorm variant.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
-    clamp: float = 10.0
-
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
-        eps: float = 1e-8,
         weight_decay: float = 0.0,
-        adamd_debias_term: bool = False,
-        pre_norm: bool = False,
+        rectify: bool = False,
         n_sma_threshold: int = 5,
-        degenerated_to_sgd: bool = False,
+        degenerated_to_sgd: bool = True,
+        amsgrad: bool = False,
+        r: float = 0.95,
+        adanorm: bool = False,
+        adam_debias: bool = False,
+        eps: float = 1e-8,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
-        self.eps = eps
-        self.adamd_debias_term = adamd_debias_term
-        self.pre_norm = pre_norm
+        self.rectify = rectify
         self.n_sma_threshold = n_sma_threshold
         self.degenerated_to_sgd = degenerated_to_sgd
+        self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
-            'adamd_debias_term': adamd_debias_term,
-            'buffer': [[None, None, None] for _ in range(10)],
+            'rectify': rectify,
+            'amsgrad': amsgrad,
+            'adanorm': adanorm,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
+        if adanorm:
+            defaults.update({'r': r})
+
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
-        return 'RaLamb'
+        return 'diffRGrad' if self.rectify else 'diffGrad'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['step'] = 0
                 state['exp_avg'] = torch.zeros_like(p)
                 state['exp_avg_sq'] = torch.zeros_like(p)
-
-    @torch.no_grad()
-    def get_global_gradient_norm(self) -> torch.Tensor:
-        device = self.param_groups[0]['params'][0].device
-
-        global_grad_norm = torch.zeros(1, device=device)
-
-        for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is not None:
-                    global_grad_norm.add_(torch.linalg.norm(p.grad).pow(2))
-
-        return torch.sqrt(global_grad_norm) + self.eps
+                state['previous_grad'] = torch.zeros_like(p)
+                if group['amsgrad']:
+                    state['max_exp_avg_sq'] = torch.zeros_like(p)
+                if group['adanorm']:
+                    state['exp_grad_norm'] = torch.zeros((1,), dtype=p.dtype, device=p.device)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        grad_norm = 1.0
-        if self.pre_norm:
-            grad_norm = self.get_global_gradient_norm()
-
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
-            n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
+
+            bias_correction1 = 1.0 - beta1 ** group['step']
+
+            if group['rectify']:
+                n_sma_max: float = 2.0 / (1.0 - beta2) - 1.0
+                beta2_t: float = beta2 ** group['step']
+                n_sma: float = n_sma_max - 2 * group['step'] * beta2_t / (1.0 - beta2_t)
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
-                if self.pre_norm:
-                    grad.div_(grad_norm)
-
                 state = self.state[p]
-
                 if len(state) == 0:
-                    state['step'] = 0
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
+                    state['previous_grad'] = torch.zeros_like(p)
+                    if group['amsgrad']:
+                        state['max_exp_avg_sq'] = torch.zeros_like(p)
+                    if group['adanorm']:
+                        state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
-                state['step'] += 1
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
-                exp_avg.mul_(beta1).add_(grad, alpha=1.0 - beta1)
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
+                s_grad = grad
+                if group['adanorm']:
+                    grad_norm = torch.linalg.norm(grad)
+
+                    exp_grad_norm = state['exp_grad_norm']
+                    exp_grad_norm.mul_(group['r']).add_(grad_norm, alpha=1.0 - group['r'])
 
-                buffered = group['buffer'][state['step'] % 10]
+                    if exp_grad_norm > grad_norm:
+                        s_grad *= exp_grad_norm / grad_norm
 
-                bias_correction1 = 1.0 - beta1 ** state['step']
+                exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                if state['step'] == buffered[0]:
-                    n_sma, step_size = buffered[1], buffered[2]
+                if group['amsgrad']:
+                    max_exp_avg_sq = state['max_exp_avg_sq']
+                    torch.max(max_exp_avg_sq, exp_avg_sq, out=max_exp_avg_sq)
+                    de_nom = max_exp_avg_sq.add(group['eps']).sqrt()
                 else:
-                    buffered[0] = state['step']
-                    beta2_t = beta2 ** state['step']
-                    n_sma = n_sma_max - 2 * state['step'] * beta2_t / (1 - beta2_t)
-                    buffered[1] = n_sma
-
-                    # more conservative since it's an approximated value
-                    if n_sma >= self.n_sma_threshold:
-                        step_size = math.sqrt(
-                            (1 - beta2_t)
-                            * (n_sma - 4)
-                            / (n_sma_max - 4)
-                            * (n_sma - 2)
-                            / n_sma
-                            * n_sma_max
-                            / (n_sma_max - 2)
-                        )
-                        if not group['adamd_debias_term']:
-                            step_size /= bias_correction1
-                    elif self.degenerated_to_sgd:
-                        step_size = 1.0 / bias_correction1
-                    else:
-                        step_size = group['lr'] / bias_correction1
+                    de_nom = exp_avg_sq.add(group['eps']).sqrt()
 
-                    buffered[2] = step_size
+                de_nom.add_(group['eps'])
 
-                if group['weight_decay'] > 0.0:
-                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
+                # compute diffGrad coefficient (dfc)
+                dfc = state['previous_grad'].clone()
+                dfc.sub_(grad).abs_().sigmoid_().mul_(exp_avg)
+                state['previous_grad'].copy_(grad)
+
+                if not group['rectify']:
+                    step_size: float = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
+                    p.addcdiv_(exp_avg, de_nom, value=-step_size)
+                    continue
 
-                radam_step = p.clone()
                 if n_sma >= self.n_sma_threshold:
-                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
-                    radam_step.addcdiv_(exp_avg, de_nom, value=-step_size)
+                    step_size = math.sqrt(
+                        (1 - beta2_t)
+                        * (n_sma - 4)
+                        / (n_sma_max - 4)
+                        * (n_sma - 2)
+                        / n_sma
+                        * n_sma_max
+                        / (n_sma_max - 2)
+                    )
+                elif self.degenerated_to_sgd:
+                    step_size = 1.0
                 else:
-                    radam_step.add_(exp_avg, alpha=-step_size)
+                    step_size = -1
+
+                if not group['adam_debias']:
+                    step_size /= bias_correction1
 
-                radam_norm = radam_step.norm(2.0)
-                weight_norm = p.norm(2.0).clamp(0.0, self.clamp)
-                trust_ratio: float = (
-                    1.0 if weight_norm == 0 or radam_norm == 0 else weight_norm / (radam_norm + self.eps)
-                )
-
-                state['weight_norm'] = weight_norm
-                state['adam_norm'] = radam_norm
-                state['trust_ratio'] = trust_ratio
+                if group['weight_decay'] > 0.0:
+                    p.add_(p, alpha=-group['weight_decay'] * group['lr'])
 
                 if n_sma >= self.n_sma_threshold:
-                    p.addcdiv_(exp_avg, de_nom, value=-step_size * trust_ratio)
-                else:
-                    p.add_(exp_avg, alpha=-step_size * trust_ratio)
+                    de_nom = exp_avg_sq.sqrt().add_(group['eps'])
+                    p.addcdiv_(dfc, de_nom, value=-step_size * group['lr'])
+                elif step_size > 0:
+                    p.add_(exp_avg, alpha=-step_size * group['lr'])
 
         return loss
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger21.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     :param agc_eps: float. eps for AGC
     :param centralize_gradients: bool. use GC both convolution & fc layers.
     :param normalize_gradients: bool. use gradient normalization.
     :param lookahead_merge_time: int. merge time.
     :param lookahead_blending_alpha: float. blending alpha.
     :param weight_decay: float. weight decay (L2 penalty).
     :param norm_loss_factor: float. norm loss factor.
-    :param adamd_debias_term: bool. Only correct the denominator to avoid inflating step sizes early in training.
+    :param adam_debias: bool. Only correct the denominator to avoid inflating step sizes early in training.
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(  # pylint: disable=R0913
         self,
         params: PARAMETERS,
         num_iterations: int,
@@ -65,15 +65,15 @@
         agc_eps: float = 1e-3,
         centralize_gradients: bool = True,
         normalize_gradients: bool = True,
         lookahead_merge_time: int = 5,
         lookahead_blending_alpha: float = 0.5,
         weight_decay: float = 1e-4,
         norm_loss_factor: float = 1e-4,
-        adamd_debias_term: bool = False,
+        adam_debias: bool = False,
         eps: float = 1e-8,
     ):
         self.lr = lr
         self.min_lr = warm_down_min_lr
         self.beta0 = beta0
         self.betas = betas
         self.use_softplus = use_softplus
@@ -82,15 +82,14 @@
         self.agc_eps = agc_eps
         self.centralize_gradients = centralize_gradients
         self.normalize_gradients = normalize_gradients
         self.lookahead_merge_time = lookahead_merge_time
         self.lookahead_blending_alpha = lookahead_blending_alpha
         self.weight_decay = weight_decay
         self.norm_loss_factor = norm_loss_factor
-        self.adamd_debias_term = adamd_debias_term
         self.eps = eps
 
         self.validate_parameters()
 
         # lookahead
         self.lookahead_step: int = 0
 
@@ -98,15 +97,15 @@
         self.starting_lr = lr
         self.current_lr = lr
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
-            'adamd_debias_term': adamd_debias_term,
+            'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
         # warmup iterations
         self.num_warm_up_iterations: int = (
             self.build_warm_up_iterations(num_iterations, betas[1])
@@ -287,15 +286,15 @@
 
                 grad = p.grad
                 grad = centralize_gradient(grad, gc_conv_only=False)
                 grad = normalize_gradient(grad)
 
                 grad_ma.mul_(beta1 ** 2).add_(grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
 
-                step_size: float = lr if group['adamd_debias_term'] else lr / bias_correction1
+                step_size: float = lr if group['adam_debias'] else lr / bias_correction1
 
                 if self.use_softplus:
                     de_nom = f.softplus(de_nom, beta=self.beta_softplus)
 
                 pn_momentum = grad_ma.mul(1.0 + 1.0).add(neg_grad_ma, alpha=-1.0).mul(1.0 / noise_norm)
                 p.addcdiv_(pn_momentum, de_nom, value=-step_size)
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sgdp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,40 +54,40 @@
 
     def __str__(self) -> str:
         return 'Shampoo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
-            for p in group['params']:
-                state = self.state[p]
-
-                state['step'] = 0
+            group['step'] = 0
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             momentum, weight_decay = group['momentum'], group['weight_decay']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
-
                     if momentum > 0.0:
                         state['momentum_buffer'] = grad.clone()
 
                     for dim_id, dim in enumerate(grad.size()):
                         state[f'pre_cond_{dim_id}'] = self.matrix_eps * torch.eye(dim, out=grad.new(dim, dim))
                         state[f'inv_pre_cond_{dim_id}'] = grad.new(dim, dim).zero_()
 
@@ -105,25 +105,24 @@
                     grad = grad.transpose_(0, dim_id).contiguous()
                     transposed_size = grad.size()
 
                     grad = grad.view(dim, -1)
                     grad_t = grad.t()
 
                     pre_cond.add_(grad @ grad_t)
-                    if state['step'] % self.preconditioning_compute_steps == 0:
+                    if group['step'] % self.preconditioning_compute_steps == 0:
                         inv_pre_cond.copy_(compute_power_svd(pre_cond, -1.0 / order))
 
                     if dim_id == order - 1:
                         grad = grad_t @ inv_pre_cond
                         grad = grad.view(original_size)
                     else:
                         grad = inv_pre_cond @ grad
                         grad = grad.view(transposed_size)
 
-                state['step'] += 1
                 state['momentum_buffer'] = grad
 
                 p.add_(grad, alpha=-group['lr'])
 
         return loss
 
 
@@ -201,36 +200,40 @@
         nesterov: bool = True,
         diagonal_eps: float = 1e-10,
         matrix_eps: float = 1e-6,
         use_svd: bool = False,
     ):
         self.lr = lr
         self.betas = betas
-        self.moving_average_for_momentum = moving_average_for_momentum
         self.weight_decay = weight_decay
-        self.decoupled_weight_decay = decoupled_weight_decay
-        self.decoupled_learning_rate = decoupled_learning_rate
         self.inverse_exponent_override = inverse_exponent_override
         self.start_preconditioning_step = start_preconditioning_step
         self.preconditioning_compute_steps = preconditioning_compute_steps
         self.statistics_compute_steps = statistics_compute_steps
         self.block_size = block_size
         self.skip_preconditioning_rank_lt = skip_preconditioning_rank_lt
         self.no_preconditioning_for_layers_with_dim_gt = no_preconditioning_for_layers_with_dim_gt
         self.shape_interpretation = shape_interpretation
         self.graft_type = graft_type
         self.pre_conditioner_type = pre_conditioner_type
-        self.nesterov = nesterov
         self.diagonal_eps = diagonal_eps
         self.matrix_eps = matrix_eps
         self.use_svd = use_svd
 
         self.validate_parameters()
 
-        defaults: DEFAULTS = {'lr': lr, 'betas': betas, 'weight_decay': weight_decay}
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'betas': betas,
+            'weight_decay': weight_decay,
+            'decoupled_weight_decay': decoupled_weight_decay,
+            'decoupled_learning_rate': decoupled_learning_rate,
+            'moving_average_for_momentum': moving_average_for_momentum,
+            'nesterov': nesterov,
+        }
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
         self.validate_update_frequency(self.start_preconditioning_step)
@@ -277,15 +280,15 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             is_precondition_step: bool = self.is_precondition_step(group['step'])
-            pre_conditioner_multiplier: float = group['lr'] if not self.decoupled_learning_rate else 1.0
+            pre_conditioner_multiplier: float = 1.0 if group['decoupled_learning_rate'] else group['lr']
 
             beta1, beta2 = group['betas']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
@@ -325,28 +328,28 @@
                 if self.graft_type != LayerWiseGrafting.NONE:
                     graft_norm = torch.linalg.norm(graft_grad)
                     shampoo_norm = torch.linalg.norm(shampoo_grad)
 
                     shampoo_grad.mul_(graft_norm / (shampoo_norm + 1e-16))
 
                 if group['weight_decay'] > 0.0:
-                    if not self.decoupled_weight_decay:
+                    if not group['decoupled_weight_decay']:
                         graft_grad.add_(p, alpha=group['weight_decay'])
                         shampoo_grad.add_(p, alpha=group['weight_decay'])
                     else:
                         graft_grad.mul_(1.0 - group['lr'] * group['weight_decay'])
                         shampoo_grad.mul_(1.0 - group['lr'] * group['weight_decay'])
 
                 state['momentum'].mul_(beta1).add_(shampoo_grad)
                 graft_momentum = graft.update_momentum(grad, beta1)
 
                 momentum_update = state['momentum'] if is_precondition_step else graft_momentum
 
-                if self.nesterov:
-                    w: float = (1.0 - beta1) if self.moving_average_for_momentum else 1.0
+                if group['nesterov']:
+                    w: float = (1.0 - beta1) if group['moving_average_for_momentum'] else 1.0
 
                     wd_update = shampoo_grad if is_precondition_step else graft_grad
                     wd_update.mul_(w)
 
                     momentum_update.mul_(beta1).add_(wd_update)
 
                 p.add_(momentum_update, alpha=-group['lr'])
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/sm3.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sm3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import torch
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, PARAMETERS
+from pytorch_optimizer.optimizer.utils import reduce_max_except_dim
 
 
 class SM3(Optimizer, BaseOptimizer):
     r"""Memory-Efficient Adaptive Optimization.
 
-        Reference : https://github.com/Enealor/PyTorch-SM3/blob/master/src/SM3/SM3.py
-
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param momentum: float. coefficient used to scale prior updates before adding. This drastically increases
         memory usage if `momentum > 0.0`. This is ignored if the parameter's gradient is sparse.
     :param beta: float. coefficient used for exponential moving averages.
     """
 
@@ -28,15 +27,15 @@
         self.lr = lr
         self.momentum = momentum
         self.beta = beta
         self.eps = eps
 
         self.validate_parameters()
 
-        defaults: DEFAULTS = {'lr': lr, 'momentum': momentum, 'beta': beta}
+        defaults: DEFAULTS = {'lr': lr, 'momentum': momentum, 'beta': beta, 'eps': eps}
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_momentum(self.momentum)
         self.validate_beta(self.beta)
         self.validate_epsilon(self.eps)
@@ -50,29 +49,14 @@
             for p in group['params']:
                 state = self.state[p]
 
                 state['step'] = 0
                 state['momentum_buffer'] = torch.zeros_like(p)
 
     @staticmethod
-    def max_reduce_except_dim(x: torch.Tensor, dim: int) -> torch.Tensor:
-        r"""Perform reduce-max along all dimensions except the given dim."""
-        rank: int = len(x.shape)
-        if rank == 0:
-            return x
-
-        if dim >= rank:
-            raise ValueError(f'[-] given dim is bigger than rank. {dim} >= {rank}')
-
-        for d in range(rank):
-            if d != dim:
-                x = x.max(dim=d, keepdim=True).values
-        return x
-
-    @staticmethod
     def make_sparse(grad: torch.Tensor, values: torch.Tensor) -> torch.Tensor:
         if grad._indices().dim() == 0 or values.dim() == 0:
             return grad.new().resize_as_(grad)
         return grad.new(grad._indices(), values, grad.size())
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
@@ -114,45 +98,42 @@
 
                     acc = state['accumulator_0']
                     update_values = torch.gather(acc, 0, grad._indices()[0])
                     if beta > 0.0:
                         update_values.mul_(beta)
                     update_values.addcmul_(grad._values(), grad._values(), value=1.0 - beta)
 
-                    nu_max = self.max_reduce_except_dim(
-                        x=self.make_sparse(grad, update_values).to_dense(),
-                        dim=0,
-                    ).squeeze_()
+                    nu_max = reduce_max_except_dim(self.make_sparse(grad, update_values).to_dense(), 0).squeeze_()
 
                     if beta > 0.0:
                         torch.max(acc, nu_max, out=acc)
                     else:
                         acc.copy_(nu_max)
 
-                    update_values.add_(self.eps).rsqrt_().mul_(grad._values())
+                    update_values.add_(group['eps']).rsqrt_().mul_(grad._values())
 
                     update = self.make_sparse(grad, update_values)
                 else:
                     update = state['accumulator_0'].clone()
                     for i in range(1, rank):
                         update = torch.min(update, state[f'accumulator_{i}'])
 
                     if beta > 0.0:
                         update.mul_(beta)
                     update.addcmul_(grad, grad, value=1.0 - beta)
 
                     for i in range(rank):
                         acc = state[f'accumulator_{i}']
-                        nu_max = self.max_reduce_except_dim(update, i)
+                        nu_max = reduce_max_except_dim(update, i)
                         if beta > 0.0:
                             torch.max(acc, nu_max, out=acc)
                         else:
                             acc.copy_(nu_max)
 
-                    update.add_(self.eps).rsqrt_().mul_(grad)
+                    update.add_(group['eps']).rsqrt_().mul_(grad)
 
                     if momentum > 0.0:
                         m = state['momentum_buffer']
                         m.mul_(momentum).add_(update, alpha=1.0 - momentum)
                         update = m
 
                 p.add_(update, alpha=-group['lr'])
```

### Comparing `pytorch_optimizer-2.6.1/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from torch import nn
 from torch.distributed import all_reduce
 from torch.nn import functional as f
 from torch.nn.modules.batchnorm import _BatchNorm
@@ -123,16 +123,16 @@
         for p in parameters:
             p.grad.detach().mul_(clip_coefficient)
 
     return grad_norm
 
 
 def projection(
-    p,
-    grad,
+    p: torch.Tensor,
+    grad: torch.Tensor,
     perturb: torch.Tensor,
     delta: float,
     wd_ratio: float,
     eps: float,
 ) -> Tuple[torch.Tensor, float]:
     r"""Project to remove the radial component from the update vector."""
     wd: float = 1.0
@@ -160,15 +160,15 @@
     elif x_len in (2, 3):  # linear layers
         dim = 1
     elif x_len == 4:  # conv kernels
         dim = (1, 2, 3)
     else:
         dim = tuple(range(1, x_len))
 
-    return x.norm(dim=dim, keepdim=keep_dim, p=norm)
+    return x.norm(p=norm, dim=dim, keepdim=keep_dim)
 
 
 def get_optimizer_parameters(
     model_or_parameter: Union[nn.Module, List],
     weight_decay: float,
     wd_ban_list: List[str] = ('bias', 'LayerNorm.bias', 'LayerNorm.weight'),
 ) -> PARAMETERS:
@@ -239,7 +239,40 @@
 def l2_projection(parameters: PARAMETERS, max_norm: float = 1e2):
     r"""Get l2 normalized parameter."""
     global_norm = torch.sqrt(sum(p.norm().pow(2) for p in parameters))
     if global_norm > max_norm:
         ratio = max_norm / global_norm
         for param in parameters:
             param *= ratio  # noqa: PLW2901
+
+
+@torch.no_grad()
+def get_global_gradient_norm(param_groups: List[Dict], device: torch.device) -> torch.Tensor:
+    r"""Get global gradient norm."""
+    global_grad_norm = torch.zeros(1, dtype=torch.float32, device=device)
+
+    for group in param_groups:
+        for p in group['params']:
+            if p.grad is not None:
+                global_grad_norm.add_(p.grad.norm().pow(2))
+
+    return global_grad_norm
+
+
+@torch.no_grad()
+def reduce_max_except_dim(x: torch.Tensor, dim: int) -> torch.Tensor:
+    r"""Perform reduce-max along all dimensions except the given dim.
+
+    :param x: torch.Tensor. tensor to reduce-max.
+    :param dim: int. dimension to exclude.
+    """
+    rank: int = len(x.shape)
+    if rank == 0:
+        return x
+
+    if dim >= rank:
+        raise ValueError(f'[-] given dim is bigger than rank. {dim} >= {rank}')
+
+    for d in range(rank):
+        if d != dim:
+            x = x.max(dim=d, keepdim=True).values
+    return x
```

### Comparing `pytorch_optimizer-2.6.1/PKG-INFO` & `pytorch_optimizer-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-optimizer
-Version: 2.6.1
+Version: 2.7.0
 Summary: optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas.
 Home-page: https://github.com/kozistr/pytorch_optimizer
 License: Apache-2.0
 Keywords: pytorch,deep-learning,optimizer,lr scheduler
 Author: kozistr
 Author-email: kozistr@gmail.com
 Maintainer: kozistr
@@ -179,14 +179,18 @@
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Lion         | *Symbolic Discovery of Optimization Algorithms*                                                 | `github <https://github.com/google/automl/tree/master/lion>`__                    | `https://arxiv.org/abs/2302.06675 <https://arxiv.org/abs/2302.06675>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | Ali-G        | *Adaptive Learning Rates for Interpolation with Gradients*                                      | `github <https://github.com/oval-group/ali-g>`__                                  | `https://arxiv.org/abs/1906.05661 <https://arxiv.org/abs/1906.05661>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | SM3          | *Memory-Efficient Adaptive Optimization*                                                        | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AdaNorm      | *Adaptive Gradient Norm Correction based Optimizer for CNNs*                                    | `github <https://github.com/shivram1987/AdaNorm>`__                               | `https://arxiv.org/abs/2210.06364 <https://arxiv.org/abs/2210.06364>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| RotoGrad     | *Gradient Homogenization in Multitask Learning*                                                 | `github <https://github.com/adrianjav/rotograd>`__                                | `https://openreview.net/pdf?id=T8wHz4rnuGL <https://openreview.net/pdf?id=T8wHz4rnuGL>`__     |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 
 Useful Resources
 ----------------
 
 Several optimization ideas to regularize & stabilize the training. Most
 of the ideas are applied in ``Ranger21`` optimizer.
 
@@ -386,14 +390,18 @@
 
 `Lion <https://github.com/google/automl/tree/master/lion#citation>`__
 
 `Ali-G <https://github.com/oval-group/ali-g#adaptive-learning-rates-for-interpolation-with-gradients>`__
 
 `SM3 <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__
 
+`AdaNorm <https://github.com/shivram1987/AdaNorm/tree/main#citation>`__
+
+`RotoGrad <https://github.com/adrianjav/rotograd#citing>`__
+
 Citation
 --------
 
 Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
 Or you can get from "cite this repository" button.
 
 ::
```

