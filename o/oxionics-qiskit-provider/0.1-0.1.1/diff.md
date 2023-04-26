# Comparing `tmp/oxionics_qiskit_provider-0.1.tar.gz` & `tmp/oxionics_qiskit_provider-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxionics_qiskit_provider-0.1.tar", max compression
+gzip compressed data, was "oxionics_qiskit_provider-0.1.1.tar", max compression
```

## Comparing `oxionics_qiskit_provider-0.1.tar` & `oxionics_qiskit_provider-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      755 2023-04-25 13:49:31.152251 oxionics_qiskit_provider-0.1/README.md
--rw-r--r--   0        0        0      105 2023-04-25 13:49:31.152251 oxionics_qiskit_provider-0.1/oxionics_qiskit_provider/__init__.py
--rw-r--r--   0        0        0     2288 2023-04-25 13:49:31.152251 oxionics_qiskit_provider-0.1/oxionics_qiskit_provider/backend.py
--rw-r--r--   0        0        0     4572 2023-04-25 13:49:31.152251 oxionics_qiskit_provider-0.1/oxionics_qiskit_provider/job.py
--rw-r--r--   0        0        0      373 2023-04-25 13:49:31.152251 oxionics_qiskit_provider-0.1/oxionics_qiskit_provider/provider.py
--rw-r--r--   0        0        0      863 2023-04-25 13:49:31.152251 oxionics_qiskit_provider-0.1/pyproject.toml
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 oxionics_qiskit_provider-0.1/setup.py
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 oxionics_qiskit_provider-0.1/PKG-INFO
+-rw-r--r--   0        0        0      755 2023-04-26 10:42:36.979649 oxionics_qiskit_provider-0.1.1/README.md
+-rw-r--r--   0        0        0      105 2023-04-26 10:42:36.979649 oxionics_qiskit_provider-0.1.1/oxionics_qiskit_provider/__init__.py
+-rw-r--r--   0        0        0     2291 2023-04-26 10:42:36.979649 oxionics_qiskit_provider-0.1.1/oxionics_qiskit_provider/backend.py
+-rw-r--r--   0        0        0     4572 2023-04-26 10:42:36.979649 oxionics_qiskit_provider-0.1.1/oxionics_qiskit_provider/job.py
+-rw-r--r--   0        0        0      373 2023-04-26 10:42:36.979649 oxionics_qiskit_provider-0.1.1/oxionics_qiskit_provider/provider.py
+-rw-r--r--   0        0        0      866 2023-04-26 10:42:49.895834 oxionics_qiskit_provider-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1433 1970-01-01 00:00:00.000000 oxionics_qiskit_provider-0.1.1/setup.py
+-rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 oxionics_qiskit_provider-0.1.1/PKG-INFO
```

### Comparing `oxionics_qiskit_provider-0.1/README.md` & `oxionics_qiskit_provider-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oxionics_qiskit_provider-0.1/oxionics_qiskit_provider/backend.py` & `oxionics_qiskit_provider-0.1.1/oxionics_qiskit_provider/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.api_root = api_root
         self.session = requests.Session()
         # TODO get our version from somewhere
         self.session.headers[
             "User-Agent"
         ] = f"OxIonicsQisKitBacked/0.1 {default_user_agent()}"
         self.session.headers["Authorization"] = f"Bearer {token}"
-        self.options.set_validator("shots", (1, 200))
+        self.options.set_validator("shots", (1, 10_000))
 
     @property
     def target(self):
         return self._target
 
     @property
     def max_circuits(self):
```

### Comparing `oxionics_qiskit_provider-0.1/oxionics_qiskit_provider/job.py` & `oxionics_qiskit_provider-0.1.1/oxionics_qiskit_provider/job.py`

 * *Files identical despite different names*

### Comparing `oxionics_qiskit_provider-0.1/pyproject.toml` & `oxionics_qiskit_provider-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxionics-qiskit-provider"
-version = "0.1"
+version = "0.1.1"
 description = ""
 authors = ["Oxford Ionics"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "oxionics_qiskit_provider"}]
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 flake8 = "^4.0.1"
 pytest = "^6.2.5"
 black = {extras = ["jupyter"], version = "22.3.0"}
 pre-commit = "^2.17.0"
 matplotlib = "^3.6.3"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 
 [tool.lady_jessica]
 parent_branch = "parent_public-python"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `oxionics_qiskit_provider-0.1/setup.py` & `oxionics_qiskit_provider-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['qiskit-terra>=0.23.1,<0.24.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'oxionics-qiskit-provider',
-    'version': '0.1',
+    'version': '0.1.1',
     'description': '',
     'long_description': 'OxIonics Qiskit Provider\n========================\n\nA provider and backend for Qiskit, which executes quantum circuits on the\nOxford Ionics ion traps.\n\nUsage\n-----\n\nUnlike with most Qiskit backends, the Oxford Ionics backend doesn\'t require that\nthe circuit has been transpiled before being passed to `OxIonicsBackend.run`.\nThis is because the OxIonics API accepts arbitrary QASM.\n\n\n### Create a backend\n\nAn authentication token is required:\n\n```python\nfrom oxionics_qiskit_provider import OxIonicsProvider\n\nprovider = OxIonicsProvider("my_token")\nbackend = provider.get_backend()\n```\n\n### Run circuits on the backend\n\n```python\nfrom qiskit.circuit.random import random_circuit\n\nqx = random_circuit(1, 3)\n\njob = backend.run(qx)\nresults = job.results()\n```\n',
     'author': 'Oxford Ionics',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `oxionics_qiskit_provider-0.1/PKG-INFO` & `oxionics_qiskit_provider-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxionics-qiskit-provider
-Version: 0.1
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Oxford Ionics
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

