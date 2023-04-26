# Comparing `tmp/rgfrosh-0.1.4.tar.gz` & `tmp/rgfrosh-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgfrosh-0.1.4.tar", last modified: Fri Mar 17 18:27:52 2023, max compression
+gzip compressed data, was "rgfrosh-0.2.0.tar", last modified: Wed Apr 26 16:28:32 2023, max compression
```

## Comparing `rgfrosh-0.1.4.tar` & `rgfrosh-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:27:52.061531 rgfrosh-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-17 18:27:52.061531 rgfrosh-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:27:52.061531 rgfrosh-0.1.4/rgfrosh/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/rgfrosh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/rgfrosh/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/rgfrosh/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/rgfrosh/shock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:27:52.061531 rgfrosh-0.1.4/rgfrosh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-17 18:27:52.000000 rgfrosh-0.1.4/rgfrosh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-17 18:27:52.000000 rgfrosh-0.1.4/rgfrosh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 18:27:52.000000 rgfrosh-0.1.4/rgfrosh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-17 18:27:52.000000 rgfrosh-0.1.4/rgfrosh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 18:27:52.000000 rgfrosh-0.1.4/rgfrosh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-17 18:27:52.065531 rgfrosh-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:27:52.061531 rgfrosh-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/test/test_ideal_shock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-17 18:27:33.000000 rgfrosh-0.1.4/test/test_real_gas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/rgfrosh/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25006 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/shock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/rgfrosh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/test/test_frozen_shock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/test/test_ideal_shock.py
```

### Comparing `rgfrosh-0.1.4/LICENSE` & `rgfrosh-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rgfrosh-0.1.4/PKG-INFO` & `rgfrosh-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgfrosh
-Version: 0.1.4
+Version: 0.2.0
 Summary: A frozen shock solver for ideal and real gas equations of state.
 Home-page: https://github.com/VasuLab/RGFROSH
 Author: Cory Kinney
 Author-email: corykinney@ucf.edu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -14,55 +14,49 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python Real Gas FROzen SHock (RGFROSH) Solver
+# Python Real Gas FROzen SHock (RGFROSH)
 
+![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
 [![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
 [![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
 [![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
 
 > This project is a solver for the frozen shock equations[^1] developed in Python at the
 > University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
 > University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
 > CHEMKIN[^2][^3]. 
 
 Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
-a shock tube for an arbitrary equation of state. RGFROSH requires a thermodynamic interface 
-for calculating mixture properties as a function of temperature and pressure and currently supports:
-
-- [Cantera](https://github.com/cantera/cantera)
-- [CoolProp](https://github.com/CoolProp/CoolProp) (using the built-in
-  [wrapper](https://vasulab.github.io/RGFROSH/reference/interface/#rgfrosh.interface.CPInterface) - 
-  see [example](https://vasulab.github.io/RGFROSH/guide/interfaces/#coolprop)) 
-- [User-defined interfaces](https://vasulab.github.io/RGFROSH/guide/interfaces/#user-defined-interfaces)
+a shock tube for an arbitrary equation of state. 
 
 ## Documentation
 
 The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
-[user guide](https://vasulab.github.io/RGFROSH/guide) and 
-[API reference](https://vasulab.github.io/RGFROSH/reference/shock) for the package.
+[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
+[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
 
 ## Installation
 
-RGFROSH can be installed using
+Python RGFROSH can be installed using
 
 ```
 pip install rgfrosh
 ```
 
-which also installs required dependencies. Cantera or CoolProp are optional and will 
-need to be installed separately if desired.
+which also installs required dependencies. Cantera or CoolProp are optional and must
+be installed separately if desired.
 
 ## Contributing
 
 For any bugs or feature requests, create an issue on the 
 [issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
 
 After cloning the repository, the development environment can be set up with
@@ -84,18 +78,17 @@
 ```
 
 These checks will be performed automatically for all pull requests along
 with test coverage comparisons.
 
 ## Cite
 
-To cite Python RGFROSH go to the [GitHub repository](https://github.com/VasuLab/RGFROSH) and click 
-<kbd>Cite this repository</kbd> on the right side to export the citation for the latest release of 
-`rgfrosh`. It is also encouraged to cite the original paper[^1] for the frozen shock equations that
-this work is a derived from.
+To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
+page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
+original paper[^1] for the frozen shock equations that this work is a derived from.
 
 
 [^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
 at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
 [^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
 SAND88-3188 (1988). https://doi.org/10.2172/6224858
 [^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for
```

### Comparing `rgfrosh-0.1.4/README.md` & `rgfrosh-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-# Python Real Gas FROzen SHock (RGFROSH) Solver
+# Python Real Gas FROzen SHock (RGFROSH)
 
+![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
 [![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
 [![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
 [![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
 
 > This project is a solver for the frozen shock equations[^1] developed in Python at the
 > University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
 > University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
 > CHEMKIN[^2][^3]. 
 
 Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
-a shock tube for an arbitrary equation of state. RGFROSH requires a thermodynamic interface 
-for calculating mixture properties as a function of temperature and pressure and currently supports:
-
-- [Cantera](https://github.com/cantera/cantera)
-- [CoolProp](https://github.com/CoolProp/CoolProp) (using the built-in
-  [wrapper](https://vasulab.github.io/RGFROSH/reference/interface/#rgfrosh.interface.CPInterface) - 
-  see [example](https://vasulab.github.io/RGFROSH/guide/interfaces/#coolprop)) 
-- [User-defined interfaces](https://vasulab.github.io/RGFROSH/guide/interfaces/#user-defined-interfaces)
+a shock tube for an arbitrary equation of state. 
 
 ## Documentation
 
 The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
-[user guide](https://vasulab.github.io/RGFROSH/guide) and 
-[API reference](https://vasulab.github.io/RGFROSH/reference/shock) for the package.
+[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
+[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
 
 ## Installation
 
-RGFROSH can be installed using
+Python RGFROSH can be installed using
 
 ```
 pip install rgfrosh
 ```
 
-which also installs required dependencies. Cantera or CoolProp are optional and will 
-need to be installed separately if desired.
+which also installs required dependencies. Cantera or CoolProp are optional and must
+be installed separately if desired.
 
 ## Contributing
 
 For any bugs or feature requests, create an issue on the 
 [issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
 
 After cloning the repository, the development environment can be set up with
@@ -64,18 +58,17 @@
 ```
 
 These checks will be performed automatically for all pull requests along
 with test coverage comparisons.
 
 ## Cite
 
-To cite Python RGFROSH go to the [GitHub repository](https://github.com/VasuLab/RGFROSH) and click 
-<kbd>Cite this repository</kbd> on the right side to export the citation for the latest release of 
-`rgfrosh`. It is also encouraged to cite the original paper[^1] for the frozen shock equations that
-this work is a derived from.
+To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
+page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
+original paper[^1] for the frozen shock equations that this work is a derived from.
 
 
 [^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
 at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
 [^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
 SAND88-3188 (1988). https://doi.org/10.2172/6224858
 [^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for
```

### Comparing `rgfrosh-0.1.4/rgfrosh/interface.py` & `rgfrosh-0.2.0/rgfrosh/thermo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,97 @@
+from .constants import GAS_CONSTANT
+
 from abc import abstractmethod
 from typing import Protocol, Tuple
 
 
 class ThermoInterface(Protocol):
     """
     Class defining the required interface for calculating mixture thermodynamic
     properties.
     """
 
     @property
     @abstractmethod
     def TP(self) -> Tuple[float, float]:
         """Get/set temperature [K] and pressure [Pa]."""
-        raise NotImplementedError
 
     @TP.setter
     @abstractmethod
     def TP(self, value: Tuple[float, float]):
-        raise NotImplementedError
+        """Get/set temperature [K] and pressure [Pa]."""
 
     @property
     @abstractmethod
     def mean_molecular_weight(self) -> float:
         """The mean molecular weight (molar mass) [kg/kmol]."""
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def density_mass(self) -> float:
         """(Mass) density [kg/m^3^]."""
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def cp_mass(self) -> float:
         """Specific heat capacity at constant pressure [J/kg/K]."""
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def enthalpy_mass(self) -> float:
         """Specific enthalpy [J/kg]."""
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def isothermal_compressibility(self) -> float:
         """Isothermal compressibility [1/Pa]."""
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def thermal_expansion_coeff(self) -> float:
         """Thermal expansion coefficient [1/K]."""
-        raise NotImplementedError
+
+
+def compressibility_factor(
+    thermo: ThermoInterface, T: float = None, P: float = None
+) -> float:
+    r"""
+    Calculates the compressibility factor of a gas at a specified state:
+
+    $$
+    Z = \frac{P}{\rho RT}
+    $$
+
+    Parameters:
+        thermo: Thermodynamic interface.
+        T: Temperature [K].
+        P: Pressure [Pa].
+
+    """
+    if T and P:
+        thermo.TP = T, P
+    else:
+        T, P = thermo.TP
+
+    return P / (thermo.density_mass * GAS_CONSTANT / thermo.mean_molecular_weight * T)
 
 
 try:
     import CoolProp as CP
 
     class CPInterface(ThermoInterface):
         """
         :octicons-tag-24: 0.1.4
 
+        !!! Note
+            Only available if `CoolProp` is installed.
+
         Wrapper for `CoolProp.AbstractState` objects that accounts for
         differing property names and automatically adjusts units for
         `mean_molecular_weight`.
-
-        !!! Note
-            Only available if `CoolProp` is installed.
         """
 
         def __init__(self, state: CP.AbstractState):
             self.state = state
 
         @property
         def mean_molecular_weight(self):
```

### Comparing `rgfrosh-0.1.4/rgfrosh.egg-info/PKG-INFO` & `rgfrosh-0.2.0/rgfrosh.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgfrosh
-Version: 0.1.4
+Version: 0.2.0
 Summary: A frozen shock solver for ideal and real gas equations of state.
 Home-page: https://github.com/VasuLab/RGFROSH
 Author: Cory Kinney
 Author-email: corykinney@ucf.edu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -14,55 +14,49 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python Real Gas FROzen SHock (RGFROSH) Solver
+# Python Real Gas FROzen SHock (RGFROSH)
 
+![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
 [![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
 [![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
 [![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
 
 > This project is a solver for the frozen shock equations[^1] developed in Python at the
 > University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
 > University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
 > CHEMKIN[^2][^3]. 
 
 Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
-a shock tube for an arbitrary equation of state. RGFROSH requires a thermodynamic interface 
-for calculating mixture properties as a function of temperature and pressure and currently supports:
-
-- [Cantera](https://github.com/cantera/cantera)
-- [CoolProp](https://github.com/CoolProp/CoolProp) (using the built-in
-  [wrapper](https://vasulab.github.io/RGFROSH/reference/interface/#rgfrosh.interface.CPInterface) - 
-  see [example](https://vasulab.github.io/RGFROSH/guide/interfaces/#coolprop)) 
-- [User-defined interfaces](https://vasulab.github.io/RGFROSH/guide/interfaces/#user-defined-interfaces)
+a shock tube for an arbitrary equation of state. 
 
 ## Documentation
 
 The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
-[user guide](https://vasulab.github.io/RGFROSH/guide) and 
-[API reference](https://vasulab.github.io/RGFROSH/reference/shock) for the package.
+[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
+[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
 
 ## Installation
 
-RGFROSH can be installed using
+Python RGFROSH can be installed using
 
 ```
 pip install rgfrosh
 ```
 
-which also installs required dependencies. Cantera or CoolProp are optional and will 
-need to be installed separately if desired.
+which also installs required dependencies. Cantera or CoolProp are optional and must
+be installed separately if desired.
 
 ## Contributing
 
 For any bugs or feature requests, create an issue on the 
 [issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
 
 After cloning the repository, the development environment can be set up with
@@ -84,18 +78,17 @@
 ```
 
 These checks will be performed automatically for all pull requests along
 with test coverage comparisons.
 
 ## Cite
 
-To cite Python RGFROSH go to the [GitHub repository](https://github.com/VasuLab/RGFROSH) and click 
-<kbd>Cite this repository</kbd> on the right side to export the citation for the latest release of 
-`rgfrosh`. It is also encouraged to cite the original paper[^1] for the frozen shock equations that
-this work is a derived from.
+To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
+page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
+original paper[^1] for the frozen shock equations that this work is a derived from.
 
 
 [^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
 at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
 [^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
 SAND88-3188 (1988). https://doi.org/10.2172/6224858
 [^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for
```

### Comparing `rgfrosh-0.1.4/setup.cfg` & `rgfrosh-0.2.0/setup.cfg`

 * *Files identical despite different names*

