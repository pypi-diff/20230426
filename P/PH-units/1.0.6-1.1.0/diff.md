# Comparing `tmp/PH-units-1.0.6.tar.gz` & `tmp/PH-units-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-units-1.0.6.tar", last modified: Thu Jan 12 15:00:20 2023, max compression
+gzip compressed data, was "dist/PH-units-1.1.0.tar", last modified: Wed Apr 26 11:35:47 2023, max compression
```

## Comparing `PH-units-1.0.6.tar` & `PH-units-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-12 15:00:20.000000 PH-units-1.0.6/
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-01-12 14:58:55.000000 PH-units-1.0.6/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-12 15:00:20.000000 PH-units-1.0.6/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-12 15:00:20.000000 PH-units-1.0.6/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1781 2023-01-12 14:58:55.000000 PH-units-1.0.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-01-12 14:58:55.000000 PH-units-1.0.6/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-12 15:00:20.000000 PH-units-1.0.6/PH_units.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-01-12 15:00:20.000000 PH-units-1.0.6/PH_units.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      638 2023-01-12 15:00:20.000000 PH-units-1.0.6/PH_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-12 15:00:20.000000 PH-units-1.0.6/PH_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-01-12 15:00:20.000000 PH-units-1.0.6/PH_units.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-01-12 15:00:20.000000 PH-units-1.0.6/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-01-12 14:58:55.000000 PH-units-1.0.6/README.md
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-01-12 14:58:55.000000 PH-units-1.0.6/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-12 15:00:20.000000 PH-units-1.0.6/ph_units/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5084 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/converter.py
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/parser.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-12 15:00:20.000000 PH-units-1.0.6/ph_units/unit_types/
--rw-r--r--   0 runner     (501) staff       (20)     2482 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      371 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/_base.py
--rw-r--r--   0 runner     (501) staff       (20)      479 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/area.py
--rw-r--r--   0 runner     (501) staff       (20)     2139 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/energy.py
--rw-r--r--   0 runner     (501) staff       (20)     2808 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/envelope.py
--rw-r--r--   0 runner     (501) staff       (20)     1474 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/length.py
--rw-r--r--   0 runner     (501) staff       (20)     2281 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/power.py
--rw-r--r--   0 runner     (501) staff       (20)     1286 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/speed.py
--rw-r--r--   0 runner     (501) staff       (20)      877 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/temperature.py
--rw-r--r--   0 runner     (501) staff       (20)     1017 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/volume.py
--rw-r--r--   0 runner     (501) staff       (20)     1858 2023-01-12 14:58:55.000000 PH-units-1.0.6/ph_units/unit_types/volume_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-01-12 14:58:55.000000 PH-units-1.0.6/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-01-12 15:00:20.000000 PH-units-1.0.6/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-01-12 14:58:55.000000 PH-units-1.0.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-04-26 11:33:52.000000 PH-units-1.1.0/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2023-04-26 11:33:52.000000 PH-units-1.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2023-04-26 11:33:52.000000 PH-units-1.1.0/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      699 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-04-26 11:35:47.000000 PH-units-1.1.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-04-26 11:33:52.000000 PH-units-1.1.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    18761 2023-04-26 11:33:52.000000 PH-units-1.1.0/Untitled clipping.textClipping
+-rw-r--r--   0 runner     (501) staff       (20)       50 2023-04-26 11:33:52.000000 PH-units-1.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/ph_units/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5159 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/converter.py
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/parser.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/ph_units/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/tests/test_energy.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/ph_units/unit_types/
+-rw-r--r--   0 runner     (501) staff       (20)     2784 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      371 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)      442 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/area.py
+-rw-r--r--   0 runner     (501) staff       (20)     2655 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/energy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2571 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/envelope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/length.py
+-rw-r--r--   0 runner     (501) staff       (20)     2072 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     1176 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/speed.py
+-rw-r--r--   0 runner     (501) staff       (20)      796 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/temperature.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/volume.py
+-rw-r--r--   0 runner     (501) staff       (20)     1705 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/volume_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-04-26 11:33:52.000000 PH-units-1.1.0/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-04-26 11:35:47.000000 PH-units-1.1.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-04-26 11:33:52.000000 PH-units-1.1.0/setup.py
```

### Comparing `PH-units-1.0.6/.github/workflows/ci.yaml` & `PH-units-1.1.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-units-1.0.6/LICENSE` & `PH-units-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-units-1.0.6/PH_units.egg-info/PKG-INFO` & `PH-units-1.1.0/PH_units.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.0.6
+Version: 1.1.0
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.0.6/PH_units.egg-info/SOURCES.txt` & `PH-units-1.1.0/PH_units.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 .gitattributes
 LICENSE
 README.md
+Untitled clipping.textClipping
 dev-requirements.txt
 sandbox.py
 setup.cfg
 setup.py
 .github/workflows/ci.yaml
 PH_units.egg-info/PKG-INFO
 PH_units.egg-info/SOURCES.txt
 PH_units.egg-info/dependency_links.txt
 PH_units.egg-info/top_level.txt
 ph_units/__init__.py
 ph_units/converter.py
 ph_units/parser.py
+ph_units/tests/test_energy.py
 ph_units/unit_types/__init__.py
 ph_units/unit_types/_base.py
 ph_units/unit_types/area.py
 ph_units/unit_types/energy.py
 ph_units/unit_types/envelope.py
 ph_units/unit_types/length.py
 ph_units/unit_types/power.py
```

### Comparing `PH-units-1.0.6/PKG-INFO` & `PH-units-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.0.6
+Version: 1.1.0
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.0.6/README.md` & `PH-units-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PH-units-1.0.6/ph_units/converter.py` & `PH-units-1.1.0/ph_units/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ph_units.unit_types._base import Base_UnitType
 from ph_units.unit_types import build_unit_type_dicts
 
 unit_type_dict, unit_type_alias_dict = build_unit_type_dicts()
 
 
-def _standardize_input_unit(_input, _unit_type_alias_dict):
+def _standardize_unit_name(_input, _unit_type_alias_dict):
     # type: (str, Dict[str, str]) -> str
     """Standardize unit nomenclature. ie: 'FT3/M' and 'CFM' both return 'CFM'.
     Arguments:
     ----------
         * _input (str): The input unit-type.
         * _unit_type_alias_dict (Dict[str, str]): The dictionary of unit-type aliases.
 
@@ -58,16 +58,17 @@
     --------
         * (Tuple[str, str]): The input and output unit-type strings
     """
     if not _input_unit:
         _input_unit = copy(_target_unit)
 
     input_unit = str(_input_unit).upper().strip().replace(" ", "")
-    input_unit = _standardize_input_unit(input_unit, _unit_type_alias_dict)
+    input_unit = _standardize_unit_name(input_unit, _unit_type_alias_dict)
     target_unit = str(_target_unit).upper().strip().replace(" ", "")
+    target_unit = _standardize_unit_name(target_unit, _unit_type_alias_dict)
 
     return input_unit, target_unit
 
 
 def _conversion_schema(_input_unit, _schemas_dict):
     # type: (str, Dict[str, Base_UnitType]) -> Dict[str, str]
     """Returns the conversion schema dict, given an input unit type.
```

### Comparing `PH-units-1.0.6/ph_units/parser.py` & `PH-units-1.1.0/ph_units/parser.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.0.6/ph_units/unit_types/__init__.py` & `PH-units-1.1.0/ph_units/unit_types/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     speed,
     temperature,
     volume_flow,
     volume,
 )
 
 
-def _is_unit_type(cls):
+def _is_unit_class(cls):
     # type: (type) -> bool
     """Return True if the type is a Unit."""
     return hasattr(cls, "__symbol__") and hasattr(cls, "__factors__")
 
 
 def _build_alias_dict(_module):
     # type: (ModuleType) -> Dict[str, str]
@@ -48,23 +48,23 @@
     ----------
         * _module (ModuleType): The module to read the classes of.
 
     Returns:
     --------
         * (Dict[str, str]): A dict of all the unit-type aliases.
     """
-    _ = {}
-    for cls in _module.__dict__.values():
-        if not _is_unit_type(cls):
+    d = {}
+    for unit_class in _module.__dict__.values():
+        if not _is_unit_class(unit_class):
             continue
 
-        _[cls.__symbol__] = cls.__symbol__
-        for alias in cls.__aliases__:
-            _[alias] = cls.__symbol__
-    return _
+        d[unit_class.__symbol__] = unit_class.__symbol__
+        for alias in unit_class.__aliases__:
+            d[alias] = unit_class.__symbol__
+    return d
 
 
 def build_unit_type_dicts():
     # type: () -> Tuple[Dict[str, Base_UnitType], Dict[str, str]]
     """Returns dicts of all the unit-type conversion factor classes and aliases.
 
     Arguments:
@@ -78,18 +78,24 @@
                 by the class's __symbol__ as the key.
             * (Dict[str, str]): A dict of all the unit-type alias values.
     """
 
     unit_type_dict = {}  # type: Dict[str, Base_UnitType]
     unit_type_alias_dict = {}  # type: Dict[str, str]
 
-    for _mod in UNIT_TYPE_MODULES:
-        unit_type_dict.update(
-            {
-                cls.__symbol__: cls
-                for cls in _mod.__dict__.values()
-                if _is_unit_type(cls)
-            }
-        )
-        unit_type_alias_dict.update(_build_alias_dict(_mod))
+    for unit_module in UNIT_TYPE_MODULES:
+        d = {}
+        for unit_class in unit_module.__dict__.values():
+            if not _is_unit_class(unit_class):
+                continue
+
+            # -- Add the base unit-type class to the dict.
+            d[unit_class.__symbol__] = unit_class
+
+            # -- Add the type's aliases to the dict as well.
+            for alias in unit_class.__aliases__:
+                d[alias] = unit_class
+
+        unit_type_dict.update(d)
+        unit_type_alias_dict.update(_build_alias_dict(unit_module))
 
     return (unit_type_dict, unit_type_alias_dict)
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/energy.py` & `PH-units-1.1.0/ph_units/unit_types/energy.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,48 +5,76 @@
 
 
 class WattHoursPerMeterCubed(Base_UnitType):
     """WH/M3"""
 
     __symbol__ = "WH/M3"
     __aliases__ = []
-    __factors__ = {"SI": "{}*1", "WH/M3": "{}*1", "W/CFM": "{}*1.699010796"}
+    __factors__ = {"WH/M3": "{}*1", "W/CFM": "{}*1.699010796"}
 
 
 class WattHoursPerKilometerSquared(Base_UnitType):
     """WH/KM2"""
 
     __symbol__ = "WH/KM2"
     __aliases__ = []
-    __factors__ = {"SI": "{}*1", "WH/KM2": "{}*1", "BTU/FT2": "{}*0.000000317"}
+    __factors__ = {"WH/KM2": "{}*1", "BTU/FT2": "{}*0.000000317"}
 
 
 class WattHoursPerMeterSquared(Base_UnitType):
     """WH/M2"""
 
     __symbol__ = "WH/M2"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "WH/M2": "{}*1",
         "WH/FT2": "{}*0.092903",
         "KWH/M2": "{}*0.001",
         "KWH/FT2": "{}*0.000092903",
         "BTU/FT2": "{}*0.316998",
         "KBTU/FT2": "{}*0.000316998",
     }
 
 
+class WattHoursPerFootSquared(Base_UnitType):
+    """WH/FT2"""
+
+    __symbol__ = "WH/FT2"
+    __aliases__ = []
+    __factors__ = {
+        "WH/M2": "{}*10.7639",
+        "WH/FT2": "{}*1",
+        "KWH/M2": "{}*0.0107639",
+        "KWH/FT2": "{}*0.001",
+        "BTU/FT2": "{}*3.413",
+        "KBTU/FT2": "{}*0.003413",
+    }
+
+
+class KiloWattHoursPerFootSquared(Base_UnitType):
+    """KWH/FT2"""
+
+    __symbol__ = "KWH/FT2"
+    __aliases__ = ["KWH/SF"]
+    __factors__ = {
+        "WH/M2": "{}*10763.9",
+        "WH/FT2": "{}*1000",
+        "KWH/M2": "{}*10.7639",
+        "KWH/FT2": "{}*1",
+        "BTU/FT2": "{}*3413",
+        "KBTU/FT2": "{}*3.413",
+    }
+
+
 class KilowattHoursPerMeterSquared(Base_UnitType):
     """KWH/M2"""
 
     __symbol__ = "KWH/M2"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "WH/M2": "{}*1000",
         "WH/FT2": "{}*92.903",
         "KWH/M2": "{}*1",
         "KWH/FT2": "{}*0.092903040",
         "BTU/FT2": "{}*316.998",
         "KBTU/FT2": "{}*0.316998286",
     }
@@ -54,15 +82,14 @@
 
 class KBtuPerFootSquared(Base_UnitType):
     """KBTU/FT2"""
 
     __symbol__ = "KBTU/FT2"
     __aliases__ = ["KBTU/SF"]
     __factors__ = {
-        "SI": "{}*3.15459",
         "WH/M2": "{}*3154.59",
         "WH/FT2": "{}*293.071",
         "KWH/M2": "{}*3.15459",
         "KWH/FT2": "{}*0.293071",
         "BTU/FT2": "{}*1000",
         "KBTU/FT2": "{}*1",
     }
@@ -70,23 +97,22 @@
 
 class BtuPerFootSquared(Base_UnitType):
     """BTU/FT2"""
 
     __symbol__ = "BTU/FT2"
     __aliases__ = ["BTU/SF"]
     __factors__ = {
-        "SI": "{}*0.00315459",
         "WH/M2": "{}*3.15459",
         "WH/FT2": "{}*0.293071",
         "KWH/M2": "{}*0.00315459",
         "KWH/FT2": "{}*0.000293071",
         "BTU/FT2": "{}*1",
         "KBTU/FT2": "{}*0.001",
     }
 
 
 class MegaJoulePerMeterCubedKelvin(Base_UnitType):
     """MJ/M3K"""
 
     __symbol__ = "MJ/M3K"
     __aliases__ = []
-    __factors__ = {"SI": "{}*1", "MJ/M3K": "{}*1", "BTU/FT3-F": "{}*14.91066014"}
+    __factors__ = {"MJ/M3K": "{}*1", "BTU/FT3-F": "{}*14.91066014"}
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/envelope.py` & `PH-units-1.1.0/ph_units/unit_types/envelope.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,109 +6,102 @@
 
 class WattsPerMeterSquaredKelvin(Base_UnitType):
     """W/M2K (U-Value)"""
 
     __symbol__ = "W/M2K"
     __aliases__ = ["U-SI"]
     __factors__ = {
-        "SI": "{}*1",
         "W/M2K": "{}*1",
         "M2K/W": "(1/{})",
         "BTU/HR-FT2-F": "{}*0.176110159",
         "HR-FT2-F/BTU": "(1/{})*5.678264134",
     }
 
 
 class BtuPerHourFootSquaredFahrenheit(Base_UnitType):
     """BTU/HR-FT2-F (U-Value)"""
 
     __symbol__ = "BTU/HR-FT2-F"
     __aliases__ = ["U-IP", "BTU/HR-SF-F", "BTU/H-SF-F"]
     __factors__ = {
-        "SI": "{}*5.678264134",
         "W/M2K": "{}*5.678264134",
         "M2K/W": "1/({}*5.678264134)",
         "BTU/HR-FT2-F": "{}*1",
         "HR-FT2-F/BTU": "(1/{})",
     }
 
 
 class MeterSquaredKelvinPerWatt(Base_UnitType):
     """M2K/W (R-Value)"""
 
     __symbol__ = "M2K/W"
     __aliases__ = ["R-SI"]
     __factors__ = {
-        "SI": "{}*1",
         "M2K/W": "{}*1",
         "W/M2K": "(1/{})",
         "HR-FT2-F/BTU": "{}*5.678264134",
         "BTU/HR-FT2-F": "1/({}*5.678264134)",
     }
 
 
 class HourFootSquaredFahrenheitPerBtu(Base_UnitType):
     """HR-FT2-F/BTU (R-Value)"""
 
     __symbol__ = "HR-FT2-F/BTU"
     __aliases__ = ["R-IP", "H-SF-F/BTU", "HR-SF-F/BTU"]
     __factors__ = {
-        "SI": "1/((1/{})*5.678264134)",
         "M2K/W": "1/((1/{})*5.678264134)",
         "W/M2K": "(1/{})*5.678264134",
         "HR-FT2-F/BTU": "{}*1",
         "BTU/HR-FT2-F": "(1/{})",
     }
 
 
 class HourFootSquaredFahrenheitPerBtuInch(Base_UnitType):
     """HR-FT2-F/BTU-IN (R-per-inch)"""
 
     __symbol__ = "HR-FT2-F/BTU-IN"
     __aliases__ = ["R/IN", "R-IN", "H-SF-F/BTU-IN"]
     __factors__ = {
-        "SI": "{}*1.730734908",
         "W/MK": "(1/({}*12))*1.730734908",
         "BTU/HR-FT-F": "1/({}*12)",
     }
 
 
 class WattsPerMeterKelvin(Base_UnitType):
     """W/MK (Psi-Value)"""
 
     __symbol__ = "W/MK"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "W/MK": "{}*1",
         "HR-FT2-F/BTU-IN": "{}**-1*0.144227909",
         "BTU/HR-FT-F": "{}*0.577789236",
     }
 
 
 class BtuPerHourFootFahrenheit(Base_UnitType):
     """BTU/HR-FT-F (Psi-Value)"""
 
     __symbol__ = "BTU/HR-FT-F"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1.730734908",
         "W/MK": "{}*1.730734908",
         "HR-FT2-F/BTU-IN": "1/({}*12)",
         "BTU/HR-FT-F": "{}*1",
     }
 
 
 class WattsPerKelvin(Base_UnitType):
     """W/K (Chi-Value)"""
 
     __symbol__ = "W/K"
     __aliases__ = []
-    __factors__ = {"SI": "{}*1", "W/K": "{}*1", "BTU/HR-F": "{}*1.895633976"}
+    __factors__ = {"W/K": "{}*1", "BTU/HR-F": "{}*1.895633976"}
 
 
 class BtuPerHourFahrenheit(Base_UnitType):
     """BTU/HR-F (Chi-Value)"""
 
     __symbol__ = "BTU/HR-F"
     __aliases__ = []
-    __factors__ = {"SI": "{}*0.527528", "W/K": "{}*0.527528", "BTU/HR-F": "{}*1"}
+    __factors__ = {"W/K": "{}*0.527528", "BTU/HR-F": "{}*1"}
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/length.py` & `PH-units-1.1.0/ph_units/unit_types/speed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,57 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 2.7 -*-
 
 from ph_units.unit_types._base import Base_UnitType
 
 
-class Meter(Base_UnitType):
-    """Meter"""
+class MeterPerDay(Base_UnitType):
+    """Meter/Day"""
 
-    __symbol__ = "M"
+    __symbol__ = "M/DAY"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
-        "M": "{}*1",
-        "CM": "{}*100",
-        "MM": "{}*1000",
-        "FT": "{}*3.280839895",
-        "IN": "{}*39.3701",
+        "M/DAY": "{}*1",
+        "FT/DAY": "{}*3.280839895",
+        "M/S": "{}/24/60/60",
     }
 
 
-class Centimeter(Base_UnitType):
-    """Centimeter"""
+class MeterPerSecond(Base_UnitType):
+    """Meter/Second"""
 
-    __symbol__ = "CM"
-    __aliases__ = []
+    __symbol__ = "M/S"
+    __aliases__ = ["METER/SEC", "METER/SECOND", "M/SECOND"]
     __factors__ = {
-        "SI": "{}*1",
-        "M": "{}*0.01",
-        "CM": "{}*1",
-        "MM": "{}*10",
-        "FT": "{}*0.0328",
-        "IN": "{}*0.3937",
+        "M/S": "{}*1",
+        "M/DAY": "{}*24*60*60",
+        "FT/S": "{}*3.280839895",
+        "FT/DAY": "{}*3.280839895*24*60*60",
+        "MPH": "{}/0.44704",
     }
 
 
-class Millimeter(Base_UnitType):
-    """Millimeter"""
+class MilesPerHour(Base_UnitType):
+    """MPH"""
 
-    __symbol__ = "MM"
+    __symbol__ = "M/DAY"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
-        "MM": "{}*1",
-        "M": "{}*0.001",
-        "CM": "{}*0.1",
-        "FT": "{}*0.003280842",
-        "IN": "{}*0.039370100",
+        "M/S": "{}*0.44704",
+        "M/DAY": "{}*0.44704*60*60*24",
     }
 
 
-class Inch(Base_UnitType):
-    """Inch"""
+class FeetPerSecond(Base_UnitType):
+    """FT/Second"""
 
-    __symbol__ = "IN"
-    __aliases__ = ['"', "IN."]
-    __factors__ = {
-        "SI": "{}*0.0254",
-        "M": "{}*0.0254",
-        "CM": "{}*2.54",
-        "MM": "{}*25.4",
-        "FT": "{}/12",
-        "IN": "{}*1",
-    }
+    __symbol__ = "FT/S"
+    __aliases__ = []
+    __factors__ = {"M/S": "{}*0.3048", "M/DAY": "{}*0.3048*60*60*24"}
 
 
-class Foot(Base_UnitType):
-    """Foot"""
+class FeetPerDay(Base_UnitType):
+    """FT/Day"""
 
-    __symbol__ = "FT"
-    __aliases__ = ["'", "FT."]
-    __factors__ = {
-        "SI": "{}*0.3048",
-        "M": "{}*0.3048",
-        "CM": "{}*30.48",
-        "MM": "{}*304.8",
-        "FT": "{}*1",
-        "IN": "{}*12",
-    }
+    __symbol__ = "FT/DAY"
+    __aliases__ = ["FT/D"]
+    __factors__ = {"M/DAY": "{}*0.3048"}
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/power.py` & `PH-units-1.1.0/ph_units/unit_types/power.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,105 +6,98 @@
 
 class Kilowatts(Base_UnitType):
     """KW"""
 
     __symbol__ = "KW"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "KW": "{}*1",
         "W": "{}*1000",
-        "BTU/HR": "{}*3412.141156",
-        "KBTU/HR": "{}*3.412141156",
+        "BTUH": "{}*3412.141156",
+        "KBTUH": "{}*3.412141156",
     }
 
 
 class Watts(Base_UnitType):
     """W"""
 
     __symbol__ = "W"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "KW": "{}*1",
         "BTU/HR": "{}*3.412141156",
         "KBTU/HR": "{}*0.003412141",
     }
 
 
 class WattsPerMeterSquared(Base_UnitType):
     """W/M2"""
 
     __symbol__ = "W/M2"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "W/M2": "{}*1",
         "BTU/HR-FT2": "{}*0.316998286",
         "W/FT2": "{}*0.09290304",
     }
 
 
 class WattsPerWatt(Base_UnitType):
     """W/W (SEER)"""
 
     __symbol__ = "W/W"
     __aliases__ = []
-    __factors__ = {"SI": "{}*1", "W/W": "{}*1", "BTUHR/W": "{}*3.412141156"}
+    __factors__ = {"W/W": "{}*1", "BTUHR/W": "{}*3.412141156"}
 
 
 class WattsPerFootSquared(Base_UnitType):
     """W/FT2"""
 
     __symbol__ = "W/FT2"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*10.76391042",
         "W/M2": "{}*10.76391042",
         "BTU/HR-FT2": "{}/3.412141156",
     }
 
 
 class WattsPerFootCubedPerMinute(Base_UnitType):
     """W/CFM"""
 
     __symbol__ = "W/CFM"
     __aliases__ = []
-    __factors__ = {"SI": "{}*0.588577779", "WH/M3": "{}*0.588577779"}
+    __factors__ = {"W/CFM": "{}*0.588577779", "WH/M3": "{}*0.588577779"}
 
 
 class BtuPerHourFootSquared(Base_UnitType):
     """BTU/HR-FT2"""
 
     __symbol__ = "BTU/HR-FT2"
     __aliases__ = ["BTUH/FT2", "BTU/H-SF", "BTU/H-FT2"]
     __factors__ = {
-        "SI": "{}*3.154591186",
         "W/M2": "{}*3.154591186",
         "W/FT2": "{}*0.293071111",
     }
 
 
 class BtuPerHour(Base_UnitType):
     """BTU/H"""
 
     __symbol__ = "BTUH"
     __aliases__ = ["BTU/HR", "BTU/H", "BTUHR"]
     __factors__ = {
-        "SI": "{}*0.293071111",
         "KBTUH": "{}/1000",
         "W": "{}*0.293071111",
         "KW": "{}*0.000293071",
     }
 
 
 class KiloBtuPerHour(Base_UnitType):
     """KBTU/H"""
 
     __symbol__ = "KBTUH"
     __aliases__ = ["KBTU/HR", "KBTU/H", "KBTUHR"]
     __factors__ = {
-        "SI": "{}*0.293071111",
         "BTUH": "{}*1000",
         "W": "{}*293.0711111",
         "KW": "{}*0.293071111",
     }
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/temperature.py` & `PH-units-1.1.0/ph_units/unit_types/temperature.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,35 @@
 
 
 class Celsius(Base_UnitType):
     "Celsius"
 
     __symbol__ = "C"
     __aliases__ = ["DEG C", "DEG. C", "°C"]
-    __factors__ = {"SI": "{}*1", "C": "{}*1", "F": "{}*1.8+32"}
+    __factors__ = {"C": "{}*1", "F": "{}*1.8+32"}
 
 
 class DeltaCelsius(Base_UnitType):
     "Delta-Celsius"
 
     __symbol__ = "DELTA-C"
     __aliases__ = []
-    __factors__ = {"SI": "{}*1", "DELTA-C": "{}*1", "DELTA-F": "{}*1.8"}
+    __factors__ = {"DELTA-C": "{}*1", "DELTA-F": "{}*1.8"}
 
 
 class Fahrenheit(Base_UnitType):
     "Fahrenheit"
 
     __symbol__ = "F"
     __aliases__ = ["DEG F", "DEG. F", "°F"]
-    __factors__ = {"SI": "({}-32)/1.8", "C": "({}-32)/1.8"}
+    __factors__ = {"C": "({}-32)/1.8"}
 
 
 class DeltaFahrenheit(Base_UnitType):
     "Delta-Fahrenheit"
 
     __symbol__ = "DELTA-F"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*0.555555556",
         "DELTA-C": "{}*0.555555556",
         "DELTA-F": "{}*1",
     }
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/volume.py` & `PH-units-1.1.0/ph_units/unit_types/volume.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,47 +6,44 @@
 
 class MeterCubed(Base_UnitType):
     """Meter Cubed"""
 
     __symbol__ = "M3"
     __aliases__ = []
     __factors__ = {
-        "SI": "{}*1",
         "M3": "{}*1",
         "FT3": "{}*35.31466672",
         "L": "{}*1000",
         "GA": "{}*264.1720524",
     }
 
 
 class Liter(Base_UnitType):
     """Liter"""
 
     __symbol__ = "L"
     __aliases__ = ["LITER", "LITRE"]
     __factors__ = {
-        "SI": "{}*1",
         "L": "{}*1",
         "GA": "{}*0.264172",
         "FT3": "{}*0.035314667",
         "M3": "{}*0.001",
     }
 
 
 class Gallon(Base_UnitType):
     """Gallon"""
 
     __symbol__ = "GA"
     __aliases__ = ["GALLON", "G"]
-    __factors__ = {"SI": "{}*3.785411784", "L": "{}*3.785411784"}
+    __factors__ = {"L": "{}*3.785411784"}
 
 
 class FootCubed(Base_UnitType):
     """Foot Cubed"""
 
     __symbol__ = "FT3"
     __aliases__ = ["CF"]
     __factors__ = {
-        "SI": "{}*0.028316847",
         "M3": "{}*0.028316847",
         "FT3": "{}*1",
     }
```

### Comparing `PH-units-1.0.6/ph_units/unit_types/volume_flow.py` & `PH-units-1.1.0/ph_units/unit_types/volume_flow.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,45 +6,42 @@
 
 class MeterCubedPerSecond(Base_UnitType):
     """M3/S"""
 
     __symbol__ = "M3/S"
     __aliases__ = ["M3/SECOND", "M3/SEC", "CM/S"]
     __factors__ = {
-        "SI": "{}*1",
         "M3/S": "{}*1",
         "M3/M": "{}*60",
         "M3/HR": "{}*60*60",
         "CFM": "({}*60*60)*0.588577779",
         "CFH": "({}*60*60*60)*0.588577779",
     }
 
 
 class MeterCubedPerMinute(Base_UnitType):
     """M3/M"""
 
     __symbol__ = "M3/M"
     __aliases__ = ["M3/MIN", "M3/MINUTE", "CM/M"]
     __factors__ = {
-        "SI": "{}*1",
         "M3/S": "{}/60",
         "M3/M": "{}*1",
         "M3/HR": "{}*60",
         "CFM": "({}*60)*0.588577779",
         "CFH": "({}*60*60)*0.588577779",
     }
 
 
 class MeterCubedPerHour(Base_UnitType):
     """M3/HR"""
 
     __symbol__ = "M3/HR"
     __aliases__ = ["CM/H", "CMH", "M3/H"]
     __factors__ = {
-        "SI": "{}*1",
         "M3/S": "({}/60)/60",
         "M3/M": "{}/60",
         "M3/HR": "{}*1",
         "CFM": "{}*0.588577779",
         "CFH": "({}*60)*0.588577779",
     }
 
@@ -54,29 +51,27 @@
 
 class FootCubedPerMinute(Base_UnitType):
     """CFM"""
 
     __symbol__ = "CFM"
     __aliases__ = ["FT3/M", "FT3M"]
     __factors__ = {
-        "SI": "(({}*1.699010796)/60)/60",
         "M3/S": "(({}*1.699010796)/60)/60",
         "M3/M": "({}*1.699010796)/60",
         "M3/HR": "{}*1.699010796",
         "CFM": "{}*1",
         "CFH": "{}*60",
     }
 
 
 class FootCubedPerHour(Base_UnitType):
     """CFH"""
 
     __symbol__ = "CFH"
     __aliases__ = ["FT3/H", "FT3/HR", "FT3H", "CF/HR"]
     __factors__ = {
-        "SI": "(({}/60)*1.699010796)/60/60",
         "M3/S": "(({}/60)*1.699010796)/60/60",
         "M3/M": "(({}/60)*1.699010796)/60",
         "M3/HR": "(({}/60)*1.699010796)",
         "CFM": "{}/60",
         "CFH": "{}*1",
     }
```

### Comparing `PH-units-1.0.6/setup.cfg` & `PH-units-1.1.0/setup.cfg`

 * *Files identical despite different names*

