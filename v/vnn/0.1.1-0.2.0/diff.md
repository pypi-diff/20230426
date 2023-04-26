# Comparing `tmp/vnn-0.1.1.tar.gz` & `tmp/vnn-0.2.0.tar.gz`

## Comparing `vnn-0.1.1.tar` & `vnn-0.2.0.tar`

### file list

```diff
@@ -1,68 +1,78 @@
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 vnn-0.1.1/attacked_evaluation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vnn-0.1.1/conda_environment.yml
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 vnn-0.1.1/core.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 vnn-0.1.1/evaluate_auto_encoder.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 vnn-0.1.1/losses.py
--rw-r--r--   0        0        0    30756 2020-02-02 00:00:00.000000 vnn-0.1.1/main.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 vnn-0.1.1/metrics.py
--rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 vnn-0.1.1/modeling.py
--rw-r--r--   0        0        0    13303 2020-02-02 00:00:00.000000 vnn-0.1.1/params.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 vnn-0.1.1/perturbed_evaluation.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 vnn-0.1.1/requirements.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vnn-0.1.1/requirements_new.txt
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 vnn-0.1.1/run_batchjob.sh
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 vnn-0.1.1/run_example.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/__init__.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/bayes_by_backprop.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/classic.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/const_mean_variational.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/dropout.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/ensemble.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/functional.py
--rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/hypermodel.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/network.py
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/parameter_std_variational.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/single_mean_variational.py
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/single_std_variational.py
--rw-r--r--   0        0        0    11819 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/variational.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/auto_encoder_network.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/base_vnn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/beta_vgg.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/cifar10_base.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/cifar10_base_vnn.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/cifar10_mini_base.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/densenet1.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/densenet2.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/densenet_pure.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/mnist_auto_encoder_base.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/mnist_base.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/mnist_conv_max.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/mnist_mini2_base.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/mnist_mini_base.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/mnist_mlp.py
--rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/resnet.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/resnet_classic.py
--rw-r--r--   0        0        0    13658 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/resnet_pure.py
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/resnet_vnn.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/vgg.py
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 vnn-0.1.1/networks/architectures/vgg_pure.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/create-accuracy-tex-report.py
--rw-r--r--   0        0        0    12540 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/create-evalutaion-report-r.py
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/create-grouped-tex-report.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/create-total-best-tex-report.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/create-total-tex-report.py
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/describe_models.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/r-evaluation-report-template.r
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/tex-report-template-long.tex
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/tex-report-template.tex
--rw-r--r--   0        0        0    82570 2020-02-02 00:00:00.000000 vnn-0.1.1/tools/r-reports/evaluation-report.r
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 vnn-0.1.1/vnn/__init__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 vnn-0.1.1/vnn/classic.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 vnn-0.1.1/vnn/dropout.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 vnn-0.1.1/vnn/functional.py
--rw-r--r--   0        0        0    11819 2020-02-02 00:00:00.000000 vnn-0.1.1/vnn/variational.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 vnn-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 vnn-0.1.1/LICENSE
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 vnn-0.1.1/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 vnn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 vnn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 vnn-0.2.0/attacked_evaluation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vnn-0.2.0/conda_environment.yml
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 vnn-0.2.0/core.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 vnn-0.2.0/evaluate_auto_encoder.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 vnn-0.2.0/losses.py
+-rw-r--r--   0        0        0    30756 2020-02-02 00:00:00.000000 vnn-0.2.0/main.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 vnn-0.2.0/metrics.py
+-rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 vnn-0.2.0/modeling.py
+-rw-r--r--   0        0        0    13303 2020-02-02 00:00:00.000000 vnn-0.2.0/params.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 vnn-0.2.0/perturbed_evaluation.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 vnn-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vnn-0.2.0/requirements_new.txt
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 vnn-0.2.0/run_batchjob.sh
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 vnn-0.2.0/run_example.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/bayes_by_backprop.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/classic.py
+-rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/const_mean_variational.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/dropout.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/ensemble.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/functional.py
+-rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/hypermodel.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/network.py
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/parameter_std_variational.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/single_mean_variational.py
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/single_std_variational.py
+-rw-r--r--   0        0        0    13221 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/variational.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/auto_encoder_network.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/base_vnn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/beta_vgg.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/cifar10_base.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/cifar10_base_vnn.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/cifar10_mini_base.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/densenet1.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/densenet2.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/densenet_pure.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/mnist_auto_encoder_base.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/mnist_base.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/mnist_conv_max.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/mnist_mini2_base.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/mnist_mini_base.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/mnist_mlp.py
+-rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/resnet.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/resnet_classic.py
+-rw-r--r--   0        0        0    13658 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/resnet_pure.py
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/resnet_vnn.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/vgg.py
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 vnn-0.2.0/networks/architectures/vgg_pure.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 vnn-0.2.0/results/.gitignore
+-rw-r--r--   0        0        0   765196 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/model.pth
+-rw-r--r--   0        0        0   764595 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/optimizer.pth
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/training_parameters.json
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/best/description.json
+-rw-r--r--   0        0        0   765196 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/best/model.pth
+-rw-r--r--   0        0        0   764595 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/best/optimizer.pth
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/best/training_parameters.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/results/validation_batch_20samples_1.txt
+-rw-r--r--   0        0        0   322205 2020-02-02 00:00:00.000000 vnn-0.2.0/results/mnist_mini_base_vnn/summary/events.out.tfevents.1682431400.cerberus
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/create-accuracy-tex-report.py
+-rw-r--r--   0        0        0    12540 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/create-evalutaion-report-r.py
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/create-grouped-tex-report.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/create-total-best-tex-report.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/create-total-tex-report.py
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/describe_models.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/r-evaluation-report-template.r
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/tex-report-template-long.tex
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/tex-report-template.tex
+-rw-r--r--   0        0        0    82570 2020-02-02 00:00:00.000000 vnn-0.2.0/tools/r-reports/evaluation-report.r
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 vnn-0.2.0/vnn/__init__.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 vnn-0.2.0/vnn/classic.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 vnn-0.2.0/vnn/dropout.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 vnn-0.2.0/vnn/functional.py
+-rw-r--r--   0        0        0    13221 2020-02-02 00:00:00.000000 vnn-0.2.0/vnn/variational.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 vnn-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 vnn-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 vnn-0.2.0/README.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 vnn-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 vnn-0.2.0/PKG-INFO
```

### Comparing `vnn-0.1.1/attacked_evaluation.py` & `vnn-0.2.0/attacked_evaluation.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/core.py` & `vnn-0.2.0/core.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/evaluate_auto_encoder.py` & `vnn-0.2.0/evaluate_auto_encoder.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/losses.py` & `vnn-0.2.0/losses.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/main.py` & `vnn-0.2.0/main.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/metrics.py` & `vnn-0.2.0/metrics.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/modeling.py` & `vnn-0.2.0/modeling.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/params.py` & `vnn-0.2.0/params.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/perturbed_evaluation.py` & `vnn-0.2.0/perturbed_evaluation.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/bayes_by_backprop.py` & `vnn-0.2.0/networks/bayes_by_backprop.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/classic.py` & `vnn-0.2.0/networks/classic.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/const_mean_variational.py` & `vnn-0.2.0/networks/const_mean_variational.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/dropout.py` & `vnn-0.2.0/networks/dropout.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/ensemble.py` & `vnn-0.2.0/networks/ensemble.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/functional.py` & `vnn-0.2.0/networks/functional.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/hypermodel.py` & `vnn-0.2.0/networks/hypermodel.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/network.py` & `vnn-0.2.0/networks/network.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/parameter_std_variational.py` & `vnn-0.2.0/networks/parameter_std_variational.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/single_mean_variational.py` & `vnn-0.2.0/networks/single_mean_variational.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/single_std_variational.py` & `vnn-0.2.0/networks/single_std_variational.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/variational.py` & `vnn-0.2.0/networks/variational.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, List, Optional, Literal, Tuple, Union
 import torch
 from torch import nn
 
 
 class VariationalBase(nn.Module):
-
     GLOBAL_STD: float = 0
     LOG_STDS = False
+    INIT_WEIGHTS = "usual"
 
     def __init__(self) -> None:
         super().__init__()
 
     def build(
         self,
         means: nn.Module,
@@ -39,31 +39,28 @@
         ] = "mean",
         batch_norm_eps: float = 1e-3,
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
     ) -> None:
-
         super().__init__()
 
         self.end_activation = None
         self.end_batch_norm = None
 
         self.means = means
         self.stds = stds
 
         self.global_std_mode = global_std_mode
 
         if use_batch_norm:
-
             batch_norm_targets = batch_norm_mode.split("+")
 
             for i, target in enumerate(batch_norm_targets):
-
                 if target == "mean":
                     self.means = nn.Sequential(
                         self.means,
                         batch_norm_module(
                             batch_norm_size,
                             eps=batch_norm_eps,
                             momentum=batch_norm_momentum,
@@ -85,60 +82,56 @@
                         eps=batch_norm_eps,
                         momentum=batch_norm_momentum,
                     )
                 else:
                     raise ValueError("Unknown batch norm target: " + target)
 
         if activation is not None:
-
             activation_targets = activation_mode.split("+")
 
             for i, target in enumerate(activation_targets):
-
                 if len(activation_targets) == 1:
                     current_activation: nn.Module = activation  # type: ignore
                 else:
                     current_activation: nn.Module = activation[
                         i
                     ]  # type: ignore
 
                 if target == "mean":
-                    self.means = nn.Sequential(self.means, current_activation,)
+                    self.means = nn.Sequential(
+                        self.means,
+                        current_activation,
+                    )
                 elif target == "std":
                     if self.stds is not None:
                         self.stds = nn.Sequential(
-                            self.stds, current_activation,
+                            self.stds,
+                            current_activation,
                         )
                 elif target == "end":
                     self.end_activation = current_activation
                 else:
                     raise ValueError("Unknown activation target: " + target)
 
-    def forward(self, input):
-
-        if isinstance(input, tuple):
-            x, nstd_x = input
-        else:
-            x = input
-            nstd_x = x
+        self._init_weights()
 
+    def forward(self, x):
         means = self.means(x)
 
         if self.stds:
             stds = self.stds(x)
         else:
             stds = 0
 
         if self.global_std_mode == "replace":
             stds = VariationalBase.GLOBAL_STD
         elif self.global_std_mode == "multiply":
             stds = VariationalBase.GLOBAL_STD * stds
 
         if self.LOG_STDS:
-
             pstds = stds
 
             if isinstance(stds, (int, float)):
                 pstds = torch.tensor(stds * 1.0)
 
             print(
                 "std%:",
@@ -149,29 +142,27 @@
                 ),
                 "std:",
                 float(torch.mean(pstds).detach()),
                 "mean",
                 float(torch.mean(means).detach()),
             )
 
-        # if self.is_uncertainty_layer:
-        #     result = means
-        # else:
-        #     result = torch.distributions.Normal(means, stds).rsample()
-        # result = torch.distributions.Normal(means, stds.abs() + 1e-40).rsample()
         result = means + stds * torch.normal(0, torch.ones_like(means))
 
         if self.end_batch_norm is not None:
             result = self.end_batch_norm(result)
 
         if self.end_activation is not None:
             result = self.end_activation(result)
 
         return result
 
+    def _init_weights(self):
+        init_weights(self)
+
 
 class VariationalConvolution(VariationalBase):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size: int,
@@ -200,15 +191,14 @@
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
         bias=True,
         **kwargs,
     ) -> None:
-
         super().__init__()
 
         if use_batch_norm:
             bias = False
 
         means = nn.Conv2d(
             in_channels=in_channels,
@@ -275,15 +265,14 @@
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
         bias=True,
         **kwargs,
     ) -> None:
-
         super().__init__()
 
         if use_batch_norm:
             bias = False
 
         means = nn.Linear(in_features, out_features, bias=bias, **kwargs)
 
@@ -338,15 +327,14 @@
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
         bias=True,
         **kwargs,
     ) -> None:
-
         super().__init__()
 
         if use_batch_norm:
             bias = False
 
         means = nn.ConvTranspose2d(
             in_channels=in_channels,
@@ -378,7 +366,61 @@
             activation_mode=activation_mode,
             use_batch_norm=use_batch_norm,
             batch_norm_mode=batch_norm_mode,
             batch_norm_eps=batch_norm_eps,
             batch_norm_momentum=batch_norm_momentum,
             global_std_mode=global_std_mode,
         )
+
+
+def init_weights(self):
+    init_type, *params = VariationalBase.INIT_WEIGHTS.split(":")
+
+    if init_type == "usual":
+        pass
+    elif init_type == "fill":
+        fill_what = params[0]
+        value_kernel = float(params[1])
+        value_bias = float(params[2])
+
+        def fill(target):
+            target.weight.data.fill_(value_kernel)
+            if target.bias:
+                target.bias.data.fill_(value_bias)
+
+        if "mean" in fill_what:
+            fill(self.means)
+
+        if "std" in fill_what:
+            fill(self.stds)
+    elif init_type == "xavier_uniform":
+        fill_what = params[0]
+        gain_kernel = float(params[1])
+        gain_bias = float(params[2])
+
+        def fill(target):
+            torch.nn.init.xavier_uniform_(target.weight, gain=gain_kernel)
+            if target.bias:
+                torch.nn.init.xavier_uniform_(target.bias, gain=gain_bias)
+
+        if "mean" in fill_what:
+            fill(self.means)
+
+        if "std" in fill_what:
+            fill(self.stds)
+    elif init_type == "xavier_normal":
+        fill_what = params[0]
+        gain_kernel = float(params[1])
+        gain_bias = float(params[2])
+
+        def fill(target):
+            torch.nn.init.xavier_normal_(target.weight, gain=gain_kernel)
+            if target.bias:
+                torch.nn.init.xavier_normal_(target.bias, gain=gain_bias)
+
+        if "mean" in fill_what:
+            fill(self.means)
+
+        if "std" in fill_what:
+            fill(self.stds)
+    else:
+        raise ValueError()
```

### Comparing `vnn-0.1.1/networks/architectures/auto_encoder_network.py` & `vnn-0.2.0/networks/architectures/auto_encoder_network.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/base_vnn.py` & `vnn-0.2.0/networks/architectures/base_vnn.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/cifar10_base.py` & `vnn-0.2.0/networks/architectures/cifar10_base.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/cifar10_base_vnn.py` & `vnn-0.2.0/networks/architectures/cifar10_base_vnn.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/cifar10_mini_base.py` & `vnn-0.2.0/networks/architectures/cifar10_mini_base.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/densenet1.py` & `vnn-0.2.0/networks/architectures/densenet1.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/densenet2.py` & `vnn-0.2.0/networks/architectures/densenet2.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/densenet_pure.py` & `vnn-0.2.0/networks/architectures/densenet_pure.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/mnist_auto_encoder_base.py` & `vnn-0.2.0/networks/architectures/mnist_auto_encoder_base.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/mnist_base.py` & `vnn-0.2.0/networks/architectures/mnist_base.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/mnist_conv_max.py` & `vnn-0.2.0/networks/architectures/mnist_conv_max.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/mnist_mini2_base.py` & `vnn-0.2.0/networks/architectures/mnist_mini2_base.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/mnist_mini_base.py` & `vnn-0.2.0/networks/architectures/mnist_mini_base.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/mnist_mlp.py` & `vnn-0.2.0/networks/architectures/mnist_mlp.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/resnet.py` & `vnn-0.2.0/networks/architectures/resnet.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/resnet_classic.py` & `vnn-0.2.0/networks/architectures/resnet_classic.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/resnet_pure.py` & `vnn-0.2.0/networks/architectures/resnet_pure.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/resnet_vnn.py` & `vnn-0.2.0/networks/architectures/resnet_vnn.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/vgg.py` & `vnn-0.2.0/networks/architectures/vgg.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/networks/architectures/vgg_pure.py` & `vnn-0.2.0/networks/architectures/vgg_pure.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/create-accuracy-tex-report.py` & `vnn-0.2.0/tools/create-accuracy-tex-report.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/create-evalutaion-report-r.py` & `vnn-0.2.0/tools/create-evalutaion-report-r.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/create-grouped-tex-report.py` & `vnn-0.2.0/tools/create-grouped-tex-report.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/create-total-best-tex-report.py` & `vnn-0.2.0/tools/create-total-best-tex-report.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/create-total-tex-report.py` & `vnn-0.2.0/tools/create-total-tex-report.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/describe_models.py` & `vnn-0.2.0/tools/describe_models.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/tools/r-reports/evaluation-report.r` & `vnn-0.2.0/tools/r-reports/evaluation-report.r`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/vnn/classic.py` & `vnn-0.2.0/vnn/classic.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/vnn/dropout.py` & `vnn-0.2.0/vnn/dropout.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/vnn/functional.py` & `vnn-0.2.0/vnn/functional.py`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/vnn/variational.py` & `vnn-0.2.0/vnn/variational.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, List, Optional, Literal, Tuple, Union
 import torch
 from torch import nn
 
 
 class VariationalBase(nn.Module):
-
     GLOBAL_STD: float = 0
     LOG_STDS = False
+    INIT_WEIGHTS = "usual"
 
     def __init__(self) -> None:
         super().__init__()
 
     def build(
         self,
         means: nn.Module,
@@ -39,31 +39,28 @@
         ] = "mean",
         batch_norm_eps: float = 1e-3,
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
     ) -> None:
-
         super().__init__()
 
         self.end_activation = None
         self.end_batch_norm = None
 
         self.means = means
         self.stds = stds
 
         self.global_std_mode = global_std_mode
 
         if use_batch_norm:
-
             batch_norm_targets = batch_norm_mode.split("+")
 
             for i, target in enumerate(batch_norm_targets):
-
                 if target == "mean":
                     self.means = nn.Sequential(
                         self.means,
                         batch_norm_module(
                             batch_norm_size,
                             eps=batch_norm_eps,
                             momentum=batch_norm_momentum,
@@ -85,60 +82,56 @@
                         eps=batch_norm_eps,
                         momentum=batch_norm_momentum,
                     )
                 else:
                     raise ValueError("Unknown batch norm target: " + target)
 
         if activation is not None:
-
             activation_targets = activation_mode.split("+")
 
             for i, target in enumerate(activation_targets):
-
                 if len(activation_targets) == 1:
                     current_activation: nn.Module = activation  # type: ignore
                 else:
                     current_activation: nn.Module = activation[
                         i
                     ]  # type: ignore
 
                 if target == "mean":
-                    self.means = nn.Sequential(self.means, current_activation,)
+                    self.means = nn.Sequential(
+                        self.means,
+                        current_activation,
+                    )
                 elif target == "std":
                     if self.stds is not None:
                         self.stds = nn.Sequential(
-                            self.stds, current_activation,
+                            self.stds,
+                            current_activation,
                         )
                 elif target == "end":
                     self.end_activation = current_activation
                 else:
                     raise ValueError("Unknown activation target: " + target)
 
-    def forward(self, input):
-
-        if isinstance(input, tuple):
-            x, nstd_x = input
-        else:
-            x = input
-            nstd_x = x
+        self._init_weights()
 
+    def forward(self, x):
         means = self.means(x)
 
         if self.stds:
             stds = self.stds(x)
         else:
             stds = 0
 
         if self.global_std_mode == "replace":
             stds = VariationalBase.GLOBAL_STD
         elif self.global_std_mode == "multiply":
             stds = VariationalBase.GLOBAL_STD * stds
 
         if self.LOG_STDS:
-
             pstds = stds
 
             if isinstance(stds, (int, float)):
                 pstds = torch.tensor(stds * 1.0)
 
             print(
                 "std%:",
@@ -149,29 +142,27 @@
                 ),
                 "std:",
                 float(torch.mean(pstds).detach()),
                 "mean",
                 float(torch.mean(means).detach()),
             )
 
-        # if self.is_uncertainty_layer:
-        #     result = means
-        # else:
-        #     result = torch.distributions.Normal(means, stds).rsample()
-        # result = torch.distributions.Normal(means, stds.abs() + 1e-40).rsample()
         result = means + stds * torch.normal(0, torch.ones_like(means))
 
         if self.end_batch_norm is not None:
             result = self.end_batch_norm(result)
 
         if self.end_activation is not None:
             result = self.end_activation(result)
 
         return result
 
+    def _init_weights(self):
+        init_weights(self)
+
 
 class VariationalConvolution(VariationalBase):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size: int,
@@ -200,15 +191,14 @@
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
         bias=True,
         **kwargs,
     ) -> None:
-
         super().__init__()
 
         if use_batch_norm:
             bias = False
 
         means = nn.Conv2d(
             in_channels=in_channels,
@@ -275,15 +265,14 @@
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
         bias=True,
         **kwargs,
     ) -> None:
-
         super().__init__()
 
         if use_batch_norm:
             bias = False
 
         means = nn.Linear(in_features, out_features, bias=bias, **kwargs)
 
@@ -338,15 +327,14 @@
         batch_norm_momentum: float = 0.01,
         global_std_mode: Union[
             Literal["none"], Literal["replace"], Literal["multiply"]
         ] = "none",
         bias=True,
         **kwargs,
     ) -> None:
-
         super().__init__()
 
         if use_batch_norm:
             bias = False
 
         means = nn.ConvTranspose2d(
             in_channels=in_channels,
@@ -378,7 +366,61 @@
             activation_mode=activation_mode,
             use_batch_norm=use_batch_norm,
             batch_norm_mode=batch_norm_mode,
             batch_norm_eps=batch_norm_eps,
             batch_norm_momentum=batch_norm_momentum,
             global_std_mode=global_std_mode,
         )
+
+
+def init_weights(self):
+    init_type, *params = VariationalBase.INIT_WEIGHTS.split(":")
+
+    if init_type == "usual":
+        pass
+    elif init_type == "fill":
+        fill_what = params[0]
+        value_kernel = float(params[1])
+        value_bias = float(params[2])
+
+        def fill(target):
+            target.weight.data.fill_(value_kernel)
+            if target.bias:
+                target.bias.data.fill_(value_bias)
+
+        if "mean" in fill_what:
+            fill(self.means)
+
+        if "std" in fill_what:
+            fill(self.stds)
+    elif init_type == "xavier_uniform":
+        fill_what = params[0]
+        gain_kernel = float(params[1])
+        gain_bias = float(params[2])
+
+        def fill(target):
+            torch.nn.init.xavier_uniform_(target.weight, gain=gain_kernel)
+            if target.bias:
+                torch.nn.init.xavier_uniform_(target.bias, gain=gain_bias)
+
+        if "mean" in fill_what:
+            fill(self.means)
+
+        if "std" in fill_what:
+            fill(self.stds)
+    elif init_type == "xavier_normal":
+        fill_what = params[0]
+        gain_kernel = float(params[1])
+        gain_bias = float(params[2])
+
+        def fill(target):
+            torch.nn.init.xavier_normal_(target.weight, gain=gain_kernel)
+            if target.bias:
+                torch.nn.init.xavier_normal_(target.bias, gain=gain_bias)
+
+        if "mean" in fill_what:
+            fill(self.means)
+
+        if "std" in fill_what:
+            fill(self.stds)
+    else:
+        raise ValueError()
```

### Comparing `vnn-0.1.1/LICENSE` & `vnn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/README.md` & `vnn-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vnn-0.1.1/pyproject.toml` & `vnn-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [build-system]
 requires = ["hatchling", "torch"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vnn"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
-  {name="Illia Oleksiienko", email="io@ece.au.dk"},
-  {name="Dat Thanh Tran", email="viebboy@gmail.com"},
-  {name="Alexandros Iosifidis", email="ai@ece.au.dk"},
+  {name="Illia Oleksiienko, Dat Thanh Tran, Alexandros Iosifidis", email="io@ece.au.dk"},
 ]
 description = "Variational Neural Networks"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `vnn-0.1.1/PKG-INFO` & `vnn-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: vnn
-Version: 0.1.1
+Version: 0.2.0
 Summary: Variational Neural Networks
 Project-URL: Homepage, https://github.com/iliiliiliili/variational-nn-pytorch
 Project-URL: Bug Tracker, https://github.com/iliiliiliili/variational-nn-pytorch/issues
-Author-email: Illia Oleksiienko <io@ece.au.dk>, Dat Thanh Tran <viebboy@gmail.com>, Alexandros Iosifidis <ai@ece.au.dk>
+Author-email: "Illia Oleksiienko, Dat Thanh Tran, Alexandros Iosifidis" <io@ece.au.dk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

