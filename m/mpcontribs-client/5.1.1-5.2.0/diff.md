# Comparing `tmp/mpcontribs-client-5.1.1.tar.gz` & `tmp/mpcontribs-client-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.1.1.tar", last modified: Sat Apr  1 01:13:04 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.2.0.tar", last modified: Wed Apr 26 20:00:15 2023, max compression
```

## Comparing `mpcontribs-client-5.1.1.tar` & `mpcontribs-client-5.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:13:03.999184 mpcontribs-client-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-01 01:13:03.995184 mpcontribs-client-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:13:03.983184 mpcontribs-client-5.1.1/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:13:03.987184 mpcontribs-client-5.1.1/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    80849 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:13:03.991184 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-01 01:13:03.000000 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-01 01:13:03.000000 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:13:03.000000 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:13:03.000000 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-01 01:13:03.000000 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-01 01:13:03.000000 mpcontribs-client-5.1.1/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:13:03.995184 mpcontribs-client-5.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 01:13:03.999184 mpcontribs-client-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:13:03.995184 mpcontribs-client-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-01 01:12:51.000000 mpcontribs-client-5.1.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.289482 mpcontribs-client-5.2.0/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.289482 mpcontribs-client-5.2.0/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    81148 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.289482 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-26 20:00:15.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:00:14.000000 mpcontribs-client-5.2.0/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:00:15.293482 mpcontribs-client-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-26 19:59:55.000000 mpcontribs-client-5.2.0/tests/test_client.py
```

### Comparing `mpcontribs-client-5.1.1/LICENSE` & `mpcontribs-client-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.1.1/PKG-INFO` & `mpcontribs-client-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.1.1
+Version: 5.2.0
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.1.1/README.md` & `mpcontribs-client-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.1.1/mpcontribs/client/__init__.py` & `mpcontribs-client-5.2.0/mpcontribs/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import plotly.io as pio
 import itertools
 import functools
 import requests
 import logging
 import datetime
 
+from math import isclose
 from semantic_version import Version
 from requests.exceptions import RequestException
 from bravado_core.param import Param
 from bson.objectid import ObjectId
 from typing import Union, Type, List
 from tqdm.auto import tqdm
 from hashlib import md5
@@ -278,14 +279,15 @@
 
 class Table(pd.DataFrame):
     """Wrapper class around pandas.DataFrame to provide display() and info()"""
     def display(self):
         """Display a plotly graph for the table if in IPython/Jupyter"""
         if _in_ipython():
             try:
+                # TODO make sure that attrs only contains valid kwargs
                 return self.plot(**self.attrs)
             except Exception as e:
                 logger.error(f"Can't display table: {e}")
 
         return self
 
     def info(self) -> Type[Dict]:
@@ -688,17 +690,19 @@
     def _get_per_page_default_max(self, op: str = "query", resource: str = "contributions") -> int:
         attr = f"{op}{resource.capitalize()}"
         resource = self.swagger_spec.resources[resource]
         param_spec = getattr(resource, attr).params["per_page"].param_spec
         return param_spec["default"], param_spec["maximum"]
 
     def _get_per_page(
-        self, per_page: int, op: str = "query", resource: str = "contributions"
+        self, per_page: int = -1, op: str = "query", resource: str = "contributions"
     ) -> int:
-        _, per_page_max = self._get_per_page_default_max(op=op, resource=resource)
+        per_page_default, per_page_max = self._get_per_page_default_max(op=op, resource=resource)
+        if per_page < 0:
+            per_page = per_page_default
         return min(per_page_max, per_page)
 
     def _split_query(
         self,
         query: dict,
         op: str = "query",
         resource: str = "contributions",
@@ -1092,23 +1096,25 @@
                 if existing_column:
                     # NOTE if existing_unit == "NaN":
                     #   it was set by omitting "unit" in new_column
                     new_unit = new_column.get("unit", "NaN")
                     existing_unit = existing_column.get("unit")
                     if existing_unit != new_unit:
                         try:
-                            ureg.Quantity(existing_unit).to(new_unit)
+                            factor = ureg.convert(1, ureg.Unit(existing_unit), ureg.Unit(new_unit))
                         except DimensionalityError:
                             return {
                                 "error": f"Can't convert {existing_unit} to {new_unit} for {path}"
                             }
 
-                        # TODO scale contributions to new unit
-                        return {"error": "Changing units not supported yet. Please resubmit"
-                                " contributions or update accordingly."}
+                        if not isclose(factor, 1):
+                            logger.info(f"Changing {existing_unit} to {new_unit} for {path} ...")
+                            # TODO scale contributions to new unit
+                            return {"error": "Changing units not supported yet. Please resubmit"
+                                    " contributions or update accordingly."}
 
                 new_columns.append(new_column)
 
         payload = {"columns": new_columns}
         valid, error = self._is_valid_payload("Project", payload)
         if not valid:
             return {"error": error}
@@ -1584,16 +1590,14 @@
 
         return ret
 
     def submit_contributions(
         self,
         contributions: List[dict],
         ignore_dupes: bool = False,
-        retry: bool = False,
-        per_request: int = 100,
         timeout: int = -1,
         skip_dupe_check: bool = False
     ):
         """Submit a list of contributions
 
         Example for a single contribution dictionary:
 
@@ -1613,29 +1617,26 @@
         contribution `id`s in the above dictionary and only including fields that need
         updating. Set list entries to `None` for components that are to be left untouched
         during an update.
 
         Args:
             contributions (list): list of contribution dicts to submit
             ignore_dupes (bool): force duplicate components to be submitted
-            retry (bool): keep trying until all contributions successfully submitted
-            per_request (int): number of contributions to submit per request
             timeout (int): cancel remaining requests if timeout exceeded (in seconds)
             skip_dupe_check (bool): skip duplicate check for contribution identifiers
         """
         if not contributions or not isinstance(contributions, list):
             logger.error("Please provide list of contributions to submit.")
             return
 
         # get existing contributions
         tic = time.perf_counter()
         project_names = set()
         collect_ids = []
         require_one_of = {"data"} | set(COMPONENTS)
-        per_page = self._get_per_page(per_request)
 
         for idx, c in enumerate(contributions):
             has_keys = require_one_of & c.keys()
             if not has_keys:
                 return {"error": f"Nothing to submit for contribution #{idx}!"}
             elif not all(c[k] for k in has_keys):
                 for k in has_keys:
@@ -1808,14 +1809,15 @@
 
                 valid, error = self._is_valid_payload("Contribution", contribs[project_name][-1])
                 if not valid:
                     return {"error": f"{contrib['identifier']} invalid: {error}!"}
 
         # submit contributions
         if contribs:
+            per_page = self._get_per_page()
             total, total_processed = 0, 0
 
             def post_future(track_id, payload):
                 future = self.session.post(
                     f"{self.url}/contributions/",
                     headers=self.headers,
                     hooks={'response': _response_hook},
@@ -1870,36 +1872,38 @@
                                     f"SKIPPED {project_name}/{idx}: too large, reduce per_request"
                                 )
 
                     if not futures:
                         break  # nothing to do
 
                     responses = _run_futures(
-                        futures, total=ncontribs, timeout=timeout, desc="Submit"
+                        futures, total=ncontribs-total_processed, timeout=timeout, desc="Submit"
                     )
                     processed = sum(r.get("count", 0) for r in responses.values())
                     total_processed += processed
 
-                    if processed != ncontribs and retry and retries < RETRIES and \
+                    if total_processed != ncontribs and retries < RETRIES and \
                             unique_identifiers.get(project_name):
+                        logger.info(f"{total_processed}/{ncontribs} processed -> retrying ...")
                         existing[project_name] = self.get_all_ids(
                             dict(project=project_name), include=COMPONENTS, timeout=timeout
                         ).get(project_name, {"identifiers": set()})
                         unique_identifiers[project_name] = self.projects.getProjectByName(
                             pk=project_name, _fields=["unique_identifiers"]
                         ).result()["unique_identifiers"]
                         existing_ids = existing.get(project_name, {}).get("identifiers", [])
                         contribs[project_name] = [
                             c for c in contribs[project_name]
                             if c["identifier"] not in existing_ids
                         ]
+                        per_page = int(per_page / 2)
                         retries += 1
                     else:
                         contribs[project_name] = []  # abort retrying
-                        if processed != ncontribs and retry:
+                        if total_processed != ncontribs:
                             if retries >= RETRIES:
                                 logger.error(f"{project_name}: Tried {RETRIES} times - abort.")
                             elif not unique_identifiers.get(project_name):
                                 logger.info(
                                     f"{project_name}: resubmit failed contributions manually"
                                 )
```

### Comparing `mpcontribs-client-5.1.1/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.2.0/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.1.1
+Version: 5.2.0
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.1.1/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.2.0/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.1.1/requirements/deployment.txt` & `mpcontribs-client-5.2.0/requirements/deployment.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=MPContribs/mpcontribs-client/requirements/deployment.txt --resolver=backtracking MPContribs/mpcontribs-client/setup.py python/requirements.txt
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
-attrs==22.2.0
+attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 bravado==11.0.3
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
@@ -74,61 +74,61 @@
     # via
     #   -r python/requirements.txt
     #   pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.32.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.21.6
     # via
     #   -r python/requirements.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.3
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.1
     # via
     #   -r python/requirements.txt
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -136,15 +136,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -191,15 +191,15 @@
     # via ruamel-yaml
 scipy==1.10.1
     # via
     #   -r python/requirements.txt
     #   pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -236,14 +236,16 @@
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
     # via jsonschema
 backcall==0.2.0
@@ -48,14 +46,18 @@
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
@@ -74,59 +76,61 @@
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -134,15 +138,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -151,14 +155,15 @@
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -186,15 +191,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -228,25 +233,30 @@
     # via
     #   ipython
     #   matplotlib-inline
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
+    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
+zipp==3.15.0
+    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.1.1/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
@@ -58,14 +54,16 @@
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
@@ -88,60 +86,60 @@
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
@@ -161,43 +159,44 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.3.3
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -225,15 +224,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -271,25 +270,30 @@
     # via
     #   ipython
     #   matplotlib-inline
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
+    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
+zipp==3.15.0
+    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.1.1/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.2.0/requirements/macos-latest_py3.8.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
@@ -78,61 +78,61 @@
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -140,15 +140,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -157,14 +157,15 @@
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -192,15 +193,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -238,14 +239,16 @@
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.2.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
@@ -59,17 +57,15 @@
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
@@ -92,62 +88,60 @@
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
@@ -167,43 +161,44 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.3.3
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -231,15 +226,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -281,14 +276,16 @@
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.2.0/requirements/macos-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
@@ -76,59 +76,59 @@
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -136,15 +136,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -153,14 +153,15 @@
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -188,15 +189,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -234,14 +235,16 @@
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.2.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
@@ -59,15 +57,17 @@
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via matplotlib
+    # via
+    #   jsonschema
+    #   matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
@@ -90,60 +90,62 @@
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
@@ -163,43 +165,44 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.3.3
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -227,15 +230,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -277,14 +280,16 @@
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.2.0/requirements/macos-latest_py3.10.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
     # via jsonschema
 backcall==0.2.0
@@ -72,59 +74,59 @@
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -132,15 +134,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -149,14 +151,15 @@
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -184,15 +187,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -229,14 +232,16 @@
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.2.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
@@ -86,60 +86,60 @@
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
@@ -159,43 +159,44 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.3.3
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -223,15 +224,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -272,14 +273,16 @@
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
     # via jsonschema
@@ -47,17 +47,15 @@
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via matplotlib
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
@@ -76,61 +74,59 @@
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -138,15 +134,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -155,14 +151,15 @@
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -190,15 +187,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -236,14 +233,16 @@
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
@@ -90,62 +88,62 @@
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
@@ -165,43 +163,44 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.3.3
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -229,15 +228,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -279,14 +278,16 @@
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
```

### Comparing `mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
     # via jsonschema
@@ -46,16 +46,14 @@
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via matplotlib
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
@@ -74,59 +72,59 @@
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -134,15 +132,15 @@
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pydantic==1.10.7
     # via emmet-core
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
@@ -151,14 +149,15 @@
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -186,15 +185,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -228,28 +227,27 @@
     # via
     #   ipython
     #   matplotlib-inline
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
-    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
-    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.1.1/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.2.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==22.2.0
-    # via
-    #   jsonschema
-    #   pytest
+    # via jsonschema
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.2
+coverage[toml]==7.2.3
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
@@ -56,16 +54,14 @@
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.12.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
@@ -88,60 +84,60 @@
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2022.9.9
+monty==2023.4.10
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
-mp-api==0.30.11
+mp-api==0.31.0
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via pymatgen
 numpy==1.24.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
-palettable==3.3.0
+palettable==3.3.1
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.0
+plotly==5.14.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
@@ -161,43 +157,44 @@
     # via
     #   flake8
     #   pytest-pycodestyle
 pydantic==1.10.7
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.0
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.3.3
     # via mpcontribs-client (setup.py)
 pyparsing==3.0.9
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
+    #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
@@ -225,15 +222,15 @@
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
-simplejson==3.18.4
+simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
@@ -271,28 +268,27 @@
     # via
     #   ipython
     #   matplotlib-inline
 typing-extensions==4.5.0
     # via
     #   bravado
     #   emmet-core
-    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
+tzdata==2023.3
+    # via pandas
 ujson==5.7.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
-    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.1.1/setup.py` & `mpcontribs-client-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.1.1/tests/test_client.py` & `mpcontribs-client-5.2.0/tests/test_client.py`

 * *Files identical despite different names*

