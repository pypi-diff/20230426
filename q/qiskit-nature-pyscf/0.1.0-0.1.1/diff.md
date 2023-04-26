# Comparing `tmp/qiskit-nature-pyscf-0.1.0.tar.gz` & `tmp/qiskit-nature-pyscf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-nature-pyscf-0.1.0.tar", last modified: Mon Nov  7 20:39:13 2022, max compression
+gzip compressed data, was "dist/qiskit-nature-pyscf-0.1.1.tar", last modified: Wed Apr 26 21:41:33 2023, max compression
```

## Comparing `qiskit-nature-pyscf-0.1.0.tar` & `qiskit-nature-pyscf-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11416 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3184 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9700 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/qiskit_solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:39:13.000000 qiskit-nature-pyscf-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/test/nature_pyscf_test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/test/test_qiskit_solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-11-07 20:39:00.000000 qiskit-nature-pyscf-0.1.0/test/test_readme_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/qiskit_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/nature_pyscf_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/test_qiskit_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/test_readme_sample.py
```

### Comparing `qiskit-nature-pyscf-0.1.0/LICENSE.txt` & `qiskit-nature-pyscf-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/PKG-INFO` & `qiskit-nature-pyscf-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-nature-pyscf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Qiskit Nature PySCF: Third-party integration plugin of Qiskit Nature + PySCF.
 Home-page: https://github.com/qiskit-community/qiskit-nature-pyscf
 Author: Qiskit Nature PySCF Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
 Keywords: qiskit sdk quantum nature chemistry physics pyscf
 Classifier: Environment :: Console
@@ -27,22 +27,22 @@
 
 [![License](https://img.shields.io/github/license/qiskit-community/qiskit-nature-pyscf.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
 
 **Qiskit Nature PySCF** is a third-party integration plugin of Qiskit Nature + PySCF.
 
 ## Installation
 
-We encourage installing Qiskit Nature via the pip tool (a python package manager).
+We encourage installing Qiskit Nature PySCF via the pip tool (a python package manager).
 
 ```bash
 pip install qiskit-nature-pyscf
 ```
 
 **pip** will handle all dependencies automatically and you will always install the latest
-(and well-tested) version.
+(and well-tested) version. It will also install Qiskit Nature if needed.
 
 If you want to work on the very latest work-in-progress versions, either to try features ahead of
 their official release or if you want to contribute to Qiskit Nature PySCF, then you can install from source.
 
 
 ## Usage
 
@@ -56,38 +56,64 @@
 directly into your `CASCI` or `CASSCF` simulation objects of PySCF.
 
 Below we show a simple example of how to do this.
 
 ```python
 from pyscf import gto, scf, mcscf
 
+import numpy as np
+
+from qiskit.algorithms.minimum_eigensolvers import VQE
 from qiskit.algorithms.optimizers import SLSQP
 from qiskit.primitives import Estimator
-from qiskit_nature.second_q.algorithms import GroundStateEigensolver, VQEUCCFactory
-from qiskit_nature.second_q.circuit.library import UCCSD
-from qiskit_nature.second_q.mappers import ParityMapper, QubitConverter
+from qiskit_nature.second_q.algorithms import GroundStateEigensolver
+from qiskit_nature.second_q.circuit.library import HartreeFock, UCCSD
+from qiskit_nature.second_q.mappers import ParityMapper
 
 from qiskit_nature_pyscf import QiskitSolver
 
 mol = gto.M(atom="Li 0 0 0; H 0 0 1.6", basis="sto-3g")
 
 h_f = scf.RHF(mol).run()
 
-norb, nelec = 2, 2
+norb = 2
+nalpha, nbeta = 1, 1
+nelec = nalpha + nbeta
 
 cas = mcscf.CASCI(h_f, norb, nelec)
 
-converter = QubitConverter(ParityMapper(), two_qubit_reduction=True)
+mapper = ParityMapper(num_particles=(nalpha, nbeta))
+
+ansatz = UCCSD(
+    norb,
+    (nalpha, nbeta),
+    mapper,
+    initial_state=HartreeFock(
+        norb,
+        (nalpha, nbeta),
+        mapper,
+    ),
+)
 
-vqe = VQEUCCFactory(Estimator(), UCCSD(), SLSQP())
+vqe = VQE(Estimator(), ansatz, SLSQP())
+vqe.initial_point = np.zeros(ansatz.num_parameters)
 
-algorithm = GroundStateEigensolver(converter, vqe)
+algorithm = GroundStateEigensolver(mapper, vqe)
 
 cas.fcisolver = QiskitSolver(algorithm)
 
 cas.run()
 ```
 
 More detailed documentation can be found at
 [Documentation](https://qiskit-community.github.io/qiskit-nature-pyscf/). For more detailed 
 explanations we recommend to check out the documentation of
 [PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/documentation/nature/).
+
+
+## Citation
+
+If you use this plugin, please cite the following references:
+
+- PySCF, as per [these instructions](https://github.com/pyscf/pyscf#citing-pyscf).
+- Qiskit, as per the provided [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+- Qiskit Nature, as per https://doi.org/10.5281/zenodo.7828767
```

### Comparing `qiskit-nature-pyscf-0.1.0/README.md` & `qiskit-nature-pyscf-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 [![License](https://img.shields.io/github/license/qiskit-community/qiskit-nature-pyscf.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)<!--- long-description-skip-begin -->[![Build Status](https://github.com/qiskit-community/qiskit-nature-pyscf/workflows/Nature%20PySCF%20Unit%20Tests/badge.svg?branch=main)](https://github.com/qiskit-community/qiskit-nature-pyscf/actions?query=workflow%3A"Nature%20PySCF%20Unit%20Tests"+branch%3Amain+event%3Apush)[![](https://img.shields.io/github/release/qiskit-community/qiskit-nature-pyscf.svg?style=popout-square)](https://github.com/qiskit-community/qiskit-nature-pyscf/releases)[![](https://img.shields.io/pypi/dm/qiskit-nature-pyscf.svg?style=popout-square)](https://pypi.org/project/qiskit-nature-pyscf/)[![Coverage Status](https://coveralls.io/repos/github/qiskit-community/qiskit-nature-pyscf/badge.svg?branch=main)](https://coveralls.io/github/qiskit-community/qiskit-nature-pyscf?branch=main)<!--- long-description-skip-end -->
 
 **Qiskit Nature PySCF** is a third-party integration plugin of Qiskit Nature + PySCF.
 
 ## Installation
 
-We encourage installing Qiskit Nature via the pip tool (a python package manager).
+We encourage installing Qiskit Nature PySCF via the pip tool (a python package manager).
 
 ```bash
 pip install qiskit-nature-pyscf
 ```
 
 **pip** will handle all dependencies automatically and you will always install the latest
-(and well-tested) version.
+(and well-tested) version. It will also install Qiskit Nature if needed.
 
 If you want to work on the very latest work-in-progress versions, either to try features ahead of
 their official release or if you want to contribute to Qiskit Nature PySCF, then you can install from source.
 
 
 ## Usage
 
@@ -31,38 +31,64 @@
 directly into your `CASCI` or `CASSCF` simulation objects of PySCF.
 
 Below we show a simple example of how to do this.
 
 ```python
 from pyscf import gto, scf, mcscf
 
+import numpy as np
+
+from qiskit.algorithms.minimum_eigensolvers import VQE
 from qiskit.algorithms.optimizers import SLSQP
 from qiskit.primitives import Estimator
-from qiskit_nature.second_q.algorithms import GroundStateEigensolver, VQEUCCFactory
-from qiskit_nature.second_q.circuit.library import UCCSD
-from qiskit_nature.second_q.mappers import ParityMapper, QubitConverter
+from qiskit_nature.second_q.algorithms import GroundStateEigensolver
+from qiskit_nature.second_q.circuit.library import HartreeFock, UCCSD
+from qiskit_nature.second_q.mappers import ParityMapper
 
 from qiskit_nature_pyscf import QiskitSolver
 
 mol = gto.M(atom="Li 0 0 0; H 0 0 1.6", basis="sto-3g")
 
 h_f = scf.RHF(mol).run()
 
-norb, nelec = 2, 2
+norb = 2
+nalpha, nbeta = 1, 1
+nelec = nalpha + nbeta
 
 cas = mcscf.CASCI(h_f, norb, nelec)
 
-converter = QubitConverter(ParityMapper(), two_qubit_reduction=True)
+mapper = ParityMapper(num_particles=(nalpha, nbeta))
+
+ansatz = UCCSD(
+    norb,
+    (nalpha, nbeta),
+    mapper,
+    initial_state=HartreeFock(
+        norb,
+        (nalpha, nbeta),
+        mapper,
+    ),
+)
 
-vqe = VQEUCCFactory(Estimator(), UCCSD(), SLSQP())
+vqe = VQE(Estimator(), ansatz, SLSQP())
+vqe.initial_point = np.zeros(ansatz.num_parameters)
 
-algorithm = GroundStateEigensolver(converter, vqe)
+algorithm = GroundStateEigensolver(mapper, vqe)
 
 cas.fcisolver = QiskitSolver(algorithm)
 
 cas.run()
 ```
 
 More detailed documentation can be found at
 [Documentation](https://qiskit-community.github.io/qiskit-nature-pyscf/). For more detailed 
 explanations we recommend to check out the documentation of
 [PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/documentation/nature/).
+
+
+## Citation
+
+If you use this plugin, please cite the following references:
+
+- PySCF, as per [these instructions](https://github.com/pyscf/pyscf#citing-pyscf).
+- Qiskit, as per the provided [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+- Qiskit Nature, as per https://doi.org/10.5281/zenodo.7828767
```

### Comparing `qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/__init__.py` & `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/qiskit_solver.py` & `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/qiskit_solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -45,35 +45,50 @@
 
     Here is an example use case:
 
     .. code-block:: python
 
         from pyscf import gto, scf, mcscf
 
+        from qiskit.algorithms.minimum_eigensolvers import VQE
         from qiskit.algorithms.optimizers import SLSQP
         from qiskit.primitives import Estimator
-        from qiskit_nature.second_q.algorithms import GroundStateEigensolver, VQEUCCFactory
-        from qiskit_nature.second_q.circuit.library import UCCSD
-        from qiskit_nature.second_q.mappers import ParityMapper, QubitConverter
+        from qiskit_nature.second_q.algorithms import GroundStateEigensolver
+        from qiskit_nature.second_q.circuit.library import HartreeFock, UCCSD
+        from qiskit_nature.second_q.mappers import ParityMapper
 
         from qiskit_nature_pyscf import QiskitSolver
 
         mol = gto.M(atom="Li 0 0 0; H 0 0 1.51", basis="631g*")
 
         h_f = scf.RHF(mol).run()
 
-        norb, nelec = 2, 2
+        norb = 2
+        nalpha, nbeta = 1, 1
+        nelec = nalpha + nbeta
 
         cas = mcscf.CASCI(h_f, norb, nelec)
 
-        converter = QubitConverter(ParityMapper(), two_qubit_reduction=True)
+        mapper = ParityMapper(num_particles=(nalpha, nbeta))
 
-        vqe = VQEUCCFactory(Estimator(), UCCSD(), SLSQP())
+        ansatz = UCCSD(
+            norb,
+            (nalpha, nbeta),
+            mapper,
+            initial_state=HartreeFock(
+                norb,
+                (nalpha, nbeta),
+                mapper,
+            ),
+        )
 
-        algorithm = GroundStateEigensolver(converter, vqe)
+        vqe = VQE(Estimator(), ansatz, SLSQP())
+        vqe.initial_point = np.zeros(ansatz.num_parameters)
+
+        algorithm = GroundStateEigensolver(mapper, vqe)
 
         cas.fcisolver = QiskitSolver(algorithm)
 
         cas.run()
 
     For more details please to the documentation of [PySCF](https://pyscf.org/) and
     [Qiskit Nature](https://qiskit.org/documentation/nature/).
```

### Comparing `qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf/version.py` & `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/PKG-INFO` & `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-nature-pyscf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Qiskit Nature PySCF: Third-party integration plugin of Qiskit Nature + PySCF.
 Home-page: https://github.com/qiskit-community/qiskit-nature-pyscf
 Author: Qiskit Nature PySCF Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
 Keywords: qiskit sdk quantum nature chemistry physics pyscf
 Classifier: Environment :: Console
@@ -27,22 +27,22 @@
 
 [![License](https://img.shields.io/github/license/qiskit-community/qiskit-nature-pyscf.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
 
 **Qiskit Nature PySCF** is a third-party integration plugin of Qiskit Nature + PySCF.
 
 ## Installation
 
-We encourage installing Qiskit Nature via the pip tool (a python package manager).
+We encourage installing Qiskit Nature PySCF via the pip tool (a python package manager).
 
 ```bash
 pip install qiskit-nature-pyscf
 ```
 
 **pip** will handle all dependencies automatically and you will always install the latest
-(and well-tested) version.
+(and well-tested) version. It will also install Qiskit Nature if needed.
 
 If you want to work on the very latest work-in-progress versions, either to try features ahead of
 their official release or if you want to contribute to Qiskit Nature PySCF, then you can install from source.
 
 
 ## Usage
 
@@ -56,38 +56,64 @@
 directly into your `CASCI` or `CASSCF` simulation objects of PySCF.
 
 Below we show a simple example of how to do this.
 
 ```python
 from pyscf import gto, scf, mcscf
 
+import numpy as np
+
+from qiskit.algorithms.minimum_eigensolvers import VQE
 from qiskit.algorithms.optimizers import SLSQP
 from qiskit.primitives import Estimator
-from qiskit_nature.second_q.algorithms import GroundStateEigensolver, VQEUCCFactory
-from qiskit_nature.second_q.circuit.library import UCCSD
-from qiskit_nature.second_q.mappers import ParityMapper, QubitConverter
+from qiskit_nature.second_q.algorithms import GroundStateEigensolver
+from qiskit_nature.second_q.circuit.library import HartreeFock, UCCSD
+from qiskit_nature.second_q.mappers import ParityMapper
 
 from qiskit_nature_pyscf import QiskitSolver
 
 mol = gto.M(atom="Li 0 0 0; H 0 0 1.6", basis="sto-3g")
 
 h_f = scf.RHF(mol).run()
 
-norb, nelec = 2, 2
+norb = 2
+nalpha, nbeta = 1, 1
+nelec = nalpha + nbeta
 
 cas = mcscf.CASCI(h_f, norb, nelec)
 
-converter = QubitConverter(ParityMapper(), two_qubit_reduction=True)
+mapper = ParityMapper(num_particles=(nalpha, nbeta))
+
+ansatz = UCCSD(
+    norb,
+    (nalpha, nbeta),
+    mapper,
+    initial_state=HartreeFock(
+        norb,
+        (nalpha, nbeta),
+        mapper,
+    ),
+)
 
-vqe = VQEUCCFactory(Estimator(), UCCSD(), SLSQP())
+vqe = VQE(Estimator(), ansatz, SLSQP())
+vqe.initial_point = np.zeros(ansatz.num_parameters)
 
-algorithm = GroundStateEigensolver(converter, vqe)
+algorithm = GroundStateEigensolver(mapper, vqe)
 
 cas.fcisolver = QiskitSolver(algorithm)
 
 cas.run()
 ```
 
 More detailed documentation can be found at
 [Documentation](https://qiskit-community.github.io/qiskit-nature-pyscf/). For more detailed 
 explanations we recommend to check out the documentation of
 [PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/documentation/nature/).
+
+
+## Citation
+
+If you use this plugin, please cite the following references:
+
+- PySCF, as per [these instructions](https://github.com/pyscf/pyscf#citing-pyscf).
+- Qiskit, as per the provided [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+- Qiskit Nature, as per https://doi.org/10.5281/zenodo.7828767
```

### Comparing `qiskit-nature-pyscf-0.1.0/qiskit_nature_pyscf.egg-info/SOURCES.txt` & `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/setup.py` & `qiskit-nature-pyscf-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/test/__init__.py` & `qiskit-nature-pyscf-0.1.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/test/nature_pyscf_test_case.py` & `qiskit-nature-pyscf-0.1.1/test/nature_pyscf_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.0/test/test_qiskit_solver.py` & `qiskit-nature-pyscf-0.1.1/test/test_qiskit_solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -12,16 +12,17 @@
 
 """Tests for the QiskitSolver."""
 
 from test import QiskitNaturePySCFTestCase
 
 from pyscf import gto, scf, mcscf
 
-from qiskit_nature.second_q.algorithms import GroundStateEigensolver, NumPyMinimumEigensolverFactory
-from qiskit_nature.second_q.mappers import JordanWignerMapper, QubitConverter
+from qiskit.algorithms.minimum_eigensolvers import NumPyMinimumEigensolver
+from qiskit_nature.second_q.algorithms import GroundStateEigensolver
+from qiskit_nature.second_q.mappers import JordanWignerMapper
 from qiskit_nature_pyscf.qiskit_solver import QiskitSolver
 
 
 class TestQiskitSolver(QiskitNaturePySCFTestCase):
     """Tests for the QiskitSolver."""
 
     def test_rhf_casci_h2(self):
@@ -33,16 +34,16 @@
         norb, nelec = 2, 2
 
         cas_ref = mcscf.CASCI(h_f, norb, nelec).run()
 
         qcas = mcscf.CASCI(h_f, norb, nelec)
 
         ground_state_solver = GroundStateEigensolver(
-            QubitConverter(JordanWignerMapper()),
-            NumPyMinimumEigensolverFactory(),
+            JordanWignerMapper(),
+            NumPyMinimumEigensolver(),
         )
 
         qcas.fcisolver = QiskitSolver(ground_state_solver)
 
         qcas.run()
 
         self.assertAlmostEqual(qcas.e_tot, cas_ref.e_tot)
@@ -56,16 +57,16 @@
         norb, nelec = 2, 2
 
         cas_ref = mcscf.UCASCI(h_f, norb, nelec).run()
 
         qcas = mcscf.UCASCI(h_f, norb, nelec)
 
         ground_state_solver = GroundStateEigensolver(
-            QubitConverter(JordanWignerMapper()),
-            NumPyMinimumEigensolverFactory(),
+            JordanWignerMapper(),
+            NumPyMinimumEigensolver(),
         )
 
         qcas.fcisolver = QiskitSolver(ground_state_solver)
 
         qcas.run()
 
         self.assertAlmostEqual(qcas.e_tot, cas_ref.e_tot)
@@ -79,16 +80,16 @@
         norb, nelec = 2, 2
 
         cas_ref = mcscf.CASSCF(h_f, norb, nelec).run()
 
         qcas = mcscf.CASSCF(h_f, norb, nelec)
 
         ground_state_solver = GroundStateEigensolver(
-            QubitConverter(JordanWignerMapper()),
-            NumPyMinimumEigensolverFactory(),
+            JordanWignerMapper(),
+            NumPyMinimumEigensolver(),
         )
 
         qcas.fcisolver = QiskitSolver(ground_state_solver)
 
         qcas.run()
 
         self.assertAlmostEqual(qcas.e_tot, cas_ref.e_tot)
@@ -102,16 +103,16 @@
         norb, nelec = 2, 2
 
         cas_ref = mcscf.UCASSCF(h_f, norb, nelec).run()
 
         qcas = mcscf.UCASSCF(h_f, norb, nelec)
 
         ground_state_solver = GroundStateEigensolver(
-            QubitConverter(JordanWignerMapper()),
-            NumPyMinimumEigensolverFactory(),
+            JordanWignerMapper(),
+            NumPyMinimumEigensolver(),
         )
 
         qcas.fcisolver = QiskitSolver(ground_state_solver)
 
         qcas.run()
 
         self.assertAlmostEqual(qcas.e_tot, cas_ref.e_tot)
```

### Comparing `qiskit-nature-pyscf-0.1.0/test/test_readme_sample.py` & `qiskit-nature-pyscf-0.1.1/test/test_readme_sample.py`

 * *Files identical despite different names*

