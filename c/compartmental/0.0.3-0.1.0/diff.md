# Comparing `tmp/compartmental-0.0.3.tar.gz` & `tmp/compartmental-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compartmental-0.0.3.tar", last modified: Sat Mar 18 13:05:16 2023, max compression
+gzip compressed data, was "compartmental-0.1.0.tar", last modified: Tue Apr 25 21:50:30 2023, max compression
```

## Comparing `compartmental-0.0.3.tar` & `compartmental-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:05:16.000567 compartmental-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-03-18 13:04:59.000000 compartmental-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-18 13:04:59.000000 compartmental-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-18 13:05:16.000567 compartmental-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-18 13:04:59.000000 compartmental-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:05:16.000567 compartmental-0.0.3/compartmental/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-18 13:04:59.000000 compartmental-0.0.3/compartmental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-03-18 13:04:59.000000 compartmental-0.0.3/compartmental/generic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:05:16.000567 compartmental-0.0.3/compartmental/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-18 13:04:59.000000 compartmental-0.0.3/compartmental/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-18 13:04:59.000000 compartmental-0.0.3/compartmental/parameters/parameters_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-03-18 13:04:59.000000 compartmental-0.0.3/compartmental/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:05:16.000567 compartmental-0.0.3/compartmental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-18 13:05:15.000000 compartmental-0.0.3/compartmental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-18 13:04:59.000000 compartmental-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-18 13:05:16.000567 compartmental-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-18 13:04:59.000000 compartmental-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:50:30.463274 compartmental-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-25 21:50:00.000000 compartmental-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-25 21:50:00.000000 compartmental-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-25 21:50:30.467274 compartmental-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-25 21:50:00.000000 compartmental-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:50:30.463274 compartmental-0.1.0/compartmental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 21:50:00.000000 compartmental-0.1.0/compartmental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-25 21:50:00.000000 compartmental-0.1.0/compartmental/generic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:50:30.463274 compartmental-0.1.0/compartmental/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-25 21:50:00.000000 compartmental-0.1.0/compartmental/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-25 21:50:00.000000 compartmental-0.1.0/compartmental/parameters/parameters_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-04-25 21:50:00.000000 compartmental-0.1.0/compartmental/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:50:30.463274 compartmental-0.1.0/compartmental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-25 21:50:30.000000 compartmental-0.1.0/compartmental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 21:50:00.000000 compartmental-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 21:50:30.467274 compartmental-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 21:50:00.000000 compartmental-0.1.0/setup.py
```

### Comparing `compartmental-0.0.3/LICENSE` & `compartmental-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compartmental-0.0.3/PKG-INFO` & `compartmental-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: compartmental
-Version: 0.0.3
-Author-email: Unai Lería Fortea <unaileria@gmail.com>
-Maintainer-email: Unai Lería Fortea <unaileria@gmail.com>
-License: Apache License 2.0
-Project-URL: GitHub, https://github.com/${USERNAME}/compartmental
-Project-URL: Documentation, https://${USERNAME}/.github.io/compartmental/
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- Copyright 2023 Unai Lería Fortea & Pablo Vizcaíno García
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
@@ -35,24 +23,56 @@
 [![Wheel](https://img.shields.io/pypi/wheel/compartmental)](https://pypi.org/project/compartmental/)
 
 <br></br>
 <h1 align="center">
 compartmental
 </h1>
 <h2 align="center">
-.
-</h2><br></br>
-<h3 align="center">
-.
-</h3><br></br>
-
-
+Utility tools for Approximate Bayesian computation on compartmental models 
+</h2>
 
+<br>
 <div align="center">
 
 <a href="https://quanticpony.github.io/compartmental/">
 <img src=https://img.shields.io/github/deployments/QuanticPony/compartmental/github-pages?label=documentation>
 </a>
-<br></br>
+<br></br></br>
+<h3 align="center">
+
+</h3>
+
+
+
+
 
 </div>
-<br></br>
+
+# Instalation
+**compartmental** releases are available as wheel packages on [PyPI](https://pypi.org/project/compartmental/). You can install the last version using `pip`:
+```
+pip install compartmental
+```
+
+
+# Documentation
+Documentations is automatically generated from code on main push and hosted in github-pages [here](https://quanticpony.github.io/compartmental/).
+
+# Help
+Just open an issue with the `question` tag ([or clic here](https://github.com/QuanticPony/compartmental/issues/new?assignees=QuanticPony&labels=question&template=question.md&title=)), I would love to help!
+
+# Contributing
+You can contribute with:
+
+* Examples
+* Documentation
+* [Bug report/fix](https://github.com/QuanticPony/compartmental/issues/new?assignees=QuanticPony&labels=bug&template=bug_report.md&title=)
+* [Features](https://github.com/QuanticPony/compartmental/issues/new?assignees=QuanticPony&labels=new-feature&template=feature_request.md&title=)
+* Code
+
+Even only feedback is greatly apreciated. 
+
+Just create an issue and let me know you want to help! 
+
+
+# Licensing
+**compartmental** is released under the **Apache License Version 2.0**.
```

#### html2text {}

```diff
@@ -1,26 +1,34 @@
-Metadata-Version: 2.1 Name: compartmental Version: 0.0.3 Author-email: Unai
-LerÃ­a Fortea
-gmail.com> Maintainer-email: Unai LerÃ­a Fortea
-gmail.com> License: Apache License 2.0 Project-URL: GitHub, https://github.com/
-${USERNAME}/compartmental Project-URL: Documentation, https://$
-{USERNAME}/.github.io/compartmental/ Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE  [![PyPI Downloads](https://
-img.shields.io/pypi/dm/compartmental.svg?label=downloads)](https://pypi.org/
-project/compartmental/) [![PyPI Version](https://img.shields.io/pypi/v/
-compartmental?)](https://pypi.org/project/compartmental/) ![Commit activity]
-(https://img.shields.io/github/commit-activity/m/QuanticPony/compartmental) [!
-[License](https://img.shields.io/pypi/l/compartmental)](LICENSE) [![Build]
-(https://img.shields.io/github/actions/workflow/status/QuanticPony/
-compartmental/ci-master.yml)](https://github.com/QuanticPony/compartmental/
-actions) [![Python Version](https://img.shields.io/pypi/pyversions/
-compartmental)](https://pypi.org/project/compartmental/) [![Wheel](https://
-img.shields.io/pypi/wheel/compartmental)](https://pypi.org/project/
-compartmental/)
+ [![PyPI Downloads](https://img.shields.io/pypi/dm/
+compartmental.svg?label=downloads)](https://pypi.org/project/compartmental/) [!
+[PyPI Version](https://img.shields.io/pypi/v/compartmental?)](https://pypi.org/
+project/compartmental/) ![Commit activity](https://img.shields.io/github/
+commit-activity/m/QuanticPony/compartmental) [![License](https://
+img.shields.io/pypi/l/compartmental)](LICENSE) [![Build](https://
+img.shields.io/github/actions/workflow/status/QuanticPony/compartmental/ci-
+master.yml)](https://github.com/QuanticPony/compartmental/actions) [![Python
+Version](https://img.shields.io/pypi/pyversions/compartmental)](https://
+pypi.org/project/compartmental/) [![Wheel](https://img.shields.io/pypi/wheel/
+compartmental)](https://pypi.org/project/compartmental/)
                           ****** compartmental ******
-                                 ***** . *****
-
-                                  **** . ****
+   ***** Utility tools for Approximate Bayesian computation on compartmental
+                                 models *****
 
  [https://img.shields.io/github/deployments/QuanticPony/compartmental/github-
                           pages?label=documentation]
-
+# Instalation **compartmental** releases are available as wheel packages on
+[PyPI](https://pypi.org/project/compartmental/). You can install the last
+version using `pip`: ``` pip install compartmental ``` # Documentation
+Documentations is automatically generated from code on main push and hosted in
+github-pages [here](https://quanticpony.github.io/compartmental/). # Help Just
+open an issue with the `question` tag ([or clic here](https://github.com/
+QuanticPony/compartmental/issues/
+new?assignees=QuanticPony&labels=question&template=question.md&title=)), I
+would love to help! # Contributing You can contribute with: * Examples *
+Documentation * [Bug report/fix](https://github.com/QuanticPony/compartmental/
+issues/new?assignees=QuanticPony&labels=bug&template=bug_report.md&title=) *
+[Features](https://github.com/QuanticPony/compartmental/issues/
+new?assignees=QuanticPony&labels=new-
+feature&template=feature_request.md&title=) * Code Even only feedback is
+greatly apreciated. Just create an issue and let me know you want to help! #
+Licensing **compartmental** is released under the **Apache License Version
+2.0**.
```

### Comparing `compartmental-0.0.3/compartmental/__init__.py` & `compartmental-0.1.0/compartmental/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
  
-__version__ = "0.0.3"
+__version__ = "0.1.0"
 _CUPY_MODE_: bool
 
 from . import generic_model
 from . import util
 from . import parameters
 
 def use_cupy():
@@ -34,8 +34,8 @@
 def update_packages(CNP):
     generic_model.CNP = CNP
     util.CNP = CNP
     parameters.parameters_manager.CNP = CNP
 
 use_numpy()
 
-GenericModel = generic_model.GenericModel
+from .generic_model import GenericModel
```

### Comparing `compartmental-0.0.3/compartmental/generic_model.py` & `compartmental-0.1.0/compartmental/generic_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
  
-import __future__
-from io import TextIOWrapper
+from __future__ import annotations
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     import numpy as CNP
 
-from .parameters import ParametersManager
+
 from .util import *
+from .parameters import ParametersManager
+
 import copy
 
 class GenericModel:
-    """Creates a compartimental model from a dictionary and setting an `evolve` method.
+    """Creates a compartmental model from a dictionary and setting an `evolve` method.
     """
 
     def get_all_params_names(self):
         """Returns a set of all parameters names, fixed or not.
 
         Returns:
             (set[str]): Set of all parameters names.
@@ -42,80 +43,74 @@
         Args:
             configuration (dict[str, Any]): Model configuration.
         """
         self.configuration: dict[str, Any] = copy.deepcopy(configuration)
         
         self.param_to_index: dict[str, int] = { k:i for i,k in enumerate(self.configuration["params"].keys()) }
         self.fixed_param_to_index: dict[str, int] = { k:i for i,k in enumerate(self.configuration["fixed_params"].keys()) }
-        self.compartiment_name_to_index: dict[str, int] = { k:i for i,k in enumerate(self.configuration["compartiments"].keys()) }
+        self.compartment_name_to_index: dict[str, int] = { k:i for i,k in enumerate(self.configuration["compartments"].keys()) }
 
 
     def populate_model_parameters(self, **kargs):
         """Populates params array. Assigns shortcuts to call them by their name as an attribute.
         """
         parameter_manager = ParametersManager(self.configuration, self)
         
         REFERENCE_OFFSET = self.configuration["reference"].get("offset", 0)
         # Set offset value if it is a str reference
         if isinstance(REFERENCE_OFFSET, str):
             self.configuration["params"][REFERENCE_OFFSET].update({"type":"int"})
-        
-        N_SIMULATIONS = self.configuration["simulation"]["n_simulations"]
-        self.params = CNP.zeros(
-            (len(self.configuration["params"]), N_SIMULATIONS), dtype=CNP.float64
-        )
-        self.fixed_params = CNP.zeros(
-            (len(self.configuration["fixed_params"]), 1), dtype=CNP.float64
-        )
+
+        parameter_manager.populate_params(**kargs)
+        parameter_manager.populate_fixed_params()
         
         for param in self.configuration["params"].keys():
-            setattr(self, param, self.params[self.param_to_index[param]])
+            setattr(self, param, self.params[param])
             
         for fparam in self.configuration["fixed_params"].keys():
             setattr(self, fparam, self.fixed_params[self.fixed_param_to_index[fparam]])
             
         if isinstance(REFERENCE_OFFSET, str):
-            self.reference_offset = self.params[self.param_to_index[REFERENCE_OFFSET]]
+            self.reference_offset = self.params[REFERENCE_OFFSET]
         else:
             self.reference_offset = 0
             
-        parameter_manager.populate_params(self.params, **kargs)
-        parameter_manager.populate_fixed_params(self.fixed_params)
+
         
         
-    def populate_model_compartiments(self, **kargs):
-        """Populates compartiments array. Assigns shortcuts to call them by their name as an attribute.
+    def populate_model_compartments(self, **kargs):
+        """Populates compartments array. Assigns shortcuts to call them by their name as an attribute.
         """
         N_SIMULATIONS = self.configuration["simulation"]["n_simulations"]
         self.state = CNP.zeros(
-            (len(self.configuration["compartiments"]), N_SIMULATIONS), dtype=CNP.float64
+            (len(self.configuration["compartments"]), N_SIMULATIONS), dtype=CNP.float64
         )
         self.log_diff = CNP.zeros((N_SIMULATIONS, 1), dtype=CNP.float64)
         
-        for c,i in self.compartiment_name_to_index.items():
-            C = self.configuration["compartiments"][c]
+        for c,i in self.compartment_name_to_index.items():
+            C = self.configuration["compartments"][c]
             initial_value = C["initial_value"]
             if isinstance(initial_value, str):
                 if initial_value in self.param_to_index.keys():
-                    self.state[i,:] = self.params[self.param_to_index[initial_value]]
+                    self.state[i,:] = self.params[initial_value]
                 continue
             self.state[i,:] = initial_value
            
-        for c,i in self.compartiment_name_to_index.items():
-            C = self.configuration["compartiments"][c]
-            minus = C.get("minus_compartiments", False)
+        for c,i in self.compartment_name_to_index.items():
+            C = self.configuration["compartments"][c]
+            minus = C.get("minus_compartments", False)
             if not minus:
                 continue
             if not isinstance(minus, list):
                 minus = [minus]
             for m in minus:
-                self.state[i,:] -= self.state[self.compartiment_name_to_index[m],:]
+                self.state[i,:] -= self.state[self.compartment_name_to_index[m],:]
                 
-        for comp in self.configuration["compartiments"].keys():
-            setattr(self, comp, self.state[self.compartiment_name_to_index[comp]])
+        for comp in self.configuration["compartments"].keys():
+            setattr(self, comp, self.state[self.compartment_name_to_index[comp]])
                 
 
     def evolve(self, step, *args, **kargs):
         """This method must be overwritten to complete the model initialization.
 
         Args:
             step (int): Step of simulation. Simulation ends when `step = simulation.n_steps`
@@ -131,78 +126,88 @@
             step (int): Step of simulation. Simulation ends when `step = simulation.n_steps`
             reference (list[list[float]]): Reference(s) values.
             reference_mask (list[int]): Mask to obtain simulation values to compare with the reference(s). 
 
         Returns:
             (list[float]): Distance from simulations to reference(s).
         """
-        index = CNP.clip(step + CNP.int64(self.reference_offset), 0, self.N_STEPS-1)
-        diff = CNP.absolute(CNP.take(self.state, reference_mask, 0)[0].T-reference[index])
+        index = step + self.reference_offset
+        # To only take the diff on the same range for all simulations
+        diff = CNP.absolute(CNP.take(self.state, reference_mask, 0)[0].T-reference[CNP.clip(index, 0, self.N_STEPS-1)]) * \
+               ((self.reference_offset.max()<=index) * (index<=self.N_STEPS))
+               
         return CNP.log(diff + 1)
 
 
-    def _internal_run_(self, inner, inner_args: list, outer, outer_args:list,  reference, save_file:str, *args, **kargs):
+    def _internal_run_(self, inner, inner_args: list, outer, outer_args:list,  reference, save_file:str, *args, exclude_pupulate:bool=False, **kargs):
         """Internal function that executes the model.
 
         Args:
             inner (function): Function to call in the main loop.
             inner_args (list): Args given to `inner`.
             outer (function): Function to call after the main loop.
             outer_args (list): Args given to `outer`.
             reference (list[list[float]]): Reference values used to compare with the simulation.
             save_file (str): Filename of path to file.
+            exclude_populate (bool, optional): If `False` params and compartments are populated with random values. Defaults to False.
         """
         N_EXECUTIONS = self.configuration["simulation"]["n_executions"]
-        REFERENCE_OFFSET = self.configuration["reference"].get("offset", 0)
         self.N_STEPS = self.configuration["simulation"]["n_steps"]
-        
+
         for execution in range(N_EXECUTIONS):
             progress_bar(f"Model running: ", execution, N_EXECUTIONS, len=min(20, max(N_EXECUTIONS,5)))
-            self.log_diff[:] = 0
-            self.populate_model_parameters(**kargs)
-            self.populate_model_compartiments(**kargs)
             
-            for step in range(self.N_STEPS):
+            if not exclude_pupulate:
+                self.populate_model_parameters(**kargs)
+                self.populate_model_compartments(**kargs)
+
+            self._min_offset_: int = self.reference_offset.min()
+            self.log_diff[:] = 0
+
+            # for step in range(self.N_STEPS):
+            step = CNP.int64(0)
+            while (self.reference_offset + step < self.N_STEPS).any():
                 inner(self, step, reference, *inner_args, **kargs)
+                step += 1
             outer(self, *outer_args, execution_number=execution, **kargs)
             
         progress_bar(f"Model running: ", N_EXECUTIONS, N_EXECUTIONS, len=min(20, max(N_EXECUTIONS,5)), end='\n')
 
 
     def run_no_diff(self, save_file: str, *args, **kargs):
         """Runs the model without computing the diference any reference(s).
 
         Args:
             save_file (str): Filename of path to file.
         """
         self._internal_run_(
             self.evolve, args, 
             save_parameters_no_diff, (save_file, self.param_to_index.keys(),  self.params), 
-            None, save_file, 
+            None, save_file,
             *args, **kargs
         )
 
 
     def run(self, reference, save_file: str, *args, **kargs):
         """Runs the model computing the diference from the reference(s).
 
         Args:
             reference (list[list[float]]): Reference(s) values.
             save_file (str): Filename of path to file.
         """
         
-        reference_mask = CNP.array([self.compartiment_name_to_index[c] for c in self.configuration["reference"]["compartiments"]])
+        reference_mask = CNP.array([self.compartment_name_to_index[c] for c in self.configuration["reference"]["compartments"]])
         
         def inner(model, step, reference, reference_mask, *args, **kargs):
             model.evolve(model, step, *args, **kargs)
             self.log_diff[:,0] += model.get_diff(step, reference, reference_mask)
         
-        def outer(model, save_file, *args, **kargs):
+        def outer(model, save_file, *args, execution_number, **kargs):
             best_params, best_log_diff = get_best_parameters(model.params, model.log_diff, model.configuration["results"]["save_percentage"])
-            save_parameters(save_file, model.param_to_index.keys(), best_params, best_log_diff)
+            save_parameters(save_file, model.param_to_index.keys(), best_params, best_log_diff, execution_number=execution_number)
             
         self._internal_run_(
-            inner, (reference_mask,), 
+            inner, (reference_mask, *args), 
             outer, (save_file,), 
             reference, save_file, 
             *args, **kargs
         )
```

### Comparing `compartmental-0.0.3/compartmental/parameters/__init__.py` & `compartmental-0.1.0/compartmental/parameters/__init__.py`

 * *Files identical despite different names*

