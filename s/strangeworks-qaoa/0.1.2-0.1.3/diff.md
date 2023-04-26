# Comparing `tmp/strangeworks_qaoa-0.1.2.tar.gz` & `tmp/strangeworks_qaoa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.2.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.3.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.2.tar` & `strangeworks_qaoa-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-25 11:25:54.241258 strangeworks_qaoa-0.1.2/LICENSE
--rw-r--r--   0        0        0      576 2023-04-25 11:25:54.241258 strangeworks_qaoa-0.1.2/README.md
--rw-r--r--   0        0        0      792 2023-04-25 11:26:08.277460 strangeworks_qaoa-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      128 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    16286 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    10892 2023-04-25 11:25:54.245257 strangeworks_qaoa-0.1.2/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 15:00:04.025123 strangeworks_qaoa-0.1.3/LICENSE
+-rw-r--r--   0        0        0      576 2023-04-26 15:00:04.025123 strangeworks_qaoa-0.1.3/README.md
+-rw-r--r--   0        0        0      791 2023-04-26 15:00:22.529517 strangeworks_qaoa-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    16000 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    10892 2023-04-26 15:00:04.029123 strangeworks_qaoa-0.1.3/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.3/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.2/LICENSE` & `strangeworks_qaoa-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.2/README.md` & `strangeworks_qaoa-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.2/pyproject.toml` & `strangeworks_qaoa-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.2"
+version = "0.1.3"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 networkx = "^3.0"
 numpy = "1.23.2"
 qiskit = "^0.41.0"
-strangeworks = "^0.4.0" 
+strangeworks = "^0.4.0"
 dimod = "^0.12.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
```

### Comparing `strangeworks_qaoa-0.1.2/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.3/strangeworks_qaoa/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,43 +237,37 @@
             QUBO = problem["BQM"].to_numpy_matrix(
                 variable_order=problem.get("variable_order")
             )
             H = utils.get_Ham_from_QUBO(QUBO)
         else:
             raise StrangeworksError("Problem not in currently supported format")
 
-        problem_params["H"] = serializer.pickle_serializer(H, "json")
-        problem_params["nqubits"] = str(len(H[0][1]))
-        problem_params["theta0"] = (
-            str(problem_params.get("theta0")) if problem_params.get("theta0") else None
-        )
+        problem_params["H"] = json.dumps(H)
+        problem_params["nqubits"] = len(H[0][1])
         problem_params["ising"] = (
             json.dumps(problem_params["ising"])
             if problem_params.get("ising")
             else json.dumps(False)
         )
 
         if aws is True:
             input_params = {
                 "provider": "aws",
-                "dev_str": backend_id,
-                "hyperparams": problem_params,
+                "backend": backend_id,
+                "hyperparams": json.dumps(problem_params),
             }
         elif ibm is True:
             input_params = {
                 "provider": "ibm",
                 "channel": channel,
                 "backend": backend_id,
-                "hyperparams": problem_params,
+                "hyperparams": json.dumps(problem_params),
             }
 
-        input_json = serializer.pickle_serializer(input_params, "json")
-        input_json = {"payload": input_json}
-
-        sw_job = strangeworks.execute(self.rsc, input_json, "run_hybrid_job")
+        sw_job = strangeworks.execute(self.rsc, input_params, "run_hybrid_job")
 
         return sw_job
 
     def update_status(self, sw_job):
         if type(sw_job) is dict:
             job_slug = sw_job.get("slug")
         else:
@@ -319,15 +313,15 @@
 
         if calculate_exact_sol:
             inputs_url = strangeworks.execute(
                 self.rsc, {"payload": {"job_slug": job_slug}}, "get_inputs_url"
             )
             inputs = strangeworks.download_job_files([inputs_url])[0]
 
-            H = serializer.pickle_deserializer(inputs["H"], "json")
+            H = json.loads(inputs["H"])
 
             try:
                 En_exact = utils.get_exact_en(
                     utils.get_graph_from_Ham(H),
                     len(H[0][1]),
                     ising=json.loads(inputs["ising"]) if inputs.get("ising") else False,
                 )
```

### Comparing `strangeworks_qaoa-0.1.2/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.3/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.2/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.3/strangeworks_qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.2/PKG-INFO` & `strangeworks_qaoa-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

