# Comparing `tmp/vaxadium-0.2.0.tar.gz` & `tmp/vaxadium-0.2.0rc0.tar.gz`

## Comparing `vaxadium-0.2.0.tar` & `vaxadium-0.2.0rc0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/_version.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/axes.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/cli_density.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/cli_dls.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/cli_macros.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/cli_vaxadium.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/configuration.py
--rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/constants.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/data_descriptors.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/defaults.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/experiment.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/logging_setup.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/physics.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/processors.py
--rw-r--r--   0        0        0    12554 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/runner.py
--rw-r--r--   0        0        0    14340 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/scaler.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/basechecker.py
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/calibration.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/convergence.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/data.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/extractor.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/checks/sample.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/core/axis_generators.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/core/detector.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/core/form_factors.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/core/fourier.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/core/units.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/g4diffsim/fitting.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/g4diffsim/macro_maker.py
--rw-r--r--   0        0        0    11483 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/g4diffsim/macros.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/g4diffsim/simulation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/io/__init__.py
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/io/nexus_reader.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/io/outputs.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/io/serializer_factory.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/io/serializers.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/__init__.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/attenuator.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/beam.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/cylinder_yz.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/cylinder_yz_runner.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/direction.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/illuminated_yz.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/illuminated_yz_runner.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/scatterer.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/transmission_map.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 vaxadium-0.2.0/vaxadium/transmission/yz_generator.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 vaxadium-0.2.0/.gitignore
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 vaxadium-0.2.0/AUTHORS.rst
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 vaxadium-0.2.0/LICENSE
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 vaxadium-0.2.0/README.rst
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 vaxadium-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 vaxadium-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/_version.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/axes.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_density.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_dls.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_macros.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/cli_vaxadium.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/configuration.py
+-rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/constants.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/data_descriptors.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/defaults.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/experiment.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/logging_setup.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/physics.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/processors.py
+-rw-r--r--   0        0        0    12554 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/runner.py
+-rw-r--r--   0        0        0    14340 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/scaler.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/basechecker.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/calibration.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/convergence.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/data.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/extractor.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/checks/sample.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/axis_generators.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/detector.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/form_factors.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/fourier.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/core/units.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/fitting.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/macro_maker.py
+-rw-r--r--   0        0        0    11483 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/macros.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/g4diffsim/simulation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/__init__.py
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/nexus_reader.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/outputs.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/serializer_factory.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/io/serializers.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/__init__.py
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/attenuator.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/beam.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz_runner.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/direction.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz_runner.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/scatterer.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/transmission_map.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/vaxadium/transmission/yz_generator.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/.gitignore
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/AUTHORS.rst
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/LICENSE
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/README.rst
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vaxadium-0.2.0rc0/PKG-INFO
```

### Comparing `vaxadium-0.2.0/vaxadium/cli_density.py` & `vaxadium-0.2.0rc0/vaxadium/cli_density.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/cli_dls.py` & `vaxadium-0.2.0rc0/vaxadium/cli_dls.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/cli_macros.py` & `vaxadium-0.2.0rc0/vaxadium/cli_macros.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/cli_vaxadium.py` & `vaxadium-0.2.0rc0/vaxadium/cli_vaxadium.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/configuration.py` & `vaxadium-0.2.0rc0/vaxadium/configuration.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/constants.py` & `vaxadium-0.2.0rc0/vaxadium/constants.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/data_descriptors.py` & `vaxadium-0.2.0rc0/vaxadium/data_descriptors.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/experiment.py` & `vaxadium-0.2.0rc0/vaxadium/experiment.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/logging_setup.py` & `vaxadium-0.2.0rc0/vaxadium/logging_setup.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/physics.py` & `vaxadium-0.2.0rc0/vaxadium/physics.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/processors.py` & `vaxadium-0.2.0rc0/vaxadium/processors.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/runner.py` & `vaxadium-0.2.0rc0/vaxadium/runner.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/scaler.py` & `vaxadium-0.2.0rc0/vaxadium/scaler.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/__init__.py` & `vaxadium-0.2.0rc0/vaxadium/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/basechecker.py` & `vaxadium-0.2.0rc0/vaxadium/checks/basechecker.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/calibration.py` & `vaxadium-0.2.0rc0/vaxadium/checks/calibration.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/convergence.py` & `vaxadium-0.2.0rc0/vaxadium/checks/convergence.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/data.py` & `vaxadium-0.2.0rc0/vaxadium/checks/data.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/extractor.py` & `vaxadium-0.2.0rc0/vaxadium/checks/extractor.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/checks/sample.py` & `vaxadium-0.2.0rc0/vaxadium/checks/sample.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/core/detector.py` & `vaxadium-0.2.0rc0/vaxadium/core/detector.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/core/form_factors.py` & `vaxadium-0.2.0rc0/vaxadium/core/form_factors.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/core/fourier.py` & `vaxadium-0.2.0rc0/vaxadium/core/fourier.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/g4diffsim/fitting.py` & `vaxadium-0.2.0rc0/vaxadium/g4diffsim/fitting.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/g4diffsim/macros.py` & `vaxadium-0.2.0rc0/vaxadium/g4diffsim/macros.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/io/nexus_reader.py` & `vaxadium-0.2.0rc0/vaxadium/io/nexus_reader.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/io/outputs.py` & `vaxadium-0.2.0rc0/vaxadium/io/outputs.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/io/serializer_factory.py` & `vaxadium-0.2.0rc0/vaxadium/io/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/io/serializers.py` & `vaxadium-0.2.0rc0/vaxadium/io/serializers.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/attenuator.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/attenuator.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/beam.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/beam.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/cylinder_yz.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/cylinder_yz_runner.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/cylinder_yz_runner.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/direction.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/direction.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/illuminated_yz.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/illuminated_yz_runner.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/illuminated_yz_runner.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/scatterer.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/scatterer.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/transmission_map.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/transmission_map.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/vaxadium/transmission/yz_generator.py` & `vaxadium-0.2.0rc0/vaxadium/transmission/yz_generator.py`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/.gitignore` & `vaxadium-0.2.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/LICENSE` & `vaxadium-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/README.rst` & `vaxadium-0.2.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/pyproject.toml` & `vaxadium-0.2.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vaxadium-0.2.0/PKG-INFO` & `vaxadium-0.2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaxadium
-Version: 0.2.0
+Version: 0.2.0rc0
 Summary: Processes total scattering data using Monte Carlo simulations
 Project-URL: Homepage, https://github.com/DiamondLightSource/vaxadium
 Project-URL: Issues, https://github.com/DiamondLightSource/vaxadium/issues
 Author-email: Dean Keeble <dean.keeble@diamond.ac.uk>
 License-Expression: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
```

