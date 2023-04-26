# Comparing `tmp/bioexplorer-1.4.0.tar.gz` & `tmp/bioexplorer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioexplorer-1.4.0.tar", last modified: Fri Sep  2 07:38:37 2022, max compression
+gzip compressed data, was "bioexplorer-1.5.0.tar", last modified: Wed Feb  1 15:42:48 2023, max compression
```

## Comparing `bioexplorer-1.4.0.tar` & `bioexplorer-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 07:38:37.494256 bioexplorer-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-09-02 07:38:37.494256 bioexplorer-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 07:38:37.494256 bioexplorer-1.4.0/bioexplorer/
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   121696 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/bio_explorer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17904 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/metabolism.py
--rw-r--r--   0 runner    (1001) docker     (121)    19889 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/movie_maker.py
--rw-r--r--   0 runner    (1001) docker     (121)    11676 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/movie_scenario.py
--rw-r--r--   0 runner    (1001) docker     (121)    32207 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/notebook_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     8983 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/transfer_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-02 07:37:16.000000 bioexplorer-1.4.0/bioexplorer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 07:38:37.494256 bioexplorer-1.4.0/bioexplorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-09-02 07:38:37.000000 bioexplorer-1.4.0/bioexplorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-02 07:38:37.000000 bioexplorer-1.4.0/bioexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 07:38:37.000000 bioexplorer-1.4.0/bioexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-02 07:38:37.000000 bioexplorer-1.4.0/bioexplorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-02 07:38:37.000000 bioexplorer-1.4.0/bioexplorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-09-02 07:37:17.000000 bioexplorer-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-09-02 07:37:17.000000 bioexplorer-1.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-02 07:38:37.494256 bioexplorer-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-09-02 07:37:17.000000 bioexplorer-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:42:48.211297 bioexplorer-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-02-01 15:42:48.211297 bioexplorer-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:42:48.211297 bioexplorer-1.5.0/bioexplorer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129887 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/bio_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:42:48.211297 bioexplorer-1.5.0/bioexplorer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/core/api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/core/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/metabolism.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/movie_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/movie_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34076 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/notebook_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/transfer_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/bioexplorer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:42:48.211297 bioexplorer-1.5.0/bioexplorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-02-01 15:42:48.000000 bioexplorer-1.5.0/bioexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-01 15:42:48.000000 bioexplorer-1.5.0/bioexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 15:42:48.000000 bioexplorer-1.5.0/bioexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 15:42:48.000000 bioexplorer-1.5.0/bioexplorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-01 15:42:48.000000 bioexplorer-1.5.0/bioexplorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-01 15:42:48.211297 bioexplorer-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-01 15:41:28.000000 bioexplorer-1.5.0/setup.py
```

### Comparing `bioexplorer-1.4.0/PKG-INFO` & `bioexplorer-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioexplorer
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python API for the Blue Brain BioExplorer
 Home-page: https://github.com/BlueBrain/BioExplorer.git
 Author: Blue Brain Project, EPFL
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Project-URL: Documentation, https://bluebrain.github.io/BioExplorer/
 Project-URL: Source, https://github.com/BlueBrain/BioExplorer
```

### Comparing `bioexplorer-1.4.0/README.md` & `bioexplorer-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bioexplorer-1.4.0/bioexplorer/bio_explorer.py` & `bioexplorer-1.5.0/bioexplorer/bio_explorer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """BioExplorer class"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -24,15 +24,15 @@
 import math
 import os
 
 from pyquaternion import Quaternion
 
 import seaborn as sns
 
-from brayns import Client
+from .core.client import Client
 from .transfer_function import TransferFunction
 from .version import VERSION as __version__
 
 # pylint: disable=no-member
 # pylint: disable=dangerous-default-value
 # pylint: disable=invalid-name
 # pylint: disable=too-many-lines
@@ -44,23 +44,30 @@
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-statements
 # pylint: disable=missing-return-type-doc
 # pylint: disable=missing-return-doc
 # pylint: disable=missing-raises-doc
 
 
-class AnimationParams:
+class MolecularSystemAnimationParams:
     """
     Parameters used to introduce some randomness in the position and orientation of the protein.
 
     This is mainly used to make assemblies more realistic, and for animation purpose too.
     """
 
-    def __init__(self, seed=0, position_seed=0, position_strength=0.0, rotation_seed=0,
-                 rotation_strength=0.0, morphing_step=0.0):
+    def __init__(
+        self,
+        seed=0,
+        position_seed=0,
+        position_strength=0.0,
+        rotation_seed=0,
+        rotation_strength=0.0,
+        morphing_step=0.0,
+    ):
         """
         Animation parameters are used to define how molecules should be animated
 
         :seed: (int, optional): Randomization seed. Defaults to 0.
         :position_seed: (int, optional): Randomization seed for the position of the molecule.
         Defaults to 0.
         :position_strength: (float, optional): Strength of the position alteration. Defaults to 0.0.
@@ -80,25 +87,74 @@
     def to_list(self):
         """
         A list containing the values of class members
 
         :return: A list containing the values of class members
         :rtype: list
         """
-        return [self.seed, self.position_seed, self.position_strength, self.rotation_seed,
-                self.rotation_strength, self.morphing_step]
+        return [
+            self.seed,
+            self.position_seed,
+            self.position_strength,
+            self.rotation_seed,
+            self.rotation_strength,
+            self.morphing_step,
+        ]
+
+    def copy(self):
+        """
+        Copy the current object
+
+        :return: MolecularSystemAnimationParams: A copy of the object
+        """
+        return MolecularSystemAnimationParams(
+            self.seed,
+            self.position_seed,
+            self.position_strength,
+            self.rotation_seed,
+            self.rotation_strength,
+            self.morphing_step,
+        )
+
+
+class CellAnimationParams:
+    """Parameters used to introduce some sinusoidal function in a cell structure"""
+
+    def __init__(self, seed=0, offset=0, amplitude=1.0, frequency=1.0):
+        """
+        Animation parameters are used to define how cells should be animated
+
+        :seed: (int, optional): Initial position in the sinusoidal function. Defaults to 0.
+        :offset: (int, optional): offset in the sinusoidal function. Defaults to 0.
+        :amplitude: (float, optional): Amplitude of the sinusoidal function
+        :frequency: (float, optional): Frequency of the sinusoidal function
+        """
+        self.seed = seed
+        self.offset = offset
+        self.amplitude = amplitude
+        self.frequency = frequency
+
+    def to_list(self):
+        """
+        A list containing the values of class members
+
+        :return: A list containing the values of class members
+        :rtype: list
+        """
+        return [self.seed, self.offset, self.amplitude, self.frequency]
 
     def copy(self):
         """
         Copy the current object
 
-        :return: AnimationParams: A copy of the object
+        :return: MolecularSystemAnimationParams: A copy of the object
         """
-        return AnimationParams(self.seed, self.position_seed, self.position_strength,
-                               self.rotation_seed, self.rotation_strength, self.morphing_step)
+        return CellAnimationParams(
+            self.seed, self.offset, self.amplitude, self.frequency
+        )
 
 
 class Vector3:
     """A Vector3 is an array of 3 floats representing a 3D vector"""
 
     def __init__(self, *args):
         """
@@ -167,16 +223,16 @@
         """
         return Vector2(self.x, self.y)
 
 
 class BioExplorer:
     """Blue Brain BioExplorer"""
 
-    PLUGIN_API_PREFIX = 'be-'
-    CONTENTS_DELIMITER = '||||'
+    PLUGIN_API_PREFIX = "be-"
+    CONTENTS_DELIMITER = "||||"
 
     COLOR_SCHEME_NONE = 0
     COLOR_SCHEME_ATOMS = 1
     COLOR_SCHEME_CHAINS = 2
     COLOR_SCHEME_RESIDUES = 3
     COLOR_SCHEME_AMINO_ACID_SEQUENCE = 4
     COLOR_SCHEME_GLYCOSYLATION_SITE = 5
@@ -193,14 +249,18 @@
     SHADING_MODE_CHECKER = 8
     SHADING_MODE_GOODSELL = 9
 
     SHADING_CHAMELEON_MODE_NONE = 0
     SHADING_CHAMELEON_MODE_EMITTER = 1
     SHADING_CHAMELEON_MODE_RECEIVER = 2
 
+    SHADING_CLIPPING_MODE_NONE = 0
+    SHADING_CLIPPING_PLANE = 1
+    SHADING_CLIPPING_SPHERE = 2
+
     CAMERA_PROJECTION_PERSPECTIVE = 0
     CAMERA_PROJECTION_FISHEYE = 1
     CAMERA_PROJECTION_PANORAMIC = 2
     CAMERA_PROJECTION_CYLINDRIC = 3
 
     RNA_SHAPE_TREFOIL_KNOT = 0
     RNA_SHAPE_TORUS = 1
@@ -270,62 +330,80 @@
 
     POSITION_CONSTRAINT_INSIDE = 0
     POSITION_CONSTRAINT_OUTSIDE = 1
 
     VASCULATURE_REPRESENTATION_GRAPH = 0
     VASCULATURE_REPRESENTATION_SECTION = 1
     VASCULATURE_REPRESENTATION_SEGMENT = 2
+    VASCULATURE_REPRESENTATION_OPTIMIZED_SEGMENT = 3
 
     VASCULATURE_COLOR_SCHEME_NONE = 0
     VASCULATURE_COLOR_SCHEME_NODE = 1
     VASCULATURE_COLOR_SCHEME_SECTION = 2
     VASCULATURE_COLOR_SCHEME_SUBGRAPH = 3
     VASCULATURE_COLOR_SCHEME_PAIR = 4
     VASCULATURE_COLOR_SCHEME_ENTRYNODE = 5
     VASCULATURE_COLOR_SCHEME_RADIUS = 6
     VASCULATURE_COLOR_SCHEME_SECTION_POINTS = 7
     VASCULATURE_COLOR_SCHEME_SECTION_ORIENTATION = 8
+    VASCULATURE_COLOR_SCHEME_REGION = 9
+
+    VASCULATURE_REALISM_LEVEL_NONE = 0
+    VASCULATURE_REALISM_LEVEL_SECTION = 1
+    VASCULATURE_REALISM_LEVEL_BIFURCATION = 2
+    VASCULATURE_REALISM_LEVEL_ALL = 255
 
     MORPHOLOGY_COLOR_SCHEME_NONE = 0
     MORPHOLOGY_COLOR_SCHEME_SECTION_TYPE = 1
     MORPHOLOGY_COLOR_SCHEME_SECTION_ORIENTATION = 2
 
     POPULATION_COLOR_SCHEME_NONE = 0
     POPULATION_COLOR_SCHEME_ID = 1
 
     MORPHOLOGY_REPRESENTATION_GRAPH = 0
     MORPHOLOGY_REPRESENTATION_SECTION = 1
     MORPHOLOGY_REPRESENTATION_SEGMENT = 2
     MORPHOLOGY_REPRESENTATION_ORIENTATION = 3
 
+    MORPHOLOGY_REALISM_LEVEL_NONE = 0
+    MORPHOLOGY_REALISM_LEVEL_SOMA = 1
+    MORPHOLOGY_REALISM_LEVEL_AXON = 2
+    MORPHOLOGY_REALISM_LEVEL_DENDRITE = 4
+    MORPHOLOGY_REALISM_LEVEL_INTERNALS = 8
+    MORPHOLOGY_REALISM_LEVEL_EXTERNALS = 16
+    MORPHOLOGY_REALISM_LEVEL_SPINE = 32
+    MORPHOLOGY_REALISM_LEVEL_ALL = 255
+
     # Material offsets in neurons
     NB_MATERIALS_PER_MORPHOLOGY = 10
     NEURON_MATERIAL_VARICOSITY = 0
     NEURON_MATERIAL_SOMA = 1
     NEURON_MATERIAL_AXON = 2
     NEURON_MATERIAL_BASAL_DENDRITE = 3
     NEURON_MATERIAL_APICAL_DENDRITE = 4
-    NEURON_MATERIAL_AFFERENT_SYNPASE = 5
-    NEURON_MATERIAL_EFFERENT_SYNPASE = 6
+    NEURON_MATERIAL_SYNAPSE = 5
     NEURON_MATERIAL_MITOCHONDRION = 7
     NEURON_MATERIAL_NUCLEUS = 8
-    NEURON_MATERIAL_MYELIN_STEATH = 9
+    NEURON_MATERIAL_MYELIN_sheath = 9
 
-    def __init__(self, url='localhost:5000'):
+    def __init__(self, url="localhost:5000"):
         """Create a new BioExplorer instance"""
         self._url = url
         self._client = Client(url)
         self._v1_compatibility = False
 
         backend_version = self.version()
         if __version__ != backend_version:
             raise RuntimeError(
-                "Wrong version of the back-end (" + backend_version +
-                "). Use version " + __version__ +
-                " for this version of the BioExplorer python library")
+                "Wrong version of the back-end ("
+                + backend_version
+                + "). Use version "
+                + __version__
+                + " for this version of the BioExplorer python library"
+            )
 
     def __str__(self):
         """
         A pretty-print of the class
 
         :rtype: string
         """
@@ -344,20 +422,22 @@
         if not response["status"]:
             raise RuntimeError(response["contents"])
         return response
 
     def _invoke(self, method, params=None):
         prefixed_method = self.PLUGIN_API_PREFIX + method
         return self._client.rockets_client.request(
-            method=prefixed_method, params=params)
+            method=prefixed_method, params=params
+        )
 
     def _invoke_and_check(self, method, params=None):
         prefixed_method = self.PLUGIN_API_PREFIX + method
         response = self._client.rockets_client.request(
-            method=prefixed_method, params=params)
+            method=prefixed_method, params=params
+        )
         return self._check(response)
 
     def version(self):
         """
         Version of the BioExplorer application
 
         :rtype: string
@@ -377,15 +457,15 @@
         :rtype: Metrics
         """
         if self._client is None:
             return __version__
 
         return self._invoke_and_check("get-scene-information")
 
-    @ staticmethod
+    @staticmethod
     def authors():
         """
         List of authors
 
         :rtype: string
         """
         return "Cyrille Favreau (cyrille.favreau@epfl.ch)"
@@ -404,16 +484,22 @@
         Reset the camera for the current scene
 
         :return: Result of the call to the BioExplorer backend
         :rtype: Response
         """
         return self._invoke_and_check("reset-camera")
 
-    def set_focus_on(self, model_id, instance_id=0, distance=0.0,
-                     direction=Vector3(0.0, 0.0, 1.0), max_number_of_instances=1e6):
+    def set_focus_on(
+        self,
+        model_id,
+        instance_id=0,
+        distance=0.0,
+        direction=Vector3(0.0, 0.0, 1.0),
+        max_number_of_instances=1e6,
+    ):
         """
         Set focus on a specific instance of a model
 
         :return: Result of the call to the BioExplorer backend
         :rtype: Response
         """
         assert isinstance(direction, Vector3)
@@ -425,16 +511,20 @@
         params["direction"] = direction.to_list()
         params["maxNbInstances"] = max_number_of_instances
         result = self._invoke_and_check("set-focus-on", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def export_to_file(self, filename, low_bounds=Vector3(-1e38, -1e38, -1e38),
-                       high_bounds=Vector3(1e38, 1e38, 1e38)):
+    def export_to_file(
+        self,
+        filename,
+        low_bounds=Vector3(-1e38, -1e38, -1e38),
+        high_bounds=Vector3(1e38, 1e38, 1e38),
+    ):
         """
         Export current scene to file as an optimized binary cache file
 
         :filename: Full path of the binary cache file
         :low_bounds: Brick low bounds
         :high_bounds: Brick high bounds
         :return: Result of the call to the BioExplorer backend
@@ -446,17 +536,22 @@
         params["highBounds"] = high_bounds.to_list()
         params["fileFormat"] = BioExplorer.FILE_FORMAT_UNSPECIFIED
         result = self._invoke_and_check("export-to-file", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def export_to_database(self, connection_string, schema, brick_id,
-                           low_bounds=Vector3(-1e38, -1e38, -1e38),
-                           high_bounds=Vector3(1e38, 1e38, 1e38)):
+    def export_to_database(
+        self,
+        connection_string,
+        schema,
+        brick_id,
+        low_bounds=Vector3(-1e38, -1e38, -1e38),
+        high_bounds=Vector3(1e38, 1e38, 1e38),
+    ):
         """
         Export current scene to file as an optimized binary database entry
 
         :connection_string: Connection string to the database
         :schema: Database schema
         :schema: Id of the brick
         :low_bounds: Brick low bounds
@@ -490,16 +585,21 @@
         params["filename"] = filename
         params["fileFormat"] = BioExplorer.FILE_FORMAT_UNSPECIFIED
         result = self._invoke_and_check("import-from-cache", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def export_to_xyz(self, filename, file_format, low_bounds=Vector3(-1e38, -1e38, -1e38),
-                      high_bounds=Vector3(1e38, 1e38, 1e38)):
+    def export_to_xyz(
+        self,
+        filename,
+        file_format,
+        low_bounds=Vector3(-1e38, -1e38, -1e38),
+        high_bounds=Vector3(1e38, 1e38, 1e38),
+    ):
         """
         Exports current scene to file as a XYZ file
 
         :filename: Full path of the XYZ file
         :file_format: Defines the format of the XYZ file
         :return: Result of the call to the BioExplorer backend
         :rtype: Response
@@ -510,22 +610,33 @@
         params["highBounds"] = high_bounds.to_list()
         params["fileFormat"] = file_format
         result = self._invoke_and_check("export-to-xyz", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def add_sars_cov_2(self, name, resource_folder,
-                       shape_params=Vector3(45.0, 0.0, 0.0),
-                       animation_params=AnimationParams(0, 1, 0.25, 1, 0.1),
-                       nb_protein_s=62, nb_protein_m=50, nb_protein_e=42,
-                       open_protein_s_indices=[0], atom_radius_multiplier=1.0,
-                       add_glycans=False, add_rna_sequence=False,
-                       representation=REPRESENTATION_ATOMS_AND_STICKS, clipping_planes=list(),
-                       position=Vector3(), rotation=Quaternion(), apply_colors=False):
+    def add_sars_cov_2(
+        self,
+        name,
+        resource_folder,
+        shape_params=Vector3(45.0, 0.0, 0.0),
+        animation_params=MolecularSystemAnimationParams(0, 1, 0.25, 1, 0.1),
+        nb_protein_s=62,
+        nb_protein_m=50,
+        nb_protein_e=42,
+        open_protein_s_indices=[0],
+        atom_radius_multiplier=1.0,
+        add_glycans=False,
+        add_rna_sequence=False,
+        representation=REPRESENTATION_ATOMS_AND_STICKS,
+        clipping_planes=list(),
+        position=Vector3(),
+        rotation=Quaternion(),
+        apply_colors=False,
+    ):
         """
         Add a virus with the default SARS-COV-2 coronavirus parameters
 
         :name: Name of the SARS-COV-2 coronavirus
         :resource_folder: Folder containing the resources of the virus components (PDB and
                                  RNA files)
         :radius: Radius of the virus in nanometers
@@ -555,105 +666,121 @@
             if i not in open_conformation_indices:
                 closed_conformation_indices.append(i)
 
         ap = animation_params.copy()
 
         # Protein S (open)
         ap.seed = 0
-        membrane_proteins.append(Protein(
-            name=name + '_' + self.NAME_PROTEIN_S_OPEN,
-            source=os.path.join(pdb_folder, "6vyb.pdb"),
-            occurrences=nb_protein_s,
-            rotation=Quaternion(0.0, 1.0, 0.0, 0.0),
-            allowed_occurrences=open_conformation_indices,
-            transmembrane_params=Vector2(10.5, 10.5),
-            animation_params=ap
-        ))
+        membrane_proteins.append(
+            Protein(
+                name=name + "_" + self.NAME_PROTEIN_S_OPEN,
+                source=os.path.join(pdb_folder, "6vyb.pdb"),
+                occurrences=nb_protein_s,
+                rotation=Quaternion(0.0, 1.0, 0.0, 0.0),
+                allowed_occurrences=open_conformation_indices,
+                transmembrane_params=Vector2(10.5, 10.5),
+                animation_params=ap,
+            )
+        )
 
         # Protein S (closed)
-        membrane_proteins.append(Protein(
-            name=name + '_' + self.NAME_PROTEIN_S_CLOSED,
-            source=os.path.join(pdb_folder, "sars-cov-2-v1.pdb"),
-            occurrences=nb_protein_s,
-            rotation=Quaternion(0.0, 1.0, 0.0, 0.0),
-            allowed_occurrences=closed_conformation_indices,
-            transmembrane_params=Vector2(10.5, 10.5),
-            animation_params=ap
-        ))
+        membrane_proteins.append(
+            Protein(
+                name=name + "_" + self.NAME_PROTEIN_S_CLOSED,
+                source=os.path.join(pdb_folder, "sars-cov-2-v1.pdb"),
+                occurrences=nb_protein_s,
+                rotation=Quaternion(0.0, 1.0, 0.0, 0.0),
+                allowed_occurrences=closed_conformation_indices,
+                transmembrane_params=Vector2(10.5, 10.5),
+                animation_params=ap,
+            )
+        )
 
         # Protein M (QHD43419)
         ap.seed = 1
-        membrane_proteins.append(Protein(
-            name=name + '_' + self.NAME_PROTEIN_M,
-            source=os.path.join(pdb_folder, "QHD43419a.pdb"),
-            occurrences=nb_protein_m,
-            position=Vector3(2.5, 0.0, 0.0),
-            rotation=Quaternion(0.135, 0.99, 0.0, 0.0),
-            transmembrane_params=Vector2(0.5, 2.0),
-            animation_params=ap
-        ))
+        membrane_proteins.append(
+            Protein(
+                name=name + "_" + self.NAME_PROTEIN_M,
+                source=os.path.join(pdb_folder, "QHD43419a.pdb"),
+                occurrences=nb_protein_m,
+                position=Vector3(2.5, 0.0, 0.0),
+                rotation=Quaternion(0.135, 0.99, 0.0, 0.0),
+                transmembrane_params=Vector2(0.5, 2.0),
+                animation_params=ap,
+            )
+        )
 
         # Protein E (QHD43418 P0DTC4)
         ap.seed = 3
-        membrane_proteins.append(Protein(
-            name=name + '_' + self.NAME_PROTEIN_E,
-            source=os.path.join(pdb_folder, "QHD43418a.pdb"),
-            occurrences=nb_protein_e,
-            position=Vector3(2.5, 0.0, 0.0),
-            rotation=Quaternion(0.0, 0.707, 0.707, 0.0),
-            transmembrane_params=Vector2(0.5, 2.0),
-            animation_params=ap
-        ))
+        membrane_proteins.append(
+            Protein(
+                name=name + "_" + self.NAME_PROTEIN_E,
+                source=os.path.join(pdb_folder, "QHD43418a.pdb"),
+                occurrences=nb_protein_e,
+                position=Vector3(2.5, 0.0, 0.0),
+                rotation=Quaternion(0.0, 0.707, 0.707, 0.0),
+                transmembrane_params=Vector2(0.5, 2.0),
+                animation_params=ap,
+            )
+        )
 
         # Virus membrane
         ap.seed = 4
         lipid_sources = [
             os.path.join(membrane_folder, "segA.pdb"),
             os.path.join(membrane_folder, "segB.pdb"),
             os.path.join(membrane_folder, "segC.pdb"),
-            os.path.join(membrane_folder, "segD.pdb")
+            os.path.join(membrane_folder, "segD.pdb"),
         ]
 
         virus_membrane = Membrane(
             lipid_sources=lipid_sources,
             lipid_rotation=Quaternion(0.0, 1.0, 0.0, 0.0),
-            load_bonds=True, load_non_polymer_chemicals=True,
-            animation_params=ap
+            load_bonds=True,
+            load_non_polymer_chemicals=True,
+            animation_params=ap,
         )
 
         # Cell
         virus_cell = Cell(
             name=name,
             shape=self.ASSEMBLY_SHAPE_EMPTY_SPHERE,
-            shape_params=shape_params, membrane=virus_membrane,
-            proteins=membrane_proteins)
+            shape_params=shape_params,
+            membrane=virus_membrane,
+            proteins=membrane_proteins,
+        )
 
         self.add_cell(
             cell=virus_cell,
-            atom_radius_multiplier=atom_radius_multiplier, representation=representation,
-            position=position, rotation=rotation,
-            clipping_planes=clipping_planes)
+            atom_radius_multiplier=atom_radius_multiplier,
+            representation=representation,
+            position=position,
+            rotation=rotation,
+            clipping_planes=clipping_planes,
+        )
 
         # RNA Sequence
         if add_rna_sequence:
             params = Vector2(shape_params.x * 0.55, 0.5)
             rna_sequence = RNASequence(
                 source=os.path.join(rna_folder, "sars-cov-2.rna"),
                 protein_source=os.path.join(pdb_folder, "7bv1.pdb"),
                 shape=self.RNA_SHAPE_TREFOIL_KNOT,
                 shape_params=params,
                 values_range=Vector2(-8.0 * math.pi, 8.0 * math.pi),
                 curve_params=Vector3(1.51, 1.12, 1.93),
-                atom_radius_multiplier=atom_radius_multiplier, representation=representation,
-                animation_params=ap
+                atom_radius_multiplier=atom_radius_multiplier,
+                representation=representation,
+                animation_params=ap,
             )
             self.add_rna_sequence(
                 assembly_name=name,
-                name=name + '_' + BioExplorer.NAME_RNA_SEQUENCE,
-                rna_sequence=rna_sequence)
+                name=name + "_" + BioExplorer.NAME_RNA_SEQUENCE,
+                rna_sequence=rna_sequence,
+            )
 
         if add_glycans:
             glycan_representation = representation
             if representation == BioExplorer.REPRESENTATION_MESH:
                 glycan_representation = BioExplorer.REPRESENTATION_ATOMS_AND_STICKS
 
             complex_folder = os.path.join(glycan_folder, "complex")
@@ -681,120 +808,183 @@
                 assembly_name=name,
                 glycan_type=self.NAME_GLYCAN_HIGH_MANNOSE,
                 protein_name=self.NAME_PROTEIN_S_CLOSED,
                 paths=high_mannose_paths,
                 indices=indices_closed,
                 representation=glycan_representation,
                 atom_radius_multiplier=atom_radius_multiplier,
-                animation_params=AnimationParams(0, 0, 0.0,
-                                                 animation_params.rotation_seed + 7,
-                                                 animation_params.rotation_strength)
+                animation_params=MolecularSystemAnimationParams(
+                    0,
+                    0,
+                    0.0,
+                    animation_params.rotation_seed + 7,
+                    animation_params.rotation_strength,
+                ),
             )
             self.add_multiple_glycans(
                 assembly_name=name,
                 glycan_type=self.NAME_GLYCAN_HIGH_MANNOSE,
                 protein_name=self.NAME_PROTEIN_S_OPEN,
                 paths=high_mannose_paths,
                 indices=indices_open,
                 representation=glycan_representation,
                 atom_radius_multiplier=atom_radius_multiplier,
-                animation_params=AnimationParams(0, 0, 0.0,
-                                                 animation_params.rotation_seed + 7,
-                                                 animation_params.rotation_strength)
+                animation_params=MolecularSystemAnimationParams(
+                    0,
+                    0,
+                    0.0,
+                    animation_params.rotation_seed + 7,
+                    animation_params.rotation_strength,
+                ),
             )
 
             # Complex
-            indices_closed = [17, 74, 149, 165, 282, 331,
-                              343, 616, 657, 1098, 1134, 1158, 1173, 1194]
-            indices_open = [17, 74, 149, 165, 282, 331, 343, 657, 1098, 1134, 1158, 1173, 1194]
+            indices_closed = [
+                17,
+                74,
+                149,
+                165,
+                282,
+                331,
+                343,
+                616,
+                657,
+                1098,
+                1134,
+                1158,
+                1173,
+                1194,
+            ]
+            indices_open = [
+                17,
+                74,
+                149,
+                165,
+                282,
+                331,
+                343,
+                657,
+                1098,
+                1134,
+                1158,
+                1173,
+                1194,
+            ]
             self.add_multiple_glycans(
                 assembly_name=name,
                 glycan_type=self.NAME_GLYCAN_COMPLEX,
                 protein_name=self.NAME_PROTEIN_S_CLOSED,
                 paths=complex_paths,
                 indices=indices_closed,
                 representation=glycan_representation,
                 atom_radius_multiplier=atom_radius_multiplier,
-                animation_params=AnimationParams(0, 0, 0.0,
-                                                 animation_params.rotation_seed + 8,
-                                                 2.0 * animation_params.rotation_strength)
+                animation_params=MolecularSystemAnimationParams(
+                    0,
+                    0,
+                    0.0,
+                    animation_params.rotation_seed + 8,
+                    2.0 * animation_params.rotation_strength,
+                ),
             )
 
             self.add_multiple_glycans(
                 assembly_name=name,
                 glycan_type=self.NAME_GLYCAN_COMPLEX,
                 protein_name=self.NAME_PROTEIN_S_OPEN,
                 paths=complex_paths,
                 indices=indices_open,
                 representation=glycan_representation,
                 atom_radius_multiplier=atom_radius_multiplier,
-                animation_params=AnimationParams(0, 0, 0.0,
-                                                 animation_params.rotation_seed + 8,
-                                                 2.0 * animation_params.rotation_strength)
+                animation_params=MolecularSystemAnimationParams(
+                    0,
+                    0,
+                    0.0,
+                    animation_params.rotation_seed + 8,
+                    2.0 * animation_params.rotation_strength,
+                ),
             )
 
             # O-Glycans
             for index in [323, 325]:
-                o_glycan_name = (name + "_" + self.NAME_GLYCAN_O_GLYCAN + "_" +
-                                 str(index))
+                o_glycan_name = (
+                    name + "_" + self.NAME_GLYCAN_O_GLYCAN + "_" + str(index)
+                )
                 o_glycan = Sugar(
                     assembly_name=name,
                     name=o_glycan_name,
                     source=o_glycan_paths[0],
                     protein_name=name + "_" + self.NAME_PROTEIN_S_CLOSED,
                     site_indices=[index],
                     representation=glycan_representation,
                     atom_radius_multiplier=atom_radius_multiplier,
-                    animation_params=AnimationParams(0, 0, 0.0,
-                                                     animation_params.rotation_seed + 9,
-                                                     2.0 * animation_params.rotation_strength)
+                    animation_params=MolecularSystemAnimationParams(
+                        0,
+                        0,
+                        0.0,
+                        animation_params.rotation_seed + 9,
+                        2.0 * animation_params.rotation_strength,
+                    ),
                 )
                 self.add_sugar(o_glycan)
 
             # High-mannose glycans on Protein M
             indices = [5]
             protein_name = name + "_" + self.NAME_PROTEIN_M
             high_mannose_glycans = Sugar(
                 rotation=Quaternion(0.707, 0.0, 0.0, 0.707),
                 assembly_name=name,
                 name=protein_name + "_" + self.NAME_GLYCAN_HIGH_MANNOSE,
                 protein_name=protein_name,
                 source=high_mannose_paths[0],
                 site_indices=indices,
                 representation=glycan_representation,
-                animation_params=AnimationParams(0, 0, 0.0,
-                                                 animation_params.rotation_seed + 10,
-                                                 2.0 * animation_params.rotation_strength)
+                animation_params=MolecularSystemAnimationParams(
+                    0,
+                    0,
+                    0.0,
+                    animation_params.rotation_seed + 10,
+                    2.0 * animation_params.rotation_strength,
+                ),
             )
             self.add_glycan(high_mannose_glycans)
 
             # Complex glycans on Protein E
             indices = [48, 66]
             protein_name = name + "_" + self.NAME_PROTEIN_E
             complex_glycans = Sugar(
                 rotation=Quaternion(0.707, 0.0, 0.0, 0.707),
                 assembly_name=name,
                 name=protein_name + "_" + self.NAME_GLYCAN_COMPLEX,
                 protein_name=protein_name,
                 source=complex_paths[0],
                 site_indices=indices,
                 representation=glycan_representation,
-                animation_params=AnimationParams(0, 0, 0.0,
-                                                 animation_params.rotation_seed + 11,
-                                                 2.0 * animation_params.rotation_strength)
+                animation_params=MolecularSystemAnimationParams(
+                    0,
+                    0,
+                    0.0,
+                    animation_params.rotation_seed + 11,
+                    2.0 * animation_params.rotation_strength,
+                ),
             )
             self.add_glycan(complex_glycans)
 
         if apply_colors:
             # Apply default materials
-            self.apply_default_color_scheme(
-                shading_mode=self.SHADING_MODE_BASIC)
+            self.apply_default_color_scheme(shading_mode=self.SHADING_MODE_BASIC)
 
-    def add_cell(self, cell, atom_radius_multiplier=1.0, representation=REPRESENTATION_ATOMS,
-                 clipping_planes=list(), position=Vector3(), rotation=Quaternion()):
+    def add_cell(
+        self,
+        cell,
+        atom_radius_multiplier=1.0,
+        representation=REPRESENTATION_ATOMS,
+        clipping_planes=list(),
+        position=Vector3(),
+        rotation=Quaternion(),
+    ):
         """
         Add a cell assembly to the scene
 
         :cell: Description of the cell
         :atom_radius_multiplier: Representation of the protein (Atoms, atoms and sticks, etc)
         :representation: Multiplies atom radius by the specified value
         :clipping_planes: List of clipping planes to apply to the virus assembly
@@ -811,25 +1001,24 @@
         self.add_assembly(
             name=cell.name,
             shape=cell.shape,
             shape_params=cell.shape_params,
             shape_mesh_source=cell.shape_mesh_source,
             position=position,
             rotation=rotation,
-            clipping_planes=clipping_planes
+            clipping_planes=clipping_planes,
         )
 
         for protein in cell.proteins:
             if protein.occurrences != 0:
                 _protein = AssemblyProtein(
                     assembly_name=cell.name,
                     name=protein.name,
                     source=protein.source,
-                    load_non_polymer_chemicals=protein.
-                    load_non_polymer_chemicals,
+                    load_non_polymer_chemicals=protein.load_non_polymer_chemicals,
                     occurrences=protein.occurrences,
                     allowed_occurrences=protein.allowed_occurrences,
                     atom_radius_multiplier=atom_radius_multiplier,
                     load_bonds=True,
                     representation=representation,
                     transmembrane_params=protein.transmembrane_params,
                     animation_params=protein.animation_params,
@@ -841,20 +1030,26 @@
 
         cell.membrane.representation = representation
         cell.membrane.atom_radius_multiplier = atom_radius_multiplier
         return self.add_membrane(
             assembly_name=cell.name,
             name=cell.name + "_" + self.NAME_MEMBRANE,
             animation_params=cell.membrane.animation_params,
-            membrane=cell.membrane
+            membrane=cell.membrane,
         )
 
-    def add_volume(self, volume, atom_radius_multiplier=1.0,
-                   representation=REPRESENTATION_ATOMS_AND_STICKS, position=Vector3(),
-                   rotation=Quaternion(), constraints=list()):
+    def add_volume(
+        self,
+        volume,
+        atom_radius_multiplier=1.0,
+        representation=REPRESENTATION_ATOMS_AND_STICKS,
+        position=Vector3(),
+        rotation=Quaternion(),
+        constraints=list(),
+    ):
         """
         Add a volume assembly to the scene
 
         :volume: Description of the volume
         :atom_radius_multiplier: Representation of the protein (Atoms, atoms and sticks, etc)
         :representation: Multiplies atom radius by the specified value
         :position: Position of the volume in the scene
@@ -866,56 +1061,64 @@
         assert isinstance(position, Vector3)
         assert isinstance(constraints, list)
 
         _protein = AssemblyProtein(
             assembly_name=volume.name,
             name=volume.protein.name,
             source=volume.protein.source,
-            load_non_polymer_chemicals=volume.protein.
-            load_non_polymer_chemicals,
+            load_non_polymer_chemicals=volume.protein.load_non_polymer_chemicals,
             occurrences=volume.protein.occurrences,
             atom_radius_multiplier=atom_radius_multiplier,
             load_bonds=volume.protein.load_bonds,
             load_hydrogen=volume.protein.load_hydrogen,
             representation=representation,
             animation_params=volume.protein.animation_params,
             position=volume.protein.position,
             rotation=volume.protein.rotation,
-            constraints=constraints
+            constraints=constraints,
         )
 
         self.remove_assembly(volume.name)
         result = self.add_assembly(
             name=volume.name,
-            shape=volume.shape, shape_params=volume.shape_params,
-            position=position, rotation=rotation)
+            shape=volume.shape,
+            shape_params=volume.shape_params,
+            position=position,
+            rotation=rotation,
+        )
         if not result["status"]:
             raise RuntimeError(result["contents"])
         result = self.add_assembly_protein(_protein)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def add_surfactant(self, surfactant, atom_radius_multiplier=1.0,
-                       representation=REPRESENTATION_ATOMS, position=Vector3(),
-                       rotation=Quaternion(), animation_params=AnimationParams()):
+    def add_surfactant(
+        self,
+        surfactant,
+        atom_radius_multiplier=1.0,
+        representation=REPRESENTATION_ATOMS,
+        position=Vector3(),
+        rotation=Quaternion(),
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         Add a surfactant assembly to the scene
 
         :surfactant: Description of the surfactant
         :atom_radius_multiplier: Representation of the protein (Atoms, atoms and sticks, etc)
         :representation: Multiplies atom radius by the specified value
         :position: Position of the volume in the scene
         :rotation: rotation of the cell in the scene
         :animation_params: Random seed used to define the shape of the branches
         """
         assert isinstance(surfactant, Surfactant)
         assert isinstance(position, Vector3)
         assert isinstance(rotation, Quaternion)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
         shape = self.ASSEMBLY_SHAPE_EMPTY_SPHERE
         nb_branches = 1
         if surfactant.surfactant_protein == self.SURFACTANT_PROTEIN_A:
             shape = self.ASSEMBLY_SHAPE_FAN
             nb_branches = 6
         elif surfactant.surfactant_protein == self.SURFACTANT_PROTEIN_D:
@@ -938,41 +1141,46 @@
             assembly_name=surfactant.name,
             name=head_name,
             source=surfactant.head_source,
             occurrences=nb_branches,
             atom_radius_multiplier=atom_radius_multiplier,
             animation_params=animation_params,
             representation=representation,
-            position=p, rotation=r
+            position=p,
+            rotation=r,
         )
 
         collagens = list()
         for i in range(nb_collagens):
             d = collagen_size * (i + 1) - 7.0
             p = Vector3(0.0, 0.0, d)
             if self._v1_compatibility:
                 p = Vector3(0.0, 0.0, -d)
 
             collagens.append(
                 AssemblyProtein(
                     assembly_name=surfactant.name,
                     name=branch_name + str(i),
-                    position=p, atom_radius_multiplier=atom_radius_multiplier,
+                    position=p,
+                    atom_radius_multiplier=atom_radius_multiplier,
                     source=surfactant.branch_source,
                     occurrences=nb_branches,
                     animation_params=animation_params,
-                    representation=representation
-                ))
+                    representation=representation,
+                )
+            )
 
         self.remove_assembly(surfactant.name)
-        result = self.add_assembly(name=surfactant.name,
-                                   shape=shape,
-                                   shape_params=Vector3(),
-                                   position=position,
-                                   rotation=rotation)
+        result = self.add_assembly(
+            name=surfactant.name,
+            shape=shape,
+            shape_params=Vector3(),
+            position=position,
+            rotation=rotation,
+        )
         if not result["status"]:
             raise RuntimeError(result["contents"])
 
         for collagen in collagens:
             result = self.add_assembly_protein(collagen)
             if not result["status"]:
                 raise RuntimeError(result["contents"])
@@ -987,43 +1195,47 @@
 
         :enzyme_reaction: Description of the enzyme reaction
         :return: Result of the call to the BioExplorer backend
         """
         assert isinstance(enzyme_reaction, EnzymeReaction)
 
         self.remove_assembly(enzyme_reaction.assembly_name)
-        result = self.add_assembly(name=enzyme_reaction.assembly_name,
-                                   shape=BioExplorer.ASSEMBLY_SHAPE_POINT,
-                                   shape_params=Vector3())
+        result = self.add_assembly(
+            name=enzyme_reaction.assembly_name,
+            shape=BioExplorer.ASSEMBLY_SHAPE_POINT,
+            shape_params=Vector3(),
+        )
         if not result["status"]:
             raise RuntimeError(result["contents"])
 
-        substrate_names = ''
+        substrate_names = ""
         for substrate in enzyme_reaction.substrates:
             assert isinstance(substrate, Protein)
-            if substrate_names != '':
+            if substrate_names != "":
                 substrate_names += BioExplorer.CONTENTS_DELIMITER
             substrate_names += substrate.name
 
-        product_names = ''
+        product_names = ""
         for product in enzyme_reaction.products:
             assert isinstance(product, Protein)
-            if product_names != '':
+            if product_names != "":
                 product_names += BioExplorer.CONTENTS_DELIMITER
             product_names += product.name
 
         params = dict()
         params["assemblyName"] = enzyme_reaction.assembly_name
         params["name"] = enzyme_reaction.name
         params["enzymeName"] = enzyme_reaction.enzyme.name
         params["substrateNames"] = substrate_names
         params["productNames"] = product_names
         return self._invoke_and_check("add-enzyme-reaction", params)
 
-    def set_enzyme_reaction_progress(self, enzyme_reaction, instance_id=0, progress=0.0):
+    def set_enzyme_reaction_progress(
+        self, enzyme_reaction, instance_id=0, progress=0.0
+    ):
         """
         Set the progress of a given enzyme reaction
 
         :enzyme_reaction: EnzymeReaction object
         :instance_id: Enzyme protein instance. Defaults to 0.
         :progress: Progress of the enzyme reaction (between 0 and 1). Defaults to 0.
         :return: Result of the call to the BioExplorer backend
@@ -1031,63 +1243,96 @@
         params = dict()
         params["assemblyName"] = enzyme_reaction.assembly_name
         params["name"] = enzyme_reaction.name
         params["instanceId"] = instance_id
         params["progress"] = progress
         return self._invoke_and_check("set-enzyme-reaction-progress", params)
 
-    @ staticmethod
+    @staticmethod
     def get_mol():
         """
         Provide a hint to the meaning of life
 
         Provide a hint by solving a polynomial using Neville interpolation according to the given
         parameters provided by the BioExplorer. More information available at
         https://www.dcode.fr/function-equation-finder
 
         :return: A hint to the meaning of life
         """
         coefs = [
             [
-                [32341, 39916800], [89063, 1814400], [937889, 725760], [234527, 12096],
-                [221003071, 1209600], [97061099, 86400], [3289126079, 725760],
-                [106494629, 9072], [16747876289, 907200], [8214593, 525], [73270357, 13860],
-                [97, 1]
+                [32341, 39916800],
+                [89063, 1814400],
+                [937889, 725760],
+                [234527, 12096],
+                [221003071, 1209600],
+                [97061099, 86400],
+                [3289126079, 725760],
+                [106494629, 9072],
+                [16747876289, 907200],
+                [8214593, 525],
+                [73270357, 13860],
+                [97, 1],
             ],
             [
-                [2039, 13305600], [481, 43200], [251567, 725760], [6809, 1120],
-                [80200787, 1209600], [2243617, 4800], [172704437, 80640], [13473253, 2160],
-                [9901558223, 907200], [16059286, 1575], [10483043, 2772], [108, 1]
+                [2039, 13305600],
+                [481, 43200],
+                [251567, 725760],
+                [6809, 1120],
+                [80200787, 1209600],
+                [2243617, 4800],
+                [172704437, 80640],
+                [13473253, 2160],
+                [9901558223, 907200],
+                [16059286, 1575],
+                [10483043, 2772],
+                [108, 1],
             ],
             [
-                [13, 86400], [661, 72576], [269, 1120], [437929, 120960],
-                [6933401, 201600], [3696647, 17280], [7570727, 8640], [839289373, 362880],
-                [20844207, 5600], [32765923, 10080], [64229, 56], [100, 0]
-            ]
+                [13, 86400],
+                [661, 72576],
+                [269, 1120],
+                [437929, 120960],
+                [6933401, 201600],
+                [3696647, 17280],
+                [7570727, 8640],
+                [839289373, 362880],
+                [20844207, 5600],
+                [32765923, 10080],
+                [64229, 56],
+                [100, 0],
+            ],
         ]
 
         def mol(x, y):
             value = 0.0
             for i in range(len(coefs[y]) - 1):
                 j = len(coefs[y]) - i - 1
                 if i % 2 == coefs[y][len(coefs[y]) - 1][1]:
                     value -= coefs[y][i][0] * math.pow(x, j) / coefs[y][i][1]
                 else:
                     value += coefs[y][i][0] * math.pow(x, j) / coefs[y][i][1]
             value += coefs[y][len(coefs[y]) - 1][0]
             return round(value)
 
-        result = ''
+        result = ""
         for x in range(33):
             result += chr(mol(x % 12, int(x / 12)))
-        return 'You asked for the meaning of life and the answer is: ' + result
+        return "You asked for the meaning of life and the answer is: " + result
 
-    def add_assembly(self, name, shape=ASSEMBLY_SHAPE_POINT, shape_params=Vector3(),
-                     shape_mesh_source='', clipping_planes=list(), position=Vector3(),
-                     rotation=Quaternion()):
+    def add_assembly(
+        self,
+        name,
+        shape=ASSEMBLY_SHAPE_POINT,
+        shape_params=Vector3(),
+        shape_mesh_source="",
+        clipping_planes=list(),
+        position=Vector3(),
+        rotation=Quaternion(),
+    ):
         """
         Add an assembly to the scene
 
         :name: Name of the assembly
         :clipping_planes: List of clipping planes to apply to the virus assembly
         :position: Position of the scene in the scene
         :rotation: rotation of the assembly in the scene
@@ -1098,17 +1343,17 @@
         assert isinstance(rotation, Quaternion)
 
         clipping_planes_values = list()
         for plane in clipping_planes:
             for i in range(4):
                 clipping_planes_values.append(plane[i])
 
-        mesh_contents = ''
+        mesh_contents = ""
         if shape_mesh_source:
-            mesh_contents = ''.join(open(shape_mesh_source).readlines())
+            mesh_contents = "".join(open(shape_mesh_source).readlines())
 
         params = dict()
         params["name"] = name
         params["shape"] = shape
         params["shapeParams"] = shape_params.to_list()
         params["shapeMeshContents"] = mesh_contents
         params["position"] = position.to_list()
@@ -1121,25 +1366,33 @@
         Removes the specified assembly
 
         :name: Name of the assembly
         :return: Result of the call to the BioExplorer backend
         :rtype: Response
         """
         params = dict()
-        params['name'] = name
-        params['shape'] = BioExplorer.ASSEMBLY_SHAPE_POINT
-        params['shapeParams'] = list()
-        params["shapeMeshContents"] = ''
-        params['position'] = Vector3().to_list()
+        params["name"] = name
+        params["shape"] = BioExplorer.ASSEMBLY_SHAPE_POINT
+        params["shapeParams"] = list()
+        params["shapeMeshContents"] = ""
+        params["position"] = Vector3().to_list()
         params["rotation"] = list(Quaternion())
         params["clippingPlanes"] = list()
         return self._invoke_and_check("remove-assembly", params)
 
-    def set_protein_color_scheme(self, assembly_name, name, color_scheme, palette_name="",
-                                 palette_size=256, palette=list(), chain_ids=list()):
+    def set_protein_color_scheme(
+        self,
+        assembly_name,
+        name,
+        color_scheme,
+        palette_name="",
+        palette_size=256,
+        palette=list(),
+        chain_ids=list(),
+    ):
         """
         Set a color scheme to a protein
 
         :assembly_name: Name of the assembly containing the protein
         :name: Name of the protein
         :color_scheme: Color scheme
         :palette_name: Name of the Seaborn color palette
@@ -1166,49 +1419,55 @@
         params["palette"] = local_palette
         params["chainIds"] = chain_ids
         result = self._invoke_and_check("set-protein-color-scheme", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def set_protein_amino_acid_sequence_as_string(self, assembly_name, name,
-                                                  amino_acid_sequence):
+    def set_protein_amino_acid_sequence_as_string(
+        self, assembly_name, name, amino_acid_sequence
+    ):
         """
         Displays a specified amino acid sequence on the protein
 
         :assembly_name: Name of the assembly containing the protein
         :name: Name of the protein
         :amino_acid_sequence: String containing the amino acid sequence
         :return: Result of the call to the BioExplorer backend
         """
         params = dict()
         params["assemblyName"] = assembly_name
         params["name"] = name
         params["sequence"] = amino_acid_sequence
-        result = self._invoke_and_check("set-protein-amino-acid-sequence-as-string", params)
+        result = self._invoke_and_check(
+            "set-protein-amino-acid-sequence-as-string", params
+        )
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def set_protein_amino_acid_sequence_as_ranges(self, assembly_name, name,
-                                                  amino_acid_ranges):
+    def set_protein_amino_acid_sequence_as_ranges(
+        self, assembly_name, name, amino_acid_ranges
+    ):
         """
         Displays a specified amino acid range on the protein
 
         :assembly_name: Name of the assembly containing the protein
         :name: Name of the protein
         :amino_acid_ranges: Tuples containing the amino acid range
         :return: Result of the call to the BioExplorer backend
         """
         assert len(amino_acid_ranges) % 2 == 0
         params = dict()
         params["assemblyName"] = assembly_name
         params["name"] = name
         params["ranges"] = amino_acid_ranges
-        result = self._invoke_and_check("set-protein-amino-acid-sequence-as-ranges", params)
+        result = self._invoke_and_check(
+            "set-protein-amino-acid-sequence-as-ranges", params
+        )
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
     def get_protein_amino_acid_information(self, assembly_name, name):
         """
         Returns amino acid information of the protein
@@ -1221,16 +1480,17 @@
         params["assemblyName"] = assembly_name
         params["name"] = name
         result = self._invoke_and_check("get-protein-amino-acid-information", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result["contents"].split()
 
-    def set_protein_amino_acid(self, assembly_name, name, index, amino_acid_short_name,
-                               chain_ids=list()):
+    def set_protein_amino_acid(
+        self, assembly_name, name, index, amino_acid_short_name, chain_ids=list()
+    ):
         """
         Displays a specified amino acid sequence on the protein
 
         :assembly_name: Name of the assembly containing the protein
         :name: Name of the protein
         :index: Index of the amino acid in the sequence
         :amino_acid_short_name: String containing the short name of the amino acid
@@ -1247,16 +1507,22 @@
         params["aminoAcidShortName"] = amino_acid_short_name
         params["chainIds"] = chain_ids
         result = self._invoke_and_check("set-protein-amino-acid", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         return result
 
-    def set_protein_instance_transformation(self, assembly_name, name, instance_index,
-                                            position=Vector3(), rotation=Quaternion()):
+    def set_protein_instance_transformation(
+        self,
+        assembly_name,
+        name,
+        instance_index,
+        position=Vector3(),
+        rotation=Quaternion(),
+    ):
         """
         Set a transformation to an instance of a protein in an assembly
 
         :assembly_name: Name of the assembly containing the protein
         :name: Name of the protein
         :instance_index: Index of the protein instance
         :position: Position of the instance
@@ -1296,15 +1562,15 @@
         params["position"] = Vector3().to_list()
         params["rotation"] = list(Quaternion())
         result = self._invoke_and_check("get-protein-instance-transformation", params)
         if not result["status"]:
             raise RuntimeError(result["contents"])
         d = dict()
         for param in result["contents"].split("|"):
-            s = param.split('=')
+            s = param.split("=")
             d[s[0]] = s[1]
         return d
 
     def add_rna_sequence(self, assembly_name, name, rna_sequence):
         """
         Add an RNA sequence object to an assembly
 
@@ -1331,59 +1597,67 @@
                 curve_params = Vector3(0.5, 10.0, 0.0)
             elif rna_sequence.shape == self.RNA_SHAPE_TREFOIL_KNOT:
                 curve_params = Vector3(2.5, 2.0, 2.2)
 
         else:
             curve_params = rna_sequence.curve_params
 
-        protein_contents = ''
+        protein_contents = ""
         if rna_sequence.protein_source:
             protein_contents = "".join(open(rna_sequence.protein_source).readlines())
 
         params = dict()
         params["assemblyName"] = assembly_name
         params["name"] = name
-        params["pdbId"] = os.path.splitext(os.path.basename(rna_sequence.protein_source))[0].lower()
+        params["pdbId"] = os.path.splitext(
+            os.path.basename(rna_sequence.protein_source)
+        )[0].lower()
         params["contents"] = "".join(open(rna_sequence.source).readlines())
         params["proteinContents"] = protein_contents
         params["shape"] = rna_sequence.shape
         params["shapeParams"] = rna_sequence.shape_params.to_list()
         params["valuesRange"] = values_range.to_list()
         params["curveParams"] = curve_params.to_list()
         params["atomRadiusMultiplier"] = rna_sequence.atom_radius_multiplier
         params["representation"] = rna_sequence.representation
         params["animationParams"] = rna_sequence.animation_params.to_list()
         params["position"] = rna_sequence.position.to_list()
         params["rotation"] = list(rna_sequence.rotation)
         return self._invoke_and_check("add-rna-sequence", params)
 
-    def add_membrane(self, assembly_name, name, membrane, animation_params=AnimationParams()):
+    def add_membrane(
+        self,
+        assembly_name,
+        name,
+        membrane,
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         Add a membrane to the scene
 
         :assembly_name: Name of the assembly
         :name: Name of the cell
         :membrane: Description of the membrane
         :shape: Shape of the membrane
         :shape_params: Size of the membrane
         :animation_params: Seed used to randomise position the elements in the membrane
         :rotation: rotation of the proteins in the membrane
         :return: Result of the call to the BioExplorer backend
         """
         assert isinstance(membrane, Membrane)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
-        lipid_pdb_ids = ''
-        lipid_contents = ''
+        lipid_pdb_ids = ""
+        lipid_contents = ""
         for lipid_source in membrane.lipid_sources:
-            if lipid_contents != '':
+            if lipid_contents != "":
                 lipid_contents += BioExplorer.CONTENTS_DELIMITER
-            if lipid_pdb_ids != '':
+            if lipid_pdb_ids != "":
                 lipid_pdb_ids += BioExplorer.CONTENTS_DELIMITER
-            lipid_contents += ''.join(open(lipid_source).readlines())
+            lipid_contents += "".join(open(lipid_source).readlines())
             lipid_pdb_ids += os.path.splitext(os.path.basename(lipid_source))[0].lower()
 
         params = dict()
         params["assemblyName"] = assembly_name
         params["name"] = name
         params["lipidPDBIds"] = lipid_pdb_ids
         params["lipidContents"] = lipid_contents
@@ -1394,16 +1668,23 @@
         params["loadNonPolymerChemicals"] = membrane.load_non_polymer_chemicals
         params["representation"] = membrane.representation
         params["chainIds"] = membrane.chain_ids
         params["recenter"] = membrane.recenter
         params["animationParams"] = animation_params.to_list()
         return self._invoke_and_check("add-membrane", params)
 
-    def add_protein(self, protein, recenter=True, representation=REPRESENTATION_ATOMS_AND_STICKS,
-                    atom_radius_multiplier=1.0, position=Vector3(), rotation=Quaternion()):
+    def add_protein(
+        self,
+        protein,
+        recenter=True,
+        representation=REPRESENTATION_ATOMS_AND_STICKS,
+        atom_radius_multiplier=1.0,
+        position=Vector3(),
+        rotation=Quaternion(),
+    ):
         """
         Add a protein to the scene
 
         :name: Name of the protein
         :protein: Description of the protein
         :representation: Representation of the protein (Atoms, atoms and sticks, etc)
         :conformation_index: Index of the source to be used for the protein conformation
@@ -1412,49 +1693,49 @@
         :rotation: rotation of the protein in the scene
         :return: Result of the call to the BioExplorer backend
         """
         assert isinstance(protein, Protein)
 
         assembly_name = protein.name
         self.remove_assembly(assembly_name)
-        self.add_assembly(
-            name=assembly_name,
-            position=position, rotation=rotation)
+        self.add_assembly(name=assembly_name, position=position, rotation=rotation)
 
         _protein = AssemblyProtein(
             assembly_name=assembly_name,
-            name=protein.name, recenter=recenter,
+            name=protein.name,
+            recenter=recenter,
             source=protein.source,
             load_hydrogen=protein.load_hydrogen,
             atom_radius_multiplier=atom_radius_multiplier,
             load_bonds=protein.load_bonds,
             load_non_polymer_chemicals=protein.load_non_polymer_chemicals,
             representation=representation,
             position=protein.position,
-            rotation=protein.rotation, chain_ids=protein.chain_ids
+            rotation=protein.rotation,
+            chain_ids=protein.chain_ids,
         )
         return self.add_assembly_protein(_protein)
 
     def add_assembly_protein(self, protein):
         """
         Add a protein to an assembly
 
         :protein: Description of the protein
         :return: Result of the call to the BioExplorer backend
         """
         assert isinstance(protein, AssemblyProtein)
 
-        constraints = ''
+        constraints = ""
         for constraint in protein.constraints:
-            if constraints != '':
+            if constraints != "":
                 constraints += self.CONTENTS_DELIMITER
             if constraint[0] == BioExplorer.POSITION_CONSTRAINT_INSIDE:
-                constraints += '+' + constraint[1]
+                constraints += "+" + constraint[1]
             elif constraint[0] == BioExplorer.POSITION_CONSTRAINT_OUTSIDE:
-                constraints += '-' + constraint[1]
+                constraints += "-" + constraint[1]
             else:
                 raise RuntimeError("Unknown position constraint")
 
         params = dict()
         params["assemblyName"] = protein.assembly_name
         params["name"] = protein.name
         params["pdbId"] = protein.pdb_id
@@ -1497,17 +1778,27 @@
         params["chainIds"] = glycan.chain_ids
         params["siteIndices"] = glycan.site_indices
         params["rotation"] = list(glycan.rotation)
         params["animationParams"] = glycan.animation_params.to_list()
         return self._invoke_and_check("add-glycan", params)
 
     def add_multiple_glycans(
-            self, assembly_name, glycan_type, protein_name, paths, representation, chain_ids=list(),
-            indices=list(), load_bonds=True, atom_radius_multiplier=1.0, rotation=Quaternion(),
-            animation_params=AnimationParams()):
+        self,
+        assembly_name,
+        glycan_type,
+        protein_name,
+        paths,
+        representation,
+        chain_ids=list(),
+        indices=list(),
+        load_bonds=True,
+        atom_radius_multiplier=1.0,
+        rotation=Quaternion(),
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         Add glycans to a protein in a assembly
 
         :assembly_name: Name of the assembly
         :glycan_type: Type of glycans
         :protein_name: Name of the protein
         :paths: Paths to PDB files with various glycan structures
@@ -1518,39 +1809,44 @@
         :atom_radius_multiplier: Multiplies atom radius by the specified value
         :rotation: rotation applied to the glycan on the protein
         :shape_params: Extra optional parameters for positioning on the protein
         """
         assert isinstance(chain_ids, list)
         assert isinstance(indices, list)
         assert isinstance(rotation, Quaternion)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
         path_index = 0
         for source in paths:
             site_indices = list()
             if indices is not None:
                 for index in indices:
                     if index % len(paths) == path_index:
                         site_indices.append(index)
 
             if site_indices:
                 _glycan = Sugar(
                     assembly_name=assembly_name,
-                    name=assembly_name + "_" + protein_name + "_" +
-                    glycan_type + "_" + str(path_index),
+                    name=assembly_name
+                    + "_"
+                    + protein_name
+                    + "_"
+                    + glycan_type
+                    + "_"
+                    + str(path_index),
                     source=source,
                     protein_name=assembly_name + "_" + protein_name,
                     chain_ids=chain_ids,
                     atom_radius_multiplier=atom_radius_multiplier,
                     load_bonds=load_bonds,
                     representation=representation,
                     recenter=True,
                     site_indices=site_indices,
                     rotation=rotation,
-                    animation_params=animation_params
+                    animation_params=animation_params,
                 )
                 self.add_glycan(_glycan)
             path_index += 1
 
     def add_sugar(self, sugar):
         """
         Add sugar to a protein in an assembly
@@ -1581,17 +1877,21 @@
         Set rendering quality using presets
 
         :image_quality: Quality of the image (RENDERING_QUALITY_LOW or RENDERING_QUALITY_HIGH)
         :return: Result of the call to the BioExplorer backend
         """
         if image_quality == self.RENDERING_QUALITY_HIGH:
             self._client.set_renderer(
-                head_light=False, background_color=[96 / 255, 125 / 255, 139 / 255],
-                current='bio_explorer', samples_per_pixel=1, subsampling=4,
-                max_accum_frames=128)
+                head_light=False,
+                background_color=[96 / 255, 125 / 255, 139 / 255],
+                current="bio_explorer",
+                samples_per_pixel=1,
+                subsampling=4,
+                max_accum_frames=128,
+            )
             params = self._client.BioExplorerRendererParams()
             params.exposure = 1.0
             params.gi_samples = 1
             params.gi_weight = 0.3
             params.gi_distance = 5000
             params.shadows = 1.0
             params.soft_shadows = 0.1
@@ -1601,15 +1901,15 @@
             params.use_hardware_randomizer = False
             return self._client.set_renderer_params(params)
         return self._client.set_renderer(
             background_color=Vector3(),
             current="basic",
             samples_per_pixel=1,
             subsampling=4,
-            max_accum_frames=16
+            max_accum_frames=16,
         )
 
     def get_model_name(self, model_id):
         """
         Return the list of model ids in the current scene
 
         :return: List of model Ids
@@ -1656,19 +1956,32 @@
         assert isinstance(model_id, int)
 
         params = dict()
         params["modelId"] = model_id
         params["maxNbInstances"] = 0
         return self._invoke("get-material-ids", params)
 
-    def set_materials(self, model_ids, material_ids, diffuse_colors, specular_colors,
-                      specular_exponents=list(), opacities=list(), reflection_indices=list(),
-                      refraction_indices=list(), glossinesses=list(), shading_modes=list(),
-                      emissions=list(), cast_user_datas=list(), user_parameters=list(),
-                      chameleon_modes=list()):
+    def set_materials(
+        self,
+        model_ids,
+        material_ids,
+        diffuse_colors,
+        specular_colors,
+        specular_exponents=list(),
+        opacities=list(),
+        reflection_indices=list(),
+        refraction_indices=list(),
+        glossinesses=list(),
+        shading_modes=list(),
+        emissions=list(),
+        cast_user_datas=list(),
+        user_parameters=list(),
+        chameleon_modes=list(),
+        clipping_modes=list(),
+    ):
         """
         Set a list of material on a specified list of models
 
         :model_ids: IDs of the models
         :material_ids: IDs of the materials
         :diffuse_colors: List of diffuse colors (3 values between 0 and 1)
         :specular_colors: List of specular colors (3 values between 0 and 1)
@@ -1682,14 +1995,15 @@
                               SHADING_MODE_DIFFUSE, SHADING_MODE_ELECTRON, SHADING_MODE_CARTOON,
                               SHADING_MODE_ELECTRON_TRANSPARENCY, SHADING_MODE_PERLIN or
                               SHADING_MODE_DIFFUSE_TRANSPARENCY)
         :emissions: List of light emission intensities
         :user_parameters: List of convenience parameter used by some of the shaders
         :chameleon_modes: List of chameleon mode attributes. If receiver, material take the color of
         surrounding emitter geometry
+        :clipping_modes: List of clipping modes applied to the geometry attached to the material
         :return: Result of the request submission
         """
         if self._client is None:
             return
 
         d_colors = list()
         for diffuse in diffuse_colors:
@@ -1712,14 +2026,15 @@
         params["refractionIndices"] = refraction_indices
         params["emissions"] = emissions
         params["glossinesses"] = glossinesses
         params["castUserData"] = cast_user_datas
         params["shadingModes"] = shading_modes
         params["userParameters"] = user_parameters
         params["chameleonModes"] = chameleon_modes
+        params["clippingModes"] = clipping_modes
         return self._invoke_and_check("set-materials", params)
 
     def set_material_extra_attributes(self, model_id):
         """
         Set extra BioExplorer specific attributes to materials
 
         :model_id: ID of the model
@@ -1729,19 +2044,31 @@
             return
 
         params = dict()
         params["modelId"] = model_id
         params["maxNbInstances"] = 1
         return self._invoke_and_check("set-material-extra-attributes", params)
 
-    def set_materials_from_palette(self, model_ids, material_ids, palette, shading_mode,
-                                   specular_exponent, user_parameter=1.0, glossiness=1.0,
-                                   emission=0.0, opacity=1.0, reflection_index=0.0,
-                                   refraction_index=1.0, cast_user_data=False,
-                                   chameleon_mode=SHADING_CHAMELEON_MODE_NONE):
+    def set_materials_from_palette(
+        self,
+        model_ids,
+        material_ids,
+        palette,
+        shading_mode,
+        specular_exponent,
+        user_parameter=1.0,
+        glossiness=1.0,
+        emission=0.0,
+        opacity=1.0,
+        reflection_index=0.0,
+        refraction_index=1.0,
+        cast_user_data=False,
+        chameleon_mode=SHADING_CHAMELEON_MODE_NONE,
+        clipping_mode=SHADING_CLIPPING_MODE_NONE,
+    ):
         """
         Applies a palette of colors and attributes to specified materials
 
         :model_ids: Ids of the models
         :material_ids: Ids of the materials
         :palette: Palette of RGB colors
         :shading_mode: Shading mode (None, basic, diffuse, etc)
@@ -1750,14 +2077,15 @@
         :glossiness: Material glossiness
         :emission: Light emission
         :opacity: Opacity
         :reflection_index: Reflection index
         :refraction_index: Refraction index
         :chameleon_mode: Chameleon mode attributes. If receiver, material take the color of
         surrounding emitter geometry
+        :clipping_mode: Clipping mode applied to the geometry attached to the material
         """
         assert isinstance(specular_exponent, float)
         assert isinstance(user_parameter, float)
         assert isinstance(glossiness, float)
         assert isinstance(emission, float)
         assert isinstance(opacity, float)
         assert isinstance(reflection_index, float)
@@ -1772,274 +2100,297 @@
         specular_exponents = list()
         emissions = list()
         opacities = list()
         reflection_indices = list()
         refraction_indices = list()
         chameleon_modes = list()
         cast_user_datas = list()
+        clipping_modes = list()
         for color in palette:
             colors.append(color)
             shading_modes.append(shading_mode)
             user_parameters.append(user_parameter)
             specular_exponents.append(specular_exponent)
             glossinesses.append(glossiness)
             emissions.append(emission)
             opacities.append(opacity)
             reflection_indices.append(reflection_index)
             refraction_indices.append(refraction_index)
             chameleon_modes.append(chameleon_mode)
             cast_user_datas.append(cast_user_data)
+            clipping_modes.append(clipping_mode)
         self.set_materials(
             model_ids=model_ids,
             material_ids=material_ids,
             diffuse_colors=colors,
             specular_colors=colors,
             specular_exponents=specular_exponents,
             user_parameters=user_parameters,
             glossinesses=glossinesses,
             shading_modes=shading_modes,
             emissions=emissions,
             opacities=opacities,
             reflection_indices=reflection_indices,
             refraction_indices=refraction_indices,
             chameleon_modes=chameleon_modes,
-            cast_user_datas=cast_user_datas
+            cast_user_datas=cast_user_datas,
+            clipping_modes=clipping_modes,
         )
 
     def apply_default_color_scheme(
-            self, shading_mode, user_parameter=3.0, specular_exponent=5.0, glossiness=1.0,
-            glycans=True, proteins=True, membranes=True, collagen=True):
+        self,
+        shading_mode,
+        user_parameter=3.0,
+        specular_exponent=5.0,
+        glossiness=1.0,
+        glycans=True,
+        proteins=True,
+        membranes=True,
+        collagen=True,
+    ):
         """
         Apply a default color scheme to all components in the scene
 
         :shading_mode: Shading mode (None, basic, diffuse, electron, etc)
         :user_parameter: User parameter specific to each shading mode
         :specular_exponent: Specular exponent for diffuse shading modes
         :glossiness: Glossiness
         """
         glycans_colors = [[0, 1, 1], [1, 1, 0], [1, 0, 1], [0.2, 0.2, 0.7]]
 
         model_ids = self.get_model_ids()
 
         for model_id in model_ids["ids"]:
-            model_name = self.get_model_name(model_id)['name']
+            model_name = self.get_model_name(model_id)["name"]
             material_ids = self.get_material_ids(model_id)["ids"]
             nb_materials = len(material_ids)
 
             if glycans and self.NAME_GLYCAN_HIGH_MANNOSE in model_name:
                 palette = list()
                 for _ in range(nb_materials):
                     palette.append(glycans_colors[0])
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif glycans and self.NAME_GLYCAN_COMPLEX in model_name:
                 palette = list()
                 for _ in range(nb_materials):
                     palette.append(glycans_colors[1])
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif glycans and self.NAME_GLYCAN_HYBRID in model_name:
                 palette = list()
                 for _ in range(nb_materials):
                     palette.append(glycans_colors[2])
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif glycans and self.NAME_GLYCAN_O_GLYCAN in model_name:
                 palette = list()
                 for _ in range(nb_materials):
                     palette.append(glycans_colors[3])
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif membranes and self.NAME_MEMBRANE in model_name:
                 palette = sns.color_palette("gist_heat", nb_materials)
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
-            elif proteins and (self.NAME_RECEPTOR in model_name or
-                               self.NAME_TRANS_MEMBRANE in model_name or
-                               self.NAME_ION_CHANNEL in model_name or
-                               self.NAME_RNA_SEQUENCE in model_name):
+            elif proteins and (
+                self.NAME_RECEPTOR in model_name
+                or self.NAME_TRANS_MEMBRANE in model_name
+                or self.NAME_ION_CHANNEL in model_name
+                or self.NAME_RNA_SEQUENCE in model_name
+            ):
                 palette = sns.color_palette("OrRd_r", nb_materials)
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
-            elif proteins and (self.NAME_PROTEIN_S_CLOSED in model_name
-                               or self.NAME_PROTEIN_S_OPEN in model_name
-                               or self.NAME_PROTEIN_E in model_name
-                               or self.NAME_PROTEIN_M in model_name):
+            elif proteins and (
+                self.NAME_PROTEIN_S_CLOSED in model_name
+                or self.NAME_PROTEIN_S_OPEN in model_name
+                or self.NAME_PROTEIN_E in model_name
+                or self.NAME_PROTEIN_M in model_name
+            ):
                 palette = sns.color_palette("Greens", nb_materials)
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif proteins and self.NAME_GLUCOSE in model_name:
                 palette = sns.color_palette("Blues", nb_materials)
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif proteins and self.NAME_LACTOFERRIN in model_name:
                 palette = sns.color_palette("afmhot", nb_materials)
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif proteins and self.NAME_DEFENSIN in model_name:
                 palette = sns.color_palette("plasma_r", nb_materials)
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif proteins and (self.NAME_SURFACTANT_HEAD in model_name):
                 palette = sns.color_palette("OrRd_r", nb_materials)
                 emission = 0.0
                 if self.NAME_COLLAGEN in model_name:
                     emission = 0.1
                 self.set_materials_from_palette(
                     model_ids=[model_id],
                     material_ids=material_ids,
                     palette=palette,
                     shading_mode=shading_mode,
                     emission=emission,
                     user_parameter=user_parameter,
                     glossiness=glossiness,
-                    specular_exponent=specular_exponent
+                    specular_exponent=specular_exponent,
                 )
             elif collagen and self.NAME_COLLAGEN in model_name:
                 palette = list()
                 emissions = list()
                 for _ in range(nb_materials):
                     palette.append([1, 1, 1])
                     emissions.append(0.2)
                 self.set_materials(
-                    model_ids=[model_id], material_ids=material_ids,
-                    diffuse_colors=palette, specular_colors=palette,
-                    emissions=emissions
+                    model_ids=[model_id],
+                    material_ids=material_ids,
+                    diffuse_colors=palette,
+                    specular_colors=palette,
+                    emissions=emissions,
                 )
 
     def set_material_colors_from_id(self, model_id):
         """
         Set material color according to material id.
-        
+
         The id of the model represents a 16bit RGB value for which the corresponding color is set
 
         :model_id: Id of the model
         """
         if self._client is None:
             return
 
-        material_ids = self.get_material_ids(model_id)['ids']
+        material_ids = self.get_material_ids(model_id)["ids"]
         palette = list()
         for material_id in material_ids:
             r = (material_id >> 16) & 255
             g = (material_id >> 8) & 255
             b = material_id & 255
             palette.append([r / 255.0, g / 255.0, b / 255.0])
         return self.set_materials(
-            [model_id], material_ids,
-            diffuse_colors=palette,
-            specular_colors=palette)
+            [model_id], material_ids, diffuse_colors=palette, specular_colors=palette
+        )
 
     def go_magnetic(
-            self, colormap_filename=None, colormap_range=[0, 0.008], voxel_size=0.01,
-            density=1.0, samples_per_pixel=64):
+        self,
+        colormap_filename=None,
+        colormap_range=[0, 0.008],
+        voxel_size=0.01,
+        density=1.0,
+        samples_per_pixel=64,
+    ):
         """
         Build fields from current scene and switch to default rendering settings
 
         :colormap_filename: Colormap full file name
         :colormap_range: Colormap value range
         :voxel_size: Voxel size
         :voxel_size: Density of atoms to consider (between 0 and 1)
         :samples_per_pixel: Samples per pixel
         """
         if self._client is None:
             return
 
         # Rendering settings
         self._client.set_renderer(
-            current='bio_explorer_fields',
-            samples_per_pixel=1, subsampling=8,
-            max_accum_frames=samples_per_pixel)
+            current="bio_explorer_fields",
+            samples_per_pixel=1,
+            subsampling=8,
+            max_accum_frames=samples_per_pixel,
+        )
         params = self._client.BioExplorerFieldsRendererParams()
         params.cutoff = 5000
         params.exposure = 2.0
         params.alpha_correction = 0.1
         params.nb_ray_steps = 16
         params.nb_ray_refinement_steps = samples_per_pixel
         params.use_hardware_randomizer = True
         self._client.set_renderer_params(params)
 
         # Build fields acceleration structures
         result = self.build_fields(voxel_size=voxel_size, density=density)
-        fields_model_id = int(result['contents'])
+        fields_model_id = int(result["contents"])
 
         if colormap_filename:
             tf = TransferFunction(
-                bioexplorer=self, model_id=fields_model_id,
-                filename=colormap_filename)
+                bioexplorer=self, model_id=fields_model_id, filename=colormap_filename
+            )
             tf.set_range(colormap_range)
             return tf
         return None
 
     def build_fields(self, voxel_size, density=1.0):
         """
         Build fields acceleration structures and creates according data handler
@@ -2086,16 +2437,27 @@
             return
 
         params = dict()
         params["modelId"] = model_id
         params["filename"] = filename
         return self._invoke_and_check("export-fields-to-file", params)
 
-    def add_grid(self, min_value, max_value, interval, radius=1.0, opacity=0.5, show_axis=True,
-                 show_planes=True, show_full_grid=False, colored=True, position=Vector3()):
+    def add_grid(
+        self,
+        min_value,
+        max_value,
+        interval,
+        radius=1.0,
+        opacity=0.5,
+        show_axis=True,
+        show_planes=True,
+        show_full_grid=False,
+        colored=True,
+        position=Vector3(),
+    ):
         """
         Add a reference grid to the scene
 
         :min_value: Minimum value for all axis
         :max_value: Maximum value for all axis
         :interval: Interval at which lines should appear on the grid
         :radius: Radius of grid lines
@@ -2120,16 +2482,22 @@
         params["showAxis"] = show_axis
         params["showPlanes"] = show_planes
         params["showFullGrid"] = show_full_grid
         params["useColors"] = colored
         params["position"] = position.to_list()
         return self._invoke_and_check("add-grid", params)
 
-    def add_bounding_box(self, name, bottom_left_corner, top_right_corner, radius=1.0,
-                         color=Vector3(1.0, 1.0, 1.0)):
+    def add_bounding_box(
+        self,
+        name,
+        bottom_left_corner,
+        top_right_corner,
+        radius=1.0,
+        color=Vector3(1.0, 1.0, 1.0),
+    ):
         """
         Add a bounding box to the scene
 
         :bottom_left_corner: Bottom left corner
         :top_right_corner: Top right corner
         :radius: Radius of box lines
         :color: Color of the bounding box
@@ -2146,15 +2514,41 @@
         params["name"] = name
         params["bottomLeft"] = bottom_left_corner.to_list()
         params["topRight"] = top_right_corner.to_list()
         params["radius"] = radius
         params["color"] = color.to_list()
         return self._invoke_and_check("add-bounding-box", params)
 
-    def add_sphere(self, name, position, radius, color=Vector3(1.0, 1.0, 1.0), opacity=1.0):
+    def add_box(
+        self, name, bottom_left_corner, top_right_corner, color=Vector3(1.0, 1.0, 1.0)
+    ):
+        """
+        Add a box to the scene
+
+        :bottom_left_corner: Bottom left corner
+        :top_right_corner: Top right corner
+        :color: Color of the bounding box
+        :return: Result of the request submission
+        """
+        if self._client is None:
+            return
+
+        assert isinstance(bottom_left_corner, Vector3)
+        assert isinstance(top_right_corner, Vector3)
+        assert isinstance(color, Vector3)
+        params = dict()
+        params["name"] = name
+        params["bottomLeft"] = bottom_left_corner.to_list()
+        params["topRight"] = top_right_corner.to_list()
+        params["color"] = color.to_list()
+        return self._invoke_and_check("add-box", params)
+
+    def add_sphere(
+        self, name, position, radius, color=Vector3(1.0, 1.0, 1.0), opacity=1.0
+    ):
         """
         Add a reference grid to the scene
 
         :name: Name of the sphere
         :position: Position of the sphere
         :radius: Radius of the sphere
         :color: RGB Color of the sphere (0..1)
@@ -2171,16 +2565,23 @@
         params["position"] = position.to_list()
         params["radius"] = radius
         params["color"] = color.to_list()
         params["opacity"] = opacity
         return self._invoke_and_check("add-sphere", params)
 
     def add_cone(
-            self, name, origin, target, origin_radius, target_radius,
-            color=Vector3(1.0, 1.0, 1.0), opacity=1.0):
+        self,
+        name,
+        origin,
+        target,
+        origin_radius,
+        target_radius,
+        color=Vector3(1.0, 1.0, 1.0),
+        opacity=1.0,
+    ):
         """
         Add a cone to the scene
 
         :name: Name of the cone
         :origin: Origin of the cone
         :target: Target of the cone
         :origin_radius: Origin radius of the cone
@@ -2236,29 +2637,38 @@
         params = dict()
         params["name"] = name
         params["indices"] = indices
         params["vertices"] = vertices
         params["colors"] = colors
         return self._invoke_and_check("add-streamlines", params)
 
-    def set_general_settings(self, model_visibility_on_creation=True, mesh_folder='/tmp',
-                             logging_level=0, v1_compatibility=False):
+    def set_general_settings(
+        self,
+        model_visibility_on_creation=True,
+        mesh_folder="/tmp",
+        logging_level=1,
+        database_logging_level=1,
+        v1_compatibility=False,
+    ):
         """
         Set general settings for the plugin
 
         :model_visibility_on_creation: Visibility of the model on creation
         :off_folder: Folder where off files are stored (to avoid recomputation of molecular surface)
         :logging_level: Back-end logging level (0=no information logs, 3=full logging)
+        :database_logging_level: Back-end logging level for database (0=no information logs, 3=full
+        logging)
         :return: Result of the request submission
         """
         self._v1_compatibility = v1_compatibility
         params = dict()
         params["modelVisibilityOnCreation"] = model_visibility_on_creation
         params["meshFolder"] = mesh_folder
         params["loggingLevel"] = logging_level
+        params["databaseLoggingLevel"] = database_logging_level
         params["v1Compatibility"] = v1_compatibility
         response = self._invoke_and_check("set-general-settings", params)
         return response
 
     def set_models_visibility(self, visible):
         """
         Set the visibility of all models in the scene
@@ -2275,15 +2685,15 @@
         Returns the out-of-core configuration
 
         :rtype: string
         """
         result = self._invoke_and_check("get-out-of-core-configuration")
         d = dict()
         for param in result["contents"].split("|"):
-            s = param.split('=')
+            s = param.split("=")
             d[s[0]] = s[1]
         return d
 
     def get_out_of_core_progress(self):
         """
         Returns the out-of-core loading progress
 
@@ -2296,18 +2706,26 @@
         Returns the out-of-core average loading time (per brick, in milliseconds)
 
         :rtype: float
         """
         return self._invoke_and_check("get-out-of-core-average-loading-time")
 
     def add_atlas(
-            self, assembly_name,
-            load_cells=True, cell_radius=1.0, load_meshes=False,
-            region_sql_filter='', cell_sql_filter='', scale=Vector3(1.0, 1.0, 1.0),
-            mesh_position=Vector3(), mesh_rotation=Quaternion(), mesh_scale=Vector3()):
+        self,
+        assembly_name,
+        load_cells=True,
+        cell_radius=1.0,
+        load_meshes=False,
+        region_sql_filter="",
+        cell_sql_filter="",
+        scale=Vector3(1.0, 1.0, 1.0),
+        mesh_position=Vector3(),
+        mesh_rotation=Quaternion(),
+        mesh_scale=Vector3(),
+    ):
         """
         Add a brain atlas the 3D scene
 
         :assembly_name: Name of the assembly to which the astrocytes should be added
         :load_cells: Load cells if set to true
         :cell_radius: Cell radius
         :load_meshes: Load meshes if set to true
@@ -2329,87 +2747,104 @@
         params["loadMeshes"] = load_meshes
         params["cellSqlFilter"] = cell_sql_filter
         params["regionSqlFilter"] = region_sql_filter
         params["scale"] = scale.to_list()
         params["meshPosition"] = mesh_position.to_list()
         params["meshRotation"] = list(mesh_rotation)
         params["meshScale"] = mesh_scale.to_list()
-        return self._invoke_and_check('add-atlas', params)
+        return self._invoke_and_check("add-atlas", params)
 
     def add_vasculature(
-            self, assembly_name, population_name, color_scheme=VASCULATURE_COLOR_SCHEME_NONE,
-            use_sdf=False, section_gids=list(),
-            load_capilarities=False, representation=VASCULATURE_REPRESENTATION_SEGMENT,
-            radius_multiplier=1.0, sql_filter='', scale=Vector3(1.0, 1.0, 1.0)):
+        self,
+        assembly_name,
+        population_name,
+        color_scheme=VASCULATURE_COLOR_SCHEME_NONE,
+        realism_level=VASCULATURE_REALISM_LEVEL_NONE,
+        section_gids=list(),
+        load_capilarities=False,
+        representation=VASCULATURE_REPRESENTATION_SEGMENT,
+        radius_multiplier=1.0,
+        sql_filter="",
+        scale=Vector3(1.0, 1.0, 1.0),
+        animation_params=CellAnimationParams(),
+    ):
         """
         Add a vasculature to the 3D scene
 
         :assembly_name: Name of the assembly to which the vasculature should be added
         :population_name Name of the node population
         :color_scheme: Color scheme applied to the vasculature (node, graph, section, etc)
-        :use_sdf: Use sign distance fields geometry to create the vasculature. Defaults to False
+        :realism_level: Use sign distance fields geometry to create the vasculature. Defaults to
+        none
         :node_gids: List of segment GIDs to load. Defaults to list()
         :representation: Representation of the vasculature geometry (Graph, sections or segments)
-        :radius_muliplier: Applies the multiplier to all radii of the vasculature sections
+        :radius_multiplier: Applies the multiplier to all radii of the vasculature sections
         :sql_filter: Condition added to the SQL statement loading the vasculature
         :scale: Scale in the 3D scene
+        :animation_params: Extra optional parameters for animation purposes
 
         :return: Result of the request submission
         """
         assert isinstance(section_gids, list)
         assert isinstance(scale, Vector3)
+        assert isinstance(animation_params, CellAnimationParams)
 
         params = dict()
         params["assemblyName"] = assembly_name
         params["populationName"] = population_name
         params["colorScheme"] = color_scheme
-        params["useSdf"] = use_sdf
+        params["realismLevel"] = realism_level
         params["gids"] = section_gids
         params["loadCapilarities"] = load_capilarities
         params["representation"] = representation
         params["radiusMultiplier"] = radius_multiplier
         params["sqlFilter"] = sql_filter
         params["scale"] = scale.to_list()
-        return self._invoke_and_check('add-vasculature', params)
+        params["animationParams"] = animation_params.to_list()
+        return self._invoke_and_check("add-vasculature", params)
 
     def get_vasculature_info(self, assembly_name):
         """
         Return information about the vasculature
 
         :return: A dictionary of attributes (Model Id, Number of edges, pairs, sections and
                  sub-graphs)
         """
         params = dict()
         params["name"] = assembly_name
-        response = self._invoke_and_check('get-vasculature-info', params)
+        response = self._invoke_and_check("get-vasculature-info", params)
         vasculature_info = dict()
         for param in response["contents"].split(self.CONTENTS_DELIMITER):
-            s = param.split('=')
+            s = param.split("=")
             vasculature_info[s[0]] = int(s[1])
         return vasculature_info
 
-    def set_vasculature_report(self, assembly_name, population_name, report_simulation_id):
+    def set_vasculature_report(
+        self, assembly_name, population_name, report_simulation_id, show_evolution=False
+    ):
         """
         Attach a simulation report to the vasculature
 
         :assembly_name: Name of the assembly containing the vasculature
         :population_name: Name of the node population in the report. Defaults to 'vasculature'
         :report_simulation_id: Report simulation identifier
+        :show_evolution: Show value evolution (percentage) between 2 time steps. Raw value otherwise
 
         :return: Result of the request submission
         """
         params = dict()
         params["assemblyName"] = assembly_name
         params["populationName"] = population_name
         params["simulationReportId"] = report_simulation_id
-        return self._invoke_and_check('set-vasculature-report', params)
+        params["showEvolution"] = show_evolution
+        return self._invoke_and_check("set-vasculature-report", params)
 
     def set_vasculature_radius_report(
-            self, assembly_name, population_name, report_simulation_id,
-            frame, amplitude=1.0):
+        self, assembly_name, population_name, report_simulation_id, frame, amplitude=1.0
+    ):
         """
         Attach a radius report to the vasculature
 
         :assembly_name: Name of the assembly containing the vasculature
         :population_name: Name of the node population in the report. Defaults to 'vasculature'
         :report_simulation_id: Report simulation identifier
         :frame: Index of the frame in the simulation report
@@ -2417,135 +2852,153 @@
 
         :return: Result of the request submission
         """
         params = dict()
         params["assemblyName"] = assembly_name
         params["populationName"] = population_name
         params["simulationReportId"] = report_simulation_id
-        params['frame'] = frame
-        params['amplitude'] = amplitude
-        return self._invoke_and_check('set-vasculature-radius-report', params)
+        params["frame"] = frame
+        params["amplitude"] = amplitude
+        return self._invoke_and_check("set-vasculature-radius-report", params)
 
     def add_astrocytes(
-            self, assembly_name, population_name, vasculature_population_name='',
-            use_sdf=False, load_somas=True,
-            load_dendrites=True, load_end_feet=True, generate_internals=False,
-            morphology_representation=MORPHOLOGY_REPRESENTATION_SEGMENT,
-            morphology_color_scheme=MORPHOLOGY_COLOR_SCHEME_NONE,
-            population_color_scheme=POPULATION_COLOR_SCHEME_NONE,
-            radius_multiplier=1.0, sql_filter='', scale=Vector3(1.0, 1.0, 1.0),
-            animation_params=AnimationParams()):
+        self,
+        assembly_name,
+        population_name,
+        vasculature_population_name="",
+        realism_level=MORPHOLOGY_REALISM_LEVEL_NONE,
+        load_somas=True,
+        load_dendrites=True,
+        generate_internals=False,
+        morphology_representation=MORPHOLOGY_REPRESENTATION_SEGMENT,
+        morphology_color_scheme=MORPHOLOGY_COLOR_SCHEME_NONE,
+        population_color_scheme=POPULATION_COLOR_SCHEME_NONE,
+        radius_multiplier=1.0,
+        sql_filter="",
+        scale=Vector3(1.0, 1.0, 1.0),
+        animation_params=CellAnimationParams(),
+    ):
         """
         Add a population of astrocytes to the 3D scene
 
         :assembly_name: Name of the assembly to which the astrocytes should be added
         :population_name: Name of the population of astrocytes
         :vasculature_population_name: Name of the vasculature population. Automatically load
                                       end-feet if not empty
         :load_somas: Load somas if set to true
         :load_dendrites: Load dendrites if set to true
         :generate_internals: Generate internals (Nucleus and mitochondria)
-        :use_sdf: Use sign distance fields geometry to create the astrocytes. Defaults to False
+        :realism_level: Use sign distance fields geometry to create the astrocytes. Defaults to none
         :morphology_representation: Geometry representation (graph, section or segment)
         :morphology_color_scheme: Color scheme of the sections of the astrocytes
         :populationColorScheme: Color scheme of the population of astrocytes
-        :radius_muliplier: Applies the multiplier to all radii of the astrocyte sections
+        :radius_multiplier: Applies the multiplier to all radii of the astrocyte sections
         :sql_filter: Condition added to the SQL statement loading the astrocytes
         :scale: Scale in the 3D scene
         :animation_params: Extra optional parameters for animation purposes
 
         :return: Result of the request submission
         """
         assert isinstance(scale, Vector3)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, CellAnimationParams)
 
         params = dict()
         params["assemblyName"] = assembly_name
         params["populationName"] = population_name
         params["vasculaturePopulationName"] = vasculature_population_name
         params["loadSomas"] = load_somas
         params["loadDendrites"] = load_dendrites
         params["generateInternals"] = generate_internals
-        params["useSdf"] = use_sdf
+        params["realismLevel"] = realism_level
         params["morphologyRepresentation"] = morphology_representation
         params["morphologyColorScheme"] = morphology_color_scheme
         params["populationColorScheme"] = population_color_scheme
         params["radiusMultiplier"] = radius_multiplier
         params["sqlFilter"] = sql_filter
         params["scale"] = scale.to_list()
         params["animationParams"] = animation_params.to_list()
-        return self._invoke_and_check('add-astrocytes', params)
+        return self._invoke_and_check("add-astrocytes", params)
 
     def add_neurons(
-            self, assembly_name, population_name,
-            use_sdf=False,
-            load_somas=True, load_axon=True,
-            load_basal_dendrites=True, load_apical_dendrites=True,
-            load_synapses=False,
-            generate_internals=False, generate_externals=False,
-            generate_varicosities=False, show_membrane=True,
-            morphology_representation=MORPHOLOGY_REPRESENTATION_SEGMENT,
-            morphology_color_scheme=MORPHOLOGY_COLOR_SCHEME_NONE,
-            population_color_scheme=POPULATION_COLOR_SCHEME_NONE,
-            radius_multiplier=1.0, simulation_report_id=-1,
-            sql_node_filter='', sql_section_filter='',
-            scale=Vector3(1.0, 1.0, 1.0), animation_params=AnimationParams()):
+        self,
+        assembly_name,
+        population_name,
+        realism_level=MORPHOLOGY_REALISM_LEVEL_NONE,
+        load_somas=True,
+        load_axon=True,
+        load_basal_dendrites=True,
+        load_apical_dendrites=True,
+        load_synapses=False,
+        generate_internals=False,
+        generate_externals=False,
+        generate_varicosities=False,
+        show_membrane=True,
+        morphology_representation=MORPHOLOGY_REPRESENTATION_SEGMENT,
+        morphology_color_scheme=MORPHOLOGY_COLOR_SCHEME_NONE,
+        population_color_scheme=POPULATION_COLOR_SCHEME_NONE,
+        radius_multiplier=1.0,
+        simulation_report_id=-1,
+        sql_node_filter="",
+        sql_section_filter="",
+        scale=Vector3(1.0, 1.0, 1.0),
+        animation_params=CellAnimationParams(),
+    ):
         """
         Add a population of astrocytes to the 3D scene
 
         :assembly_name: Name of the assembly to which the astrocytes should be added
         :population_name: Name of the population of astrocytes
-        :use_sdf: Use sign distance fields geometry to create the astrocytes. Defaults to False
+        :realism_level: Use sign distance fields geometry to create the astrocytes. Defaults to none
         :load_somas: Load somas if set to true
         :load_axon: Load axon if set to true
         :load_basal_dendrites: Load basal dendrites if set to true
         :load_apical_dendrites: Load apical dendrites if set to true
         :load_synapses: Load synapses if set to true
         :generate_internals: Generate internals (Nucleus and mitochondria)
-        :generate_externals: Generate externals (Myelin steath)
+        :generate_externals: Generate externals (Myelin sheath)
         :show_membrane: Show membrane (Typically used to isolate internal and external components
         :generate_varicosities: Generate random varicosities along the axon
         :morphology_representation: Geometry representation (graph, section or segment)
         :morphology_color_scheme: Color scheme of the sections of the astrocytes
         :populationColorScheme: Color scheme of the population of astrocytes
-        :radius_muliplier: Applies the multiplier to all radii of the astrocyte sections
+        :radius_multiplier: Applies the multiplier to all radii of the astrocyte sections
         :simulation_report_id: Identifier of the simulation report (Optional)
         :sql_node_filter: Condition added to the SQL statement loading the nodes
         :sql_section_filter: Condition added to the SQL statement loading the sections
         :scale: Scale in the 3D scene
         :animation_params: Extra optional parameters for animation purposes
 
         :return: Result of the request submission
         """
         assert isinstance(scale, Vector3)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, CellAnimationParams)
 
         params = dict()
         params["assemblyName"] = assembly_name
         params["populationName"] = population_name
         params["loadSomas"] = load_somas
         params["loadAxon"] = load_axon
         params["loadBasalDendrites"] = load_basal_dendrites
         params["loadApicalDendrites"] = load_apical_dendrites
         params["loadSynapses"] = load_synapses
         params["generateInternals"] = generate_internals
         params["generateExternals"] = generate_externals
         params["showMembrane"] = show_membrane
         params["generateVaricosities"] = generate_varicosities
-        params["useSdf"] = use_sdf
+        params["realismLevel"] = realism_level
         params["morphologyRepresentation"] = morphology_representation
         params["morphologyColorScheme"] = morphology_color_scheme
         params["populationColorScheme"] = population_color_scheme
         params["radiusMultiplier"] = radius_multiplier
         params["simulationReportId"] = simulation_report_id
         params["sqlNodeFilter"] = sql_node_filter
         params["sqlSectionFilter"] = sql_section_filter
         params["scale"] = scale.to_list()
         params["animationParams"] = animation_params.to_list()
-        return self._invoke_and_check('add-neurons', params)
+        return self._invoke_and_check("add-neurons", params)
 
     def get_neuron_section_points(self, assembly_name, neuron_guid, section_guid):
         """
         Return the list of 3D points for a given section of a given neuron
 
         :assembly_name: Name of the assembly
         :neuron_guid: Neuron identifier
@@ -2553,23 +3006,23 @@
 
         :return: A list of 3D points
         """
         params = dict()
         params["assemblyName"] = assembly_name
         params["neuronId"] = neuron_guid
         params["sectionId"] = section_guid
-        response = self._invoke('get-neuron-section-points', params)
-        if not response['status']:
+        response = self._invoke("get-neuron-section-points", params)
+        if not response["status"]:
             raise "Failed to get neuron section points"
-        points = response['points']
+        points = response["points"]
         ps = list()
         for i in range(0, len(points), 4):
             p = list()
             for j in range(4):
-                p.append(points[i+j])
+                p.append(points[i + j])
             ps.append(p)
         return ps
 
     def get_neuron_varicosities(self, assembly_name, neuron_guid):
         """
         Return the list of 3D locations for the varicosities of a given neuron
 
@@ -2577,29 +3030,34 @@
         :neuron_guid: Neuron identifier
 
         :return: A list of 3D points
         """
         params = dict()
         params["assemblyName"] = assembly_name
         params["neuronId"] = neuron_guid
-        response = self._invoke('get-neuron-varicosities', params)
-        if not response['status']:
+        response = self._invoke("get-neuron-varicosities", params)
+        if not response["status"]:
             raise "Failed to get neuron varicosities"
-        points = response['points']
+        points = response["points"]
         ps = list()
         for i in range(0, len(points), 3):
             p = list()
             for j in range(3):
-                p.append(points[i+j])
+                p.append(points[i + j])
             ps.append(p)
         return ps
 
     def add_white_matter(
-            self, assembly_name, population_name, radius=1.0,
-            sql_filter='', scale=Vector3(1.0, 1.0, 1.0)):
+        self,
+        assembly_name,
+        population_name,
+        radius=1.0,
+        sql_filter="",
+        scale=Vector3(1.0, 1.0, 1.0)
+    ):
         """
         Add white matter to the 3D scene
 
         :assembly_name: Name of the assembly to which the vasculature should be added
         :population_name Name of the node population
         :radius: Applies the radius to the white matter streamlines
         :sql_filter: Condition added to the SQL statement loading the white matter streamlines
@@ -2611,51 +3069,92 @@
 
         params = dict()
         params["assemblyName"] = assembly_name
         params["populationName"] = population_name
         params["radius"] = radius
         params["sqlFilter"] = sql_filter
         params["scale"] = scale.to_list()
-        return self._invoke_and_check('add-white-matter', params)
+        return self._invoke_and_check("add-white-matter", params)
+
+    def add_synapse_efficacy_report(
+        self,
+        assembly_name,
+        population_name,
+        simulation_report_id,
+        radius=1.0,
+        sql_filter=""
+    ):
+        """
+        Add synapse efficacy report to the 3D scene
+
+        :assembly_name: Name of the assembly to which the vasculature should be added
+        :population_name Name of the node population
+        :simulation_report_id: Identifier of the simulation report
+        :radius: Applies the radius to the white matter streamlines
+        :sql_filter: Condition added to the SQL statement loading the synapses
+
+        :return: Result of the request submission
+        """
+        params = dict()
+        params["assemblyName"] = assembly_name
+        params["populationName"] = population_name
+        params["radius"] = radius
+        params["sqlFilter"] = sql_filter
+        params["simulationReportId"] = simulation_report_id
+        return self._invoke_and_check("add-synapse-efficacy", params)
 
     def look_at(self, source, target):
         """
         Computes quaternion from given direction
-        
+
         Generate a quaternion to make a object rotate in the direction of a vector
         defined by two 3D points, a source and a target
 
         :source: Source 3d point
         :target: Target 3d point
 
         :return: The resulting rotation
         """
         assert isinstance(source, Vector3)
         assert isinstance(target, Vector3)
 
         params = dict()
         params["source"] = source.to_list()
         params["target"] = target.to_list()
-        response = self._invoke('look-at', params)
-        q = response['rotation']
+        response = self._invoke("look-at", params)
+        q = response["rotation"]
         return Quaternion(q[3], q[0], q[1], q[2])
 
+
 # Private classes
 
 
 class AssemblyProtein:
     """An AssemblyProtein is a Protein that belongs to an assembly"""
 
-    def __init__(self, assembly_name, name, source,
-                 atom_radius_multiplier=1.0,
-                 load_bonds=True, representation=BioExplorer.REPRESENTATION_ATOMS,
-                 load_non_polymer_chemicals=False, load_hydrogen=True, chain_ids=list(),
-                 recenter=True, occurrences=1, transmembrane_params=Vector2(),
-                 position=Vector3(), rotation=Quaternion(), allowed_occurrences=list(),
-                 animation_params=AnimationParams(), constraints=list()):
+    def __init__(
+        self,
+        assembly_name,
+        name,
+        source,
+        atom_radius_multiplier=1.0,
+        load_bonds=True,
+        representation=BioExplorer.REPRESENTATION_ATOMS,
+        load_non_polymer_chemicals=False,
+        load_hydrogen=True,
+        chain_ids=list(),
+        recenter=True,
+        occurrences=1,
+        transmembrane_params=Vector2(),
+        position=Vector3(),
+        rotation=Quaternion(),
+        allowed_occurrences=list(),
+        animation_params=MolecularSystemAnimationParams(),
+        constraints=list(),
+    ):
         """
         An AssemblyProtein is a protein that belongs to an assembly
 
         :assembly_name: Name of the assembly
         :name: Name of the protein
         :contents: PDB representation of the protein
         :atom_radius_multiplier: Multiplier applied to atom radius
@@ -2671,15 +3170,15 @@
         :rotation: Relative rotation of the protein in the assembly
         :allowed_occurrences: Indices of protein occurrences in the assembly for
                                     which proteins are added
         :constraints: List of assemblies that constraint the placememnt of the proteins
         """
         assert isinstance(position, Vector3)
         assert isinstance(rotation, Quaternion)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
         self.assembly_name = assembly_name
         self.name = name
         self.pdb_id = os.path.splitext(os.path.basename(source))[0].lower()
         self.source = source
         self.atom_radius_multiplier = atom_radius_multiplier
         self.load_bonds = load_bonds
@@ -2699,19 +3198,27 @@
 
 # Public classes
 
 
 class Membrane:
     """A membrane is a shaped assembly of phospholipids"""
 
-    def __init__(self, lipid_sources, lipid_rotation=Quaternion(), lipid_density=1.0,
-                 atom_radius_multiplier=1.0, load_bonds=False,
-                 representation=BioExplorer.REPRESENTATION_ATOMS_AND_STICKS,
-                 load_non_polymer_chemicals=False, chain_ids=list(), recenter=True,
-                 animation_params=AnimationParams()):
+    def __init__(
+        self,
+        lipid_sources,
+        lipid_rotation=Quaternion(),
+        lipid_density=1.0,
+        atom_radius_multiplier=1.0,
+        load_bonds=False,
+        representation=BioExplorer.REPRESENTATION_ATOMS_AND_STICKS,
+        load_non_polymer_chemicals=False,
+        chain_ids=list(),
+        recenter=True,
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         A membrane is an assembly of proteins with a given size and shape
 
         :size: Size of the cell in the scene (in nanometers)
         :shape: Shape of the membrane (Spherical, planar, sinusoidal, cubic, etc)
         :lipid_sources: Full paths of the PDB files containing the building blocks of the membrane
         :atom_radius_multiplier: Multiplies atom radius by the specified value
@@ -2720,15 +3227,15 @@
         :load_non_polymer_chemicals: Defines if non-polymer chemical should be loaded
         :chain_ids: IDs of the protein chains to be loaded
         :recenter: Defines if proteins should be centered when loaded from PDB files
         :position: Relative position of the membrane in the assembly
         :rotation: Relative rotation of the membrane in the assembly
         """
         assert isinstance(lipid_rotation, Quaternion)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
         assert lipid_density > 0.0
         assert lipid_density <= 10.0
 
         self.lipid_sources = lipid_sources
         self.lipid_rotation = lipid_rotation
         self.lipid_density = lipid_density
         self.atom_radius_multiplier = atom_radius_multiplier
@@ -2739,18 +3246,29 @@
         self.recenter = recenter
         self.animation_params = animation_params.copy()
 
 
 class Sugar:
     """Sugars are glycan trees that can be added to the glycosylation sites of a given protein"""
 
-    def __init__(self, assembly_name, name, source, protein_name, atom_radius_multiplier=1.0,
-                 load_bonds=True, representation=BioExplorer.REPRESENTATION_ATOMS,
-                 recenter=True, chain_ids=list(), site_indices=list(), rotation=Quaternion(),
-                 animation_params=AnimationParams()):
+    def __init__(
+        self,
+        assembly_name,
+        name,
+        source,
+        protein_name,
+        atom_radius_multiplier=1.0,
+        load_bonds=True,
+        representation=BioExplorer.REPRESENTATION_ATOMS,
+        recenter=True,
+        chain_ids=list(),
+        site_indices=list(),
+        rotation=Quaternion(),
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         Sugar descriptor
 
         :assembly_name: Name of the assembly in the scene
         :name: Name of sugar in the scene
         :source: Full path to the PDB file
         :protein_name: Name of the protein to which sugars are added
@@ -2762,15 +3280,15 @@
         :site_indices: Indices on which sugars should be added on the protein
         :rotation: Rotation of the sugar on the protein
         :shape_params: Extra optional parameters for positioning on the protein
         """
         assert isinstance(chain_ids, list)
         assert isinstance(site_indices, list)
         assert isinstance(rotation, Quaternion)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
         self.assembly_name = assembly_name
         self.name = name
         self.pdb_id = os.path.splitext(os.path.basename(source))[0].lower()
         self.contents = "".join(open(source).readlines())
         self.protein_name = protein_name
         self.atom_radius_multiplier = atom_radius_multiplier
@@ -2782,18 +3300,28 @@
         self.rotation = rotation
         self.animation_params = animation_params.copy()
 
 
 class RNASequence:
     """An RNASequence is an assembly of a given shape holding a given genetic code"""
 
-    def __init__(self, source, shape, shape_params, protein_source='', values_range=Vector2(),
-                 curve_params=Vector3(), position=Vector3(), rotation=Quaternion(),
-                 atom_radius_multiplier=1.0, representation=BioExplorer.REPRESENTATION_ATOMS,
-                 animation_params=AnimationParams()):
+    def __init__(
+        self,
+        source,
+        shape,
+        shape_params,
+        protein_source="",
+        values_range=Vector2(),
+        curve_params=Vector3(),
+        position=Vector3(),
+        rotation=Quaternion(),
+        atom_radius_multiplier=1.0,
+        representation=BioExplorer.REPRESENTATION_ATOMS,
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         RNA sequence descriptor
 
         :source: Full path of the file containing the RNA sequence
         :lipid_sources: Full path of the file containing the PDB representation of the N protein
         :shape: Shape of the sequence (Trefoil knot, torus, star, spring, heart, Moebiusknot, etc)
         :shape_params: Assembly parameters (radius, etc.)
@@ -2803,15 +3331,15 @@
         :rotation: Relative position of the RNA sequence in the assembly
         """
         assert isinstance(values_range, Vector2)
         assert isinstance(shape_params, Vector2)
         assert isinstance(curve_params, Vector3)
         assert isinstance(position, Vector3)
         assert isinstance(rotation, Quaternion)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
         self.source = source
         self.protein_source = protein_source
         self.shape = shape
         self.shape_params = shape_params.copy()
         self.values_range = values_range.copy()
         self.curve_params = curve_params.copy()
@@ -2839,15 +3367,17 @@
         self.head_source = head_source
         self.branch_source = branch_source
 
 
 class Cell:
     """A Cell is a membrane with transmembrane proteins"""
 
-    def __init__(self, name, shape, shape_params, membrane, proteins=list(), shape_mesh_source=''):
+    def __init__(
+        self, name, shape, shape_params, membrane, proteins=list(), shape_mesh_source=""
+    ):
         """
         Cell descriptor
 
         :name: Name of the cell in the scene
         :membrane: Membrane descriptor
         :proteins: List of trans-membrane proteins
         """
@@ -2881,18 +3411,29 @@
         self.shape_params = shape_params.copy()
         self.protein = protein
 
 
 class Protein:
     """A Protein holds the 3D structure of a protein as well as it Amino Acid sequences"""
 
-    def __init__(self, name, source, occurrences=1, load_bonds=False,
-                 load_hydrogen=False, load_non_polymer_chemicals=False, position=Vector3(),
-                 rotation=Quaternion(), allowed_occurrences=list(), chain_ids=list(),
-                 transmembrane_params=Vector2(), animation_params=AnimationParams()):
+    def __init__(
+        self,
+        name,
+        source,
+        occurrences=1,
+        load_bonds=False,
+        load_hydrogen=False,
+        load_non_polymer_chemicals=False,
+        position=Vector3(),
+        rotation=Quaternion(),
+        allowed_occurrences=list(),
+        chain_ids=list(),
+        transmembrane_params=Vector2(),
+        animation_params=MolecularSystemAnimationParams(),
+    ):
         """
         Protein descriptor
 
         :source: Full path to the protein PDB file
         :occurrences: Number of occurrences to be added to the assembly
         :load_bonds: Loads bonds if True
         :load_hydrogen: Loads hydrogens if True
@@ -2902,15 +3443,15 @@
         :allowed_occurrences: Specific occurrences for which an instance is added to the assembly
         """
         assert isinstance(occurrences, int)
         assert isinstance(position, Vector3)
         assert isinstance(rotation, Quaternion)
         assert isinstance(transmembrane_params, Vector2)
         assert isinstance(allowed_occurrences, list)
-        assert isinstance(animation_params, AnimationParams)
+        assert isinstance(animation_params, MolecularSystemAnimationParams)
 
         self.name = name
         self.pdb_id = os.path.splitext(os.path.basename(source))[0].lower()
         self.source = source
         self.occurrences = occurrences
         self.load_bonds = load_bonds
         self.load_hydrogen = load_hydrogen
@@ -2922,16 +3463,24 @@
         self.transmembrane_params = transmembrane_params.copy()
         self.animation_params = animation_params.copy()
 
 
 class Virus:
     """A Virus is an assembly of proteins (S, M and E), a membrane, and an RNA sequence"""
 
-    def __init__(self, name, shape_params, protein_s=None, protein_e=None, protein_m=None,
-                 membrane=None, rna_sequence=None):
+    def __init__(
+        self,
+        name,
+        shape_params,
+        protein_s=None,
+        protein_e=None,
+        protein_m=None,
+        membrane=None,
+        rna_sequence=None,
+    ):
         """
         Virus descriptor
 
         :name: Name of the virus in the scene
         :shape_params: Assembly parameters (Virus radius and maximum range for random
                                 positions of membrane components)
         :protein_s: Protein S descriptor
```

### Comparing `bioexplorer-1.4.0/bioexplorer/metabolism.py` & `bioexplorer-1.5.0/bioexplorer/metabolism.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """BioExplorer class"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue Brain Project / EPFL
+# Copyright 2020-2023 Blue Brain Project / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -38,54 +38,79 @@
 class Metabolism:
     """
     The Metabolism class defines an API to access and render metabolism information.
 
     Metabolism data is stored in a PostgreSQL database.
     """
 
-    PLUGIN_API_PREFIX = 'mb-'
+    PLUGIN_API_PREFIX = "mb-"
 
     def __init__(
-            self, bioexplorer, model_id, db_host, db_name, db_user, db_password,
-            db_schema, simulation_timestamp, relative_concentration=False):
+        self,
+        bioexplorer,
+        model_id,
+        db_host,
+        db_name,
+        db_user,
+        db_password,
+        db_schema,
+        simulation_timestamp,
+        reference_frame,
+        relative_concentration=False,
+    ):
         """
         Metabolism class initialization
 
         :bioexplorer: Reference to a instance of the BioExplorer
         :model_id: Id of the model
         :db_host: Host name of the PostgreSQL server
         :db_host: Database name
         :db_host: Database user name
         :db_host: Database password
         :db_schema: Database scheme
         :simulation_timestamp: Simulation timestamp
+        :reference_frame: Reference frame to compute the metabolite baseline (frame when the stimuli
+        is injected)
         :relative_concentration: Get concentration as relative to initial simulation value (frame 0)
         """
         self._be = bioexplorer
         self._core = self._be.core_api()
         self._db_host = db_host
         self._db_name = db_name
         self._db_user = db_user
         self._db_password = db_password
         self._db_schema = db_schema
         self._relative_concentration = relative_concentration
+        self._reference_frame = reference_frame
 
-        db_connection_string = 'postgresql+psycopg2://%s:%s@%s:5432/%s' % (
-            db_user, db_password, db_host, db_name)
+        db_connection_string = "postgresql+psycopg2://%s:%s@%s:5432/%s" % (
+            db_user,
+            db_password,
+            db_host,
+            db_name,
+        )
         self._engine = create_engine(db_connection_string)
         self._db_connection = self._engine.connect()
 
         self._simulation_guid = self._get_simulation_guid(simulation_timestamp)
         self._metabolite_ids = dict()
         self._model_id = model_id
 
     def set_renderer(
-            self, max_accum_frames=None, subsampling=None, alpha_correction=0.1,
-            exposure=1.0, near_plane=10.0, far_plane=200.0, ray_step=3.0,
-            noise_frequency=1.0, noise_amplitude=1.0):
+        self,
+        max_accum_frames=None,
+        subsampling=None,
+        alpha_correction=0.1,
+        exposure=1.0,
+        near_plane=10.0,
+        far_plane=200.0,
+        ray_step=3.0,
+        noise_frequency=1.0,
+        noise_amplitude=1.0,
+    ):
         """
         Set the metabolism renderer
 
         The renderer travels through the scene using
         the ray-marching technique. For every voxel, the region is identified and
         the metabolite concentration is used to define the opacity of the voxel.
 
@@ -96,16 +121,18 @@
         :near_plane: Volume near plane
         :far_plane: Volume far plane
         :ray_step: Step for the ray marching process
         :noise_frequency: Noise frequency for the cloud rendering effect
         :noise_amplitude: Noise amplitude for the cloud rendering effect
         """
         self._core.set_renderer(
-            current='metabolism', subsampling=subsampling,
-            max_accum_frames=max_accum_frames)
+            current="metabolism",
+            subsampling=subsampling,
+            max_accum_frames=max_accum_frames,
+        )
         params = self._core.MetabolismRendererParams()
         params.alpha_correction = alpha_correction
         params.exposure = exposure
         params.near_plane = near_plane
         params.far_plane = far_plane
         params.ray_step = ray_step
         params.refinement_steps = max_accum_frames
@@ -122,26 +149,31 @@
         in the 3D scene. 0 is transparent, 1 is opaque.
         :return: Result of the call to the BioExplorer backend
         :rtype: Response
         """
         assert isinstance(opacity_range, list)
         assert len(opacity_range) == 2
 
-        db_connection_string = 'host=%s port=5432 dbname=%s user=%s password=%s' % (
-            self._db_host, self._db_name, self._db_user, self._db_password)
+        db_connection_string = "host=%s port=5432 dbname=%s user=%s password=%s" % (
+            self._db_host,
+            self._db_name,
+            self._db_user,
+            self._db_password,
+        )
 
         params = dict()
-        params['connectionString'] = db_connection_string
-        params['schema'] = self._db_schema
-        params['simulationId'] = self._simulation_guid
-        params['metaboliteIds'] = metabolite_ids
-        params['relativeConcentration'] = self._relative_concentration
-        params['opacityRange'] = opacity_range
+        params["connectionString"] = db_connection_string
+        params["schema"] = self._db_schema
+        params["simulationId"] = self._simulation_guid
+        params["metaboliteIds"] = metabolite_ids
+        params["referenceFrame"] = self._reference_frame
+        params["relativeConcentration"] = self._relative_concentration
         return self._core.rockets_client.request(
-            method=self.PLUGIN_API_PREFIX + 'attach-handler', params=params)
+            method=self.PLUGIN_API_PREFIX + "attach-handler", params=params
+        )
 
     def callback(self, location, metabolite_id):
         """
         Call back function used by the Metabolism widget to update the rendering
 
         :location: Location (Neuron cytosol, Astrocyte mitochondrion, etc)
         :metabolite_id: Metabolite id
@@ -167,14 +199,15 @@
                 """
                 self._core = metabolism._core
                 self._model_id = metabolism._model_id
                 self._db_connection = metabolism._db_connection
                 self._db_schema = metabolism._db_schema
                 self._simulation_guid = metabolism._simulation_guid
                 self._relative_concentration = metabolism._relative_concentration
+                self._reference_frame = metabolism._reference_frame
                 self._location = None
                 self._grid = None
                 self._metabolite_slider = None
                 self._metabolite_selector = None
                 self._callback = metabolism.callback
                 self._metabolites = dict()
                 self._locations = dict()
@@ -188,70 +221,81 @@
             def get_locations(self):
                 """
                 Get locations from database
 
                 :return: List of locations
                 :rtype: list
                 """
-                sql = "SELECT guid, description FROM %s.location "\
-                      "ORDER BY description" % (self._db_schema)
+                sql = (
+                    "SELECT guid, description FROM %s.location "
+                    "ORDER BY description" % (self._db_schema)
+                )
                 data = pd.read_sql(sql, self._db_connection)
                 for i in range(len(data)):
                     if i == 0:
-                        self._location = data['guid'][i]
-                    self._locations[data['description'][i]] = data['guid'][i]
+                        self._location = data["guid"][i]
+                    self._locations[data["description"][i]] = data["guid"][i]
                 return self._locations
 
             def populate_location_colors(self):
                 """Populate location colors from database"""
-                sql = "SELECT guid, red, green, blue FROM %s.location ORDER BY guid" \
+                sql = (
+                    "SELECT guid, red, green, blue FROM %s.location ORDER BY guid"
                     % self._db_schema
+                )
                 data = pd.read_sql(sql, self._db_connection)
                 for i in range(len(data)):
-                    guid = int(data['guid'][i])
+                    guid = int(data["guid"][i])
                     color = self._html_color(
-                        [data['red'][i], data['green'][i], data['blue'][i]])
+                        [data["red"][i], data["green"][i], data["blue"][i]]
+                    )
                     self._location_colors[guid] = color
                     self._location_colors_opacity[guid] = 1.0
 
             def get_metabolites(self):
                 """
                 Get metabolites from database
 
                 :return: List of metabolites
                 :rtype: list
                 """
                 self._metabolites = dict()
-                sql = "SELECT v.guid, v.description "\
-                      "FROM %s.variable AS v, %s.concentration AS c " \
-                      "WHERE v.location_guid=%d AND " \
-                      "v.unit_guid=0 AND v.guid=c.variable_guid AND " \
-                      "c.simulation_guid=%d " \
-                      "ORDER BY description" % (
-                          self._db_schema, self._db_schema,
-                          self._location, self._simulation_guid)
+                sql = (
+                    "SELECT v.guid, v.description "
+                    "FROM %s.variable AS v, %s.concentration AS c "
+                    "WHERE v.location_guid=%d AND "
+                    "v.unit_guid=0 AND v.guid=c.variable_guid AND "
+                    "c.simulation_guid=%d "
+                    "ORDER BY description"
+                    % (
+                        self._db_schema,
+                        self._db_schema,
+                        self._location,
+                        self._simulation_guid,
+                    )
+                )
                 data = pd.read_sql(sql, self._db_connection)
-                self._metabolites['<none>'] = -1
+                self._metabolites["<none>"] = -1
                 for i in range(len(data)):
-                    self._metabolites[data['description'][i]] = data['guid'][i]
+                    self._metabolites[data["description"][i]] = data["guid"][i]
                 return self._metabolites
 
             def update_metabolite_plot(self, change):
                 """
                 Update plot in the notebook for new metabolite
 
                 :change: New metabolite identifier
                 """
                 if change.new:
                     y = self._get_data(change.new)
                     x = np.linspace(0, len(y), len(y))
                     line.set_xdata(x)
                     line.set_ydata(y)
-                    ax.axes.set_xlabel('Seconds')
-                    ax.axes.set_ylabel('mM')
+                    ax.axes.set_xlabel("Seconds")
+                    ax.axes.set_ylabel("mM")
                     ax.axes.relim()
                     ax.axes.autoscale_view()
                     figure.canvas.draw()
                     self._callback(self._location, change.new)
 
             def update_location(self, change):
                 """
@@ -259,15 +303,16 @@
 
                 :change: New list of locations
                 """
                 self._selections[self._location] = metabolite_selector.value
                 self._location = change.new
                 location_color_picker.value = self._location_colors[self._location]
                 location_color_opacity_slider.value = self._location_colors_opacity[
-                    self._location]
+                    self._location
+                ]
                 metabolite_selector.options = self.get_metabolites()
                 if self._location in self._selections:
                     metabolite_selector.value = self._selections[self._location]
 
             def update_location_color(self, change):
                 """
                 Update location color
@@ -288,66 +333,81 @@
 
             def _update_palette(self):
                 """
                 Update transfer function palette in the BioExplorer backend
 
                 :change: New palette
                 """
-                btf = self._core.get_model_transfer_function(
-                    id=self._model_id)
+                btf = self._core.get_model_transfer_function(id=self._model_id)
                 colors = list()
                 points = list()
                 nb_points = len(self._locations)
                 step = 1.0 / float(nb_points - 1)
                 for i in range(nb_points):
                     color = self._hex_to_rgb(self._location_colors[i])
-                    colors.append([
-                        float(color[0]) / 256.0,
-                        float(color[1]) / 256.0,
-                        float(color[2]) / 256.0])
+                    colors.append(
+                        [
+                            float(color[0]) / 256.0,
+                            float(color[1]) / 256.0,
+                            float(color[2]) / 256.0,
+                        ]
+                    )
                     points.append([i * step, self._location_colors_opacity[i]])
 
-                btf['colormap']['name'] = 'TransferFunctionEditor'
-                btf['colormap']['colors'] = colors
-                btf['opacity_curve'] = points
-                btf['range'] = [0, nb_points - 1]
+                btf["colormap"]["name"] = "TransferFunctionEditor"
+                btf["colormap"]["colors"] = colors
+                btf["opacity_curve"] = points
+                btf["range"] = [0, nb_points - 1]
                 self._core.set_model_transfer_function(
-                    id=self._model_id, transfer_function=btf)
+                    id=self._model_id, transfer_function=btf
+                )
 
-            @ staticmethod
+            @staticmethod
             def _html_color(rgb_color):
-                color_as_string = '#' + \
-                    '%02x' % (int)(rgb_color[0] * 255) + \
-                    '%02x' % (int)(rgb_color[1] * 255) + \
-                    '%02x' % (int)(rgb_color[2] * 255)
+                color_as_string = (
+                    "#"
+                    + "%02x" % (int)(rgb_color[0] * 255)
+                    + "%02x" % (int)(rgb_color[1] * 255)
+                    + "%02x" % (int)(rgb_color[2] * 255)
+                )
                 return color_as_string
 
-            @ staticmethod
+            @staticmethod
             def _hex_to_rgb(value):
-                value = value.lstrip('#')
+                value = value.lstrip("#")
                 lv = len(value)
-                return tuple(int(value[i:i + lv // 3], 16) for i in range(0, lv, lv // 3))
+                return tuple(
+                    int(value[i: i + lv // 3], 16) for i in range(0, lv, lv // 3)
+                )
 
             def _get_data(self, guid):
-                sql = "SELECT c.value as value, (SELECT value FROM %s.concentration " \
-                      "WHERE variable_guid=c.variable_guid AND " \
-                      "simulation_guid=c.simulation_guid AND " \
-                      "frame=0) AS base_value "\
-                      "FROM %s.concentration AS c, %s.variable AS v "\
-                      "WHERE c.variable_guid=v.guid AND "\
-                      "v.guid=%d AND c.simulation_guid=%d" % (
-                        self._db_schema, self._db_schema, self._db_schema,
-                        guid, self._simulation_guid)
+                sql = (
+                    "SELECT c.value as value, (SELECT value FROM %s.concentration "
+                    "WHERE variable_guid=c.variable_guid AND "
+                    "simulation_guid=c.simulation_guid AND "
+                    "frame=%d) AS base_value "
+                    "FROM %s.concentration AS c, %s.variable AS v "
+                    "WHERE c.variable_guid=v.guid AND "
+                    "v.guid=%d AND c.simulation_guid=%d"
+                    % (
+                        self._db_schema,
+                        self._reference_frame,
+                        self._db_schema,
+                        self._db_schema,
+                        guid,
+                        self._simulation_guid,
+                    )
+                )
                 data = pd.read_sql(sql, self._db_connection)
                 values = list()
                 for i in range(len(data)):
-                    value = float(data['value'][i])
+                    value = float(data["value"][i])
                     if self._relative_concentration:
-                        base_value = float(data['base_value'][i])
-                        values.append(100 * (value - base_value) / value)
+                        base_value = float(data["base_value"][i])
+                        values.append((value - base_value) / value)
                     else:
                         values.append(value)
                 return np.array(values, np.float32)
 
         def update_location(value):
             update_class.update_location(value)
 
@@ -366,67 +426,80 @@
         locations = update_class.get_locations()
         for location in update_class.get_locations():
             self._metabolite_ids[locations[location]] = -1
 
         y = np.linspace(0, 1, 1)
         x = np.linspace(0, 1, 1)
         figure, ax = plt.subplots(figsize=(7.5, 2))
-        line, = ax.plot(x, y)
+        (line,) = ax.plot(x, y)
         ax.grid(True)
-        grid = GridspecLayout(n_rows=3, n_columns=2, height='170px')
+        grid = GridspecLayout(n_rows=3, n_columns=2, height="170px")
         location_selector = Select(
-            options=update_class.get_locations(), description='Location',
-            layout=Layout(height="100px", width="350px"))
+            options=update_class.get_locations(),
+            description="Location",
+            layout=Layout(height="100px", width="350px"),
+        )
         metabolite_selector = Select(
-            options=update_class.get_metabolites(), description='Metabolite',
-            layout=Layout(height="100px", width="350px"))
+            options=update_class.get_metabolites(),
+            description="Metabolite",
+            layout=Layout(height="100px", width="350px"),
+        )
         location_color_opacity_slider = FloatSlider(
-            value=1.0, min=0.0, max=1.0, step=0.1, description='Opacity',
-            layout=Layout(width="350px"))
+            value=1.0,
+            min=0.0,
+            max=1.0,
+            step=0.1,
+            description="Opacity",
+            layout=Layout(width="350px"),
+        )
         location_color_picker = ColorPicker(
-            description='Color', layout=Layout(width="350px"))
+            description="Color", layout=Layout(width="350px")
+        )
 
         grid[0, 0] = location_selector
         grid[1, 0] = location_color_picker
         grid[2, 0] = location_color_opacity_slider
         grid[0, 1] = metabolite_selector
-        location_selector.observe(update_location, 'value')
-        metabolite_selector.observe(update_metabolite_plot, 'value')
-        location_color_picker.observe(update_location_color, 'value')
-        location_color_opacity_slider.observe(
-            update_location_color_opacity, 'value')
+        location_selector.observe(update_location, "value")
+        metabolite_selector.observe(update_metabolite_plot, "value")
+        location_color_picker.observe(update_location_color, "value")
+        location_color_opacity_slider.observe(update_location_color_opacity, "value")
         display(grid)
 
     def _get_simulation_guid(self, timestamp):
         """
         Get simulation identifier in the database, according to specified timestamp
 
         :timestamp: Simulation timestamp
         :return: Simulation identifier
         :rtype: int
         """
         try:
             sql_command = "SELECT guid FROM %s.simulation WHERE timestamp='%s'" % (
-                self._db_schema, timestamp)
+                self._db_schema,
+                timestamp,
+            )
             data = pd.read_sql(sql_command, self._db_connection)
-            return int(data['guid'])
+            return int(data["guid"])
         except Exception as e:
             print(e)
 
     def _put_metabolite_ids(self):
         """Set metabolites to the BioExplorer backend, with the corresponding value range"""
-        sql = "SELECT min(value) AS min, max(value) AS max " \
-              "FROM %s.concentration "\
-              "WHERE simulation_guid=%d AND "\
-              "variable_guid IN (" % (self._db_schema, self._simulation_guid)
+        sql = (
+            "SELECT min(value) AS min, max(value) AS max "
+            "FROM %s.concentration "
+            "WHERE simulation_guid=%d AND "
+            "variable_guid IN (" % (self._db_schema, self._simulation_guid)
+        )
 
         metabolite_ids = list()
         for metabolite_id in self._metabolite_ids:
             variable_id = int(self._metabolite_ids[metabolite_id])
-            sql += '%d,' % variable_id
+            sql += "%d," % variable_id
             metabolite_ids.append(variable_id)
-        sql = sql[:-1] + ')'
+        sql = sql[:-1] + ")"
         data = pd.read_sql(sql, self._db_connection)
         opacity_range = [0, 1]
         if len(data) != 0:
-            opacity_range = [data['min'][0], data['max'][0]]
+            opacity_range = [data["min"][0], data["max"][0]]
         return self.set_metabolites(metabolite_ids, opacity_range)
```

### Comparing `bioexplorer-1.4.0/bioexplorer/movie_maker.py` & `bioexplorer-1.5.0/bioexplorer/movie_maker.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Provides a class that ease the definition of smoothed camera paths"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -34,15 +34,15 @@
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-locals
 
 
 class MovieMaker:
     """Movie maker"""
 
-    PLUGIN_API_PREFIX = 'mm-'
+    PLUGIN_API_PREFIX = "mm-"
     FRAME_BUFFER_MODE_COLOR = 0
     FRAME_BUFFER_MODE_DEPTH = 1
 
     def __init__(self, bioexplorer):
         """
         Initialize the MovieMaker object
 
@@ -58,15 +58,17 @@
         Get the version of the SDK
 
         :return: The version of the SDK
         :rtype: string
         """
         return __version__
 
-    def build_camera_path(self, control_points, nb_steps_between_control_points, smoothing_size=1):
+    def build_camera_path(
+        self, control_points, nb_steps_between_control_points, smoothing_size=1
+    ):
         """
         Build a camera path from control points
 
         :control_points: List of control points
         :nb_steps_between_control_points: Number of steps between two control points
         :smoothing_size: Number of steps to be considered for the smoothing of the path
         """
@@ -87,31 +89,37 @@
                 direction = [0, 0, 0]
                 up = [0, 0, 0]
 
                 t_origin = [0, 0, 0]
                 t_direction = [0, 0, 0]
                 t_up = [0, 0, 0]
                 for k in range(3):
-                    t_origin[k] = (p1['origin'][k] - p0['origin'][k]) / \
-                        float(nb_steps_between_control_points)
-                    t_direction[k] = (p1['direction'][k] - p0['direction'][k]) / \
-                        float(nb_steps_between_control_points)
-                    t_up[k] = (p1['up'][k] - p0['up'][k]) / float(nb_steps_between_control_points)
-
-                    origin[k] = p0['origin'][k] + t_origin[k] * float(i)
-                    direction[k] = p0['direction'][k] + t_direction[k] * float(i)
-                    up[k] = p0['up'][k] + t_up[k] * float(i)
-
-                t_aperture_radius = (p1['apertureRadius'] - p0['apertureRadius']) / float(
-                    nb_steps_between_control_points)
-                aperture_radius = p0['apertureRadius'] + t_aperture_radius * float(i)
-
-                t_focus_distance = (p1['focusDistance'] - p0['focusDistance']) / \
-                    float(nb_steps_between_control_points)
-                focus_distance = p0['focusDistance'] + t_focus_distance * float(i)
+                    t_origin[k] = (p1["origin"][k] - p0["origin"][k]) / float(
+                        nb_steps_between_control_points
+                    )
+                    t_direction[k] = (p1["direction"][k] - p0["direction"][k]) / float(
+                        nb_steps_between_control_points
+                    )
+                    t_up[k] = (p1["up"][k] - p0["up"][k]) / float(
+                        nb_steps_between_control_points
+                    )
+
+                    origin[k] = p0["origin"][k] + t_origin[k] * float(i)
+                    direction[k] = p0["direction"][k] + t_direction[k] * float(i)
+                    up[k] = p0["up"][k] + t_up[k] * float(i)
+
+                t_aperture_radius = (
+                    p1["apertureRadius"] - p0["apertureRadius"]
+                ) / float(nb_steps_between_control_points)
+                aperture_radius = p0["apertureRadius"] + t_aperture_radius * float(i)
+
+                t_focus_distance = (p1["focusDistance"] - p0["focusDistance"]) / float(
+                    nb_steps_between_control_points
+                )
+                focus_distance = p0["focusDistance"] + t_focus_distance * float(i)
 
                 origins.append(origin)
                 directions.append(direction)
                 ups.append(up)
                 aperture_radii.append(aperture_radius)
                 focus_distances.append(focus_distance)
 
@@ -128,23 +136,43 @@
                     o[k] = o[k] + origins[index][k]
                     d[k] = d[k] + directions[index][k]
                     u[k] = u[k] + ups[index][k]
                 aperture_radius = aperture_radius + aperture_radii[index]
                 focus_distance = focus_distance + focus_distances[index]
             self._smoothed_key_frames.append(
                 [
-                    (o[0] / smoothing_size, o[1] / smoothing_size, o[2] / smoothing_size),
-                    (d[0] / smoothing_size, d[1] / smoothing_size, d[2] / smoothing_size),
-                    (u[0] / smoothing_size, u[1] / smoothing_size, u[2] / smoothing_size),
-                    aperture_radius / smoothing_size, focus_distance / smoothing_size
-                ])
+                    (
+                        o[0] / smoothing_size,
+                        o[1] / smoothing_size,
+                        o[2] / smoothing_size,
+                    ),
+                    (
+                        d[0] / smoothing_size,
+                        d[1] / smoothing_size,
+                        d[2] / smoothing_size,
+                    ),
+                    (
+                        u[0] / smoothing_size,
+                        u[1] / smoothing_size,
+                        u[2] / smoothing_size,
+                    ),
+                    aperture_radius / smoothing_size,
+                    focus_distance / smoothing_size,
+                ]
+            )
         last = control_points[len(control_points) - 1]
         self._smoothed_key_frames.append(
-            (last['origin'], last['direction'], last['up'], last['apertureRadius'],
-             last['focusDistance']))
+            (
+                last["origin"],
+                last["direction"],
+                last["up"],
+                last["apertureRadius"],
+                last["focusDistance"],
+            )
+        )
 
     def get_nb_frames(self):
         """
         Get the number of smoothed frames
 
         :return: The number of smoothed frames
         :rtype: integer
@@ -171,33 +199,48 @@
         :origin: Origin of the camera
         :direction: Direction in which the camera is looking
         :up: Up vector
         :return: Result of the request submission
         :rtype: Response
         """
         params = dict()
-        params['origin'] = origin
-        params['direction'] = direction
-        params['up'] = up
+        params["origin"] = origin
+        params["direction"] = direction
+        params["up"] = up
         return self._client.rockets_client.request(
-            self.PLUGIN_API_PREFIX + 'set-odu-camera', params)
+            self.PLUGIN_API_PREFIX + "set-odu-camera", params
+        )
 
     def get_camera(self):
         """
         Get the origin, direction and up vector of the camera
 
         :return: A JSon representation of the origin, direction and up vectors
         :rtype: Response
         """
-        return self._client.rockets_client.request(self.PLUGIN_API_PREFIX + 'get-odu-camera')
+        return self._client.rockets_client.request(
+            self.PLUGIN_API_PREFIX + "get-odu-camera"
+        )
 
-    def export_frames(self, size, path, base_name, image_format='png',
-                      animation_frames=list(), quality=100, samples_per_pixel=1, start_frame=0,
-                      end_frame=0, interpupillary_distance=0.0, export_intermediate_frames=False,
-                      frame_buffer_mode=FRAME_BUFFER_MODE_COLOR):
+    def export_frames(
+        self,
+        size,
+        path,
+        base_name,
+        image_format="png",
+        animation_frames=list(),
+        quality=100,
+        samples_per_pixel=1,
+        start_frame=0,
+        end_frame=0,
+        interpupillary_distance=0.0,
+        export_intermediate_frames=False,
+        frame_buffer_mode=FRAME_BUFFER_MODE_COLOR,
+        keywords=list(),
+    ):
         """
         Exports frames to disk. Frames are named using a 6 digit representation of the frame number
 
         :path: Folder into which frames are exported
         :image_format: Image format (the ones supported par Brayns: PNG, JPEG, etc)
         :quality: Quality of the exported image (Between 0 and 100)
         :samples_per_pixel: Number of samples per pixels
@@ -216,34 +259,45 @@
         assert isinstance(size, list)
         assert len(size) == 2
         if len(animation_frames) != 0:
             assert len(animation_frames) == nb_frames
         assert start_frame <= end_frame
         assert end_frame <= nb_frames
 
-        self._client.set_application_parameters(viewport=size)
         self._client.set_renderer(
-            accumulation=True, samples_per_pixel=1, max_accum_frames=samples_per_pixel + 1,
-            subsampling=1)
+            accumulation=True,
+            samples_per_pixel=1,
+            max_accum_frames=samples_per_pixel + 1,
+            subsampling=1,
+        )
 
         camera_definitions = list()
         for i in range(start_frame, end_frame):
             camera_definitions.append(self.get_key_frame(i))
 
+        assert isinstance(keywords, list)
+        keywords_as_string = ""
+        for keyword in keywords:
+            if keywords_as_string != "":
+                keywords_as_string += ","
+            keywords_as_string += keyword
+
         params = dict()
-        params['path'] = path
-        params['baseName'] = base_name
-        params['format'] = image_format
-        params['quality'] = quality
-        params['spp'] = samples_per_pixel
-        params['startFrame'] = start_frame
-        params['endFrame'] = end_frame
-        params['exportIntermediateFrames'] = export_intermediate_frames
-        params['animationInformation'] = animation_frames
-        params['frameBufferMode'] = frame_buffer_mode
+        params["path"] = path
+        params["baseName"] = base_name
+        params["format"] = image_format
+        params["size"] = size
+        params["quality"] = quality
+        params["spp"] = samples_per_pixel
+        params["startFrame"] = start_frame
+        params["endFrame"] = end_frame
+        params["exportIntermediateFrames"] = export_intermediate_frames
+        params["animationInformation"] = animation_frames
+        params["frameBufferMode"] = frame_buffer_mode
+        params["keywords"] = keywords_as_string
         values = list()
         for camera_definition in camera_definitions:
             # Origin
             for i in range(3):
                 values.append(camera_definition[0][i])
             # Direction
             for i in range(3):
@@ -254,51 +308,56 @@
             # Aperture radius
             values.append(camera_definition[3])
             # Focus distance
             values.append(camera_definition[4])
             # Interpupillary distance
             values.append(interpupillary_distance)
 
-        params['cameraInformation'] = values
+        params["cameraInformation"] = values
         return self._client.rockets_client.request(
-            self.PLUGIN_API_PREFIX + 'export-frames-to-disk', params)
+            self.PLUGIN_API_PREFIX + "export-frames-to-disk", params
+        )
 
     def get_export_frames_progress(self):
         """
         Queries the progress of the last export of frames to disk request
 
         :return: Dictionary with the result: "frameNumber" with the number of
         the last written-to-disk frame, and "done", a boolean flag stating wether
         the exporting is finished or is still in progress
         :rtype: Response
         """
         return self._client.rockets_client.request(
-            self.PLUGIN_API_PREFIX + 'get-export-frames-progress')
+            self.PLUGIN_API_PREFIX + "get-export-frames-progress"
+        )
 
     def cancel_frames_export(self):
         """
         Cancel the exports of frames to disk
 
         :return: Result of the request submission
         :rtype: Response
         """
         params = dict()
-        params['path'] = '/tmp'
-        params['baseName'] = ''
-        params['format'] = 'png'
-        params['quality'] = 100
-        params['spp'] = 1
-        params['startFrame'] = 0
-        params['endFrame'] = 0
-        params['exportIntermediateFrames'] = False
-        params['animationInformation'] = []
-        params['cameraInformation'] = []
-        params['frameBufferMode'] = MovieMaker.FRAME_BUFFER_MODE_COLOR
+        params["path"] = "/tmp"
+        params["baseName"] = ""
+        params["format"] = "png"
+        params["size"] = [64, 64]
+        params["quality"] = 100
+        params["spp"] = 1
+        params["startFrame"] = 0
+        params["endFrame"] = 0
+        params["exportIntermediateFrames"] = False
+        params["animationInformation"] = []
+        params["cameraInformation"] = []
+        params["frameBufferMode"] = MovieMaker.FRAME_BUFFER_MODE_COLOR
+        params["keywords"] = ""
         return self._client.rockets_client.request(
-            self.PLUGIN_API_PREFIX + 'export-frames-to-disk', params)
+            self.PLUGIN_API_PREFIX + "export-frames-to-disk", params
+        )
 
     def set_current_frame(self, frame, camera_params=None):
         """
         Set the current animation frame
 
         :frame: Frame number
         :camera_params: Camera parameters. Defaults to None.
@@ -319,129 +378,166 @@
             camera_params.aperture_radius = cam[3]
             camera_params.focus_distance = cam[4]
             camera_params.enable_clipping_planes = False
             self._client.set_camera_params(camera_params)
 
     def display(self):
         """Displays a widget giving access to the movie frames"""
-        frame = IntSlider(description='frame', min=0, max=self.get_nb_frames()-1)
+        frame = IntSlider(description="frame", min=0, max=self.get_nb_frames() - 1)
 
         def update_frame(args):
-            frame.value = args['new']
+            frame.value = args["new"]
             self.set_current_frame(frame.value)
 
-        frame.observe(update_frame, 'value')
+        frame.observe(update_frame, "value")
         display(frame)
 
     def _set_renderer_params(self, name, samples_per_pixel, gi_length=5.0):
         """
         Set renderer with default parameters
 
         :name: (string): Name of the renderer
         :gi_length: (float, optional): Max length of global illumination rays. Defaults to 5.0.
 
         :return: Frame buffer mode (color or depth)
         :rtype: int
         """
         spp = samples_per_pixel
         frame_buffer_mode = MovieMaker.FRAME_BUFFER_MODE_COLOR
-        if name == 'ambient_occlusion':
+        if name == "ambient_occlusion":
             params = self._client.AmbientOcclusionRendererParams()
             params.samples_per_frame = 16
             params.ray_length = gi_length
             self._client.set_renderer_params(params)
             spp = 4
-        elif name == 'depth':
+        elif name == "depth":
             frame_buffer_mode = MovieMaker.FRAME_BUFFER_MODE_DEPTH
             spp = 1
-        elif name in ['albedo', 'raycast_Ns']:
+        elif name in ["albedo", "raycast_Ns"]:
             spp = 4
-        elif name == 'shadow':
+        elif name == "shadow":
             params = self._client.ShadowRendererParams()
             params.samples_per_frame = 16
             params.ray_length = gi_length
             self._client.set_renderer_params(params)
             spp = 4
         return frame_buffer_mode, spp
 
     def create_snapshot(
-            self, renderer, size, path, base_name, samples_per_pixel,
-            export_intermediate_frames=False, gi_length=1e6, show_progress=False):
+        self,
+        renderer,
+        size,
+        path,
+        base_name,
+        samples_per_pixel,
+        export_intermediate_frames=False,
+        gi_length=1e6,
+        show_progress=False,
+        keywords=list(),
+    ):
         """
         Create a snapshot of the current frame
 
         :renderer: Name of the renderer
         :size: Frame buffer size
         :path: Path where the snapshot file is exported
         :base_name: Base name of the snapshot file
         :samples_per_pixel: Samples per pixel
         :export_intermediate_frames: If True, intermediate samples are stored to disk. Otherwise,
         only the final accumulation is exported
         gi_length (float, optional): Max length of global illumination rays. Defaults to 5.0.
+        :keywords: List of keywords that will be added to the Xmp.dc.Subject tag
         """
         assert isinstance(size, list)
         assert isinstance(samples_per_pixel, int)
         assert len(size) == 2
         assert isinstance(export_intermediate_frames, bool)
         assert isinstance(gi_length, float)
 
         application_params = self._client.get_application_parameters()
         renderer_params = self._client.get_renderer()
-        old_image_stream_fps = application_params['image_stream_fps']
-        old_viewport_size = application_params['viewport']
-        old_samples_per_pixel = renderer_params['samples_per_pixel']
-        old_max_accum_frames = renderer_params['max_accum_frames']
+        old_image_stream_fps = application_params["image_stream_fps"]
+        old_viewport_size = application_params["viewport"]
+        old_samples_per_pixel = renderer_params["samples_per_pixel"]
+        old_max_accum_frames = renderer_params["max_accum_frames"]
         old_smoothed_key_frames = copy.deepcopy(self._smoothed_key_frames)
 
-        self._client.set_renderer(current=renderer, samples_per_pixel=1, max_accum_frames=1)
+        self._client.set_renderer(
+            current=renderer, samples_per_pixel=1, max_accum_frames=1
+        )
         self._client.set_application_parameters(viewport=size)
         self._client.set_application_parameters(image_stream_fps=0)
 
-        frame_buffer_mode, spp = self._set_renderer_params(renderer, samples_per_pixel, gi_length)
+        frame_buffer_mode, spp = self._set_renderer_params(
+            renderer, samples_per_pixel, gi_length
+        )
         self._client.set_renderer(max_accum_frames=spp)
 
         control_points = [self.get_camera()]
-        current_animation_frame = int(self._client.get_animation_parameters()['current'])
+        current_animation_frame = int(
+            self._client.get_animation_parameters()["current"]
+        )
         animation_frames = [current_animation_frame]
 
         self.build_camera_path(
-            control_points=control_points, nb_steps_between_control_points=1, smoothing_size=1)
+            control_points=control_points,
+            nb_steps_between_control_points=1,
+            smoothing_size=1,
+        )
 
         if show_progress:
-            progress_widget = IntProgress(description='In progress...', min=0, max=100, value=0)
+            progress_widget = IntProgress(
+                description="In progress...", min=0, max=100, value=0
+            )
             display(progress_widget)
 
         self.export_frames(
-            path=path, base_name=base_name, animation_frames=animation_frames, size=size,
+            path=path,
+            base_name=base_name,
+            animation_frames=animation_frames,
+            size=size,
             samples_per_pixel=spp,
             export_intermediate_frames=export_intermediate_frames,
-            frame_buffer_mode=frame_buffer_mode)
+            frame_buffer_mode=frame_buffer_mode,
+            keywords=keywords,
+        )
 
         done = False
         while not done:
             time.sleep(1)
             if show_progress:
-                progress = self.get_export_frames_progress()['progress']
+                progress = self.get_export_frames_progress()["progress"]
                 progress_widget.value = progress * 100
-            done = self.get_export_frames_progress()['done']
+            done = self.get_export_frames_progress()["done"]
 
         if show_progress:
-            progress_widget.description = 'Done'
+            progress_widget.description = "Done"
             progress_widget.value = 100
 
-        self._client.set_application_parameters(image_stream_fps=old_image_stream_fps,
-                                                viewport=old_viewport_size)
-        self._client.set_renderer(samples_per_pixel=old_samples_per_pixel,
-                                  max_accum_frames=old_max_accum_frames)
+        self._client.set_application_parameters(
+            image_stream_fps=old_image_stream_fps, viewport=old_viewport_size
+        )
+        self._client.set_renderer(
+            samples_per_pixel=old_samples_per_pixel,
+            max_accum_frames=old_max_accum_frames,
+        )
         self._smoothed_key_frames = copy.deepcopy(old_smoothed_key_frames)
 
     def create_movie(
-            self, path, size, animation_frames=list(), quality=100, samples_per_pixel=1,
-            start_frame=0, end_frame=0, interpupillary_distance=0.0,
-            export_intermediate_frames=True):
+        self,
+        path,
+        size,
+        animation_frames=list(),
+        quality=100,
+        samples_per_pixel=1,
+        start_frame=0,
+        end_frame=0,
+        interpupillary_distance=0.0,
+        export_intermediate_frames=True,
+    ):
         """
         Create and export a set of PNG frames for later movie generation
 
         :path: Full path of the snapshot folder
         :size: Frame buffer size
         :animation_frames: Optional list of animation frames
         :quality: PNG quality
@@ -452,38 +548,52 @@
         is disabled
         :export_intermediate_frames: If True, intermediate samples are stored to disk. Otherwise,
         only the final accumulation is exported
         """
         application_params = self._client.get_application_parameters()
         renderer_params = self._client.get_renderer()
 
-        old_image_stream_fps = application_params['image_stream_fps']
-        old_viewport_size = application_params['viewport']
-        old_samples_per_pixel = renderer_params['samples_per_pixel']
-        old_max_accum_frames = renderer_params['max_accum_frames']
-        self._client.set_renderer(samples_per_pixel=1, max_accum_frames=samples_per_pixel)
+        old_image_stream_fps = application_params["image_stream_fps"]
+        old_viewport_size = application_params["viewport"]
+        old_samples_per_pixel = renderer_params["samples_per_pixel"]
+        old_max_accum_frames = renderer_params["max_accum_frames"]
+        self._client.set_renderer(
+            samples_per_pixel=1, max_accum_frames=samples_per_pixel
+        )
         self._client.set_application_parameters(viewport=size)
         self._client.set_application_parameters(image_stream_fps=0)
 
-        progress_widget = IntProgress(description='In progress...', min=0, max=100, value=0)
+        progress_widget = IntProgress(
+            description="In progress...", min=0, max=100, value=0
+        )
         display(progress_widget)
 
         self.export_frames(
-            path=path, base_name='', animation_frames=animation_frames, start_frame=start_frame,
-            end_frame=end_frame, size=size, samples_per_pixel=samples_per_pixel, quality=quality,
+            path=path,
+            base_name="",
+            animation_frames=animation_frames,
+            start_frame=start_frame,
+            end_frame=end_frame,
+            size=size,
+            samples_per_pixel=samples_per_pixel,
+            quality=quality,
             interpupillary_distance=interpupillary_distance,
-            export_intermediate_frames=export_intermediate_frames)
+            export_intermediate_frames=export_intermediate_frames,
+        )
 
         done = False
         while not done:
             time.sleep(1)
-            progress = self.get_export_frames_progress()['progress']
+            progress = self.get_export_frames_progress()["progress"]
             progress_widget.value = progress * 100
-            done = self.get_export_frames_progress()['done']
+            done = self.get_export_frames_progress()["done"]
 
-        self._client.set_application_parameters(image_stream_fps=old_image_stream_fps,
-                                                viewport=old_viewport_size)
-        self._client.set_renderer(samples_per_pixel=old_samples_per_pixel,
-                                  max_accum_frames=old_max_accum_frames)
+        self._client.set_application_parameters(
+            image_stream_fps=old_image_stream_fps, viewport=old_viewport_size
+        )
+        self._client.set_renderer(
+            samples_per_pixel=old_samples_per_pixel,
+            max_accum_frames=old_max_accum_frames,
+        )
 
-        progress_widget.description = 'Done'
+        progress_widget.description = "Done"
         progress_widget.value = 100
```

### Comparing `bioexplorer-1.4.0/bioexplorer/movie_scenario.py` & `bioexplorer-1.5.0/bioexplorer/movie_scenario.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Movie scenario"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -34,17 +34,28 @@
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-locals
 
 
 class MovieScenario:
     """Super class for creating movies"""
 
-    def __init__(self, hostname, port, projection, output_folder, image_k=4,
-                 image_samples_per_pixel=64, log_level=1, v1_compatibility=False,
-                 shaders=list(['bio_explorer']), draft=False, gi_length=1e6):
+    def __init__(
+        self,
+        hostname,
+        port,
+        projection,
+        output_folder,
+        image_k=4,
+        image_samples_per_pixel=64,
+        log_level=1,
+        v1_compatibility=False,
+        shaders=list(["bio_explorer"]),
+        draft=False,
+        gi_length=1e6,
+    ):
         """
         Initialize movie scenario
 
         :hostname: Host name where BioExplorer is running
         :port: Port of the BioExplorer WebSocket
         :projection: Camera projection (Perspective, Orthographic, etc)
         :output_folder: Folder where frame are savec
@@ -52,64 +63,78 @@
         :image_samples_per_pixel: Number of samples per pixel. Defaults to 64.
         :log_level: Logging level. Defaults to 1
         :v1_compatibility: Used to regenerated movies from BioExplorer version 1. Defaults to False.
         :shaders: List of shaders to render. Defaults to list(['bio_explorer']).
         """
         self._log_level = log_level
         self._hostname = hostname
-        self._url = hostname + ':' + str(port)
+        self._url = hostname + ":" + str(port)
         self._be = BioExplorer(self._url)
         self._core = self._be.core_api()
         self._mm = MovieMaker(self._be)
 
         self._image_size = [image_k * 960, image_k * 540]
         self._image_samples_per_pixel = image_samples_per_pixel
         self._image_projection = projection
         self._image_output_folder = output_folder
         self._shaders = shaders
         self._gi_length = gi_length
         self._draft = draft
         self._prepare_movie(projection, image_k)
         self._be.set_general_settings(
-            model_visibility_on_creation=False,
-            v1_compatibility=v1_compatibility
+            model_visibility_on_creation=False, v1_compatibility=v1_compatibility
+        )
+        self._log(
+            1,
+            "============================================================================",
+        )
+        self._log(1, "- Version          : " + self._be.version())
+        self._log(1, "- URL              : " + self._url)
+        self._log(1, "- Projection       : " + projection)
+        self._log(1, "- Frame size       : " + str(self._image_size))
+        self._log(1, "- Export folder    : " + self._image_output_folder)
+        self._log(1, "- Samples per pixel: " + str(self._image_samples_per_pixel))
+        self._log(
+            1,
+            "============================================================================",
         )
-        self._log(1, '============================================================================')
-        self._log(1, '- Version          : ' + self._be.version())
-        self._log(1, '- URL              : ' + self._url)
-        self._log(1, '- Projection       : ' + projection)
-        self._log(1, '- Frame size       : ' + str(self._image_size))
-        self._log(1, '- Export folder    : ' + self._image_output_folder)
-        self._log(1, '- Samples per pixel: ' + str(self._image_samples_per_pixel))
-        self._log(1, '============================================================================')
 
     def build_frame(self, frame):
         """
         Build the specified frame
 
         :frame: Index of the frame to build
         """
-        raise NotImplementedError('You need to define a build_frame method!')
+        raise NotImplementedError("You need to define a build_frame method!")
 
     def render_movie(
-            self, cameras_key_frames, nb_frames_between_keys, nb_smoothing_frames, start_frame=0,
-            end_frame=0, frame_step=1, frame_list=list()):
+        self,
+        cameras_key_frames,
+        nb_frames_between_keys,
+        nb_smoothing_frames,
+        start_frame=0,
+        end_frame=0,
+        frame_step=1,
+        frame_list=list(),
+    ):
         """
         Render the speficied frames
 
         :cameras_key_frames: List of camera key-frames
         :nb_frames_between_keys: Number of frames between each key frame
         :nb_smoothing_frames: Number of frames used to average the camera position and orientation
         :start_frame: Index of the first frame to render. Defaults to 0
         :end_frame: Index of the last frame to render. Defaults to 0
         :frame_step: Number of frames to skip. Defaults to 1
         :frame_list: Explicit list of frames to render. Defaults to list().
         """
-        self._mm.build_camera_path(cameras_key_frames, nb_frames_between_keys, nb_smoothing_frames)
-        self._log(1, '- Total number of frames: %d' % self._mm.get_nb_frames())
+        self._mm.build_camera_path(
+            cameras_key_frames, nb_frames_between_keys, nb_smoothing_frames
+        )
+        self._log(1, "- Total number of frames: %d" % self._mm.get_nb_frames())
 
         self._core.set_application_parameters(viewport=self._image_size)
         self._core.set_application_parameters(image_stream_fps=0)
 
         frames_to_render = list()
         if len(frame_list) != 0:
             frames_to_render = frame_list
@@ -122,133 +147,210 @@
         cumulated_rendering_time = 0
         nb_frames = len(frames_to_render)
         frame_count = 1
 
         # Frames
         for frame in frames_to_render:
             start = time.time()
-            self._log(1, '- Rendering frame %i (%i/%i)' % (frame, frame_count, nb_frames))
-            self._log(1, '------------------------------')
+            self._log(
+                1, "- Rendering frame %i (%i/%i)" % (frame, frame_count, nb_frames)
+            )
+            self._log(1, "------------------------------")
 
             # Stop rendering during the loading of the scene
             self._core.set_renderer(
-                samples_per_pixel=1, subsampling=1, max_accum_frames=1)
+                samples_per_pixel=1, subsampling=1, max_accum_frames=1
+            )
 
             # Set camera
             self._mm.set_current_frame(
-                frame=frame, camera_params=self._core.BioExplorerPerspectiveCameraParams())
+                frame=frame,
+                camera_params=self._core.BioExplorerPerspectiveCameraParams(),
+            )
 
             # Frame setup
             self.build_frame(frame)
 
-            self._log(1, '- Frame buffers')
+            self._log(1, "- Frame buffers")
             for shader in self._shaders:
                 # Rendering settings
-                self._log(2, '-   ' + shader)
+                self._log(2, "-   " + shader)
                 self._render_frame(shader, frame)
 
             end = time.time()
 
             rendering_time = end - start
             cumulated_rendering_time += rendering_time
             average_rendering_time = cumulated_rendering_time / frame_count
-            remaining_rendering_time = (nb_frames - frame_count) * average_rendering_time
-            self._log(1, '------------------------------')
-            self._log(1, 'Frame %i successfully rendered in %i seconds' %
-                      (frame, rendering_time))
+            remaining_rendering_time = (
+                nb_frames - frame_count
+            ) * average_rendering_time
+            self._log(1, "------------------------------")
+            self._log(
+                1,
+                "Frame %i successfully rendered in %i seconds"
+                % (frame, rendering_time),
+            )
 
             hours = math.floor(remaining_rendering_time / 3600)
             minutes = math.floor((remaining_rendering_time - hours * 3600) / 60)
             seconds = math.floor(remaining_rendering_time - hours * 3600 - minutes * 60)
 
-            expected_end_time = datetime.now() + timedelta(seconds=remaining_rendering_time)
-            self._log(1, 'Estimated remaining time: %i hours, %i minutes, %i seconds' %
-                      (hours, minutes, seconds))
-            self._log(1, 'Expected end time       : %s' % expected_end_time)
+            expected_end_time = datetime.now() + timedelta(
+                seconds=remaining_rendering_time
+            )
             self._log(
-                1, '----------------------------------------------------------------------------')
+                1,
+                "Estimated remaining time: %i hours, %i minutes, %i seconds"
+                % (hours, minutes, seconds),
+            )
+            self._log(1, "Expected end time       : %s" % expected_end_time)
+            self._log(
+                1,
+                "----------------------------------------------------------------------------",
+            )
             frame_count += 1
 
         self._core.set_application_parameters(image_stream_fps=20)
-        self._log(1, 'Movie rendered, live long and prosper \\V/')
+        self._log(1, "Movie rendered, live long and prosper \\V/")
 
     def _log(self, level, message):
         if level <= self._log_level:
-            print('[' + str(datetime.now()) + '] ' + message)
+            print("[" + str(datetime.now()) + "] " + message)
 
     @staticmethod
     def _check(method):
         response = method
-        if not response['status']:
-            raise Exception(response['contents'])
+        if not response["status"]:
+            raise Exception(response["contents"])
 
     def _make_export_folders(self):
         for folder in self._shaders:
-            path = self._image_output_folder + '/' + folder
+            path = self._image_output_folder + "/" + folder
             if not os.path.isdir(path):
-                self._log(1, 'Creating ' + path)
+                self._log(1, "Creating " + path)
                 os.makedirs(path)
 
     def _prepare_movie(self, projection, image_k):
-        if projection == 'perspective':
-            self._image_size = [image_k*960, image_k*540]
-            self._core.set_camera(current='bio_explorer_perspective')
-        elif projection == 'fisheye':
-            self._image_size = [int(image_k*1024), int(image_k*1024)]
-            self._core.set_camera(current='fisheye')
-        elif projection == 'panoramic':
-            self._image_size = [int(image_k*1024), int(image_k*1024)]
-            self._core.set_camera(current='panoramic')
-        elif projection == 'opendeck':
-            self._log(1, 'Warning: OpenDeck resolution is set server side '
-                         '(--resolution-scaling plug-in parameter)')
+        if projection == "perspective":
+            self._image_size = [image_k * 960, image_k * 540]
+            self._core.set_camera(current="bio_explorer_perspective")
+        elif projection == "fisheye":
+            self._image_size = [int(image_k * 1024), int(image_k * 1024)]
+            self._core.set_camera(current="fisheye")
+        elif projection == "panoramic":
+            self._image_size = [int(image_k * 1024), int(image_k * 1024)]
+            self._core.set_camera(current="panoramic")
+        elif projection == "opendeck":
+            self._log(
+                1,
+                "Warning: OpenDeck resolution is set server side "
+                "(--resolution-scaling plug-in parameter)",
+            )
             self._image_size = [11940, 3424]
-            self._core.set_camera(current='cylindric')
+            self._core.set_camera(current="cylindric")
 
-        self._image_output_folder = self._image_output_folder + '/' + \
-            projection + '/' + str(self._image_size[0]) + 'x' + str(self._image_size[1])
+        self._image_output_folder = (
+            self._image_output_folder
+            + "/"
+            + projection
+            + "/"
+            + str(self._image_size[0])
+            + "x"
+            + str(self._image_size[1])
+        )
         self._make_export_folders()
-        self._log(2, '- Forcing viewport size to ' + str(self._image_size))
+        self._log(2, "- Forcing viewport size to " + str(self._image_size))
         self._core.set_application_parameters(viewport=self._image_size)
 
     def _render_frame(self, renderer, frame):
-        self._log(2, '- Creating snapshot ' + str(self._image_size))
+        self._log(2, "- Creating snapshot " + str(self._image_size))
         self._mm.create_snapshot(
             renderer=renderer,
-            size=self._image_size, path=self._image_output_folder + '/' + renderer,
-            base_name='%05d' % frame, samples_per_pixel=self._image_samples_per_pixel,
-            gi_length=self._gi_length)
+            size=self._image_size,
+            path=self._image_output_folder + "/" + renderer,
+            base_name="%05d" % frame,
+            samples_per_pixel=self._image_samples_per_pixel,
+            gi_length=self._gi_length,
+        )
 
     @staticmethod
     def parse_arguments(argv):
         """
         Parse command line arguments
 
         :argv: List of command line arguments
         """
-        parser = argparse.ArgumentParser(description='Missing frames')
-        parser.add_argument('-e', '--export-folder', help='Export folder', type=str, default='/tmp')
-        parser.add_argument('-n', '--hostname',
-                            help='BioExplorer server hostname', type=str, default='localhost')
-        parser.add_argument('-p', '--port',
-                            help='BioExplorer server port', type=int, default=5000)
-        parser.add_argument('-j', '--projection', help='Camera projection',
-                            type=str, default='perspective',
-                            choices=['perspective', 'fisheye', 'panoramic', 'opendeck'])
-        parser.add_argument('-r', '--shaders', help='Camera projection',
-                            type=str, nargs='*', default=['bio_explorer'],
-                            choices=[
-                                'albedo', 'ambient_occlusion', 'basic', 'depth', 'raycast_Ns',
-                                'bio_explorer', 'circuit_explorer_advanced'])
-        parser.add_argument('-k', '--image-resolution-k',
-                            help='Image resolution in K', type=int, default=1)
-        parser.add_argument('-s', '--image-samples-per-pixel',
-                            help='Image samples per pixel', type=int, default=32)
-        parser.add_argument('-f', '--from_frame', type=int, help='Start frame', default=0)
-        parser.add_argument('-t', '--to-frame', type=int, help='End frame', default=0)
-        parser.add_argument('-m', '--frame-step', type=int, help='Frame step', default=1)
-        parser.add_argument('-g', '--log-level', type=int, help='Frame step', default=1)
-        parser.add_argument('-l', '--frame-list', type=int, nargs='*',
-                            help='List of frames to render', default=list())
-        parser.add_argument('-z', '--magnetic', help='Magnetic fields', action='store_true')
-        parser.add_argument('-d', '--draft', help='Draft mode', action='store_true')
+        parser = argparse.ArgumentParser(description="Missing frames")
+        parser.add_argument(
+            "-e", "--export-folder", help="Export folder", type=str, default="/tmp"
+        )
+        parser.add_argument(
+            "-n",
+            "--hostname",
+            help="BioExplorer server hostname",
+            type=str,
+            default="localhost",
+        )
+        parser.add_argument(
+            "-p", "--port", help="BioExplorer server port", type=int, default=5000
+        )
+        parser.add_argument(
+            "-j",
+            "--projection",
+            help="Camera projection",
+            type=str,
+            default="perspective",
+            choices=["perspective", "fisheye", "panoramic", "opendeck"],
+        )
+        parser.add_argument(
+            "-r",
+            "--shaders",
+            help="Camera projection",
+            type=str,
+            nargs="*",
+            default=["bio_explorer"],
+            choices=[
+                "albedo",
+                "ambient_occlusion",
+                "basic",
+                "depth",
+                "raycast_Ns",
+                "bio_explorer",
+                "circuit_explorer_advanced",
+            ],
+        )
+        parser.add_argument(
+            "-k",
+            "--image-resolution-k",
+            help="Image resolution in K",
+            type=int,
+            default=1,
+        )
+        parser.add_argument(
+            "-s",
+            "--image-samples-per-pixel",
+            help="Image samples per pixel",
+            type=int,
+            default=32,
+        )
+        parser.add_argument(
+            "-f", "--from_frame", type=int, help="Start frame", default=0
+        )
+        parser.add_argument("-t", "--to-frame", type=int, help="End frame", default=0)
+        parser.add_argument(
+            "-m", "--frame-step", type=int, help="Frame step", default=1
+        )
+        parser.add_argument("-g", "--log-level", type=int, help="Frame step", default=1)
+        parser.add_argument(
+            "-l",
+            "--frame-list",
+            type=int,
+            nargs="*",
+            help="List of frames to render",
+            default=list(),
+        )
+        parser.add_argument(
+            "-z", "--magnetic", help="Magnetic fields", action="store_true"
+        )
+        parser.add_argument("-d", "--draft", help="Draft mode", action="store_true")
         return parser.parse_args(argv)
```

### Comparing `bioexplorer-1.4.0/bioexplorer/notebook_widgets.py` & `bioexplorer-1.5.0/bioexplorer/notebook_widgets.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """BioExplorer widgets"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -24,85 +24,247 @@
 import math
 import random
 import threading
 import time
 import glob
 import os
 import io
-from ipywidgets import FloatSlider, Select, HBox, VBox, Layout, Button, SelectMultiple, \
-    Checkbox, IntRangeSlider, ColorPicker, IntSlider, Label, Text, Image
+from ipywidgets import (
+    FloatSlider,
+    Select,
+    HBox,
+    VBox,
+    Layout,
+    Button,
+    SelectMultiple,
+    Checkbox,
+    IntRangeSlider,
+    ColorPicker,
+    IntSlider,
+    Label,
+    Text,
+    Image,
+)
 from IPython.display import display
 import matplotlib
 import seaborn as sns
 from stringcase import pascalcase
 from PIL import ImageDraw
 from .bio_explorer import Vector3
 
 
 # pylint: disable=unused-argument
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-statements
 
 COLOR_MAPS = [
-    'Accent', 'Accent_r', 'Blues', 'Blues_r', 'BrBG', 'BrBG_r', 'BuGn', 'BuGn_r',
-    'BuPu', 'BuPu_r', 'CMRmap', 'CMRmap_r', 'Dark2', 'Dark2_r', 'GnBu', 'GnBu_r',
-    'Greens', 'Greens_r', 'Greys', 'Greys_r', 'OrRd', 'OrRd_r', 'Oranges', 'Oranges_r',
-    'PRGn', 'PRGn_r', 'Paired', 'Paired_r', 'Pastel1', 'Pastel1_r', 'Pastel2', 'Pastel2_r',
-    'PiYG', 'PiYG_r', 'PuBu', 'PuBuGn', 'PuBuGn_r', 'PuBu_r', 'PuOr', 'PuOr_r',
-    'PuRd', 'PuRd_r', 'Purples', 'Purples_r', 'RdBu', 'RdBu_r', 'RdGy', 'RdGy_r',
-    'RdPu', 'RdPu_r', 'RdYlBu', 'RdYlBu_r', 'RdYlGn', 'RdYlGn_r', 'Reds', 'Reds_r',
-    'Set1', 'Set1_r', 'Set2', 'Set2_r', 'Set3', 'Set3_r',
-    'Wistia', 'Wistia_r', 'YlGn', 'YlGnBu', 'YlGnBu_r', 'YlGn_r', 'YlOrBr',
-    'YlOrBr_r', 'YlOrRd', 'YlOrRd_r', 'afmhot', 'afmhot_r', 'autumn', 'autumn_r',
-    'binary', 'binary_r', 'bone', 'bone_r', 'brg', 'brg_r', 'bwr', 'bwr_r', 'cool', 'cool_r',
-    'coolwarm', 'coolwarm_r', 'copper', 'copper_r', 'cubehelix', 'cubehelix_r', 'flag',
-    'flag_r', 'gist_earth', 'gist_earth_r', 'gist_gray', 'gist_gray_r', 'gist_heat',
-    'gist_heat_r', 'gist_ncar', 'gist_ncar_r', 'gist_rainbow', 'gist_rainbow_r', 'gist_stern',
-    'gist_stern_r', 'gist_yarg', 'gist_yarg_r', 'gnuplot', 'gnuplot2', 'gnuplot2_r',
-    'gnuplot_r', 'gray', 'gray_r', 'hot', 'hot_r', 'hsv', 'hsv_r', 'icefire', 'icefire_r',
-    'inferno', 'inferno_r', 'jet_r', 'magma', 'magma_r', 'mako', 'mako_r',
-    'nipy_spectral', 'nipy_spectral_r', 'ocean', 'ocean_r', 'pink', 'pink_r', 'plasma',
-    'plasma_r', 'prism', 'prism_r', 'rainbow', 'rainbow_r', 'rocket', 'rocket_r', 'seismic',
-    'seismic_r', 'spring', 'spring_r', 'summer', 'summer_r',
-    'tab10', 'tab10_r', 'tab20', 'tab20_r', 'tab20b', 'tab20b_r', 'tab20c', 'tab20c_r',
-    'terrain', 'terrain_r', 'viridis', 'viridis_r', 'vlag', 'vlag_r', 'winter', 'winter_r'
+    "Accent",
+    "Accent_r",
+    "Blues",
+    "Blues_r",
+    "BrBG",
+    "BrBG_r",
+    "BuGn",
+    "BuGn_r",
+    "BuPu",
+    "BuPu_r",
+    "CMRmap",
+    "CMRmap_r",
+    "Dark2",
+    "Dark2_r",
+    "GnBu",
+    "GnBu_r",
+    "Greens",
+    "Greens_r",
+    "Greys",
+    "Greys_r",
+    "OrRd",
+    "OrRd_r",
+    "Oranges",
+    "Oranges_r",
+    "PRGn",
+    "PRGn_r",
+    "Paired",
+    "Paired_r",
+    "Pastel1",
+    "Pastel1_r",
+    "Pastel2",
+    "Pastel2_r",
+    "PiYG",
+    "PiYG_r",
+    "PuBu",
+    "PuBuGn",
+    "PuBuGn_r",
+    "PuBu_r",
+    "PuOr",
+    "PuOr_r",
+    "PuRd",
+    "PuRd_r",
+    "Purples",
+    "Purples_r",
+    "RdBu",
+    "RdBu_r",
+    "RdGy",
+    "RdGy_r",
+    "RdPu",
+    "RdPu_r",
+    "RdYlBu",
+    "RdYlBu_r",
+    "RdYlGn",
+    "RdYlGn_r",
+    "Reds",
+    "Reds_r",
+    "Set1",
+    "Set1_r",
+    "Set2",
+    "Set2_r",
+    "Set3",
+    "Set3_r",
+    "Wistia",
+    "Wistia_r",
+    "YlGn",
+    "YlGnBu",
+    "YlGnBu_r",
+    "YlGn_r",
+    "YlOrBr",
+    "YlOrBr_r",
+    "YlOrRd",
+    "YlOrRd_r",
+    "afmhot",
+    "afmhot_r",
+    "autumn",
+    "autumn_r",
+    "binary",
+    "binary_r",
+    "bone",
+    "bone_r",
+    "brg",
+    "brg_r",
+    "bwr",
+    "bwr_r",
+    "cool",
+    "cool_r",
+    "coolwarm",
+    "coolwarm_r",
+    "copper",
+    "copper_r",
+    "cubehelix",
+    "cubehelix_r",
+    "flag",
+    "flag_r",
+    "gist_earth",
+    "gist_earth_r",
+    "gist_gray",
+    "gist_gray_r",
+    "gist_heat",
+    "gist_heat_r",
+    "gist_ncar",
+    "gist_ncar_r",
+    "gist_rainbow",
+    "gist_rainbow_r",
+    "gist_stern",
+    "gist_stern_r",
+    "gist_yarg",
+    "gist_yarg_r",
+    "gnuplot",
+    "gnuplot2",
+    "gnuplot2_r",
+    "gnuplot_r",
+    "gray",
+    "gray_r",
+    "hot",
+    "hot_r",
+    "hsv",
+    "hsv_r",
+    "icefire",
+    "icefire_r",
+    "inferno",
+    "inferno_r",
+    "jet_r",
+    "magma",
+    "magma_r",
+    "mako",
+    "mako_r",
+    "nipy_spectral",
+    "nipy_spectral_r",
+    "ocean",
+    "ocean_r",
+    "pink",
+    "pink_r",
+    "plasma",
+    "plasma_r",
+    "prism",
+    "prism_r",
+    "rainbow",
+    "rainbow_r",
+    "rocket",
+    "rocket_r",
+    "seismic",
+    "seismic_r",
+    "spring",
+    "spring_r",
+    "summer",
+    "summer_r",
+    "tab10",
+    "tab10_r",
+    "tab20",
+    "tab20_r",
+    "tab20b",
+    "tab20b_r",
+    "tab20c",
+    "tab20c_r",
+    "terrain",
+    "terrain_r",
+    "viridis",
+    "viridis_r",
+    "vlag",
+    "vlag_r",
+    "winter",
+    "winter_r",
 ]
 
 SHADING_MODES = [
-    'none', 'basic', 'diffuse', 'electron', 'cartoon', 'electron_transparency', 'perlin',
-    'diffuse_transparency', 'checker', 'goodsell'
+    "none",
+    "basic",
+    "diffuse",
+    "electron",
+    "cartoon",
+    "electron_transparency",
+    "perlin",
+    "diffuse_transparency",
+    "checker",
+    "goodsell",
 ]
 
-CHAMELEON_MODES = [
-    'none', 'emitter', 'receiver'
-]
+CHAMELEON_MODES = ["none", "emitter", "receiver"]
 
-DEFAULT_GRID_LAYOUT = Layout(border='1px solid black', margin='5px', padding='5px')
-DEFAULT_LAYOUT = Layout(width='50%', height='24px', display='flex', flex_flow='row')
-STYLE = {'description_width': 'initial', 'handle_color': 'gray'}
+DEFAULT_GRID_LAYOUT = Layout(border="1px solid black", margin="5px", padding="5px")
+DEFAULT_LAYOUT = Layout(width="50%", height="24px", display="flex", flex_flow="row")
+STYLE = {"description_width": "initial", "handle_color": "gray"}
 
 
 class Widgets:
     """Set of notebook widgets for the BioExplorer"""
 
     def __init__(self, bioexplorer):
         """Initialize with a reference to BioExplorer and underlying Brayns API"""
         self._be = bioexplorer
         self._client = bioexplorer.core_api()
 
     def display_focal_distance(self, with_preview=False):
         """Display visual controls for setting camera focal distance"""
-        x_slider = FloatSlider(description='X', min=0, max=1, value=0.5)
-        y_slider = FloatSlider(description='Y', min=0, max=1, value=0.5)
-        a_slider = FloatSlider(description='Aperture', min=0, max=1, value=0)
-        f_slider = FloatSlider(description='Focus radius', min=0, max=1, value=0.01)
-        d_slider = FloatSlider(description='Focus distance', min=0,
-                               max=10000, value=0, disabled=True)
-        f_button = Button(description='Refresh')
-        f_target = Button(description='Target')
+        x_slider = FloatSlider(description="X", min=0, max=1, value=0.5)
+        y_slider = FloatSlider(description="Y", min=0, max=1, value=0.5)
+        a_slider = FloatSlider(description="Aperture", min=0, max=1, value=0)
+        f_slider = FloatSlider(description="Focus radius", min=0, max=1, value=0.01)
+        d_slider = FloatSlider(
+            description="Focus distance", min=0, max=10000, value=0, disabled=True
+        )
+        f_button = Button(description="Refresh")
+        f_target = Button(description="Target")
 
         class Updated:
             """Class object embedding communication with remote server"""
 
             def __init__(self, client, with_preview):
                 self._client = client
                 self._widget_value = None
@@ -114,17 +276,23 @@
                 self._nb_focus_points = 20
                 self._snapshot = None
                 self._with_preview = with_preview
 
             def _update_camera(self):
                 self._focus_distance = 1e6
                 for _ in range(self._nb_focus_points):
-                    self._focus_distance = min(self._focus_distance, self._get_focal_distance(
-                        (self._x + random.random() * self._focus_radius,
-                         self._y + random.random() * self._focus_radius)))
+                    self._focus_distance = min(
+                        self._focus_distance,
+                        self._get_focal_distance(
+                            (
+                                self._x + random.random() * self._focus_radius,
+                                self._y + random.random() * self._focus_radius,
+                            )
+                        ),
+                    )
 
                 params = self._client.BioExplorerPerspectiveCameraParams()
                 params.focus_distance = self._focus_distance
                 params.aperture_radius = self._aperture
                 params.enable_clipping_planes = True
                 d_slider.value = self._focus_distance
                 self._client.set_camera_params(params)
@@ -138,61 +306,64 @@
 
                 if self._with_preview:
                     self._get_preview(True)
 
             def update_target(self):
                 """Update camera target"""
                 inspection = self._client.inspect([self._x, self._y])
-                if inspection['hit']:
-                    position = inspection['position']
+                if inspection["hit"]:
+                    position = inspection["position"]
                     self._client.set_camera(target=position)
                     self._client.set_renderer()
 
             def update_focus_radius(self, val_dict) -> None:
                 """Update camera focus radius"""
-                self._widget_value = val_dict['new']
+                self._widget_value = val_dict["new"]
                 self._focus_radius = self._widget_value
                 self._update_camera()
 
             def update_aperture(self, val_dict) -> None:
                 """Update camera aperture"""
-                self._widget_value = val_dict['new']
+                self._widget_value = val_dict["new"]
                 self._aperture = self._widget_value
                 self._update_camera()
 
             def update_x(self, val_dict) -> None:
                 """Update camera normalized horizontal focus location"""
-                self._widget_value = val_dict['new']
+                self._widget_value = val_dict["new"]
                 self._x = self._widget_value
                 self._update_camera()
 
             def update_y(self, val_dict) -> None:
                 """Update camera normalized vertical focus location"""
-                self._widget_value = val_dict['new']
+                self._widget_value = val_dict["new"]
                 self._y = self._widget_value
                 self._update_camera()
 
             def _get_focal_distance(self, coordinates=(0.5, 0.5)):
                 """
                 Return the focal distance for the specified normalized coordinates in the image
 
                 :param list coordinates: Coordinates in the image
                 :return: The focal distance
                 :rtype: float
                 """
-                target = self._client.inspect(array=coordinates)['position']
+                target = self._client.inspect(array=coordinates)["position"]
                 origin = self._client.camera.position.data
                 vector = [0, 0, 0]
                 for k in range(3):
                     vector[k] = float(target[k]) - float(origin[k])
                 return math.sqrt(
-                    vector[0] * vector[0] + vector[1] * vector[1] + vector[2] * vector[2])
+                    vector[0] * vector[0]
+                    + vector[1] * vector[1]
+                    + vector[2] * vector[2]
+                )
 
             def _get_preview(self, update_image):
-                viewport = self._client.get_application_parameters()['viewport']
+                viewport = self._client.get_application_parameters()["viewport"]
                 ratio = viewport[1] / viewport[0]
                 size = [256, int(256.0 * ratio)]
                 if update_image:
                     self._snapshot = self._client.image(size=size, samples_per_pixel=4)
 
                 if self._snapshot is None:
                     return
@@ -202,15 +373,15 @@
                 rx = self._focus_radius * size[0]
                 ry = self._focus_radius * size[1]
                 byte_io = io.BytesIO()
                 snapshot = self._snapshot.copy()
                 draw = ImageDraw.Draw(snapshot)
                 draw.ellipse((x - rx, y - ry, x + rx, y + ry))
                 draw.ellipse((x - 5, y - 5, x + 5, y + 5))
-                snapshot.save(byte_io, 'png')
+                snapshot.save(byte_io, "png")
                 preview.width = size[0]
                 preview.height = size[1]
                 preview.value = byte_io.getvalue()
 
         update_class = Updated(self._client, with_preview)
 
         def update_x(value):
@@ -227,194 +398,238 @@
 
         def update_button(_):
             update_class.update()
 
         def update_target(_):
             update_class.update_target()
 
-        x_slider.observe(update_x, 'value')
-        y_slider.observe(update_y, 'value')
-        a_slider.observe(update_aperture, 'value')
-        f_slider.observe(update_focus_radius, 'value')
+        x_slider.observe(update_x, "value")
+        y_slider.observe(update_y, "value")
+        a_slider.observe(update_aperture, "value")
+        f_slider.observe(update_focus_radius, "value")
         f_button.on_click(update_button)
         f_target.on_click(update_target)
 
         position_box = VBox([x_slider, y_slider, f_button, f_target])
         parameters_box = VBox([a_slider, f_slider, d_slider])
-        horizontal_box = HBox([position_box, parameters_box], layout=DEFAULT_GRID_LAYOUT)
+        horizontal_box = HBox(
+            [position_box, parameters_box], layout=DEFAULT_GRID_LAYOUT
+        )
         display(horizontal_box)
 
         if with_preview:
             byte_io = io.BytesIO()
-            preview = Image(value=byte_io.getvalue(), format='png', width=1, height=1)
+            preview = Image(value=byte_io.getvalue(), format="png", width=1, height=1)
             display(preview)
 
     def display_palette_for_models(self):
         """Display visual controls for color palettes applied to models"""
         def set_colormap(model_id, colormap_name, shading_mode):
-            material_ids = self._be.get_material_ids(model_id)['ids']
+            material_ids = self._be.get_material_ids(model_id)["ids"]
             nb_materials = len(material_ids)
 
             palette = sns.color_palette(colormap_name, nb_materials)
             self._be.set_materials_from_palette(
-                model_ids=[model_id], material_ids=material_ids, palette=palette,
-                specular_exponent=specular_exponent_slider.value, shading_mode=shading_mode,
+                model_ids=[model_id],
+                material_ids=material_ids,
+                palette=palette,
+                specular_exponent=specular_exponent_slider.value,
+                shading_mode=shading_mode,
                 opacity=opacity_slider.value,
                 refraction_index=refraction_index_slider.value,
                 reflection_index=reflection_index_slider.value,
                 glossiness=glossiness_slider.value,
                 user_parameter=user_param_slider.value,
                 emission=emission_slider.value,
-                chameleon_mode=chameleon_combobox.index
+                chameleon_mode=chameleon_combobox.index,
             )
             self._client.set_renderer(accumulation=True)
 
         # Models
         model_names = list()
         for model in self._client.scene.models:
-            model_names.append(model['name'])
-        model_combobox = Select(options=model_names, description='Models:', disabled=False)
+            model_names.append(model["name"])
+        model_combobox = Select(
+            options=model_names, description="Models:", disabled=False
+        )
 
         # Shading modes
-        shading_combobox = Select(options=SHADING_MODES, description='Shading:', disabled=False)
+        shading_combobox = Select(
+            options=SHADING_MODES, description="Shading:", disabled=False
+        )
 
         # Colors
-        palette_combobox = Select(options=COLOR_MAPS, description='Palette:', disabled=False)
+        palette_combobox = Select(
+            options=COLOR_MAPS, description="Palette:", disabled=False
+        )
 
         # Chameleon modes
-        chameleon_combobox = Select(options=CHAMELEON_MODES,
-                                    description='Chameleon:', disabled=False)
+        chameleon_combobox = Select(
+            options=CHAMELEON_MODES, description="Chameleon:", disabled=False
+        )
 
         # Events
         def update_materials_from_palette(value):
             """Update materials when palette is modified"""
-            set_colormap(self._client.scene.models[model_combobox.index]['id'], value['new'],
-                         shading_combobox.index)
+            set_colormap(
+                self._client.scene.models[model_combobox.index]["id"],
+                value["new"],
+                shading_combobox.index,
+            )
 
         def update_materials_from_shading_modes(_):
             """Update materials when shading is modified"""
-            set_colormap(self._client.scene.models[model_combobox.index]['id'],
-                         palette_combobox.value, shading_combobox.index)
+            set_colormap(
+                self._client.scene.models[model_combobox.index]["id"],
+                palette_combobox.value,
+                shading_combobox.index,
+            )
 
         def update_materials_from_chameleon_modes(_):
             """Update materials when chameleon mode is modified"""
-            set_colormap(self._client.scene.models[model_combobox.index]['id'],
-                         palette_combobox.value, shading_combobox.index)
+            set_colormap(
+                self._client.scene.models[model_combobox.index]["id"],
+                palette_combobox.value,
+                shading_combobox.index,
+            )
 
-        shading_combobox.observe(update_materials_from_shading_modes, 'value')
-        palette_combobox.observe(update_materials_from_palette, 'value')
-        chameleon_combobox.observe(update_materials_from_chameleon_modes, 'value')
+        shading_combobox.observe(update_materials_from_shading_modes, "value")
+        palette_combobox.observe(update_materials_from_palette, "value")
+        chameleon_combobox.observe(update_materials_from_chameleon_modes, "value")
 
         horizontal_box_list = HBox([model_combobox, shading_combobox, palette_combobox])
 
-        opacity_slider = FloatSlider(description='Opacity', min=0, max=1, value=1)
+        opacity_slider = FloatSlider(description="Opacity", min=0, max=1, value=1)
         opacity_slider.observe(update_materials_from_shading_modes)
-        refraction_index_slider = FloatSlider(description='Refraction', min=1, max=5, value=1)
+        refraction_index_slider = FloatSlider(
+            description="Refraction", min=1, max=5, value=1
+        )
         refraction_index_slider.observe(update_materials_from_shading_modes)
-        reflection_index_slider = FloatSlider(description='Reflection', min=0, max=1, value=0)
+        reflection_index_slider = FloatSlider(
+            description="Reflection", min=0, max=1, value=0
+        )
         reflection_index_slider.observe(update_materials_from_shading_modes)
-        glossiness_slider = FloatSlider(description='Glossiness', min=0, max=1, value=1)
+        glossiness_slider = FloatSlider(description="Glossiness", min=0, max=1, value=1)
         glossiness_slider.observe(update_materials_from_shading_modes)
-        specular_exponent_slider = FloatSlider(description='Specular exponent', min=1, max=100,
-                                               value=1)
+        specular_exponent_slider = FloatSlider(
+            description="Specular exponent", min=1, max=100, value=1
+        )
         specular_exponent_slider.observe(update_materials_from_shading_modes)
-        user_param_slider = FloatSlider(description='User param', min=0, max=100, value=1)
+        user_param_slider = FloatSlider(
+            description="User param", min=0, max=100, value=1
+        )
         user_param_slider.observe(update_materials_from_shading_modes)
-        emission_slider = FloatSlider(description='Emission', min=0, max=100, value=0)
+        emission_slider = FloatSlider(description="Emission", min=0, max=100, value=0)
         emission_slider.observe(update_materials_from_shading_modes)
 
-        cast_simulation_checkbox = Checkbox(description='Simulation', value=False)
+        cast_simulation_checkbox = Checkbox(description="Simulation", value=False)
         cast_simulation_checkbox.observe(update_materials_from_shading_modes)
 
-        horizontal_box_detail1 = HBox([opacity_slider, refraction_index_slider,
-                                       reflection_index_slider])
+        horizontal_box_detail1 = HBox(
+            [opacity_slider, refraction_index_slider, reflection_index_slider]
+        )
         horizontal_box_detail2 = HBox(
-            [glossiness_slider, specular_exponent_slider, user_param_slider])
+            [glossiness_slider, specular_exponent_slider, user_param_slider]
+        )
         horizontal_box_detail3 = HBox(
-            [emission_slider, cast_simulation_checkbox, chameleon_combobox])
-        vertical_box = VBox([horizontal_box_list, horizontal_box_detail1, horizontal_box_detail2,
-                             horizontal_box_detail3], layout=DEFAULT_GRID_LAYOUT)
+            [emission_slider, cast_simulation_checkbox, chameleon_combobox]
+        )
+        vertical_box = VBox(
+            [
+                horizontal_box_list,
+                horizontal_box_detail1,
+                horizontal_box_detail2,
+                horizontal_box_detail3,
+            ],
+            layout=DEFAULT_GRID_LAYOUT,
+        )
         display(vertical_box)
 
     def display_model_visibility(self):
         """Display visual controls for setting visibility of models"""
         model_names = list()
         for model in self._client.scene.models:
-            model_names.append(model['name'])
+            model_names.append(model["name"])
 
         model_select = SelectMultiple(options=model_names, disabled=False)
 
-        lbl_models = Label(value='Models:')
-        show_btn = Button(description='Show')
-        hide_btn = Button(description='Hide')
-        lbl_aabb = Label(value='Bounds:')
-        show_aabb_btn = Button(description='Show')
-        hide_aabb_btn = Button(description='Hide')
-        lbl_camera = Label(value='Camera:')
-        adjust_camera_btn = Button(description='Adjust')
+        lbl_models = Label(value="Models:")
+        show_btn = Button(description="Show")
+        hide_btn = Button(description="Hide")
+        lbl_aabb = Label(value="Bounds:")
+        show_aabb_btn = Button(description="Show")
+        hide_aabb_btn = Button(description="Hide")
+        lbl_camera = Label(value="Camera:")
+        adjust_camera_btn = Button(description="Adjust")
         vbox_visible = VBox([lbl_models, show_btn, hide_btn])
         vbox_aabb = VBox([lbl_aabb, show_aabb_btn, hide_aabb_btn])
         vbox_camera = VBox([lbl_camera, adjust_camera_btn])
         hbox_params = HBox([vbox_visible, vbox_aabb, vbox_camera])
 
         def update_models(visible):
             for model_id in model_select.index:
                 self._client.update_model(
-                    id=self._client.scene.models[model_id]['id'],
-                    visible=visible)
+                    id=self._client.scene.models[model_id]["id"], visible=visible
+                )
 
         def show_models(event):
             update_models(True)
 
         def hide_models(event):
             update_models(False)
 
         def update_aabbs(visible):
             for model_id in model_select.index:
                 self._client.update_model(
-                    id=self._client.scene.models[model_id]['id'],
-                    bounding_box=visible)
+                    id=self._client.scene.models[model_id]["id"], bounding_box=visible
+                )
 
         def show_aabbs(event):
             update_aabbs(True)
 
         def hide_aabbs(event):
             update_aabbs(False)
 
         def adjust_camera(event):
             size_min_aabb = [1e6, 1e6, 1e6]
             size_max_aabb = [-1e6, -1e6, -1e6]
             for model_id in model_select.index:
                 model = self._client.scene.models[model_id]
-                bounds = model['bounds']
-                min_aabb = bounds['min']
-                max_aabb = bounds['max']
+                bounds = model["bounds"]
+                min_aabb = bounds["min"]
+                max_aabb = bounds["max"]
                 half_size_aabb = [0, 0, 0]
                 center = [0, 0, 0]
                 for k in range(3):
                     half_size_aabb[k] = (max_aabb[k] - min_aabb[k]) / 2.0
                     center[k] = center[k] + (min_aabb[k] + max_aabb[k]) / 2.0
 
                 for k in range(3):
-                    size_min_aabb[k] = min(size_min_aabb[k], center[k] - half_size_aabb[k])
-                    size_max_aabb[k] = max(size_max_aabb[k], center[k] + half_size_aabb[k])
+                    size_min_aabb[k] = min(
+                        size_min_aabb[k], center[k] - half_size_aabb[k]
+                    )
+                    size_max_aabb[k] = max(
+                        size_max_aabb[k], center[k] + half_size_aabb[k]
+                    )
 
             center_aabb = [0, 0, 0]
             diag = 0
             for k in range(3):
                 diag = max(diag, size_max_aabb[k] - size_min_aabb[k])
                 center_aabb[k] = (size_max_aabb[k] + size_min_aabb[k]) / 2.0
 
             origin = [0, 0, 0]
             for k in range(3):
                 origin[k] = center_aabb[k]
                 if k == 2:
                     origin[k] = origin[k] + diag * 1.5
 
-            self._client.set_camera(position=origin, orientation=[0, 0, 0, 1], target=center_aabb)
+            self._client.set_camera(
+                position=origin, orientation=[0, 0, 0, 1], target=center_aabb
+            )
             # Refresh UI
             self._client.set_renderer()
 
         show_btn.on_click(show_models)
         hide_btn.on_click(hide_models)
         show_aabb_btn.on_click(show_aabbs)
         hide_aabb_btn.on_click(hide_aabbs)
@@ -422,69 +637,65 @@
 
         hbox = HBox([model_select, hbox_params], layout=DEFAULT_GRID_LAYOUT)
         display(hbox)
 
     def display_model_focus(self, max_number_of_instances=1e6):
         """Display visual controls for setting visibility of models"""
         directions = dict()
-        directions['front'] = Vector3(0, 0, -1)
-        directions['back'] = Vector3(0, 0, 1)
-        directions['top'] = Vector3(0, -1, 0)
-        directions['bottom'] = Vector3(0, 1, 0)
-        directions['right'] = Vector3(-1, 0, 0)
-        directions['left'] = Vector3(1, 0, 0)
+        directions["front"] = Vector3(0, 0, -1)
+        directions["back"] = Vector3(0, 0, 1)
+        directions["top"] = Vector3(0, -1, 0)
+        directions["bottom"] = Vector3(0, 1, 0)
+        directions["right"] = Vector3(-1, 0, 0)
+        directions["left"] = Vector3(1, 0, 0)
 
         # Model names and ids
         model_names = list()
-        model_ids = self._be.get_model_ids()['ids']
+        model_ids = self._be.get_model_ids()["ids"]
         for model_id in model_ids:
-            model_name = self._be.get_model_name(model_id)['name']
+            model_name = self._be.get_model_name(model_id)["name"]
             if self._be.NAME_MEMBRANE not in model_name:
                 model_names.append([model_name, model_id])
-        model_select = Select(
-            description='Model',
-            options=model_names)
+        model_select = Select(description="Model", options=model_names)
 
         # Instance Ids
-        instance_select = Select(
-            description='Instance',
-            options=list())
+        instance_select = Select(description="Instance", options=list())
 
         # Directions
-        direction_select = Select(
-            description='Direction',
-            options=directions)
+        direction_select = Select(description="Direction", options=directions)
 
         # Distance to instance
         distance_slider = FloatSlider(
-            description='Distance', value=25.0, min=-1e3, max=1e3)
+            description="Distance", value=25.0, min=-1e3, max=1e3
+        )
 
         # Focus button
-        focus_btn = Button(description='Focus')
+        focus_btn = Button(description="Focus")
         hbox_1 = HBox([model_select, instance_select, direction_select])
         hbox_2 = HBox([distance_slider, focus_btn])
         vbox = VBox([hbox_1, hbox_2])
 
         def update_instances(value):
             model_id = int(model_select.options[model_select.index][1])
-            ids = self._be.get_model_instances(model_id, max_number_of_instances)['ids']
+            ids = self._be.get_model_instances(model_id, max_number_of_instances)["ids"]
             instance_select.options = ids
 
         def focus_on_instance(event):
             model_id = int(model_select.options[model_select.index][1])
             instance_id = int(instance_select.options[instance_select.index])
             self._be.set_focus_on(
-                model_id=model_id, instance_id=instance_id,
+                model_id=model_id,
+                instance_id=instance_id,
                 distance=distance_slider.value,
                 direction=direction_select.value,
-                max_number_of_instances=max_number_of_instances
+                max_number_of_instances=max_number_of_instances,
             )
             self._client.set_renderer()
 
-        model_select.observe(update_instances, 'value')
+        model_select.observe(update_instances, "value")
         focus_btn.on_click(focus_on_instance)
         update_instances(0)
 
         display(vbox)
 
     def __display_advanced_settings(self, object_type, threaded):
         """Display visual controls for camera or renderer advanced settings"""
@@ -493,20 +704,20 @@
 
             def __init__(self, client, object_type):
                 self._object_type = object_type
                 self._widgets_list = dict()
                 self._native_params = None
                 self._client = client
                 class_name = None
-                if self._object_type == 'camera':
-                    class_name = pascalcase(self._client.get_camera()['current'])
-                    class_name += 'CameraParams'
-                elif self._object_type == 'renderer':
-                    class_name = pascalcase(self._client.get_renderer()['current'])
-                    class_name += 'RendererParams'
+                if self._object_type == "camera":
+                    class_name = pascalcase(self._client.get_camera()["current"])
+                    class_name += "CameraParams"
+                elif self._object_type == "renderer":
+                    class_name = pascalcase(self._client.get_renderer()["current"])
+                    class_name += "RendererParams"
 
                 # Read params from Brayns
                 self._native_params = self._get_params()
 
                 # Read params from class definition
                 class_ = getattr(self._client, class_name)
                 self._param_descriptors = class_()
@@ -531,181 +742,227 @@
                     params = self._get_params()
                     for widget in self._widgets_list:
                         self._widgets_list[widget].value = params[widget]
                     time.sleep(1)
 
             def _get_params(self):
                 """Gets camera or renderer settings from remote server"""
-                if self._object_type == 'camera':
+                if self._object_type == "camera":
                     return self._client.get_camera_params()
-                if self._object_type == 'renderer':
+                if self._object_type == "renderer":
                     return self._client.get_renderer_params()
                 return None
 
             def _update_params(self, _):
                 """Update remote camera or renderer params"""
                 for widget in self._widgets_list:
                     setattr(self._params, widget, self._widgets_list[widget].value)
 
-                if self._object_type == 'camera':
+                if self._object_type == "camera":
                     self._client.set_camera_params(self._params)
-                if self._object_type == 'renderer':
+                if self._object_type == "renderer":
                     self._client.set_renderer_params(self._params)
 
-            @ staticmethod
+            @staticmethod
             def _get_value(props, key, default_value):
                 """Return value of a property"""
                 try:
                     return props[key]
                 except KeyError as _:
                     return default_value
 
             def _create_widgets(self):
                 """Create widget in the current visual control"""
                 for param in self._param_descriptors:
                     value = self._native_params[param]
                     parameter = self._param_descriptors[param]
-                    props = parameter.__propinfo__['__literal__']
-                    description = props['title']
+                    props = parameter.__propinfo__["__literal__"]
+                    description = props["title"]
 
                     if isinstance(value, float):
-                        minimum = self._get_value(props, 'minimum', 0)
-                        maximum = self._get_value(props, 'maximum', 1e4)
+                        minimum = self._get_value(props, "minimum", 0)
+                        maximum = self._get_value(props, "maximum", 1e4)
                         float_slider = FloatSlider(
-                            description=description, min=minimum, max=maximum, value=value,
-                            STYLE=STYLE, layout=DEFAULT_LAYOUT)
-                        float_slider.observe(self._update_params, 'value')
+                            description=description,
+                            min=minimum,
+                            max=maximum,
+                            value=value,
+                            STYLE=STYLE,
+                            layout=DEFAULT_LAYOUT,
+                        )
+                        float_slider.observe(self._update_params, "value")
                         self._widgets_list[param] = float_slider
                     if isinstance(value, int):
-                        minimum = self._get_value(props, 'minimum', 0)
-                        maximum = self._get_value(props, 'maximum', 1e4)
+                        minimum = self._get_value(props, "minimum", 0)
+                        maximum = self._get_value(props, "maximum", 1e4)
                         int_slider = IntSlider(
-                            description=description, min=minimum, max=maximum, value=value,
-                            STYLE=STYLE, layout=DEFAULT_LAYOUT)
-                        int_slider.observe(self._update_params, 'value')
+                            description=description,
+                            min=minimum,
+                            max=maximum,
+                            value=value,
+                            STYLE=STYLE,
+                            layout=DEFAULT_LAYOUT,
+                        )
+                        int_slider.observe(self._update_params, "value")
                         self._widgets_list[param] = int_slider
                     if isinstance(value, bool):
                         check_box = Checkbox(
-                            description=description, value=bool(value), STYLE=STYLE,
-                            layout=DEFAULT_LAYOUT)
-                        check_box.observe(self._update_params, 'value')
+                            description=description,
+                            value=bool(value),
+                            STYLE=STYLE,
+                            layout=DEFAULT_LAYOUT,
+                        )
+                        check_box.observe(self._update_params, "value")
                         self._widgets_list[param] = check_box
                     if isinstance(value, str):
-                        text_box = Text(description=description, value=value, STYLE=STYLE,
-                                        layout=DEFAULT_LAYOUT)
-                        text_box.observe(self._update_params, 'value')
+                        text_box = Text(
+                            description=description,
+                            value=value,
+                            STYLE=STYLE,
+                            layout=DEFAULT_LAYOUT,
+                        )
+                        text_box.observe(self._update_params, "value")
                         self._widgets_list[param] = text_box
 
         update_class = Updated(self._client, object_type)
         if threaded:
             the_thread = threading.Thread(target=update_class.thread_run)
             the_thread.start()
 
         widgets_list = update_class.get_widgets()
         vboxes = list()
         nb_widgets = len(widgets_list)
         nb_columns = 2
         for i in range(0, nb_widgets, nb_columns):
             box_widgets = list()
 
-            for widget in list(widgets_list)[i:min(i + nb_columns, nb_widgets)]:
+            for widget in list(widgets_list)[i: min(i + nb_columns, nb_widgets)]:
                 box_widgets.append(widgets_list[widget])
 
             vboxes.append(HBox(box_widgets))
 
         hbox = VBox(vboxes, layout=DEFAULT_GRID_LAYOUT)
         display(hbox)
 
     def display_advanced_rendering_settings(self, is_threaded=True):
         """Display visual controls for renderer advanced settings"""
-        self.__display_advanced_settings('renderer', is_threaded)
+        self.__display_advanced_settings("renderer", is_threaded)
 
     def display_advanced_camera_settings(self, is_threaded=True):
         """Display visual controls for camera advanced settings"""
-        self.__display_advanced_settings('camera', is_threaded)
+        self.__display_advanced_settings("camera", is_threaded)
 
     def display_rendering_settings(self):
         """Display visual controls for renderer settings"""
         def update_params(_):
             """Update renderer params"""
             self._client.set_renderer(
                 accumulation=checkbox_accumulation.value,
                 background_color=matplotlib.colors.to_rgb(colorpicker_background.value),
                 head_light=checkbox_head_light.value,
                 samples_per_pixel=slider_samples_per_pixel.value,
                 max_accum_frames=slider_max_accum_frames.value,
-                subsampling=slider_sub_sampling.value
+                subsampling=slider_sub_sampling.value,
             )
 
         params = self._client.get_renderer()
-        slider_samples_per_pixel = IntSlider(description='Samples per pixel', min=1, max=1024,
-                                             value=params['samples_per_pixel'])
+        slider_samples_per_pixel = IntSlider(
+            description="Samples per pixel",
+            min=1,
+            max=1024,
+            value=params["samples_per_pixel"],
+        )
         slider_samples_per_pixel.observe(update_params)
-        slider_max_accum_frames = IntSlider(description='Max accumulation frames', min=1, max=1024,
-                                            value=params['max_accum_frames'])
-        slider_max_accum_frames.observe(update_params, 'value')
-        slider_sub_sampling = IntSlider(description='Sub-sampling', min=1, max=16,
-                                        value=params['subsampling'])
-        slider_sub_sampling.observe(update_params, 'value')
-        colorpicker_background = ColorPicker(description='Background color',
-                                             value=matplotlib.colors.to_hex(
-                                                 params['background_color']))
-        colorpicker_background.observe(update_params, 'value')
-        checkbox_head_light = Checkbox(description='Head light', value=params['head_light'])
-        checkbox_head_light.observe(update_params, 'value')
-        checkbox_accumulation = Checkbox(description='Accumulation', value=params['accumulation'])
-        checkbox_accumulation.observe(update_params, 'value')
-        hbox_1 = HBox([slider_samples_per_pixel, slider_sub_sampling, slider_max_accum_frames])
-        hbox_2 = HBox([colorpicker_background, checkbox_head_light, checkbox_accumulation])
+        slider_max_accum_frames = IntSlider(
+            description="Max accumulation frames",
+            min=1,
+            max=1024,
+            value=params["max_accum_frames"],
+        )
+        slider_max_accum_frames.observe(update_params, "value")
+        slider_sub_sampling = IntSlider(
+            description="Sub-sampling", min=1, max=16, value=params["subsampling"]
+        )
+        slider_sub_sampling.observe(update_params, "value")
+        colorpicker_background = ColorPicker(
+            description="Background color",
+            value=matplotlib.colors.to_hex(params["background_color"]),
+        )
+        colorpicker_background.observe(update_params, "value")
+        checkbox_head_light = Checkbox(
+            description="Head light", value=params["head_light"]
+        )
+        checkbox_head_light.observe(update_params, "value")
+        checkbox_accumulation = Checkbox(
+            description="Accumulation", value=params["accumulation"]
+        )
+        checkbox_accumulation.observe(update_params, "value")
+        hbox_1 = HBox(
+            [slider_samples_per_pixel, slider_sub_sampling, slider_max_accum_frames]
+        )
+        hbox_2 = HBox(
+            [colorpicker_background, checkbox_head_light, checkbox_accumulation]
+        )
         display(VBox([hbox_1, hbox_2], layout=DEFAULT_GRID_LAYOUT))
 
     def display_environment_maps(self, folder):
         """Display visual controls for setting environment map"""
-        supported_extensions = ['jpg', 'jpeg', 'png']
+        supported_extensions = ["jpg", "jpeg", "png"]
         hdri_files = list()
         for extension in supported_extensions:
-            hdri_files = hdri_files + glob.glob(folder + '/*.' + extension)
+            hdri_files = hdri_files + glob.glob(folder + "/*." + extension)
         hdri_files.sort()
         base_names = list()
         for hdri_file in hdri_files:
             base_names.append(os.path.basename(hdri_file))
 
         def update_envmap(value):
-            filename = folder + '/' + value['new']
+            filename = folder + "/" + value["new"]
             self._client.set_environment_map(filename)
 
-        cb_names = Select(description='Maps', options=base_names)
-        cb_names.observe(update_envmap, 'value')
+        cb_names = Select(description="Maps", options=base_names)
+        cb_names.observe(update_envmap, "value")
         display(cb_names)
 
-    def show_amino_acid_on_protein(self, assembly_name, name, sequence_id=0, palette_name='Set1',
-                                   palette_size=2):
+    def show_amino_acid_on_protein(
+        self, assembly_name, name, sequence_id=0, palette_name="Set1", palette_size=2
+    ):
         """
         Display visual controls for showing amino acid sequence on a protein of the scene
 
         :param: assembly_name: Name of the assembly containing the protein
         :param: name: Name of the protein
         :param: sequence_id: ID of the protein sequence
         :param: palette_name: Name of the color palette
         :param: palette_size: Size of the color palette
         """
         sequences = self._be.get_protein_amino_acid_sequences(assembly_name, name)
         if sequence_id >= len(sequences):
-            raise RuntimeError('Invalid sequence Id')
-        sequence_as_list = sequences[0].split(',')
+            raise RuntimeError("Invalid sequence Id")
+        sequence_as_list = sequences[0].split(",")
 
         value_range = [int(sequence_as_list[0]), int(sequence_as_list[1])]
-        irs = IntRangeSlider(value=[value_range[0], value_range[1]],
-                             min=value_range[0], max=value_range[1])
+        irs = IntRangeSlider(
+            value=[value_range[0], value_range[1]],
+            min=value_range[0],
+            max=value_range[1],
+        )
         lbl = Label(value="AA sequence")
 
         def update_slider(value):
-            self._be.set_protein_amino_acid_sequence_as_range(assembly_name, name, value['new'])
+            self._be.set_protein_amino_acid_sequence_as_range(
+                assembly_name, name, value["new"]
+            )
             self._be.set_protein_color_scheme(
-                assembly_name, name, self._be.COLOR_SCHEME_AMINO_ACID_SEQUENCE, palette_name,
-                palette_size)
-            lbl.value = sequence_as_list[2][value['new'][0] -
-                                            value_range[0]:value['new'][1] - value_range[0]]
+                assembly_name,
+                name,
+                self._be.COLOR_SCHEME_AMINO_ACID_SEQUENCE,
+                palette_name,
+                palette_size,
+            )
+            lbl.value = sequence_as_list[2][
+                value["new"][0] - value_range[0]: value["new"][1] - value_range[0]
+            ]
 
-        irs.observe(update_slider, 'value')
+        irs.observe(update_slider, "value")
         display(irs)
         display(lbl)
```

### Comparing `bioexplorer-1.4.0/bioexplorer/transfer_function.py` & `bioexplorer-1.5.0/bioexplorer/transfer_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Provides a transfer function widget"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -31,17 +31,25 @@
 # pylint: disable=too-many-arguments
 # pylint: disable=unused-argument
 
 
 class TransferFunction:
     """Transfer function widget"""
 
-    def __init__(self, bioexplorer, model_id, filename=None, name='rainbow',
-                 size=32, alpha=0.0, value_range=[0, 255],
-                 continuous_update=False):
+    def __init__(
+        self,
+        bioexplorer,
+        model_id,
+        filename=None,
+        name="rainbow",
+        size=32,
+        alpha=0.0,
+        value_range=[0, 255],
+        continuous_update=False,
+    ):
         """
         Initialize the TransferFunction object
 
         :bioexplorer: BioExplorer client
         :filename: Optional full file name of the transfer function
         :name: Name of the color palette
         :size: Number of control points
@@ -79,15 +87,15 @@
         :filename: Full file name of the transfer function
         """
         # Clear controls
         self._alpha_sliders.clear()
         self._color_pickers.clear()
 
         # Read colormap file
-        lines = tuple(open(filename, 'r'))
+        lines = tuple(open(filename, "r"))
         self._palette.clear()
         for line in lines:
             words = line.split()
             if len(words) == 4:
                 r = float(words[0])
                 g = float(words[1])
                 b = float(words[2])
@@ -97,19 +105,27 @@
 
     def save(self, filename):
         """
         Save transfer function to file
 
         :filename: Full file name of the transfer function
         """
-        with open(filename, 'w') as f:
-            f.write(str(len(self._palette)) + '\n')
+        with open(filename, "w") as f:
+            f.write(str(len(self._palette)) + "\n")
             for color in self._palette:
-                f.write(str(color[0]) + ' ' + str(color[1]) + ' ' + str(color[2]) + ' ' +
-                        str(color[3]) + '\n')
+                f.write(
+                    str(color[0])
+                    + " "
+                    + str(color[1])
+                    + " "
+                    + str(color[2])
+                    + " "
+                    + str(color[3])
+                    + "\n"
+                )
             f.close()
 
     def set_palette(self, name):
         """
         Set the Seaborn color palette of the transfer function
 
         :name: Name of the Seaborn color palette
@@ -134,18 +150,17 @@
     def _html_color(self, index):
         """
         Get HTML color from palette
 
         :index: Index of color in the Seaborn color palette
         """
         color = self._palette[index]
-        color_as_string = '#' \
-                          '%02x' % (int)(color[0] * 255) + \
-                          '%02x' % (int)(color[1] * 255) + \
-                          '%02x' % (int)(color[2] * 255)
+        color_as_string = "#" "%02x" % (int)(color[0] * 255) + "%02x" % (int)(
+            color[1] * 255
+        ) + "%02x" % (int)(color[2] * 255)
         return color_as_string
 
     def _update_colormap(self, change):
         """
         Update color map
 
         :change: Unused
@@ -163,45 +178,51 @@
         self._callback()
 
     def _create_controls(self):
         """Create widget controls"""
         self.send_updates_to_renderer = False
         # Layout
         alpha_slider_item_layout = Layout(
-            overflow_x='hidden', height='180px', max_width='20px')
+            overflow_x="hidden", height="180px", max_width="20px"
+        )
         color_picker_item_layout = Layout(
-            overflow_x='hidden', height='20px', max_width='20px')
-        box_layout = Layout(display='inline-flex')
+            overflow_x="hidden", height="20px", max_width="20px"
+        )
+        box_layout = Layout(display="inline-flex")
 
         # Sliders
-        self._alpha_sliders = [widgets.IntSlider(
-            continuous_update=self._continuous_update,
-            layout=alpha_slider_item_layout,
-            description=str(i),
-            orientation='vertical',
-            readout=True,
-            value=self._palette[i][3] * 256, min=0, max=255, step=1
-        ) for i in range(len(self._palette))]
+        self._alpha_sliders = [
+            widgets.IntSlider(
+                continuous_update=self._continuous_update,
+                layout=alpha_slider_item_layout,
+                description=str(i),
+                orientation="vertical",
+                readout=True,
+                value=self._palette[i][3] * 256,
+                min=0,
+                max=255,
+                step=1,
+            )
+            for i in range(len(self._palette))
+        ]
 
         # Color pickers
         self._color_pickers = [
-            ColorPicker(
-                layout=color_picker_item_layout,
-                concise=True,
-                disabled=False) for i in range(len(self._palette))
+            ColorPicker(layout=color_picker_item_layout, concise=True, disabled=False)
+            for i in range(len(self._palette))
         ]
         # Display controls
         color_box = Box(children=self._color_pickers)
         alpha_box = Box(children=self._alpha_sliders)
         box = VBox([color_box, alpha_box], layout=box_layout)
 
         # Attach observers
         for i in range(len(self._palette)):
-            self._alpha_sliders[i].observe(self._update_colormap, names='value')
-            self._color_pickers[i].observe(self._update_colorpicker, names='value')
+            self._alpha_sliders[i].observe(self._update_colormap, names="value")
+            self._color_pickers[i].observe(self._update_colorpicker, names="value")
         display(box)
         self._send_updates_to_renderer = True
 
     def _update_controls(self):
         """Udpate widget controls"""
         self._send_updates_to_renderer = False
         for i in range(len(self._palette)):
@@ -221,40 +242,43 @@
             except ValueError:
                 color = hex_to_rgb(self._color_pickers[i].value)
 
             c = [
                 float(color.red) / 255.0,
                 float(color.green) / 255.0,
                 float(color.blue) / 255.0,
-                float(self._alpha_sliders[i].value) / 255.0
+                float(self._alpha_sliders[i].value) / 255.0,
             ]
             self._palette[i] = c
         self._update_palette()
 
     @staticmethod
     def _hex_to_rgb(value):
         """Concert hex value into RGB values"""
-        value = value.lstrip('#')
+        value = value.lstrip("#")
         lv = len(value)
-        return tuple(int(value[i:i + lv // 3], 16) for i in range(0, lv, lv // 3))
+        return tuple(int(value[i: i + lv // 3], 16) for i in range(0, lv, lv // 3))
 
     def _update_palette(self):
         """Update color palette"""
         intensity = 1
         btf = self._core.get_model_transfer_function(id=self._model_id)
         colors = list()
         points = list()
         nb_points = len(self._alpha_sliders)
         step = 1.0 / float(nb_points - 1)
         for i in range(nb_points):
             color = self._hex_to_rgb(self._color_pickers[i].value)
-            colors.append([
-                intensity * float(color[0]) / 256.0,
-                intensity * float(color[1]) / 256.0,
-                intensity * float(color[2]) / 256.0])
+            colors.append(
+                [
+                    intensity * float(color[0]) / 256.0,
+                    intensity * float(color[1]) / 256.0,
+                    intensity * float(color[2]) / 256.0,
+                ]
+            )
             points.append([i * step, self._alpha_sliders[i].value / 255.0])
 
-        btf['colormap']['name'] = 'TransferFunctionEditor'
-        btf['colormap']['colors'] = colors
-        btf['opacity_curve'] = points
-        btf['range'] = [self._value_range[0], self._value_range[1]]
+        btf["colormap"]["name"] = "TransferFunctionEditor"
+        btf["colormap"]["colors"] = colors
+        btf["opacity_curve"] = points
+        btf["range"] = [self._value_range[0], self._value_range[1]]
         self._core.set_model_transfer_function(id=self._model_id, transfer_function=btf)
```

### Comparing `bioexplorer-1.4.0/bioexplorer/version.py` & `bioexplorer-1.5.0/bioexplorer/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 """The version of the bioexplorer package"""
 
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
 
-VERSION = '1.4.0'
+VERSION = "1.5.0"
```

### Comparing `bioexplorer-1.4.0/bioexplorer.egg-info/PKG-INFO` & `bioexplorer-1.5.0/bioexplorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioexplorer
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python API for the Blue Brain BioExplorer
 Home-page: https://github.com/BlueBrain/BioExplorer.git
 Author: Blue Brain Project, EPFL
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Project-URL: Documentation, https://bluebrain.github.io/BioExplorer/
 Project-URL: Source, https://github.com/BlueBrain/BioExplorer
```

### Comparing `bioexplorer-1.4.0/requirements.txt` & `bioexplorer-1.5.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 # All rights reserved. Do not distribute without further notice.
 
 
+rockets~=1.0.3
+requests~=2.22.0
+python-jsonschema-objects~=0.4.1
+semver~=2.8.1
 stringcase~=1.2.0
 pyquaternion~=0.9.9
 webcolors~=1.8.1
-seaborn~=0.11.1
-ipywidgets~=7.6.3
-jsonschema~=3.2.0
+seaborn~=0.12.2
+ipywidgets~=8.0.4
+jsonschema~=4.17.3
 sqlalchemy~=1.4.31
-tqdm~=4.62.0
 psycopg2-binary~=2.9.2
+tqdm~=4.62.0
```

### Comparing `bioexplorer-1.4.0/requirements_dev.txt` & `bioexplorer-1.5.0/requirements_dev.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,32 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 # All rights reserved. Do not distribute without further notice.
 
 
+rockets~=1.0.3
+requests~=2.22.0
+python-jsonschema-objects~=0.4.1
+semver~=2.8.1
 setuptools~=46.0.0
 stringcase~=1.2.0
 pygments~=2.4.1
 pylint~=2.6.0
 pycodestyle~=2.7.0
 pydocstyle~=3.0.0
 nose~=1.3.7
-coverage~=4.5.2
+coverage~=7.1.0
 nosexcover~=1.0.11
 tox~=3.6.1
 mock~=2.0.0
 sphinx==1.8.3
 sphinx_rtd_theme==0.4.2
 nbsphinx==0.8.3
 m2r~=0.2.1
 pyquaternion~=0.9.9
 webcolors~=1.8.1
-seaborn~=0.11.1
-ipywidgets~=7.6.3
-tqdm~=4.62.0
+seaborn~=0.12.2
+ipywidgets~=8.0.4
 psycopg2-binary~=2.9.2
+tqdm~=4.62.0
```

### Comparing `bioexplorer-1.4.0/setup.cfg` & `bioexplorer-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.4.0
+version = 1.5.0
 name = bioexplorer
 summary = Blue Brain BioExplorer python API
 long_description = file: README.md
 long_description_content_type = text/markdown
 home-page = https://github.com/BlueBrain/BioExplorer
 author = Cyrille Favreau
 author-email = bbp-open-source@googlegroups.com
```

### Comparing `bioexplorer-1.4.0/setup.py` & `bioexplorer-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # The Blue Brain BioExplorer is a tool for scientists to extract and analyse
 # scientific data from visualization
 #
-# Copyright 2020-2022 Blue BrainProject / EPFL
+# Copyright 2020-2023 Blue BrainProject / EPFL
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

