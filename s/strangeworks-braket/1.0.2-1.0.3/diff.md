# Comparing `tmp/strangeworks_braket-1.0.2.tar.gz` & `tmp/strangeworks_braket-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_braket-1.0.2.tar", max compression
+gzip compressed data, was "strangeworks_braket-1.0.3.tar", max compression
```

## Comparing `strangeworks_braket-1.0.2.tar` & `strangeworks_braket-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      457 2023-04-19 11:08:30.783253 strangeworks_braket-1.0.2/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-19 11:08:30.783253 strangeworks_braket-1.0.2/LICENSE
--rw-r--r--   0        0        0     1261 2023-04-19 11:08:44.351207 strangeworks_braket-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      232 2023-04-19 11:08:30.783253 strangeworks_braket-1.0.2/strangeworks_braket/__init__.py
--rw-r--r--   0        0        0     3228 2023-04-19 11:08:30.783253 strangeworks_braket-1.0.2/strangeworks_braket/device.py
--rw-r--r--   0        0        0    10391 2023-04-19 11:08:30.783253 strangeworks_braket-1.0.2/strangeworks_braket/task.py
--rw-r--r--   0        0        0      691 2023-04-19 11:08:30.783253 strangeworks_braket-1.0.2/strangeworks_braket/utils/serializer.py
--rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1317 2023-04-25 15:47:50.529147 strangeworks_braket-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/__init__.py
+-rw-r--r--   0        0        0     6022 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/device.py
+-rw-r--r--   0        0        0    10889 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/task.py
+-rw-r--r--   0        0        0      691 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/utils/serializer.py
+-rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.3/PKG-INFO
```

### Comparing `strangeworks_braket-1.0.2/LICENSE` & `strangeworks_braket-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.2/pyproject.toml` & `strangeworks_braket-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "strangeworks-braket"
-version = "1.0.2"
+version = "1.0.3"
 description = "Strangeworks Braket SDK extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_braket"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.11"
 amazon-braket-sdk = "^1.31.1"
 strangeworks-python-core = "^0.1.6"
 python-jose = "^3.3.0"
 strangeworks = "^0.4.1"
+llvmlite = "0.39.1"
+strawberryfields = "^0.23.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 pytest = "^7.0.1"
 Flake8-pyproject = "^1.1.0"
 mdformat = "^0.7.14"
```

### Comparing `strangeworks_braket-1.0.2/strangeworks_braket/task.py` & `strangeworks_braket-1.0.3/strangeworks_braket/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.schema_common import BraketSchemaBase
 from braket.tasks.annealing_quantum_task_result import AnnealingQuantumTaskResult
 from braket.tasks.gate_model_quantum_task_result import GateModelQuantumTaskResult
 from braket.tasks.quantum_task import QuantumTask
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.types.job import Job, Status
+from strawberryfields.tdm.program import TDMProgram
 
 from strangeworks_braket.utils.serializer import pickle_serializer
 
 
 class StrangeworksQuantumTask(QuantumTask):
     _product_slug = "amazon-braket"
 
@@ -152,14 +153,16 @@
         if len(contents) != 1:
             raise StrangeworksError("Unable to download result file.")
         bsh = BraketSchemaBase.parse_raw_schema(json.dumps(contents[0]))
 
         if (
             bsh.taskMetadata.deviceId
             != "arn:aws:braket:us-east-1::device/qpu/quera/Aquila"
+            and bsh.taskMetadata.deviceId
+            != "arn:aws:braket:us-east-1::device/qpu/xanadu/Borealis"
         ):
             task_result = GateModelQuantumTaskResult.from_object(bsh)
         else:
             task_result = bsh
         return task_result
 
     def async_result(self) -> asyncio.Task:
@@ -196,15 +199,17 @@
             raise StrangeworksError("Multiple jobs found for slug")
         job = jobs[0]
         return StrangeworksQuantumTask(job)
 
     @staticmethod
     def create(
         device_arn: str,
-        task_specification: Union[Circuit, Problem, OpenQasmProgram],
+        task_specification: Union[
+            Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation, TDMProgram
+        ],
         shots: int,
         device_parameters: Optional[Dict[str, Any]] = None,
         tags: Optional[Dict[str, str]] = None,
         *args,
         **kwargs,
     ) -> StrangeworksQuantumTask:
         """Create a task.
@@ -262,15 +267,15 @@
         remix = {to_camel_case(key): value for key, value in d.items()}
         return Job.from_dict(remix)
 
 
 @singledispatch
 def _sw_task_specification(
     task_specification: Union[
-        Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation
+        Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation, TDMProgram
     ]
 ) -> Tuple[str, str]:
     raise NotImplementedError
 
 
 # register a function for each type
 @_sw_task_specification.register
@@ -292,7 +297,15 @@
 
 @_sw_task_specification.register
 def _sw_task_specification_aquila(
     task_specification: AnalogHamiltonianSimulation,
 ) -> Tuple[str, str]:
     task_new_specification = json.dumps(pickle_serializer(task_specification, "json"))
     return "aquila", task_new_specification
+
+
+@_sw_task_specification.register
+def _sw_task_specification_xanadu(
+    task_specification: TDMProgram,
+) -> Tuple[str, str]:
+    task_new_specification = json.dumps(pickle_serializer(task_specification, "json"))
+    return "xanadu", task_new_specification
```

### Comparing `strangeworks_braket-1.0.2/strangeworks_braket/utils/serializer.py` & `strangeworks_braket-1.0.3/strangeworks_braket/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.2/PKG-INFO` & `strangeworks_braket-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: strangeworks-braket
-Version: 1.0.2
+Version: 1.0.3
 Summary: Strangeworks Braket SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: amazon-braket-sdk (>=1.31.1,<2.0.0)
+Requires-Dist: llvmlite (==0.39.1)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: strangeworks (>=0.4.1,<0.5.0)
 Requires-Dist: strangeworks-python-core (>=0.1.6,<0.2.0)
+Requires-Dist: strawberryfields (>=0.23.0,<0.24.0)
 Description-Content-Type: text/markdown
 
 | ⚠️ | This SDK is currently in pre-release alpha state and subject to change. To get
 more info or access to test features check out the
 [Strangeworks Backstage Pass Program](https://strangeworks.com/backstage). |
 |---------------|:------------------------|
```

