# Comparing `tmp/ionics_fits-1.0.3.tar.gz` & `tmp/ionics_fits-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionics_fits-1.0.3.tar", max compression
+gzip compressed data, was "ionics_fits-1.0.4.tar", max compression
```

## Comparing `ionics_fits-1.0.3.tar` & `ionics_fits-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/LICENSE
--rw-r--r--   0        0        0     8952 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/README.md
--rw-r--r--   0        0        0      124 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/__init__.py
--rw-r--r--   0        0        0    31655 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/common.py
--rw-r--r--   0        0        0      390 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/__init__.py
--rw-r--r--   0        0        0     4705 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/benchmarking.py
--rw-r--r--   0        0        0     4015 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/exponential.py
--rw-r--r--   0        0        0     5507 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/gaussian.py
--rw-r--r--   0        0        0     3235 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/lorentzian.py
--rw-r--r--   0        0        0    12420 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/polynomial.py
--rw-r--r--   0        0        0    16336 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/rabi.py
--rw-r--r--   0        0        0     4332 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/rectangle.py
--rw-r--r--   0        0        0     6081 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/sinc.py
--rw-r--r--   0        0        0     6849 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/sinusoid.py
--rw-r--r--   0        0        0     7341 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/triangle.py
--rw-r--r--   0        0        0    11659 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/models/utils.py
--rw-r--r--   0        0        0     4855 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/normal.py
--rw-r--r--   0        0        0      655 2023-03-22 12:14:37.930850 ionics_fits-1.0.3/ionics_fits/utils.py
--rw-r--r--   0        0        0      992 2023-03-22 12:14:53.778892 ionics_fits-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9955 1970-01-01 00:00:00.000000 ionics_fits-1.0.3/setup.py
--rw-r--r--   0        0        0     9552 1970-01-01 00:00:00.000000 ionics_fits-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/LICENSE
+-rw-r--r--   0        0        0     9752 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/README.md
+-rw-r--r--   0        0        0      124 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/__init__.py
+-rw-r--r--   0        0        0    31655 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/common.py
+-rw-r--r--   0        0        0      434 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/__init__.py
+-rw-r--r--   0        0        0     4794 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/aggregate_model.py
+-rw-r--r--   0        0        0     4705 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/benchmarking.py
+-rw-r--r--   0        0        0     4015 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/exponential.py
+-rw-r--r--   0        0        0     5507 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/gaussian.py
+-rw-r--r--   0        0        0     3235 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/lorentzian.py
+-rw-r--r--   0        0        0    12420 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/polynomial.py
+-rw-r--r--   0        0        0    16336 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/rabi.py
+-rw-r--r--   0        0        0     4332 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/rectangle.py
+-rw-r--r--   0        0        0     6081 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/sinc.py
+-rw-r--r--   0        0        0     6849 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/sinusoid.py
+-rw-r--r--   0        0        0     7341 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/triangle.py
+-rw-r--r--   0        0        0    11659 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/utils.py
+-rw-r--r--   0        0        0     4855 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/normal.py
+-rw-r--r--   0        0        0      655 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/utils.py
+-rw-r--r--   0        0        0     1032 2023-04-25 15:19:19.130362 ionics_fits-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10840 1970-01-01 00:00:00.000000 ionics_fits-1.0.4/setup.py
+-rw-r--r--   0        0        0    10434 1970-01-01 00:00:00.000000 ionics_fits-1.0.4/PKG-INFO
```

### Comparing `ionics_fits-1.0.3/LICENSE` & `ionics_fits-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/README.md` & `ionics_fits-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -127,20 +127,24 @@
 ## Extensibility
 
 The library is designed to be extensible and ergonomic to user. Want to use different
 statistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some
 custom post-fit processing? Override the `calculate_derived_parameters` method. Want to
 tweak the parameter estimator for a model? Create a new model class that inherits from
 the original model and modify away. If you're struggling to do what you want, it's
-probably a bug in the library so report it.
+probably a bug in the library so please report it.
 
-`ionics_fits` provides a number of tools in [`models.utils`](../master/ionics_fits/models/utils.py) to make it easier to
-extend models. For example, say you want to fit some frequency-domain Rabi oscillation
-data. However, the model works in angular units, but your tooling needs linear units. No
-problem! Simply use the `rescale_model_x` tool:
+`ionics_fits` provides a number of tools to make it easier to extend models (see, for
+example in [`models.utils`](../master/ionics_fits/models/utils.py)). Say you want to...
+
+## Rescaling models
+
+...fit some frequency-domain Rabi oscillation data. However, the model works in angular
+units, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`
+tool.
 
 ```python
 detuning_model = fits.models.utils.rescale_model_x(fits.models.RabiFlopFreq, 2 * np.pi)
 ```
 
 Or, suppose you actually want to scan the magnetic field and find the field offset which
 puts the transition at a particular frequency?
@@ -165,17 +169,43 @@
         derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB
 
         return derived_params, derived_uncertainties
 
 RabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)
 ```
 
-At present the library is still an MVP. While we do provide some hooks there aren't
-many. The addition of further hooks will be driven by use cases, so please open an issue
-if you find you can't easily extend the library in the way you want.
+## Aggregating models
+
+...fit multiple independent models simultaneously and do some post-processing on the
+results. Use an `AggregateModel`.
+
+```python
+class LineAndTriange(fits.models.AggregateModel):
+  def __init__(self):
+    line = fits.models.Line()
+    triangle = fits.models.Triangle()
+    super().__init__(models=[("line", line), "triangle", triangle])
+
+  def calculate_derived_params(
+      self,
+      x: Array[("num_samples",), np.float64],
+      y: Array[("num_samples",), np.float64],
+      fitted_params: Dict[str, float],
+      fit_uncertainties: Dict[str, float],
+  ) -> Tuple[Dict[str, float], Dict[str, float]]:
+      derived_params, derived_uncertainties = super().calculate_derived_params()
+      # derive new results from the two fits
+      return derived_params, derived_uncertainties
+```
+
+## And more!
+
+At present the library is still an MVP. Further work will be driven by use cases, so
+please open an issue if you find you can't easily extend the library in the way you
+want.
 
 # Ontology
 
 There are two main kinds of object in the library: `fit`s and `model`s. Models are
 general-purpose functions to be fitted, such as sinusoids or Lorentzians, but are
 agnostic about the statistics. Fits do the fitting (maximum likelihood parameter
 estimation) and validation based on some underlying statistics (normal, binomial, etc).
```

### Comparing `ionics_fits-1.0.3/ionics_fits/common.py` & `ionics_fits-1.0.4/ionics_fits/common.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/benchmarking.py` & `ionics_fits-1.0.4/ionics_fits/models/benchmarking.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/exponential.py` & `ionics_fits-1.0.4/ionics_fits/models/exponential.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/gaussian.py` & `ionics_fits-1.0.4/ionics_fits/models/gaussian.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/lorentzian.py` & `ionics_fits-1.0.4/ionics_fits/models/lorentzian.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/polynomial.py` & `ionics_fits-1.0.4/ionics_fits/models/polynomial.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/rabi.py` & `ionics_fits-1.0.4/ionics_fits/models/rabi.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/rectangle.py` & `ionics_fits-1.0.4/ionics_fits/models/rectangle.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/sinc.py` & `ionics_fits-1.0.4/ionics_fits/models/sinc.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/sinusoid.py` & `ionics_fits-1.0.4/ionics_fits/models/sinusoid.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/triangle.py` & `ionics_fits-1.0.4/ionics_fits/models/triangle.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/models/utils.py` & `ionics_fits-1.0.4/ionics_fits/models/utils.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/normal.py` & `ionics_fits-1.0.4/ionics_fits/normal.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/ionics_fits/utils.py` & `ionics_fits-1.0.4/ionics_fits/utils.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.3/pyproject.toml` & `ionics_fits-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "ionics-fits"
-version = "1.0.3"
+version = "1.0.4"
 description = "Lightweight Python data fitting library with an emphasis on AMO/Quantum Information"
 authors = ["hartytp <thomas.peter.harty@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 numpy = "^1.21.2"
 scipy = "^1.7.1"
 statsmodels = "^0.13.2"
+pyqt5 = "^5.15.9"
+pyqt5-qt5 = "^5.15.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 poethepoet = "^0.12.1"
 flake8 = "^4.0.1"
 black = "^22.6.0"
 matplotlib = "^3.5.3"
```

### Comparing `ionics_fits-1.0.3/setup.py` & `ionics_fits-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 packages = \
 ['ionics_fits', 'ionics_fits.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.21.2,<2.0.0', 'scipy>=1.7.1,<2.0.0', 'statsmodels>=0.13.2,<0.14.0']
+['numpy>=1.21.2,<2.0.0',
+ 'pyqt5-qt5>=5.15.2,<6.0.0',
+ 'pyqt5>=5.15.9,<6.0.0',
+ 'scipy>=1.7.1,<2.0.0',
+ 'statsmodels>=0.13.2,<0.14.0']
 
 setup_kwargs = {
     'name': 'ionics-fits',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'Lightweight Python data fitting library with an emphasis on AMO/Quantum Information',
-    'long_description': 'Lightweight Python library for data fitting with an emphasis on AMO (Atomic Molecular\nand Optical physics) and Quantum Information.\n\n`fits` was inspired by the [Oxford Ion Trap Group fitting library](https://github.com/OxfordIonTrapGroup/oitg/tree/master/oitg/fitting) originally\nauthored by @tballance. It is still in the alpha phase and is likely to be renamed\n(although `fits` is still available on pypi)...please feel free to help bikeshed names.\n\n# Getting started\n\n## Installation\n\nInstall from `pypi` with `pip install ionics_fits` or add to your poetry project with\n`poetry add fits`.\n\n## Example Usage\n\nBasic usage\n```python\nimport numpy as np\nimport ionics_fits as fits\n\na = 3.2\ny0 = -9\n\nx = np.linspace(-10, 10)\ny = a*x + y0\n\nfit = fits.NormalFitter(x, y, model=fits.models.Line())\nprint(f"Fitted: y = {fit.values[\'a\']:.3f} * x + {fit.values[\'y0\']:.3f}")\n```\n\nThe fit can be configured in various ways by modifying the model\'s `parameters`\ndictionary (see the `fits.common.ModelParameter` class for more information). This\nallows one to:\n- change the bounds for parameters\n- change which parameters are fixed to a constant value / floated\n- supply initial values for parameters instead of relying on the heuristics\n\nExample usage:\n```python\nimport numpy as np\nfrom matplotlib import pyplot as plt\nimport ionics_fits as fits\n\n# Example problem: fit the amplitude and phase of a sinusoid whose frequency is known\n# exactly\n\nomega = 2 * np.pi  # we know the frequency\nmodel = fits.models.Sinusoid()\nmodel.parameters["omega"].fixed_to = omega\n\n# generate synthetic data to fit\nparams = {\n    "a": np.random.uniform(low=1, high=5),\n    "omega": omega,\n    "phi": np.random.uniform(-1, 1) * 2 * np.pi,\n    "y0": 0,\n    "x0": 0,\n    "tau": np.inf,\n}\nx = np.linspace(-3, 3, 100)\ny = model.func(x, params)\n\nfit = fits.NormalFitter(x, y, model=model)\nprint(f"Amplitude: dataset = {params[\'a\']:.3f}, fit = {fit.values[\'a\']:.3f}")\nprint(f"Phase: dataset = {params[\'phi\']:.3f}, fit = {fit.values[\'phi\']:.3f}")\n\nplt.plot(x, y, label="data")\nplt.plot(*fit.evaluate(), \'-.o\', label="fit")\nplt.grid()\nplt.legend()\nplt.show()\n```\n\n# Developing\n\nBefore committing:\n- Update formatting: `poe fmt`\n- Lints: `poe flake`\n- Run test suite: `poe test`\n- Optionally: [fuzz](#Fuzzing) any new models\n\n# Design Philosophy\n\n## Good Heuristics\n\nLife is too short for failed fits. We can\'t guarantee to fit every dataset without any\nhelp from the user (e.g. specifying initial parameter values) no matter how noisy or\nincomplete it is...but we do our best!\n\nEvery fit model has a "parameter estimator" which uses heuristics to find good estimates\nof the values of the model\'s free parameters. We expect these heuristics to be good\nenough to allow the optimizer to fit any "reasonable" dataset. Fit failures are viewed\nas a bug and we encourage our users to file issues where they find them (please post an\nexample dataset in the issue).\n\nCurrently this project is a MVP and many of the heuristics need some work. Expect there\nto be cases where we could easily do better. Please report them where you find them!\n\n## Validation\n\nIt\'s not enough to just fit the data, we want to know if we can trust the fit results\nbefore acting on them.  There are two distinct aspects to the validation problem: did\nthe fit find the model parameters which best match the data (as opposed to getting stuck\nin a local minimum in parameter space far from the global optimum)? and, are the fitted\nparameter values consistent with our prior knowledge of the system (e.g. we know that a\nfringe contrast must lie within certain bounds).\n\nFirst, any prior knowledge about the system should be incorporated by specifying fixed\nparameter values and parameter bounds. After that, the fit is validated. At present,\nvalidation is done using the Chi-squared as a test for goodness of fit. It is likely\nthat additional validation tests will be added as the package grows.\n\n## General purpose\n\nThis library is designed to be general purpose; rather than tackling specific problems\nwe try to target sets of problems -- we want to fit sinusoids not *your* sinusoid. This\nis reflected, for example, in the choices of parametrisation, which are intended to be\nextremely flexible, and the effort put into heuristics. If you find you can\'t easily fit\nyour sinusoid with the standard model/heuristics it\'s probably a bug in the model design\nso please open an issue.\n\nWe encourage contributions of new fit models, but please consider generality before\nsubmission. If you want to solve a specific problem in front of you, that\'s fine but\nprobably better suited to your own codebase.\n\n## Extensibility\n\nThe library is designed to be extensible and ergonomic to user. Want to use different\nstatistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some\ncustom post-fit processing? Override the `calculate_derived_parameters` method. Want to\ntweak the parameter estimator for a model? Create a new model class that inherits from\nthe original model and modify away. If you\'re struggling to do what you want, it\'s\nprobably a bug in the library so report it.\n\n`ionics_fits` provides a number of tools in [`models.utils`](../master/ionics_fits/models/utils.py) to make it easier to\nextend models. For example, say you want to fit some frequency-domain Rabi oscillation\ndata. However, the model works in angular units, but your tooling needs linear units. No\nproblem! Simply use the `rescale_model_x` tool:\n\n```python\ndetuning_model = fits.models.utils.rescale_model_x(fits.models.RabiFlopFreq, 2 * np.pi)\n```\n\nOr, suppose you actually want to scan the magnetic field and find the field offset which\nputs the transition at a particular frequency?\n```python\nclass _RabiBField(fits.models.RabiFlopFreq):\n    def __init__(self, dfdB, B_0, f_0, start_excited):\n        super().__init__(start_excited=start_excited)\n        self.dfdB = dfdB\n        self.B_0 = B_0\n        self.f_0 = f_0\n\n    def calculate_derived_params(self, x, y, fitted_params, fit_uncertainties):\n        derived_params, derived_uncertainties = super().calculate_derived_params(\n            x, y, fitted_params, fit_uncertainties\n        )\n\n        df = derived_params["f_0"] - self.f_0\n        dB = df / self.dfdB\n        B_0 = dB + self.B_0\n\n        derived_params["B_0"] = B_0\n        derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB\n\n        return derived_params, derived_uncertainties\n\nRabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)\n```\n\nAt present the library is still an MVP. While we do provide some hooks there aren\'t\nmany. The addition of further hooks will be driven by use cases, so please open an issue\nif you find you can\'t easily extend the library in the way you want.\n\n# Ontology\n\nThere are two main kinds of object in the library: `fit`s and `model`s. Models are\ngeneral-purpose functions to be fitted, such as sinusoids or Lorentzians, but are\nagnostic about the statistics. Fits do the fitting (maximum likelihood parameter\nestimation) and validation based on some underlying statistics (normal, binomial, etc). \n\n# Testing methodology\n\nThis package uses both `unit test`s and `fuzzing`.\n\n## Unit Tests\n\n- run using `poe test`\n- to run a subset of tests use the `-k` flag e.g. `poe test -k "rabi"` to run only tests\n  with the word `rabi` in their name. For more information about configuring pytest see\n  the [documentation](https://docs.pytest.org/en/7.1.x/)\n- all tests must pass before a PR can be merged into master\n- PRs to add new models will only be merged once they have reasonable test coverage\n- unit tests aim to provide good coverage over the space of "reasonable datasets". There\n  will always be corner-cases where the fits fail and that\'s fine; the aim here is to\n  cover the main cases users will hit in the wild\n- when a user hits a case in the wild where the fit fails unexpectedly (i.e. we think\n  the fit code should have handled it), a `regression test` based on the failing\n  dataset should be added\n- unit tests should be deterministic. Synthetic datasets should be included in the test\n  rather than randomly generated at run time. Tip: while writing a test it\'s fine to let\n  the test code generate datasets for you. Once you\'re happy, run the test in verbose\n  mode and copy the dataset from the log output\n\n## Fuzzing\n\n- fuzzing is non-deterministic (random parameter values, randomly generated datasets)\n  exploration of the parameter space.\n- used when developing / debugging fits, but not automatically run by CI\n- run with `poe fuzz` (see `--help` for details)\n- fit failures during fuzzing are not automatically considered a bug; unlike unit tests,\n  fuzzing explores the "unreasonable" part of parameter space as well. Indeed, a large\n  part of the point of fuzzing is to help the developer understand what should be\n  considered "reasonable" (this information should end up in the documentation for the\n  fuzzed model).\n',
+    'long_description': 'Lightweight Python library for data fitting with an emphasis on AMO (Atomic Molecular\nand Optical physics) and Quantum Information.\n\n`fits` was inspired by the [Oxford Ion Trap Group fitting library](https://github.com/OxfordIonTrapGroup/oitg/tree/master/oitg/fitting) originally\nauthored by @tballance. It is still in the alpha phase and is likely to be renamed\n(although `fits` is still available on pypi)...please feel free to help bikeshed names.\n\n# Getting started\n\n## Installation\n\nInstall from `pypi` with `pip install ionics_fits` or add to your poetry project with\n`poetry add fits`.\n\n## Example Usage\n\nBasic usage\n```python\nimport numpy as np\nimport ionics_fits as fits\n\na = 3.2\ny0 = -9\n\nx = np.linspace(-10, 10)\ny = a*x + y0\n\nfit = fits.NormalFitter(x, y, model=fits.models.Line())\nprint(f"Fitted: y = {fit.values[\'a\']:.3f} * x + {fit.values[\'y0\']:.3f}")\n```\n\nThe fit can be configured in various ways by modifying the model\'s `parameters`\ndictionary (see the `fits.common.ModelParameter` class for more information). This\nallows one to:\n- change the bounds for parameters\n- change which parameters are fixed to a constant value / floated\n- supply initial values for parameters instead of relying on the heuristics\n\nExample usage:\n```python\nimport numpy as np\nfrom matplotlib import pyplot as plt\nimport ionics_fits as fits\n\n# Example problem: fit the amplitude and phase of a sinusoid whose frequency is known\n# exactly\n\nomega = 2 * np.pi  # we know the frequency\nmodel = fits.models.Sinusoid()\nmodel.parameters["omega"].fixed_to = omega\n\n# generate synthetic data to fit\nparams = {\n    "a": np.random.uniform(low=1, high=5),\n    "omega": omega,\n    "phi": np.random.uniform(-1, 1) * 2 * np.pi,\n    "y0": 0,\n    "x0": 0,\n    "tau": np.inf,\n}\nx = np.linspace(-3, 3, 100)\ny = model.func(x, params)\n\nfit = fits.NormalFitter(x, y, model=model)\nprint(f"Amplitude: dataset = {params[\'a\']:.3f}, fit = {fit.values[\'a\']:.3f}")\nprint(f"Phase: dataset = {params[\'phi\']:.3f}, fit = {fit.values[\'phi\']:.3f}")\n\nplt.plot(x, y, label="data")\nplt.plot(*fit.evaluate(), \'-.o\', label="fit")\nplt.grid()\nplt.legend()\nplt.show()\n```\n\n# Developing\n\nBefore committing:\n- Update formatting: `poe fmt`\n- Lints: `poe flake`\n- Run test suite: `poe test`\n- Optionally: [fuzz](#Fuzzing) any new models\n\n# Design Philosophy\n\n## Good Heuristics\n\nLife is too short for failed fits. We can\'t guarantee to fit every dataset without any\nhelp from the user (e.g. specifying initial parameter values) no matter how noisy or\nincomplete it is...but we do our best!\n\nEvery fit model has a "parameter estimator" which uses heuristics to find good estimates\nof the values of the model\'s free parameters. We expect these heuristics to be good\nenough to allow the optimizer to fit any "reasonable" dataset. Fit failures are viewed\nas a bug and we encourage our users to file issues where they find them (please post an\nexample dataset in the issue).\n\nCurrently this project is a MVP and many of the heuristics need some work. Expect there\nto be cases where we could easily do better. Please report them where you find them!\n\n## Validation\n\nIt\'s not enough to just fit the data, we want to know if we can trust the fit results\nbefore acting on them.  There are two distinct aspects to the validation problem: did\nthe fit find the model parameters which best match the data (as opposed to getting stuck\nin a local minimum in parameter space far from the global optimum)? and, are the fitted\nparameter values consistent with our prior knowledge of the system (e.g. we know that a\nfringe contrast must lie within certain bounds).\n\nFirst, any prior knowledge about the system should be incorporated by specifying fixed\nparameter values and parameter bounds. After that, the fit is validated. At present,\nvalidation is done using the Chi-squared as a test for goodness of fit. It is likely\nthat additional validation tests will be added as the package grows.\n\n## General purpose\n\nThis library is designed to be general purpose; rather than tackling specific problems\nwe try to target sets of problems -- we want to fit sinusoids not *your* sinusoid. This\nis reflected, for example, in the choices of parametrisation, which are intended to be\nextremely flexible, and the effort put into heuristics. If you find you can\'t easily fit\nyour sinusoid with the standard model/heuristics it\'s probably a bug in the model design\nso please open an issue.\n\nWe encourage contributions of new fit models, but please consider generality before\nsubmission. If you want to solve a specific problem in front of you, that\'s fine but\nprobably better suited to your own codebase.\n\n## Extensibility\n\nThe library is designed to be extensible and ergonomic to user. Want to use different\nstatistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some\ncustom post-fit processing? Override the `calculate_derived_parameters` method. Want to\ntweak the parameter estimator for a model? Create a new model class that inherits from\nthe original model and modify away. If you\'re struggling to do what you want, it\'s\nprobably a bug in the library so please report it.\n\n`ionics_fits` provides a number of tools to make it easier to extend models (see, for\nexample in [`models.utils`](../master/ionics_fits/models/utils.py)). Say you want to...\n\n## Rescaling models\n\n...fit some frequency-domain Rabi oscillation data. However, the model works in angular\nunits, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`\ntool.\n\n```python\ndetuning_model = fits.models.utils.rescale_model_x(fits.models.RabiFlopFreq, 2 * np.pi)\n```\n\nOr, suppose you actually want to scan the magnetic field and find the field offset which\nputs the transition at a particular frequency?\n```python\nclass _RabiBField(fits.models.RabiFlopFreq):\n    def __init__(self, dfdB, B_0, f_0, start_excited):\n        super().__init__(start_excited=start_excited)\n        self.dfdB = dfdB\n        self.B_0 = B_0\n        self.f_0 = f_0\n\n    def calculate_derived_params(self, x, y, fitted_params, fit_uncertainties):\n        derived_params, derived_uncertainties = super().calculate_derived_params(\n            x, y, fitted_params, fit_uncertainties\n        )\n\n        df = derived_params["f_0"] - self.f_0\n        dB = df / self.dfdB\n        B_0 = dB + self.B_0\n\n        derived_params["B_0"] = B_0\n        derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB\n\n        return derived_params, derived_uncertainties\n\nRabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)\n```\n\n## Aggregating models\n\n...fit multiple independent models simultaneously and do some post-processing on the\nresults. Use an `AggregateModel`.\n\n```python\nclass LineAndTriange(fits.models.AggregateModel):\n  def __init__(self):\n    line = fits.models.Line()\n    triangle = fits.models.Triangle()\n    super().__init__(models=[("line", line), "triangle", triangle])\n\n  def calculate_derived_params(\n      self,\n      x: Array[("num_samples",), np.float64],\n      y: Array[("num_samples",), np.float64],\n      fitted_params: Dict[str, float],\n      fit_uncertainties: Dict[str, float],\n  ) -> Tuple[Dict[str, float], Dict[str, float]]:\n      derived_params, derived_uncertainties = super().calculate_derived_params()\n      # derive new results from the two fits\n      return derived_params, derived_uncertainties\n```\n\n## And more!\n\nAt present the library is still an MVP. Further work will be driven by use cases, so\nplease open an issue if you find you can\'t easily extend the library in the way you\nwant.\n\n# Ontology\n\nThere are two main kinds of object in the library: `fit`s and `model`s. Models are\ngeneral-purpose functions to be fitted, such as sinusoids or Lorentzians, but are\nagnostic about the statistics. Fits do the fitting (maximum likelihood parameter\nestimation) and validation based on some underlying statistics (normal, binomial, etc). \n\n# Testing methodology\n\nThis package uses both `unit test`s and `fuzzing`.\n\n## Unit Tests\n\n- run using `poe test`\n- to run a subset of tests use the `-k` flag e.g. `poe test -k "rabi"` to run only tests\n  with the word `rabi` in their name. For more information about configuring pytest see\n  the [documentation](https://docs.pytest.org/en/7.1.x/)\n- all tests must pass before a PR can be merged into master\n- PRs to add new models will only be merged once they have reasonable test coverage\n- unit tests aim to provide good coverage over the space of "reasonable datasets". There\n  will always be corner-cases where the fits fail and that\'s fine; the aim here is to\n  cover the main cases users will hit in the wild\n- when a user hits a case in the wild where the fit fails unexpectedly (i.e. we think\n  the fit code should have handled it), a `regression test` based on the failing\n  dataset should be added\n- unit tests should be deterministic. Synthetic datasets should be included in the test\n  rather than randomly generated at run time. Tip: while writing a test it\'s fine to let\n  the test code generate datasets for you. Once you\'re happy, run the test in verbose\n  mode and copy the dataset from the log output\n\n## Fuzzing\n\n- fuzzing is non-deterministic (random parameter values, randomly generated datasets)\n  exploration of the parameter space.\n- used when developing / debugging fits, but not automatically run by CI\n- run with `poe fuzz` (see `--help` for details)\n- fit failures during fuzzing are not automatically considered a bug; unlike unit tests,\n  fuzzing explores the "unreasonable" part of parameter space as well. Indeed, a large\n  part of the point of fuzzing is to help the developer understand what should be\n  considered "reasonable" (this information should end up in the documentation for the\n  fuzzed model).\n',
     'author': 'hartytp',
     'author_email': 'thomas.peter.harty@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ionics_fits-1.0.3/PKG-INFO` & `ionics_fits-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ionics-fits
-Version: 1.0.3
+Version: 1.0.4
 Summary: Lightweight Python data fitting library with an emphasis on AMO/Quantum Information
 Author: hartytp
 Author-email: thomas.peter.harty@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
+Requires-Dist: pyqt5-qt5 (>=5.15.2,<6.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Description-Content-Type: text/markdown
 
 Lightweight Python library for data fitting with an emphasis on AMO (Atomic Molecular
 and Optical physics) and Quantum Information.
 
@@ -143,20 +145,24 @@
 ## Extensibility
 
 The library is designed to be extensible and ergonomic to user. Want to use different
 statistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some
 custom post-fit processing? Override the `calculate_derived_parameters` method. Want to
 tweak the parameter estimator for a model? Create a new model class that inherits from
 the original model and modify away. If you're struggling to do what you want, it's
-probably a bug in the library so report it.
+probably a bug in the library so please report it.
 
-`ionics_fits` provides a number of tools in [`models.utils`](../master/ionics_fits/models/utils.py) to make it easier to
-extend models. For example, say you want to fit some frequency-domain Rabi oscillation
-data. However, the model works in angular units, but your tooling needs linear units. No
-problem! Simply use the `rescale_model_x` tool:
+`ionics_fits` provides a number of tools to make it easier to extend models (see, for
+example in [`models.utils`](../master/ionics_fits/models/utils.py)). Say you want to...
+
+## Rescaling models
+
+...fit some frequency-domain Rabi oscillation data. However, the model works in angular
+units, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`
+tool.
 
 ```python
 detuning_model = fits.models.utils.rescale_model_x(fits.models.RabiFlopFreq, 2 * np.pi)
 ```
 
 Or, suppose you actually want to scan the magnetic field and find the field offset which
 puts the transition at a particular frequency?
@@ -181,17 +187,43 @@
         derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB
 
         return derived_params, derived_uncertainties
 
 RabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)
 ```
 
-At present the library is still an MVP. While we do provide some hooks there aren't
-many. The addition of further hooks will be driven by use cases, so please open an issue
-if you find you can't easily extend the library in the way you want.
+## Aggregating models
+
+...fit multiple independent models simultaneously and do some post-processing on the
+results. Use an `AggregateModel`.
+
+```python
+class LineAndTriange(fits.models.AggregateModel):
+  def __init__(self):
+    line = fits.models.Line()
+    triangle = fits.models.Triangle()
+    super().__init__(models=[("line", line), "triangle", triangle])
+
+  def calculate_derived_params(
+      self,
+      x: Array[("num_samples",), np.float64],
+      y: Array[("num_samples",), np.float64],
+      fitted_params: Dict[str, float],
+      fit_uncertainties: Dict[str, float],
+  ) -> Tuple[Dict[str, float], Dict[str, float]]:
+      derived_params, derived_uncertainties = super().calculate_derived_params()
+      # derive new results from the two fits
+      return derived_params, derived_uncertainties
+```
+
+## And more!
+
+At present the library is still an MVP. Further work will be driven by use cases, so
+please open an issue if you find you can't easily extend the library in the way you
+want.
 
 # Ontology
 
 There are two main kinds of object in the library: `fit`s and `model`s. Models are
 general-purpose functions to be fitted, such as sinusoids or Lorentzians, but are
 agnostic about the statistics. Fits do the fitting (maximum likelihood parameter
 estimation) and validation based on some underlying statistics (normal, binomial, etc).
```

