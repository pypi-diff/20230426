# Comparing `tmp/bloptools-0.1.0.tar.gz` & `tmp/bloptools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloptools-0.1.0.tar", last modified: Sat Mar 11 02:09:26 2023, max compression
+gzip compressed data, was "bloptools-0.2.0.tar", last modified: Tue Apr 25 16:05:18 2023, max compression
```

## Comparing `bloptools-0.1.0.tar` & `bloptools-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-11 02:09:18.000000 bloptools-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-03-11 02:09:18.000000 bloptools-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-11 02:09:18.000000 bloptools-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-11 02:09:18.000000 bloptools-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-11 02:09:26.065558 bloptools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-11 02:09:18.000000 bloptools-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/bloptools/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-11 02:09:26.065558 bloptools-0.1.0/bloptools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/bloptools/gp/
--rw-r--r--   0 runner    (1001) docker     (123)    38473 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/gp/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/gp/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/gp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/bloptools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-11 02:09:18.000000 bloptools-0.1.0/bloptools/tests/test_gp_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/bloptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-11 02:09:26.000000 bloptools-0.1.0/bloptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-11 02:09:26.000000 bloptools-0.1.0/bloptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 02:09:26.000000 bloptools-0.1.0/bloptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-11 02:09:26.000000 bloptools-0.1.0/bloptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-11 02:09:26.000000 bloptools-0.1.0/bloptools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 02:09:26.065558 bloptools-0.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-11 02:09:18.000000 bloptools-0.1.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-11 02:09:18.000000 bloptools-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-11 02:09:18.000000 bloptools-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-11 02:09:26.065558 bloptools-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-11 02:09:18.000000 bloptools-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-03-11 02:09:18.000000 bloptools-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.037809 bloptools-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 16:05:06.000000 bloptools-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-25 16:05:06.000000 bloptools-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-25 16:05:06.000000 bloptools-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-25 16:05:06.000000 bloptools-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-25 16:05:18.037809 bloptools-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-25 16:05:06.000000 bloptools-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.037809 bloptools-0.2.0/bloptools/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 16:05:18.037809 bloptools-0.2.0/bloptools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/bo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools/de/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/de_opt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26559 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/de_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/de/hardware_flyer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/atf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/atf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/atf/atf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/nsls2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/nsls2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/nsls2/iss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/nsls2/tes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/shadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/shadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/shadow/chx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/shadow/tes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/experiments/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/experiments/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/bloptools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/test_bayesian_himmelblau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/tests/test_bayesian_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-25 16:05:06.000000 bloptools-0.2.0/bloptools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.029809 bloptools-0.2.0/bloptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 16:05:17.000000 bloptools-0.2.0/bloptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.033809 bloptools-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:05:18.037809 bloptools-0.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 16:05:06.000000 bloptools-0.2.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 16:05:06.000000 bloptools-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 16:05:06.000000 bloptools-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-25 16:05:18.037809 bloptools-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-25 16:05:06.000000 bloptools-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-04-25 16:05:06.000000 bloptools-0.2.0/versioneer.py
```

### Comparing `bloptools-0.1.0/CONTRIBUTING.rst` & `bloptools-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/LICENSE` & `bloptools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/PKG-INFO` & `bloptools-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloptools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Beamline Optimization Tools
 Home-page: https://github.com/NSLS-II/bloptools
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -24,13 +24,8 @@
 .. image:: https://img.shields.io/pypi/v/bloptools.svg
         :target: https://pypi.python.org/pypi/bloptools
 
 
 Beamline Optimization Tools
 
 * Free software: 3-clause BSD license
-* Documentation: (COMING SOON!) https://NSLS-II.github.io/bloptools.
-
-Features
---------
-
-* TODO
+* Documentation: https://NSLS-II.github.io/bloptools.
```

### Comparing `bloptools-0.1.0/bloptools/gp/kernels.py` & `bloptools-0.2.0/bloptools/bo/kernels.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,119 +3,134 @@
 import torch
 
 
 class LatentMaternKernel(gpytorch.kernels.Kernel):
     def __init__(
         self,
         n_dof,
-        length_scale_bounds,
         off_diag=True,
         **kwargs,
     ):
         super(LatentMaternKernel, self).__init__()
 
         self.n_dof = n_dof
         self.n_off_diag = int(n_dof * (n_dof - 1) / 2)
         self.off_diag = off_diag
 
-        inv_length_scale_bounds = (1 / length_scale_bounds[1], 1 / length_scale_bounds[0])
-
-        output_scale_constraint = gpytorch.constraints.Positive()
-        trans_diagonal_constraint = gpytorch.constraints.Interval(*inv_length_scale_bounds)
+        # output_scale_constraint = gpytorch.constraints.Positive()
+        trans_diagonal_constraint = gpytorch.constraints.Interval(2e0, 2e1)
         trans_off_diag_constraint = gpytorch.constraints.Interval(-1e0, 1e0)
 
         trans_diagonal_initial = np.sqrt(
             trans_diagonal_constraint.lower_bound * trans_diagonal_constraint.upper_bound
         )
         raw_trans_diagonal_initial = trans_diagonal_constraint.inverse_transform(trans_diagonal_initial)
 
-        self.register_parameter(
-            name="raw_output_scale", parameter=torch.nn.Parameter(torch.ones(*self.batch_shape, 1))
-        )
+        # self.register_parameter(
+        #    name="raw_output_scale", parameter=torch.nn.Parameter(torch.ones(*self.batch_shape, 1).double())
+        # )
         self.register_parameter(
             name="raw_trans_diagonal",
-            parameter=torch.nn.Parameter(raw_trans_diagonal_initial * torch.ones(*self.batch_shape, self.n_dof)),
+            parameter=torch.nn.Parameter(
+                raw_trans_diagonal_initial * torch.ones(*self.batch_shape, self.n_dof).double()
+            ),
         )
 
-        self.register_constraint("raw_output_scale", output_scale_constraint)
+        # self.register_constraint("raw_output_scale", output_scale_constraint)
         self.register_constraint("raw_trans_diagonal", trans_diagonal_constraint)
 
         if self.off_diag:
             self.register_parameter(
                 name="raw_trans_off_diag",
-                parameter=torch.nn.Parameter(torch.zeros(*self.batch_shape, self.n_off_diag)),
+                parameter=torch.nn.Parameter(torch.zeros(*self.batch_shape, self.n_off_diag).double()),
             )
             self.register_constraint("raw_trans_off_diag", trans_off_diag_constraint)
 
-    @property
-    def output_scale(self):
-        return self.raw_output_scale_constraint.transform(self.raw_output_scale)
+    # @property
+    # def output_scale(self):
+    #     return self.raw_output_scale_constraint.transform(self.raw_output_scale)
 
     @property
     def trans_diagonal(self):
         return self.raw_trans_diagonal_constraint.transform(self.raw_trans_diagonal)
 
     @property
     def trans_off_diag(self):
         return self.raw_trans_off_diag_constraint.transform(self.raw_trans_off_diag)
 
-    @output_scale.setter
-    def output_scale(self, value):
-        self._set_output_scale(value)
+    # @output_scale.setter
+    # def output_scale(self, value):
+    #     self._set_output_scale(value)
 
     @trans_diagonal.setter
     def trans_diagonal(self, value):
         self._set_trans_diagonal(value)
 
     @trans_off_diag.setter
     def trans_off_diag(self, value):
         self._set_trans_off_diag(value)
 
     def _set_trans_off_diag(self, value):
         if not torch.is_tensor(value):
             value = torch.as_tensor(value).to(self.raw_trans_off_diag)
         self.initialize(raw_trans_off_diag=self.raw_trans_off_diag_constraint.inverse_transform(value))
 
-    def _set_output_scale(self, value):
-        if not torch.is_tensor(value):
-            value = torch.as_tensor(value).to(self.raw_output_scale)
-        self.initialize(raw_output_scale=self.raw_output_scale_constraint.inverse_transform(value))
+    # def _set_output_scale(self, value):
+    #     if not torch.is_tensor(value):
+    #         value = torch.as_tensor(value).to(self.raw_output_scale)
+    #     self.initialize(raw_output_scale=self.raw_output_scale_constraint.inverse_transform(value))
 
     def _set_trans_diagonal(self, value):
         if not torch.is_tensor(value):
             value = torch.as_tensor(value).to(self.raw_trans_diagonal)
         self.initialize(raw_trans_diagonal=self.raw_trans_diagonal_constraint.inverse_transform(value))
 
     @property
     def trans_matrix(self):
-        T = torch.eye(self.n_dof)
-        if self.off_diag:
-            T[np.triu_indices(self.n_dof, k=1)] = self.trans_off_diag
+        # no rotations
+        if not self.off_diag:
+            T = torch.eye(self.n_dof).double()
+
+        # construct an orthogonal matrix. fun fact: exp(skew(N)) is the generator of SO(N)
+        else:
+            A = torch.zeros((self.n_dof, self.n_dof)).double()
+            A[np.triu_indices(self.n_dof, k=1)] = self.trans_off_diag
+            A += -A.T
+            T = torch.linalg.matrix_exp(A)
+
         T = torch.matmul(torch.diag(self.trans_diagonal), T)
+
         return T
 
-    def forward(self, x1, x2, diag=False, last_dim_is_batch=False, **params):
+    def forward(self, x1, x2=None, diag=False, auto=False, last_dim_is_batch=False, **params):
         # returns the homoskedastic diagonal
         if diag:
-            return torch.square(self.output_scale[0]) * torch.ones((*self.batch_shape, *x1.shape[:-1]))
+            # return torch.square(self.output_scale[0]) * torch.ones((*self.batch_shape, *x1.shape[:-1]))
+            return torch.ones((*self.batch_shape, *x1.shape[:-1]))
+
+        # computes the autocovariance of the process at the parameters
+        if auto:
+            x2 = x1
 
         # x1 and x2 are arrays of shape (..., n_1, n_dof) and (..., n_2, n_dof)
-        _x1, _x2 = torch.as_tensor(x1).float(), torch.as_tensor(x2).float()
+        _x1, _x2 = torch.as_tensor(x1).double(), torch.as_tensor(x2).double()
 
         # dx has shape (..., n_1, n_2, n_dof)
         dx = _x1.unsqueeze(-2) - _x2.unsqueeze(-3)
 
-        # transform coordinate frame with hyperparameters (this applies lengthscale and rotations)
+        # transform coordinates with hyperparameters (this applies lengthscale and rotations)
         trans_dx = torch.matmul(self.trans_matrix, dx.unsqueeze(-1))
 
         # total transformed distance. D has shape (..., n_1, n_2)
         d_eff = torch.sqrt(torch.matmul(trans_dx.transpose(-1, -2), trans_dx).sum((-1, -2)) + 1e-12)
 
         # Matern covariance of effective order nu=3/2.
         # nu=3/2 is a special case and has a concise closed-form expression
         # In general, this is something between an exponential (n=1/2) and a Gaussian (n=infinity)
         # https://en.wikipedia.org/wiki/Matern_covariance_function
-        C = torch.square(self.output_scale[0]) * (1 + d_eff) * torch.exp(-d_eff)
+        C = (1 + d_eff) * torch.exp(-d_eff)
+
+        # C = torch.square(self.output_scale[0]) * torch.exp(-torch.square(d_eff))
 
         # print(f'{diag = } {C.shape = }')
 
         return C
```

### Comparing `bloptools-0.1.0/bloptools/tests/conftest.py` & `bloptools-0.2.0/bloptools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/bloptools/tests/test_gp_optimizer.py` & `bloptools-0.2.0/bloptools/tests/test_bayesian_shadow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 import numpy as np
+import pytest
 from sirepo_bluesky.sirepo_ophyd import create_classes
 
-from bloptools.gp import Optimizer
+from bloptools.bo import BayesianOptimizationAgent
+from bloptools.experiments.shadow import tes
 
 
-def test_shadow_gp_optimizer(RE, db, shadow_tes_simulation):
+@pytest.mark.shadow
+def test_tes_shadow_boa(RE, db, shadow_tes_simulation):
     data, schema = shadow_tes_simulation.auth("shadow", "00000002")
     classes, objects = create_classes(shadow_tes_simulation.data, connection=shadow_tes_simulation)
     globals().update(**objects)
 
     data["models"]["simulation"]["npoint"] = 100000
     data["models"]["watchpointReport12"]["histogramBins"] = 32
 
-    dofs = [kbv.x_rot, kbv.offz]  # noqa F821
+    kbs = [kbv.x_rot, kbv.offz]
+    kb_bounds = np.array([[-0.10, +0.10], [-0.50, +0.50]])
 
-    hard_bounds = np.array([[-0.10, +0.10], [-0.50, +0.50]])
-
-    for dof in dofs:
+    for dof in kbs:
         dof.kind = "hinted"
 
-    gpo = Optimizer(
-        init_scheme="quasi-random",
-        n_init=4,
-        run_engine=RE,
-        db=db,
-        detector=w9,  # noqa F821
-        detector_type="image",
-        dofs=dofs,
-        dof_bounds=hard_bounds,
-        fitness_model="max_sep_density",
-        training_iter=100,
-        verbose=True,
-    )
+    boa = BayesianOptimizationAgent(dofs=kbs, dets=[w9], bounds=kb_bounds, db=db, experiment=tes)
+
+    RE(boa.initialize(init_scheme="quasi-random", n_init=8))
 
-    gpo.learn(n_iter=1, n_per_iter=1, strategy="explore", greedy=True, reuse_hypers=False)
-    gpo.learn(n_iter=1, n_per_iter=1, strategy="exploit", greedy=True, reuse_hypers=False)
+    RE(boa.learn(strategy="eI", n_iter=2, n_per_iter=3))
+    RE(boa.learn(strategy="eGIBBON", n_iter=2, n_per_iter=3))
 
-    gpo.plot_state(gridded=True)
-    gpo.plot_fitness()
+    boa.plot_state(gridded=True)
```

### Comparing `bloptools-0.1.0/bloptools.egg-info/PKG-INFO` & `bloptools-0.2.0/bloptools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloptools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Beamline Optimization Tools
 Home-page: https://github.com/NSLS-II/bloptools
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -24,13 +24,8 @@
 .. image:: https://img.shields.io/pypi/v/bloptools.svg
         :target: https://pypi.python.org/pypi/bloptools
 
 
 Beamline Optimization Tools
 
 * Free software: 3-clause BSD license
-* Documentation: (COMING SOON!) https://NSLS-II.github.io/bloptools.
-
-Features
---------
-
-* TODO
+* Documentation: https://NSLS-II.github.io/bloptools.
```

### Comparing `bloptools-0.1.0/docs/Makefile` & `bloptools-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/docs/make.bat` & `bloptools-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/docs/source/conf.py` & `bloptools-0.2.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "IPython.sphinxext.ipython_directive",
     "IPython.sphinxext.ipython_console_highlighting",
     "matplotlib.sphinxext.plot_directive",
     "numpydoc",
     "sphinx_copybutton",
+    "nbsphinx",
 ]
 
 # Configuration options for plot_directive. See:
 # https://github.com/matplotlib/matplotlib/blob/f3ed922d935751e08494e5fb5311d3050a3b637b/lib/matplotlib/sphinxext/plot_directive.py#L81
 plot_html_show_source_link = False
 plot_html_show_formats = False
```

### Comparing `bloptools-0.1.0/docs/source/min_versions.rst` & `bloptools-0.2.0/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/docs/source/release-history.rst` & `bloptools-0.2.0/docs/source/release-history.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 ===============
 Release History
 ===============
 
 
+v0.2.0 (2023-04-25)
+-------------------
+
+- Rebased the Bayesian optimization models to be compatible with ``botorch`` code.
+- Optimization objectives can be customized with ``experiment`` modules.
+- Added optimization test functions for quicker testing and development.
+
+
 v0.1.0 (2023-03-10)
 -------------------
 
 - Changed from using ``SafeConfigParser`` to ``ConfigParser``.
 - Implemented the initial version of the GP optimizer.
 - Updated the repo structure based on the new cookiecutter.
 - Added tests to the CI.
```

### Comparing `bloptools-0.1.0/setup.py` & `bloptools-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.1.0/versioneer.py` & `bloptools-0.2.0/versioneer.py`

 * *Files identical despite different names*

