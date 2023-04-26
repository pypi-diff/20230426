# Comparing `tmp/krisi-0.1.0.tar.gz` & `tmp/krisi-0.1.1.tar.gz`

## Comparing `krisi-0.1.0.tar` & `krisi-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,46 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.0/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.0/.isort.cfg
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 krisi-0.1.0/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0   106892 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/a_full_rundown_notebook.ipynb
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_df.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_loading.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_pdf_report.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_report_rolling.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_saving.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/basic_scorecard.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/compare_classification.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/compare_regression.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/default_metric_selection.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/extended_scorecard.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/loading_generating_report.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_classification.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_html_report.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_pdf_report.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/minimal_regression.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/printing_methods.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 krisi-0.1.0/examples/training_arima_report.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/dataset.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    15797 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/console.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/report.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/type.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/default/template.css
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/default/template.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/data.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/io.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/modeling_types.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/models.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/printing.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 krisi-0.1.0/src/krisi/utils/runner.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 krisi-0.1.0/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.0/LICENSE
--rw-r--r--   0        0        0    27699 2020-02-02 00:00:00.000000 krisi-0.1.0/README.md
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 krisi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    32200 2020-02-02 00:00:00.000000 krisi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.1/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.1/.isort.cfg
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 krisi-0.1.1/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/dataset.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/type.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/default/template.css
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/default/template.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.1/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.1/LICENSE
+-rw-r--r--   0        0        0    27691 2020-02-02 00:00:00.000000 krisi-0.1.1/README.md
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 krisi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    32385 2020-02-02 00:00:00.000000 krisi-0.1.1/PKG-INFO
```

### Comparing `krisi-0.1.0/.vscode/settings.json` & `krisi-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/evaluate/assertions.py` & `krisi-0.1.1/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/evaluate/compare.py` & `krisi-0.1.1/src/krisi/evaluate/compare.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,31 @@
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 import pandas as pd
 
 from krisi.evaluate.scorecard import ScoreCard
+from krisi.evaluate.utils import handle_empty_metrics_to_display
 from krisi.utils.printing import bold
 
 
-def __handle_empty_metrics_to_display(
-    scorecard: ScoreCard, sort_by: Optional[str], metric_keys: Optional[List[str]]
-) -> Tuple[List[str], Optional[str]]:
-    if metric_keys is None:
-        metric_keys = [
-            metric.key
-            for metric in scorecard.get_all_metrics(only_evaluated=True)
-            if isinstance(metric.result, (float, int))
-        ]
-
-    if sort_by is not None:
-        if sort_by not in metric_keys:
-            metric_keys.insert(0, sort_by)
-        else:
-            metric_keys.remove(sort_by)
-            metric_keys.insert(0, sort_by)
-
-    else:
-        sort_by = metric_keys[0]
-    return metric_keys, sort_by
-
-
 def compare(
     scorecards: List[ScoreCard],
     metric_keys: Optional[List[str]] = None,
     sort_by: Optional[str] = None,
     dataframe: bool = True,
 ) -> Union[pd.DataFrame, str]:
     """Creates a table where each column is a metric and each row is
     a scorecard and its corresponding results.
 
     Parameters
     ----------
     scorecards : List[ScoreCard]
         ScoreCards to compare.
     metric_keys : Optional[List[str]], optional
-        List of metrics to dispaly. If not set it will return all
+        List of metrics to display. If not set it will return all
         evaluated metrics on the first scorecard.
         Sorts the results by the first element of this list if `sort_by` is not specified., by default None
     sort_by : Optional[str], optional
         `Metric` to sort results by. Selected `Metric` will be displayed in the first row.
         If not specified metrics will be sorted by the first element of `metric_keys`.
         If `metric_keys` is not specified it will default to the first metric found on the first `ScoreCard`, by default None
     dataframe : bool, optional
@@ -54,15 +33,15 @@
 
     Returns
     -------
     Union[pd.DataFrame, str]
         A comparison table, either in `pd.DataFrame` or `string` format.
     """
 
-    metric_keys, sort_by = __handle_empty_metrics_to_display(
+    metric_keys, sort_by = handle_empty_metrics_to_display(
         scorecards[0], sort_by, metric_keys
     )
 
     scorecards.sort(reverse=True, key=lambda x: x[sort_by].result)
     if dataframe:
         return pd.concat(
             [
```

### Comparing `krisi-0.1.0/src/krisi/evaluate/metric.py` & `krisi-0.1.1/src/krisi/evaluate/metric.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,79 @@
 import logging
 from dataclasses import dataclass, field
 from typing import Any, Generic, List, Optional, Union
 
-from krisi.evaluate.assertions import check_valid_pred_target
+import pandas as pd
+
 from krisi.evaluate.type import (
     ComputationalComplexity,
     MetricCategories,
     MetricFunction,
     MetricResult,
     Predictions,
+    PredictionsDS,
     SampleTypes,
     Targets,
+    TargetsDS,
 )
 from krisi.report.console import print_metric
 from krisi.report.type import InteractiveFigure, PlotFunction, plotly_interactive
 from krisi.utils.iterable_helpers import isiterable, string_to_id
 
 
 @dataclass
 class Metric(Generic[MetricResult]):
+    """
+    Class representing a metric.
+
+    Parameters
+    ----------
+    name: str
+        The name of the metric.
+    key: str
+        The key used to reference the metric.
+    category: MetricCategories
+        The category of the metric.
+    result: Optional[Union[Exception, MetricResult, List[MetricResult]]]
+        The result of the evaluated `Metric`, by default None
+    result_rolling: Optional[Union[Exception, MetricResult, List[MetricResult]]]
+        The result of the evaluated `Metric` over time, by default None
+    parameters: dict
+        The paramaters that are passed into the evaluation function (param: `func`), by default field(default_factory=dict)
+    func: Callable
+        The function used to compute the metric.
+    plot_funcs: List[Callable]
+        List of functions used to plot the metric.
+    plot_func_rolling: Callable
+        Function used to plot the rolling metric value.
+    info: str
+        Additional information about the metric.
+    restrict_to_sample: Optional[SampleTypes]
+        Weather the `Metric` should only be evaluated on insample or out of sample data, by default None
+    comp_complexity: Optional[ComputationalComplexity]
+        How resource intensive the calculation is, by default None
+    disable_rolling: bool
+        Whether the metric should not be evaluated on a rolling basis, by default False
+        If this is switched on, the metric will still be evaluated when `evaluate_over_time` is called
+        but not on a rolling basis.
+    """
+
     name: str
     key: str = ""
     category: Optional[MetricCategories] = None
     result: Optional[Union[Exception, MetricResult, List[MetricResult]]] = None
     result_rolling: Optional[Union[Exception, MetricResult, List[MetricResult]]] = None
     parameters: dict = field(default_factory=dict)
-    func: MetricFunction = lambda x, y: None
+    func: Optional[MetricFunction] = None
     plot_funcs: Optional[List[PlotFunction]] = None
     plot_func_rolling: Optional[PlotFunction] = None
     info: str = ""
     restrict_to_sample: Optional[SampleTypes] = None
     comp_complexity: Optional[ComputationalComplexity] = None
+    disable_rolling: bool = False
 
     def __post_init__(self):
         if self.key == "":
             self.key = string_to_id(self.name)
 
     def __setitem__(self, key: str, item: Any) -> None:
         setattr(self, key, item)
@@ -44,46 +83,55 @@
 
     def __str__(self) -> str:
         return print_metric(self)
 
     def __repr__(self) -> str:
         return print_metric(self, repr=True)
 
-    def evaluate(self, y: Targets, predictions: Predictions) -> None:
-        check_valid_pred_target(y, predictions)
-
+    def _evaluation(self, *args) -> "Metric":
         try:
-            result = self.func(y, predictions, **self.parameters)
+            result = self.func(*args, **self.parameters)
         except Exception as e:
             result = e
         self.__safe_set(result, key="result")
+        return self
+
+    def evaluate(self, y: Targets, predictions: Predictions) -> None:
+        assert (
+            self.func is not None
+        ), "`func` has to be set on Metric to calculate result."
+
+        self._evaluation(y, predictions)
+
+    def _rolling_evaluation(self, *args, rolling_args: dict) -> "Metric":
+        if self.disable_rolling:
+            self._evaluation(*args)
+        else:
+            _df = pd.concat(args, axis="columns")
+            try:
+                df_rolled = (
+                    _df.expanding()
+                    if rolling_args["window"] is None
+                    else _df.rolling(**rolling_args)
+                )
 
-    def evaluate_over_time(
-        self, y: Targets, predictions: Predictions, window: Optional[int] = None
-    ) -> None:
-        try:
-            if window:
-                result_rolling = [
-                    self.func(
-                        y[i : i + window],
-                        predictions[i : i + window],
-                        **self.parameters,
-                    )
-                    for i in range(0, len(y) - 1, window)
-                ]
-            else:
-                # expanding
                 result_rolling = [
-                    self.func(y[: i + 1], predictions[: i + 1], **self.parameters)
-                    for i in range(len(y) - 1)
+                    self.func(*single_window.values.T, **self.parameters)
+                    for single_window in df_rolled
                 ]
-        except Exception as e:
-            result_rolling = e
+            except Exception as e:
+                result_rolling = e
+            self.__safe_set(result_rolling, key="result_rolling")
+
+        return self
 
-        self.__safe_set(result_rolling, key="result_rolling")
+    def evaluate_over_time(
+        self, y: TargetsDS, predictions: PredictionsDS, rolling_args: dict
+    ) -> None:
+        self._rolling_evaluation(y, predictions, rolling_args=rolling_args)
 
     def is_evaluated(self, rolling: bool = False):
         if rolling:
             return self.result_rolling is not None
         else:
             return self.result is not None
```

### Comparing `krisi-0.1.0/src/krisi/evaluate/scorecard.py` & `krisi-0.1.1/src/krisi/evaluate/scorecard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import datetime
 from copy import deepcopy
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Union
 
+import numpy as np
 import pandas as pd
+from IPython.display import display
 from rich import print
 from rich.pretty import Pretty
 
-from krisi.evaluate.assertions import is_dataset_classification_like
+from krisi.evaluate.assertions import (
+    check_valid_pred_target,
+    is_dataset_classification_like,
+)
+from krisi.evaluate.group import Group
 from krisi.evaluate.library.default_metrics_classification import (
     all_classification_metrics,
 )
 from krisi.evaluate.library.default_metrics_regression import all_regression_metrics
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import (
     MetricCategories,
@@ -28,49 +34,109 @@
 from krisi.report.console import (
     get_large_metric_summary,
     get_minimal_summary,
     get_summary,
 )
 from krisi.report.report import create_report_from_scorecard
 from krisi.report.type import DisplayModes, InteractiveFigure
+from krisi.utils.environment import is_notebook
 from krisi.utils.io import save_console, save_minimal_summary, save_object
 from krisi.utils.iterable_helpers import (
     flatten,
     map_newdict_on_olddict,
     remove_nans,
     strip_builtin_functions,
     wrap_in_list,
 )
 
 
+def convert_to_series(
+    data: Union[List[float], List[int], pd.Series, np.ndarray], name: str
+) -> pd.Series:
+    """Converts a list[floats or ints] or a numpy array to a pandas Series.
+
+    Parameters
+    ----------
+    data : Union[List[float], List[int], pd.Series, np.ndarray]
+        The data to convert.
+
+    Returns
+    -------
+    pd.Series
+        The converted data.
+    """
+    if isinstance(data, pd.Series):
+        return data.rename(name)
+    return pd.Series(data, name=name)
+
+
 @dataclass
 class ScoreCard:
-    """ScoreCard Object.
+    """
+    ScoreCard Object.
 
     Krisi's main object holding and evaluating metrics.
     Stores, evaluates and generates vizualisations of predefined
     and custom metrics for regression and classification.
 
+    Parameters
+    -------
+    y: Targets
+        True Targets to which the metrics are evaluated to.
+    predictions: Predictions
+        The single point predictions to which the metrics are evaluated to.
+    model_name: Optional[str]
+        The name of the model that the predictions were generated by. Used for identifying scorecards.
+    model_description: str
+        A description of the model that the predictions were generated by. Used for reporting.
+    dataset_name: Optional[str]
+        The name of the dataset from which the `y` (targets) orginate from. Used for reporting.
+    dataset_description: str = ""
+        A description of the dataset from which the `y` (targets) orginate from. Used for reporting.
+    project_name: Optional[str]
+        The name of the project. Used for reporting and saving to a directory (eg.: multiple scorecards)
+    project_description: str = ""
+        A description of the project. Used for reporting.
+    classification: Optional[bool]
+        Whether the task was classifiction of regression. If set to `None` it will guess from the targets.
+    sample_type: SampleTypes = SampleTypes.outofsample
+        Whether we should evaluate it on insample or out of sample.
+
+            - `SampleTypes.outofsample`
+            - `SampleTypes.insample`
+    default_metrics: Optional[List[Metric]]
+        Default metrics that get evaluated. See `library`.
+    custom_metrics: Optional[List[Metric]]
+        Custom metrics that get evaluated. If specified it will evaluate these after `default_metric`
+        See `library`.
+    rolling_args : Dict[str, Any], optional
+        Arguments to be passed onto `pd.DataFrame.rolling`.
+        Default:
+
+        - The window size of the rolling metric evaluation. If `None` evaluation over time will be on expanding window basis, by default `None`.
+        - The step size of the rolling metric evaluation, by default `1`.
+
     Examples
     --------
     >>> from krisi import ScoreCard
     ... y_pred, y_true = [0, 2, 1, 3], [0, 1, 2, 3]
     ... sc = ScoreCard()
     ... sc.evaluate(y_pred, y_true, defaults=True) # Calculate predefined metrics
     ... sc["own_metric"] = (y_pred - y_true).mean() # Add a metric result directly
-    ... sc.print('extended')
+    ... sc.print()
     """
 
     y: Targets
     predictions: Predictions
     sample_type: SampleTypes
     default_metrics_keys: List[str]
     custom_metrics_keys: List[str]
     classification: bool  # TODO: Support multilabel classification
     metadata: ScoreCardMetadata
+    rolling_args: Dict[str, Any]
 
     def __init__(
         self,
         y: Targets,
         predictions: Predictions,
         model_name: Optional[str] = None,
         model_description: str = "",
@@ -78,18 +144,25 @@
         dataset_description: str = "",
         project_name: Optional[str] = None,
         project_description: str = "",
         classification: Optional[bool] = None,
         sample_type: SampleTypes = SampleTypes.outofsample,
         default_metrics: Optional[List[Metric]] = None,
         custom_metrics: Optional[List[Metric]] = None,
+        rolling_args: Optional[Dict[str, Any]] = None,
     ) -> None:
-        self.__dict__["y"] = y
-        self.__dict__["predictions"] = predictions
+        check_valid_pred_target(y, predictions)
+        self.__dict__["y"] = convert_to_series(y, "y")
+        self.__dict__["predictions"] = convert_to_series(predictions, "predictions")
         self.__dict__["sample_type"] = sample_type
+        self.__dict__["rolling_args"] = (
+            rolling_args
+            if rolling_args is not None
+            else dict(window=len(y) // 100, step=len(y) // 100)
+        )
         self.__dict__["classification"] = (
             is_dataset_classification_like(y)
             if classification is None
             else classification
         )
         model_name_, dataset_name_, project_name_ = handle_unnamed(
             y, predictions, model_name, dataset_name, project_name
@@ -145,48 +218,50 @@
         del self[key]
 
     def __str__(self) -> str:
         print(Pretty(self.__dict__))
         return ""
 
     def __setattr__(self, key: str, item: Any) -> None:
-        """Defines Dictionary like behaviour and ensures that a Metric can be
-        added as a
-            - Metric object,
-            - Dictionary,
-            - Direct result (float, int or a List of float or int). Gets wrapped in a ``Metric`` object
+        """
+        Defines Dictionary like behaviour and ensures that a Metric can be
+        added as a:
 
-        See examples for behaviour.
+            - `Metric` object,
+            - Dictionary,
+            - Direct result (float, int or a List of float or int). Gets wrapped in a `Metric` object
 
         Parameters
         ----------
         key : string
-            The key to which the object will be assign to on this object
-
+            The key to which the object will be assigned to.
         item : Dictionary, Metric, Float, Int or List of Float or Int, or pd.Series
-            Always ignored, exists for compatibility.
+            The result that gets stored with the key. Depending on the type of object it will result in
+            different behaviours:
 
-        Returns
-        -------
-        None
+                - If `Metric` or `Dict` it will store the object on `ScoreCard[key]`
+                - If (`Float`, `Int`, `List of Float`, `List of Int`, `pd.Series`) it will check if a `Metric` on `key`
+                already exists on `ScoreCard`. If yes, it will assign item to the result field of the
+                existing `Metric`. If not it will wrap the item in a new `Metric` first then assign it to
+                `ScoreCard[key]`.
 
         Examples
         --------
         >>> from krisi import ScoreCard
         ... sc = ScoreCard()
         ... sc['metric_result'] = 0.53 # Direct result assignment as a Dictionary
         Metric(result=0.53, key='metric_result', category=None, parameters=None, info="", ...)
 
         >>> sc.another_metric_result = 1 # Direct object assignment
         Metric(result=1, key='another_metric_result', category=None, parameters=None, info="", ...)
 
         >>> from krisi.evaluate.metric import Metric
         ... from krisi.evaluate.type import MetricCategories
-        ... sc.full_metric = Metric("My own metric", category=MetricCategories.class_err, info="A fictious metric with metadata")
-        Metric("My own metric", key="my_own_metric", func: lambda y, y_hat: (y - y_hat)/2, category=MetricCategories.class_err, info="A fictious metric with metadata", ...)
+        ... sc.full_metric = Metric("My own metric", category=MetricCategories.class_err, info="A fictious metric with metadata", func: lambda y, y_hat: (y - y_hat)/2)
+        Metric("My own metric", key="my_own_metric", category=MetricCategories.class_err, info="A fictious metric with metadata", ...)
 
         >>> sc.metric_as_dictionary = {name: "My other metric", info: "A Metric created with a dictionary", func: lambda y, y_hat: y - y_hat}
         Metric("My other metric", key="my_other_metric", info="A Metric created with a dictionary", ...)
 
         """
         metric = getattr(self, key, None)
 
@@ -214,42 +289,51 @@
                 )
                 self.__dict__[key] = Metric(**metric_dict)
             else:
                 metric["result"] = item
                 self.__dict__[key] = metric
 
     def get_ds(self) -> pd.Series:
+        """
+        Returns a `pd.Series` where each index is the name of a `Metric` and
+        the value is the corresponding `result`
+
+        Returns
+        -------
+        pd.Series
+        """
         metrics = [
             metric
             for metric in self.get_all_metrics()
             if not isinstance(metric.result, Iterable)
         ]
 
         return pd.Series(
-            [metric.result for metric in metrics],
-            index=[metric.name for metric in metrics],
+            [metric["result"] for metric in metrics],
+            index=[metric["name"] for metric in metrics],
         )
 
     def get_default_metrics(self) -> List[Metric]:
-        """Returns a List of Predefined Metrics according to task type:
+        """
+        Returns a List of Predefined Metrics according to task type:
         regression, classification, multi-label classification.
 
-
         Returns
         -------
         List of Metrics
         """
         return [
             self.__dict__[key]
             for key in self.default_metrics_keys
             if key in self.__dict__
         ]
 
     def get_custom_metrics(self) -> List[Metric]:
-        """Returns a List of Custom ``Metric``s defined by the user on initalization
+        """
+        Returns a List of Custom ``Metric``s defined by the user on initalization
         of the ``ScoreCard``
 
         Returns
         -------
         List of Metrics
         """
         predifined_custom_metrics = [
@@ -265,79 +349,98 @@
         ]
 
         return predifined_custom_metrics + modified_custom_metrics
 
     def get_all_metrics(
         self, defaults: bool = True, only_evaluated: bool = False
     ) -> List[Metric]:
+        """
+        Helper function that returns both `default_metrics` and `custom_metrics`.
+
+        Parameters
+        -------
+        only_evaluated: bool
+            Only return `Metric`s that were already evaluated
+        defauls: bool
+            Whether `default_metrics` should be return or not.
+
+        Returns
+        -------
+        List of Metrics
+        """
         if defaults:
             metrics = self.get_default_metrics() + self.get_custom_metrics()
         else:
             metrics = self.get_custom_metrics()
 
         if only_evaluated:
             return [metric for metric in metrics if metric.is_evaluated()]
         else:
             return metrics
 
     def evaluate(self, defaults: bool = True) -> "ScoreCard":
-        """Evaluates ``Metric``s present on the ``ScoreCard``
+        """
+        Evaluates `Metric`s present on the `ScoreCard`
 
         Parameters
         ----------
         y: Targets = Union[np.ndarray, pd.Series, List[Union[int, float]]]
-        The true labels to compare values to
-
+            The true labels to compare `Predictions` to.
         predictions: Predictions = Union[np.ndarray, pd.Series, List[Union[int, float]]]
-        The predicted values. Integers or whole floats if classification, else floats.
-
+            The predicted values. Integers or whole floats if classification, else floats.
         defaults: boolean
-        Wether the default ``Metric``s should be evaluated or not. Default value = True
+            Wether the default `Metric`s should be evaluated or not.
 
         Returns
         -------
-        self: ScoreCard
+        ScoreCard
         """
 
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
-                metric.evaluate(self.y, self.predictions)
+                if isinstance(metric, Group):
+                    for metric in metric.evaluate(self.y, self.predictions):
+                        self[metric.key] = metric
+                else:
+                    metric.evaluate(self.y, self.predictions)
 
         return self
 
-    def evaluate_over_time(
-        self,
-        defaults: bool = True,
-        window: Optional[int] = None,
-    ) -> "ScoreCard":
-        """Evaluates ``Metric``s present on the ``ScoreCard`` over time, either with expanding
-        or fixed sized window. Assigns list of results to ``results_over_time``.
+    def evaluate_over_time(self, defaults: bool = True) -> "ScoreCard":
+        """
+        Evaluates `Metric`s present on the `ScoreCard` over time, either with expanding
+        or fixed sized window. Assigns list of results to `results_over_time`.
 
         Parameters
         ----------
         y: Targets = Union[np.ndarray, pd.Series, List[Union[int, float]]]
-        The true labels to compare values to
-
+            The true labels to compare values to.
         predictions: Predictions = Union[np.ndarray, pd.Series, List[Union[int, float]]]
-        The predicted values. Integers or whole floats if classification, else floats.
-
-        defaults: boolean
-        Wether the default ``Metric``s should be evaluated or not. Default value = True
-
-        window: int - Optional
-        Size of window. If number is provided then evaluation happens on a fixed window size,
-        otherwise it evaluates it on an expanding window basis.
+            The predicted values. Integers or whole floats if classification, else floats.
+        defaults: bool
+            Wether the default ``Metric``s should be evaluated or not. Default value = True
+        window: int
+            Size of window. If number is provided then evaluation happens on a fixed window size,
+            otherwise it evaluates it on an expanding window basis.
 
         Returns
         -------
-        self: ScoreCard
+        ScoreCard
         """
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
-                metric.evaluate_over_time(self.y, self.predictions, window=window)
+                if isinstance(metric, Group):
+                    for metric in metric.evaluate_over_time(
+                        self.y, self.predictions, rolling_args=self.rolling_args
+                    ):
+                        self[metric.key] = metric
+                else:
+                    metric.evaluate_over_time(
+                        self.y, self.predictions, rolling_args=self.rolling_args
+                    )
         return self
 
     def print(
         self,
         mode: Union[str, PrintMode, List[PrintMode], List[str]] = PrintMode.extended,
         with_info: bool = False,
         input_analysis: bool = True,
@@ -346,46 +449,46 @@
     ) -> None:
         """
         Prints the ScoreCard to the console.
 
         Parameters
         ----------
         mode: Union[str, PrintMode, List[PrintMode], List[str]] = PrintMode.extended
-            - PrintMode.extended or 'extended' prints the full ScoreCard, with targets, predictions, residuals, etc.
-            - PrintMode.minimal or 'minimal' prints the name and the matching result of each metric in the ScoreCard, without fancy formatting
-            - PrintMode.minimal_table or 'minimal_table' creates a table format of just the metric name and the accompanying result
-
+            - `PrintMode.extended` or `'extended'` prints the full ScoreCard, with targets, predictions, residuals, etc.
+            - `PrintMode.minimal` or `'minimal'` prints the name and the matching result of each metric in the ScoreCard, without fancy formatting
+            - `PrintMode.minimal_table` or `'minimal_table'` creates a table format of just the metric name and the accompanying result
         with_info: bool
             Wether descriptions of each metrics should be printed or not
-
         input_analysis: bool = True
             Wether it should print analysis about the raw `targets` and `predictions`
-
         title: Optional[str] = None
-            Title of the table when mode = 'minimal_table'
+            Title of the table when mode = `'minimal_table'`
         """
 
         modes = [PrintMode.from_str(mode_) for mode_ in wrap_in_list(mode)]
         if title is None:
             title = self.metadata.project_name
         for mode in modes:
             if mode is PrintMode.extended:
-                print(
-                    get_summary(
-                        self,
-                        repr=True,
-                        categories=[el.value for el in MetricCategories],
-                        with_info=with_info,
-                        input_analysis=input_analysis,
-                    )
+                to_display = get_summary(
+                    self,
+                    repr=True,
+                    categories=[el.value for el in MetricCategories],
+                    with_info=with_info,
+                    input_analysis=input_analysis,
                 )
+
             elif mode is PrintMode.minimal:
-                print(get_minimal_summary(self, dataframe=frame_or_series))
+                to_display = get_minimal_summary(self, dataframe=frame_or_series)
             elif mode is PrintMode.minimal_table:
-                print(get_large_metric_summary(self, title))
+                to_display = get_large_metric_summary(self, title)
+            if isinstance(to_display, (pd.DataFrame, pd.Series)) and is_notebook():
+                display(to_display)
+            else:
+                print(to_display)
 
     def save(
         self,
         path: Path = PathConst.default_eval_output_path,
         with_info: bool = False,
         save_modes: List[Union[SaveModes, str]] = [
             SaveModes.minimal,
```

### Comparing `krisi-0.1.0/src/krisi/evaluate/type.py` & `krisi-0.1.1/src/krisi/evaluate/type.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 MetricResult = TypeVar(
     "MetricResult", bound=Union[float, int, str, List, Tuple, pd.DataFrame]
 )
 
 
 Predictions = Union[np.ndarray, pd.Series, List[Union[int, float]]]
 Targets = Union[np.ndarray, pd.Series, List[Union[int, float]]]
-MetricFunction = Callable[[Predictions, Targets], MetricResult]
+PredictionsDS = pd.Series
+TargetsDS = pd.Series
+MetricFunction = Callable[[PredictionsDS, TargetsDS], MetricResult]
 
 
 class MetricCategories(Enum):
     residual = "Residual Diagnostics"
     entropy = "Information Entropy"
     class_err = "Forecast Errors - Classification"
     reg_err = "Forecast Errors - Regression"
```

### Comparing `krisi-0.1.0/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-0.1.1/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,50 +15,56 @@
     key="accuracy",
     category=MetricCategories.class_err,
     info="In multilabel classification, this function computes subset accuracy: the set of labels predicted for a sample must exactly match the corresponding set of labels in y_true. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.accuracy_score.html",
     func=accuracy_score,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 recall = Metric[float](
     name="Recall",
     key="recall",
     category=MetricCategories.class_err,
     info="The recall is the ratio tp / (tp + fn) where tp is the number of true positives and fn the number of false negatives. The recall is intuitively the ability of the classifier to find all the positive samples.\nThe best value is 1 and the worst value is 0. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html",
     parameters={"average": "binary"},
     func=recall_score,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+"""~"""
 precision = Metric[float](
     name="Precision",
     key="precision",
     category=MetricCategories.class_err,
     info="The precision is the ratio tp / (tp + fp) where tp is the number of true positives and fp the number of false positives. The precision is intuitively the ability of the classifier not to label as positive a sample that is negative.\nThe best value is 1 and the worst value is 0. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html",
     parameters={"average": "binary"},
     func=precision_score,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+"""~"""
 f_one_score = Metric[float](
     name="F1 Score",
     key="f_one_score",
     category=MetricCategories.class_err,
     info="The F1 score can be interpreted as a harmonic mean of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html",
     parameters={"average": "macro"},
     func=f1_score,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+"""~"""
 matthew_corr = Metric[float](
     name="Matthew Correlation Coefficient",
     key="matthew_corr",
     category=MetricCategories.class_err,
     info="The Matthews correlation coefficient is used in machine learning as a measure of the quality of binary and multiclass classifications. It takes into account true and false positives and negatives and is generally regarded as a balanced measure which can be used even if the classes are of very different sizes. The MCC is in essence a correlation coefficient value between -1 and +1. A coefficient of +1 represents a perfect prediction, 0 an average random prediction and -1 an inverse prediction. The statistic is also known as the phi coefficient.",
     func=matthews_corrcoef,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
-
-
+"""~"""
 all_classification_metrics = [accuracy, recall, precision, f_one_score, matthew_corr]
+"""~"""
 minimal_classification_metrics = [accuracy, f_one_score]
+"""~"""
```

### Comparing `krisi-0.1.0/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-0.1.1/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     mean_absolute_error,
     mean_absolute_percentage_error,
     mean_squared_error,
     mean_squared_log_error,
     r2_score,
 )
 
+from krisi.evaluate.group import Group
 from krisi.evaluate.library.diagrams import (
     display_acf_plot,
     display_density_plot,
     display_single_value,
     display_time_series,
 )
 from krisi.evaluate.library.metric_wrappers import ljung_box
@@ -25,128 +26,156 @@
     key="mae",
     category=MetricCategories.reg_err,
     info="(Mean absolute error) represents the difference between the original and predicted values extracted by averaged the absolute difference over the data set.",
     func=mean_absolute_error,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
 
 mape = Metric[float](
     name="Mean Absolute Percentage Error",
     key="mape",
     category=MetricCategories.reg_err,
     func=mean_absolute_percentage_error,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
 
 smape = Metric[float](
     name="Symmetric Mean Absolute Percentage Error",
     key="smape",
     category=MetricCategories.reg_err,
     func=lambda y_true, y_pred: np.mean(
         np.abs(y_pred - y_true) / (np.abs(y_true) + np.abs(y_pred)), axis=0
     ),
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
 
 mse = Metric[float](
     name="Mean Squared Error",
     key="mse",
     category=MetricCategories.reg_err,
     info="(Mean Squared Error) represents the difference between the original and predicted values extracted by squared the average difference over the data set.",
     parameters={"squared": True},
     func=mean_squared_error,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 rmse = Metric[float](
     name="Root Mean Squared Error",
     key="rmse",
     category=MetricCategories.reg_err,
     info="(Root Mean Squared Error) is the error rate by the square root of Mean Squared Error.",
     parameters={"squared": False},
     func=mean_squared_error,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 rmsle = Metric[float](
     name="Root Mean Squared Log Error",
     key="rmsle",
     category=MetricCategories.reg_err,
     parameters={"squared": False},
     func=mean_squared_log_error,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 r_two = Metric[float](
     name="R-squared",
     key="r_two",
     category=MetricCategories.reg_err,
     info="(Coefficient of determination) represents the coefficient of how well the values fit compared to the original values. The value from 0 to 1 interpreted as percentages. The higher the value is, the better the model is.",
     func=r2_score,
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 residuals = Metric[List[float]](
     name="Residuals",
     key="residuals",
     category=MetricCategories.residual,
     func=lambda y, pred: y - pred,
-    plot_func_rolling=display_time_series,
     plot_funcs=[display_acf_plot, display_density_plot, display_time_series],
+    disable_rolling=True,
 )
+""" ~ """
+
 residuals_mean = Metric[float](
     name="Mean of the Residuals",
     key="residuals_mean",
     category=MetricCategories.residual,
-    func=lambda y, pred: (y - pred).mean(),
+    func=lambda res: res.mean(),
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 residuals_std = Metric[float](
     name="Standard Deviation of the Residuals",
     key="residuals_std",
     category=MetricCategories.residual,
-    func=lambda y, pred: (y - pred).std(),
+    func=lambda res: res.std(),
     plot_funcs=[display_single_value],
     plot_func_rolling=display_time_series,
 )
+""" ~ """
+
 ljung_box_statistics = Metric[pd.DataFrame](
     name="Ljung Box Statistics",
     key="ljung_box_statistics",
     category=MetricCategories.residual,
     func=ljung_box,
     info="If p is larger than our significance level then we cannot dismiss the null-hypothesis that the residuals are a random walk.",
     restrict_to_sample=SampleTypes.insample,
     comp_complexity=ComputationalComplexity.high,
 )
+""" ~ """
+
+residual_group = Group(
+    name="residual_group",
+    key="residual_group",
+    metrics=[residuals_mean, residuals_std],
+    func=lambda y, preds: y - preds,
+)
+""" ~ """
 
 all_regression_metrics = [
     mae,
     mape,
     smape,
     mse,
     rmse,
     rmsle,
     r_two,
     residuals,
-    residuals_mean,
-    residuals_std,
+    residual_group,
     ljung_box_statistics,
 ]
+""" ~ """
 
 minimal_regression_metrics = [
     mae,
     mape,
     mse,
     rmse,
     rmsle,
     r_two,
 ]
+""" ~ """
 
 low_computation_regression_mterics = [
     metric
     for metric in all_regression_metrics
     if metric.comp_complexity is not ComputationalComplexity.high
 ]
+""" ~ """
```

### Comparing `krisi-0.1.0/src/krisi/evaluate/library/diagrams.py` & `krisi-0.1.1/src/krisi/evaluate/library/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/console.py` & `krisi-0.1.1/src/krisi/report/console.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/interactive.py` & `krisi-0.1.1/src/krisi/report/interactive.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/pdf.py` & `krisi-0.1.1/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/report.py` & `krisi-0.1.1/src/krisi/report/report.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/type.py` & `krisi-0.1.1/src/krisi/report/type.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/vizualise.py` & `krisi-0.1.1/src/krisi/report/vizualise.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/library/console/diagrams.py` & `krisi-0.1.1/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/library/pdf_layouts/default/template.html` & `krisi-0.1.1/src/krisi/report/library/pdf_layouts/default/template.html`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-0.1.1/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/utils/console_plot.py` & `krisi-0.1.1/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/utils/data.py` & `krisi-0.1.1/src/krisi/utils/data.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/utils/io.py` & `krisi-0.1.1/src/krisi/utils/io.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/src/krisi/utils/iterable_helpers.py` & `krisi-0.1.1/src/krisi/utils/iterable_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     flat_list: List[Union["Metric", "InteractiveFigure"]], categories: List[str]
 ) -> Dict[str, Union["Metric", "InteractiveFigure"]]:
     category_groups = dict()
     for category in categories:
         category_groups[category] = list(
             filter(
                 lambda x: x.category.value == category
-                if hasattr(x, "category")
+                if (hasattr(x, "category") and x.category is not None)
                 else False,
                 flat_list,
             )
         )
     category_groups[None] = list(
         filter(
-            lambda x: x.category.value is None if hasattr(x, "category") else False,
+            lambda x: x.category is None if hasattr(x, "category") else False,
             flat_list,
         )
     )
     return category_groups
 
 
 def type_converter(type_to_ensure: Any) -> Callable:
```

### Comparing `krisi-0.1.0/src/krisi/utils/printing.py` & `krisi-0.1.1/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/.gitignore` & `krisi-0.1.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -125,7 +125,8 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 output/**
+docs/generated/*
```

### Comparing `krisi-0.1.0/LICENSE` & `krisi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-0.1.0/README.md` & `krisi-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     <img src="https://raw.githubusercontent.com/dream-faster/krisi/main/docs/images/logo.svg" alt="Logo" width="90" >
   </a>
 
 <h3 align="center"> <b>KRISI</b><br> <i>(/creesee/)</i></h3>
   <p align="center">
     Testing and Reporting Framework for Time Series Analysis
     <br />
-    <a href="https://github.com/dream-faster/krisi">View Demo</a>  ~
-    <a href="https://github.com/dream-faster/krisi/tree/main/src/krisi/examples">Check Examples</a> ~
+    <!-- <a href="https://github.com/dream-faster/krisi">View Demo</a>  ~ -->
+    <a href="https://dream-faster.github.io/krisi/generated/gallery/">Check Examples</a> ~
     <a href="https://dream-faster.github.io/krisi/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 Krisi is a Scoring library for Time-Series Forecasting. It calculates, stores and vizualises the performance of your predictions!
 
@@ -278,15 +278,15 @@
 ## Our Open-core Time Series Toolkit
 
 [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
 [![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
 [![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
 [![Fold/Wrapper](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
 
-If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/mark-szulyovszky/consultation)!
+If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/nowcasting/consultation)!
 
 ## Contribution
 
 Join our [Discord](https://discord.gg/EKJQgfuBpE) for live discussion!
 
 Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
             [Docs] [Code_style:_black] [Tests] [Discord_Community]
 
                                     [Logo]
                                   **** KRISI
                                (/creesee/) ****
            Testing and Reporting Framework for Time Series Analysis
-               View_Demo ~ Check_Examples ~ Explore_the_docs_Â»
+                      Check_Examples ~ Explore_the_docs_Â»
 
 Krisi is a Scoring library for Time-Series Forecasting. It calculates, stores
 and vizualises the performance of your predictions! Krisi is from the ground-up
 extensible and lightweight and comes with the fundamental metrics for
 regression and classification. It can generate reports in: - static **PDF**
 (with ``plotly``) - interactive **HTML** (with ``plotly``) - pretty formatted
 for **console** (with ``rich`` and ``plotext``)
@@ -164,11 +164,11 @@
 dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold) [![Fold/
 Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
 overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/
 dream-faster/fold-models) [![Fold/Wrapper](https://raw.githubusercontent.com/
 dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-
 wrappers) If you want to try them out, we'd love to hear about your use case
-and help, [please book a free 30-min call with us](https://calendly.com/mark-
-szulyovszky/consultation)! ## Contribution Join our [Discord](https://
+and help, [please book a free 30-min call with us](https://calendly.com/
+nowcasting/consultation)! ## Contribution Join our [Discord](https://
 discord.gg/EKJQgfuBpE) for live discussion! Submit an issue or reach out to us
 on info at dream-faster.ai for any inquiries.
```

### Comparing `krisi-0.1.0/pyproject.toml` & `krisi-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -67,15 +67,19 @@
   "pytest~=7.1.2",
   "pytest-cov>=4.0",
 ]
 docs = [
   "mkdocs-material",
   "mkdocstrings-python",
   "mkdocs-include-markdown-plugin",
-  "mkdocs-autorefs"
+  "mkdocs-autorefs",
+  "mkdocs-jupyter",
+  "image",
+  "mkdocs-gallery==0.7.6",
+  "mkdocs-glightbox>=0.3"
 ]
 plotting = [
   "plotly",
   "dash",
   "jupyter_dash",
   "weasyprint",
   "kaleido",
@@ -129,15 +133,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-0.1.0/PKG-INFO` & `krisi-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -61,16 +61,20 @@
 Requires-Dist: pytest
 Requires-Dist: rich
 Requires-Dist: scikit-learn
 Requires-Dist: statsmodels>=0.12.1
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Provides-Extra: docs
+Requires-Dist: image; extra == 'docs'
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
+Requires-Dist: mkdocs-gallery==0.7.6; extra == 'docs'
+Requires-Dist: mkdocs-glightbox>=0.3; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin; extra == 'docs'
+Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: plotting
 Requires-Dist: dash; extra == 'plotting'
 Requires-Dist: jupyter-dash; extra == 'plotting'
 Requires-Dist: kaleido; extra == 'plotting'
 Requires-Dist: pangocffi; extra == 'plotting'
@@ -101,16 +105,16 @@
     <img src="https://raw.githubusercontent.com/dream-faster/krisi/main/docs/images/logo.svg" alt="Logo" width="90" >
   </a>
 
 <h3 align="center"> <b>KRISI</b><br> <i>(/creesee/)</i></h3>
   <p align="center">
     Testing and Reporting Framework for Time Series Analysis
     <br />
-    <a href="https://github.com/dream-faster/krisi">View Demo</a>  ~
-    <a href="https://github.com/dream-faster/krisi/tree/main/src/krisi/examples">Check Examples</a> ~
+    <!-- <a href="https://github.com/dream-faster/krisi">View Demo</a>  ~ -->
+    <a href="https://dream-faster.github.io/krisi/generated/gallery/">Check Examples</a> ~
     <a href="https://dream-faster.github.io/krisi/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 Krisi is a Scoring library for Time-Series Forecasting. It calculates, stores and vizualises the performance of your predictions!
 
@@ -366,15 +370,15 @@
 ## Our Open-core Time Series Toolkit
 
 [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
 [![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
 [![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
 [![Fold/Wrapper](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
 
-If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/mark-szulyovszky/consultation)!
+If you want to try them out, we'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/nowcasting/consultation)!
 
 ## Contribution
 
 Join our [Discord](https://discord.gg/EKJQgfuBpE) for live discussion!
 
 Submit an issue or reach out to us on info at dream-faster.ai for any inquiries.
```

