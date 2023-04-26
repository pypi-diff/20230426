# Comparing `tmp/slot_machine_serializers-0.2.2.tar.gz` & `tmp/slot_machine_serializers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slot_machine_serializers-0.2.2.tar", last modified: Tue Apr 25 09:38:29 2023, max compression
+gzip compressed data, was "slot_machine_serializers-0.3.0.tar", last modified: Wed Apr 26 12:07:26 2023, max compression
```

## Comparing `slot_machine_serializers-0.2.2.tar` & `slot_machine_serializers-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 09:38:29.929191 slot_machine_serializers-0.2.2/
--rw-r--r--   0 ochsner    (502) staff       (20)     1918 2023-04-25 09:38:29.929256 slot_machine_serializers-0.2.2/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)     1660 2023-04-25 08:58:48.000000 slot_machine_serializers-0.2.2/README.md
--rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.2.2/pyproject.toml
--rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-25 09:38:29.929543 slot_machine_serializers-0.2.2/setup.cfg
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 09:38:29.927322 slot_machine_serializers-0.2.2/slot_machine/
--rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.2.2/slot_machine/__init__.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2763 2023-04-25 08:52:11.000000 slot_machine_serializers-0.2.2/slot_machine/samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     4085 2023-04-25 09:36:49.000000 slot_machine_serializers-0.2.2/slot_machine/serializers.py
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 09:38:29.928463 slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/
--rw-r--r--   0 ochsner    (502) staff       (20)     1918 2023-04-25 09:38:29.000000 slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-25 09:38:29.000000 slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/SOURCES.txt
--rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-25 09:38:29.000000 slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/dependency_links.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-25 09:38:29.000000 slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/requires.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-25 09:38:29.000000 slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/top_level.txt
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 09:38:29.928912 slot_machine_serializers-0.2.2/tests/
--rw-r--r--   0 ochsner    (502) staff       (20)      599 2023-04-25 08:51:02.000000 slot_machine_serializers-0.2.2/tests/test_samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.2.2/tests/test_serializers.py
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.361143 slot_machine_serializers-0.3.0/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1912 2023-04-26 12:07:26.361224 slot_machine_serializers-0.3.0/PKG-INFO
+-rw-r--r--   0 ochsner    (502) staff       (20)     1654 2023-04-26 11:52:54.000000 slot_machine_serializers-0.3.0/README.md
+-rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.3.0/pyproject.toml
+-rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-26 12:07:26.361548 slot_machine_serializers-0.3.0/setup.cfg
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.359373 slot_machine_serializers-0.3.0/slot_machine/
+-rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.3.0/slot_machine/__init__.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     3167 2023-04-26 12:04:52.000000 slot_machine_serializers-0.3.0/slot_machine/samplers.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     4085 2023-04-26 11:53:00.000000 slot_machine_serializers-0.3.0/slot_machine/serializers.py
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.360335 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1912 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/PKG-INFO
+-rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/SOURCES.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/dependency_links.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/requires.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/top_level.txt
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.360831 slot_machine_serializers-0.3.0/tests/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1869 2023-04-26 12:03:58.000000 slot_machine_serializers-0.3.0/tests/test_samplers.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.3.0/tests/test_serializers.py
```

### Comparing `slot_machine_serializers-0.2.2/PKG-INFO` & `slot_machine_serializers-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot_machine_serializers
-Version: 0.2.2
+Version: 0.3.0
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
@@ -28,16 +28,16 @@
 With `slot_machine` your next choice will be one you look forward to.
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
-chicken_nuggets: !RangeSampler 5..20
-price: !UniformSampler 9..99..20
+chicken_nuggets: !SampleRange 5..20
+price: !SampleUniform 9..99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
@@ -45,16 +45,16 @@
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     price: float
 
 yaml_file = """
 basket:
-  chicken_nuggets: !RangeSampler 5..10
-  price: !UniformSampler 9.99..20
+  chicken_nuggets: !SampleRange 5..10
+  price: !SampleUniform 9.99..20
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
 
 ### Build your own
 
@@ -63,25 +63,25 @@
 from slot_machine import SlotsSerializer, MappingSampler
 
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     splits: list[int]
 
-class SplitsSampler(MappingSampler):
+class SampleSplits(MappingSampler):
 
   @classmethod
   def get_sample(cls, n_splits: str, values: str):
     n_splits = int(n_splits)
     values = list(map(int, values.split("..")))
     return sorted([random.randint(*values) for _ in range(n_splits)])
     
 yaml_file = """
 basket:
   chicken_nuggets: 100
-  splits: !SplitsSampler
+  splits: !SampleSplits
     n_splits: 3
     values: 0..100
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
```

### Comparing `slot_machine_serializers-0.2.2/README.md` & `slot_machine_serializers-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 With `slot_machine` your next choice will be one you look forward to.
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
-chicken_nuggets: !RangeSampler 5..20
-price: !UniformSampler 9..99..20
+chicken_nuggets: !SampleRange 5..20
+price: !SampleUniform 9..99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
@@ -36,16 +36,16 @@
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     price: float
 
 yaml_file = """
 basket:
-  chicken_nuggets: !RangeSampler 5..10
-  price: !UniformSampler 9.99..20
+  chicken_nuggets: !SampleRange 5..10
+  price: !SampleUniform 9.99..20
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
 
 ### Build your own
 
@@ -54,25 +54,25 @@
 from slot_machine import SlotsSerializer, MappingSampler
 
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     splits: list[int]
 
-class SplitsSampler(MappingSampler):
+class SampleSplits(MappingSampler):
 
   @classmethod
   def get_sample(cls, n_splits: str, values: str):
     n_splits = int(n_splits)
     values = list(map(int, values.split("..")))
     return sorted([random.randint(*values) for _ in range(n_splits)])
     
 yaml_file = """
 basket:
   chicken_nuggets: 100
-  splits: !SplitsSampler
+  splits: !SampleSplits
     n_splits: 3
     values: 0..100
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
```

### Comparing `slot_machine_serializers-0.2.2/setup.cfg` & `slot_machine_serializers-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slot_machine_serializers
-version = 0.2.2
+version = 0.3.0
 description = Ordered dataclass serializer mixin for sloted dataclasses
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 url = https://github.com/sirno/slot_machine
 license = MIT
 python_requires = ">=3.10"
```

### Comparing `slot_machine_serializers-0.2.2/slot_machine/samplers.py` & `slot_machine_serializers-0.3.0/slot_machine/samplers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 """Sampler classes."""
 
 from __future__ import annotations
 
 __all__ = [
     "Sampler",
+    # Sampler types
     "ScalarSampler",
     "MappingSampler",
-    "UniformSampler",
-    "IntegerSampler",
-    "RangeSampler",
-    "NormalSampler",
+    "SequenceSampler",
+    # Scalar Samplers
+    "SampleUniform",
+    "SampleRange",
+    # Sequence Samplers
+    "Choose",
+    "ChooseInteger",
+    "ChooseFloat",
+    # Mapping Samplers
+    "SampleNormal",
 ]
 
 from abc import ABC, abstractclassmethod
 
 import random
 import yaml
 
@@ -53,64 +60,73 @@
 
     @classmethod
     def _construct_yaml(cls, loader: yaml.Loader, node: yaml.nodes.Node) -> Self:
         mapping = loader.construct_mapping(node)
         return cls.get_sample(**mapping)
 
 
-class UniformSampler(ScalarSampler):
+class SequenceSampler(Sampler):
+    """Define list sampler."""
+
+    @classmethod
+    def _construct_yaml(cls, loader: yaml.Loader, node: yaml.nodes.Node) -> Self:
+        sequence = loader.construct_sequence(node)
+        return cls.get_sample(sequence)
+
+
+class SampleUniform(ScalarSampler):
     """Sample from uniform distribution."""
 
     @classmethod
     def get_sample(cls, value: str) -> float:
         """Get the sample."""
         return random.uniform(*map(float, value.split("..")))
 
 
-class RangeSampler(ScalarSampler):
+class SampleRange(ScalarSampler):
     """Sample from range distribution."""
 
     @classmethod
     def get_sample(cls, value: str) -> int:
         """Get the sample."""
         split = value.split("..")
 
         if not 1 < len(split) <= 3:
             raise ValueError(f"Invalid range: {value}")
 
         return random.randrange(*map(int, split))
 
 
-class ChoiceSampler(ScalarSampler):
+class Choose(SequenceSampler):
     """Sample from choices."""
 
     @classmethod
     def get_sample(cls, values: list) -> int:
         """Get the sample."""
         return random.choice(values)
 
 
-class IntegerSampler(ScalarSampler):
+class ChooseInteger(SequenceSampler):
     """Sample from integer choices."""
 
     @classmethod
     def get_sample(cls, values: list) -> int:
         """Get the sample."""
-        return random.choice(map(int, values))
+        return random.choice(list(map(int, values)))
 
 
-class FloatSampler(ScalarSampler):
+class ChooseFloat(SequenceSampler):
     """Sample from float choices."""
 
     @classmethod
     def get_sample(cls, values: list) -> float:
         """Get the sample."""
-        return random.choice(map(float, values))
+        return random.choice(list(map(float, values)))
 
 
-class NormalSampler(ScalarSampler):
+class SampleNormal(MappingSampler):
     """Sample from normal distribution."""
 
     @classmethod
     def get_sample(cls, **kwargs) -> float:
         """Get the sample."""
         return random.normalvariate(**kwargs)
```

### Comparing `slot_machine_serializers-0.2.2/slot_machine/serializers.py` & `slot_machine_serializers-0.3.0/slot_machine/serializers.py`

 * *Files identical despite different names*

### Comparing `slot_machine_serializers-0.2.2/slot_machine_serializers.egg-info/PKG-INFO` & `slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot-machine-serializers
-Version: 0.2.2
+Version: 0.3.0
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
@@ -28,16 +28,16 @@
 With `slot_machine` your next choice will be one you look forward to.
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
-chicken_nuggets: !RangeSampler 5..20
-price: !UniformSampler 9..99..20
+chicken_nuggets: !SampleRange 5..20
+price: !SampleUniform 9..99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
@@ -45,16 +45,16 @@
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     price: float
 
 yaml_file = """
 basket:
-  chicken_nuggets: !RangeSampler 5..10
-  price: !UniformSampler 9.99..20
+  chicken_nuggets: !SampleRange 5..10
+  price: !SampleUniform 9.99..20
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
 
 ### Build your own
 
@@ -63,25 +63,25 @@
 from slot_machine import SlotsSerializer, MappingSampler
 
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     splits: list[int]
 
-class SplitsSampler(MappingSampler):
+class SampleSplits(MappingSampler):
 
   @classmethod
   def get_sample(cls, n_splits: str, values: str):
     n_splits = int(n_splits)
     values = list(map(int, values.split("..")))
     return sorted([random.randint(*values) for _ in range(n_splits)])
     
 yaml_file = """
 basket:
   chicken_nuggets: 100
-  splits: !SplitsSampler
+  splits: !SampleSplits
     n_splits: 3
     values: 0..100
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
```

### Comparing `slot_machine_serializers-0.2.2/tests/test_serializers.py` & `slot_machine_serializers-0.3.0/tests/test_serializers.py`

 * *Files identical despite different names*

