# Comparing `tmp/python_ember_mug-0.7.0b2.tar.gz` & `tmp/python_ember_mug-0.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b2.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b3.tar", max compression
```

## Comparing `python_ember_mug-0.7.0b2.tar` & `python_ember_mug-0.7.0b3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/LICENSE
--rw-r--r--   0        0        0     5282 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/README.md
--rwxr-xr-x   0        0        0      189 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8471 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     4875 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/consts.py
--rw-r--r--   0        0        0     8198 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/formatting.py
--rw-r--r--   0        0        0    17544 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/mug.py
--rw-r--r--   0        0        0     2112 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/scanner.py
--rw-r--r--   0        0        0     1973 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_consts.py
--rw-r--r--   0        0        0     2383 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_formatting.py
--rw-r--r--   0        0        0     3366 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_utils.py
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/LICENSE
+-rw-r--r--   0        0        0     5282 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/README.md
+-rwxr-xr-x   0        0        0      189 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8471 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     4915 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/consts.py
+-rw-r--r--   0        0        0     8531 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/formatting.py
+-rw-r--r--   0        0        0    17544 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/mug.py
+-rw-r--r--   0        0        0     2212 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/scanner.py
+-rw-r--r--   0        0        0     1973 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_connection.py
+-rw-r--r--   0        0        0      776 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_consts.py
+-rw-r--r--   0        0        0     2383 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_formatting.py
+-rw-r--r--   0        0        0     3366 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_utils.py
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b3/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b2/LICENSE` & `python_ember_mug-0.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/README.md` & `python_ember_mug-0.7.0b3/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b3/ember_mug/cli/commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b3/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/ember_mug/consts.py` & `python_ember_mug-0.7.0b3/ember_mug/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,16 @@
     # To watch for changes from mug (Notify/Read)
     PUSH_EVENT = 18
     # To gather bytes from mug for stats (Notify)
     STATISTICS = 19
     # RGBA Colour of LED (Read/Write)
     LED = 20
     # Service
-    SERVICE = 13858
+    TRAVEL_MUG_SERVICE = 13857
+    STANDARD_SERVICE = 13858
 
     @cached_property
     def uuid(self) -> UUID:
         """Convert the ID to a full UUID and cache."""
         return UUID(UUID_TEMPLATE.format(self.value))
 
     def __str__(self) -> str:
```

### Comparing `python_ember_mug-0.7.0b2/ember_mug/data.py` & `python_ember_mug-0.7.0b3/ember_mug/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,23 @@
 
     @cached_property
     def is_travel_mug(self) -> bool:
         """Check if the model is a Travel mug."""
         return self.name.startswith(EMBER_TRAVEL_MUG_SHORT)
 
     @cached_property
+    def type(self) -> str:
+        """Model type as short string."""
+        if self.is_cup:
+            return "cup"
+        elif self.is_travel_mug:
+            return "travel_mug"
+        return "mug"
+
+    @cached_property
     def attribute_labels(self) -> dict[str, str]:
         """Calculated labels for includes attributes."""
         all_attrs = self.initial_attributes | self.update_attributes | {'use_metric'}
         return {attr: label for attr, label in ATTR_LABELS.items() if attr in all_attrs}
 
     @cached_property
     def initial_attributes(self) -> set[str]:
@@ -148,17 +157,19 @@
     @cached_property
     def update_attributes(self) -> set[str]:
         """Attributes to update based on model and extra."""
         attributes = UPDATE_ATTRS
         if self.include_extra is False:
             attributes = attributes - EXTRA_ATTRS
         if self.is_cup:
+            # The Cup cannot be named
             attributes = attributes - {'name'}
         elif self.is_travel_mug:
-            attributes = (attributes - {'led_colour', 'liquid_level'}) | {'volume'}
+            # Tge Travel Mug does not have an LED colour, but has a volume attribute
+            attributes = (attributes - {'led_colour'}) | {'volume'}
         return attributes
 
 
 @dataclass
 class MugMeta:
     """Meta data for mug."""
```

### Comparing `python_ember_mug-0.7.0b2/ember_mug/formatting.py` & `python_ember_mug-0.7.0b3/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/ember_mug/mug.py` & `python_ember_mug-0.7.0b3/ember_mug/mug.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/ember_mug/scanner.py` & `python_ember_mug-0.7.0b3/ember_mug/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
         raise ValueError('The adapter option is only valid for the Linux BlueZ Backend.')
     return {'adapter': adapter} if adapter else {}
 
 
 async def discover_mugs(mac: str | None = None, adapter: str | None = None, wait: int = 5) -> list[BLEDevice]:
     """Discover new mugs in pairing mode."""
     scanner_kwargs = build_scanner_kwargs(adapter)
-    async with BleakScanner(service_uuids=[str(MugCharacteristic.SERVICE)], **scanner_kwargs) as scanner:
+    service_uuids = [str(uuid) for uuid in (MugCharacteristic.STANDARD_SERVICE, MugCharacteristic.TRAVEL_MUG_SERVICE)]
+    async with BleakScanner(service_uuids=service_uuids, **scanner_kwargs) as scanner:
         await asyncio.sleep(wait)
         if mac:
             mac = mac.lower()
             return [d for d in scanner.discovered_devices if d.address.lower() == mac]
         return scanner.discovered_devices
```

### Comparing `python_ember_mug-0.7.0b2/ember_mug/utils.py` & `python_ember_mug-0.7.0b3/ember_mug/utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/pyproject.toml` & `python_ember_mug-0.7.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.7.0b2"
+version = "0.7.0b3"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.7.0b2/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b3/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b3/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/conftest.py` & `python_ember_mug-0.7.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_connection.py` & `python_ember_mug-0.7.0b3/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_consts.py` & `python_ember_mug-0.7.0b3/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_data.py` & `python_ember_mug-0.7.0b3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_formatting.py` & `python_ember_mug-0.7.0b3/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_mug_data.py` & `python_ember_mug-0.7.0b3/tests/test_mug_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_scanner.py` & `python_ember_mug-0.7.0b3/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/tests/test_utils.py` & `python_ember_mug-0.7.0b3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b2/PKG-INFO` & `python_ember_mug-0.7.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.7.0b2
+Version: 0.7.0b3
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

