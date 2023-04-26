# Comparing `tmp/kernel_sidecar-0.5.4.tar.gz` & `tmp/kernel_sidecar-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernel_sidecar-0.5.4.tar", max compression
+gzip compressed data, was "kernel_sidecar-0.5.5.tar", max compression
```

## Comparing `kernel_sidecar-0.5.4.tar` & `kernel_sidecar-0.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-04-19 13:33:58.397089 kernel_sidecar-0.5.4/LICENSE
--rw-r--r--   0        0        0     8256 2023-04-19 13:33:58.397089 kernel_sidecar-0.5.4/README.md
--rw-r--r--   0        0        0     1089 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/__init__.py
--rw-r--r--   0        0        0     6079 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/actions.py
--rw-r--r--   0        0        0     2678 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/cli.py
--rw-r--r--   0        0        0    24314 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/client.py
--rw-r--r--   0        0        0     5207 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/comms.py
--rw-r--r--   0        0        0        0 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/__init__.py
--rw-r--r--   0        0        0     1054 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/base.py
--rw-r--r--   0        0        0     1580 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/debug.py
--rw-r--r--   0        0        0     5919 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/output.py
--rw-r--r--   0        0        0     4395 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/log_utils.py
--rw-r--r--   0        0        0        0 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/__init__.py
--rw-r--r--   0        0        0    14893 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/messages.py
--rw-r--r--   0        0        0     2334 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/notebook.py
--rw-r--r--   0        0        0     9389 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/models/requests.py
--rw-r--r--   0        0        0     5284 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/nb_builder.py
--rw-r--r--   0        0        0      261 2023-04-19 13:33:58.401089 kernel_sidecar-0.5.4/src/kernel_sidecar/settings.py
--rw-r--r--   0        0        0     9080 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/LICENSE
+-rw-r--r--   0        0        0     8256 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/README.md
+-rw-r--r--   0        0        0     1089 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/__init__.py
+-rw-r--r--   0        0        0     6079 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/actions.py
+-rw-r--r--   0        0        0     2678 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/cli.py
+-rw-r--r--   0        0        0    24314 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/client.py
+-rw-r--r--   0        0        0     5207 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/comms.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/__init__.py
+-rw-r--r--   0        0        0     1054 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/base.py
+-rw-r--r--   0        0        0     1580 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/debug.py
+-rw-r--r--   0        0        0     5919 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/output.py
+-rw-r--r--   0        0        0     4395 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/log_utils.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/models/__init__.py
+-rw-r--r--   0        0        0    15165 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/models/messages.py
+-rw-r--r--   0        0        0     2334 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/models/notebook.py
+-rw-r--r--   0        0        0     9389 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/models/requests.py
+-rw-r--r--   0        0        0     5284 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/nb_builder.py
+-rw-r--r--   0        0        0      261 2023-04-26 17:35:39.679749 kernel_sidecar-0.5.5/src/kernel_sidecar/settings.py
+-rw-r--r--   0        0        0     9080 1970-01-01 00:00:00.000000 kernel_sidecar-0.5.5/PKG-INFO
```

### Comparing `kernel_sidecar-0.5.4/LICENSE` & `kernel_sidecar-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/README.md` & `kernel_sidecar-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/pyproject.toml` & `kernel_sidecar-0.5.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kernel-sidecar"
-version = "0.5.4"
+version = "0.5.5"
 description = "A sidecar "
 authors = ["Matt Kafonek <matt.kafonek@noteable.io>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "kernel_sidecar", from = "src"}]
 repository = "https://github.com/kafonek/kernel-sidecar"
```

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/actions.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/actions.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/cli.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/cli.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/client.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/client.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/comms.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/comms.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/base.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/debug.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/debug.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/handlers/output.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/handlers/output.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/log_utils.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/log_utils.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/models/messages.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/models/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,27 +271,29 @@
         extra = "allow"
 
 
 class DisplayDataContent(BaseModel):
     output_type: Literal["display_data"] = "display_data"
     data: dict  # mimebundle
     metadata: dict = Field(default_factory=dict)
-    transient: DisplayDataTransient
+    # R Kernel does not include the transient key, Python client always seems to though
+    transient: Optional[DisplayDataTransient] = None
 
     class Config:
         # including transient in a saved .json file would be invalid jupyter spec, so by default
         # don't write out that field when calling .json().
         # If we decide to rethink that idea, then NotebookBuilder or Notebook or something would
         # want to call something pretty gnarly liike:
         # .json(exclude={'cells': {'__all__': {'outputs': {'__all__': {'transient': True}}}}})
         fields = {"transient": {"exclude": True}}
 
     @property
     def display_id(self) -> Optional[str]:
-        return self.transient.display_id
+        if self.transient:
+            return self.transient.display_id
 
 
 class DisplayData(MessageBase):
     msg_type: Literal["display_data"]
     content: DisplayDataContent
 
 
@@ -302,19 +304,21 @@
         extra = "allow"
 
 
 class UpdateDisplayDataContent(DisplayDataContent):
     output_type: Literal["update_display_data"] = "update_display_data"
     data: dict  # mimebundle
     metadata: dict = Field(default_factory=dict)
-    transient: DisplayDataTransient
+    # R Kernel does not include the transient key, Python client always seems to though
+    transient: Optional[DisplayDataTransient] = None
 
     @property
     def display_id(self) -> Optional[str]:
-        return self.transient.display_id
+        if self.transient:
+            return self.transient.display_id
 
 
 class UpdateDisplayData(MessageBase):
     msg_type: Literal["update_display_data"]
     content: UpdateDisplayDataContent
```

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/models/notebook.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/models/notebook.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/models/requests.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/models/requests.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/src/kernel_sidecar/nb_builder.py` & `kernel_sidecar-0.5.5/src/kernel_sidecar/nb_builder.py`

 * *Files identical despite different names*

### Comparing `kernel_sidecar-0.5.4/PKG-INFO` & `kernel_sidecar-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernel-sidecar
-Version: 0.5.4
+Version: 0.5.5
 Summary: A sidecar 
 Home-page: https://github.com/kafonek/kernel-sidecar
 License: MIT
 Author: Matt Kafonek
 Author-email: matt.kafonek@noteable.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.4 Summary: A sidecar
+Metadata-Version: 2.1 Name: kernel-sidecar Version: 0.5.5 Summary: A sidecar
 Home-page: https://github.com/kafonek/kernel-sidecar License: MIT Author: Matt
 Kafonek Author-email: matt.kafonek@noteable.io Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli Requires-Dist: jupyter-client (>=7.3.4) Requires-Dist:
```

