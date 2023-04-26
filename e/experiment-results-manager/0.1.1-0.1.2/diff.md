# Comparing `tmp/experiment-results-manager-0.1.1.tar.gz` & `tmp/experiment-results-manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-results-manager-0.1.1.tar", max compression
+gzip compressed data, was "experiment-results-manager-0.1.2.tar", max compression
```

## Comparing `experiment-results-manager-0.1.1.tar` & `experiment-results-manager-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1230 2023-04-20 06:37:34.398517 experiment-results-manager-0.1.1/README.md
--rw-r--r--   0        0        0      446 2023-04-18 23:12:08.840015 experiment-results-manager-0.1.1/experiment_results_manager/__init__.py
--rw-r--r--   0        0        0      797 2023-04-18 18:29:37.900015 experiment-results-manager-0.1.1/experiment_results_manager/artifact.py
--rw-r--r--   0        0        0     4518 2023-04-21 13:57:29.047715 experiment-results-manager-0.1.1/experiment_results_manager/compare_runs.py
--rw-r--r--   0        0        0     7677 2023-04-20 18:52:12.869094 experiment-results-manager-0.1.1/experiment_results_manager/experiment_run.py
--rw-r--r--   0        0        0     2051 2023-04-21 11:34:09.217133 experiment-results-manager-0.1.1/experiment_results_manager/html_util.py
--rw-r--r--   0        0        0     3615 2023-04-18 23:45:16.069628 experiment-results-manager-0.1.1/experiment_results_manager/serde.py
--rw-r--r--   0        0        0     1161 2023-04-21 16:04:48.185974 experiment-results-manager-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1992 2023-04-21 16:05:04.075236 experiment-results-manager-0.1.1/setup.py
--rw-r--r--   0        0        0     1973 2023-04-21 16:05:04.075391 experiment-results-manager-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-25 09:20:08.302560 experiment-results-manager-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1686 2023-04-25 17:20:34.969344 experiment-results-manager-0.1.2/README.md
+-rw-r--r--   0        0        0      616 2023-04-25 17:07:55.897142 experiment-results-manager-0.1.2/experiment_results_manager/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-18 18:29:37.900015 experiment-results-manager-0.1.2/experiment_results_manager/artifact.py
+-rw-r--r--   0        0        0     4713 2023-04-25 11:35:20.853711 experiment-results-manager-0.1.2/experiment_results_manager/compare_runs.py
+-rw-r--r--   0        0        0     7485 2023-04-25 09:20:08.320822 experiment-results-manager-0.1.2/experiment_results_manager/experiment_run.py
+-rw-r--r--   0        0        0      689 2023-04-25 17:33:12.573156 experiment-results-manager-0.1.2/experiment_results_manager/fsspec_util.py
+-rw-r--r--   0        0        0     2245 2023-04-25 11:35:03.544235 experiment-results-manager-0.1.2/experiment_results_manager/html_util.py
+-rw-r--r--   0        0        0     4973 2023-04-25 17:12:00.878226 experiment-results-manager-0.1.2/experiment_results_manager/registry.py
+-rw-r--r--   0        0        0     7276 2023-04-25 17:31:34.280834 experiment-results-manager-0.1.2/experiment_results_manager/serde.py
+-rw-r--r--   0        0        0     1192 2023-04-25 17:22:34.287073 experiment-results-manager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2451 2023-04-25 17:39:22.033933 experiment-results-manager-0.1.2/setup.py
+-rw-r--r--   0        0        0     2429 2023-04-25 17:39:22.034117 experiment-results-manager-0.1.2/PKG-INFO
```

### Comparing `experiment-results-manager-0.1.1/experiment_results_manager/artifact.py` & `experiment-results-manager-0.1.2/experiment_results_manager/artifact.py`

 * *Files identical despite different names*

### Comparing `experiment-results-manager-0.1.1/experiment_results_manager/compare_runs.py` & `experiment-results-manager-0.1.2/experiment_results_manager/compare_runs.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from plotly.offline import get_plotlyjs
 
 from experiment_results_manager.artifact import ArtifactType
 from experiment_results_manager.experiment_run import ExperimentRun
 from experiment_results_manager.html_util import (
     dicts_to_html_table,
     human_readable_bytes,
-    timestamps_to_html_table,
 )
 
 
 def compare_runs(*runs: ExperimentRun, **kwargs: Dict[str, Any]) -> str:
     """
     Returns an HTML string containing tables of experiment runs, their parameters,
     metrics, and artifacts.
@@ -33,19 +32,26 @@
         html += (
             "<style>table{text-align:center}th{background-color:#ddd;color:#000}"
             "tr:nth-child(odd){background-color:#e7e6e6;color:#000}tr:nth-child(2n)"
             "{background-color:#fff;color:#000}tr:hover{background-color:#d1eaff}tbo"
             "dy{font-family:monospace;font-weight:400}</style>"
         )
 
-    html += timestamps_to_html_table(
-        [er.experiment_id for er in runs],
-        [er.variant_id for er in runs],
-        [er.run_id for er in runs],
-        [er.timestamp_utc for er in runs],
+    html += dicts_to_html_table(
+        "Metadata",
+        [
+            {
+                "Experiment id": er.experiment_id,
+                "Variant id": er.variant_id,
+                "Run id": er.run_id,
+                "Timestamp (UTC)": er.timestamp_utc.strftime("%Y-%m-%d %H:%M:%S"),
+            }
+            for er in runs
+        ],
+        sort_keys=["Experiment id", "Variant id", "Run id", "Timestamp (UTC)"],
     )
     html += dicts_to_html_table("Params", [er.params for er in runs])
     html += dicts_to_html_table(
         "Features",
         [_feature_list_to_dict(er) for er in runs],
     )
     html += dicts_to_html_table("Metrics", [er.metrics for er in runs])
```

### Comparing `experiment-results-manager-0.1.1/experiment_results_manager/experiment_run.py` & `experiment-results-manager-0.1.2/experiment_results_manager/experiment_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,46 +11,40 @@
 
 
 class ExperimentRun:
     """
     Example usage:
     ```python
     import experiment_results_manager as erm
-    from IPython.display import display, HTML
-    import seaborn as sns
-
-    # Creating arbitrary plot to log later
-    tips = sns.load_dataset('tips')
-    mpl_fig = sns.barplot(x='day', y='total_bill', data=tips)
 
     # Create an experiment run
     er = erm.ExperimentRun(
         experiment_id="my_experiment",
         variant_id="main"
     )
 
     # Log relevant data
     er.log_param("objective", "rmse")
     er.log_metric("rmse", "0.9")
     er.log_figure(mpl_fig, "ROC Curve")
     er.log_text("lorem ipsum...", "text")
+    er.log_artifact(
+        pickle.dumps(model),
+        artifact_id="model",
+        filename="model.pickle"
+    )
 
-    # Generate HTML
+    # Display the run
     html = erm.compare_runs(er)
+    # Or compare side by side with other runs
+    html = erm.compare_runs(er, er2, er3)
     display(HTML(html))
 
     # Save the run to access later
-    saved_path = erm.save_run_to_registry(er, "s3:///erm-registry")
-
-    # Load a previous run
-    er2 = erm.load_run_from_path(saved_path)
-
-    # Compare the current run with a previous one
-    html = erm.compare_runs(er, er2)
-    display(HTML(html))
+    saved_path = erm.save_run_to_registry(er, "s3://erm-registry")
     ```
     """
 
     def __init__(
         self,
         experiment_id: str,
         variant_id: str = "main",
```

### Comparing `experiment-results-manager-0.1.1/experiment_results_manager/html_util.py` & `experiment-results-manager-0.1.2/experiment_results_manager/html_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 from datetime import datetime
 from typing import Any, Dict, List, Set, Union
 
 import matplotlib.axes
 import matplotlib.figure
 
 
-def dicts_to_html_table(dict_name: str, data: List[Dict[str, Any]]) -> str:
+def dicts_to_html_table(
+    dict_name: str, data: List[Dict[str, Any]], sort_keys: Union[bool, List[str]] = True
+) -> str:
     # Get all the unique keys from all the dictionaries
-    keys: Set[str] = set()
-    for d in data:
-        keys.update(d.keys())
-    keys_list = list(keys)
-    keys_list.sort()
+    if type(sort_keys) == list:
+        keys_list = sort_keys
+    else:
+        keys: Set[str] = set()
+        for d in data:
+            keys.update(d.keys())
+        keys_list = list(keys)
+        if type(sort_keys) == bool and sort_keys:
+            keys_list.sort()
 
     if len(keys_list) == 0:
         return ""
 
     # Create the table heading & header row
     html = f"<h3>{dict_name}</h3>"
     html += "<table><tr><th></th>"
```

### Comparing `experiment-results-manager-0.1.1/pyproject.toml` & `experiment-results-manager-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "experiment-results-manager"
-version = "0.1.1"
+version = "0.1.2"
 description = "Light-weight experiment tracker"
 authors = ["sa- <name@example.com>"]
 repository = "https://github.com/ml-cyclops/experiment-results-manager"
 documentation = "https://github.com/ml-cyclops/experiment-results-manager/blob/main/README.md"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -33,14 +33,17 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
+[tool.ruff]
+line-length = 120
+
 [[tool.mypy.overrides]]
 module = "plotly.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "matplotlib.*"
 ignore_missing_imports = true
```

