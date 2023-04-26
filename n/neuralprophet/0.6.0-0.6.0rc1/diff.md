# Comparing `tmp/neuralprophet-0.6.0.tar.gz` & `tmp/neuralprophet-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralprophet-0.6.0.tar", max compression
+gzip compressed data, was "neuralprophet-0.6.0rc1.tar", max compression
```

## Comparing `neuralprophet-0.6.0.tar` & `neuralprophet-0.6.0rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1070 2022-11-24 05:34:19.680929 neuralprophet-0.6.0/LICENSE
--rw-r--r--   0        0        0     7464 2023-04-25 04:42:07.600813 neuralprophet-0.6.0/README.md
--rw-r--r--   0        0        0     1394 2023-04-15 04:16:53.703131 neuralprophet-0.6.0/neuralprophet/__init__.py
--rw-r--r--   0        0        0      398 2023-04-15 04:16:53.703711 neuralprophet-0.6.0/neuralprophet/__main__.py
--rw-r--r--   0        0        0       22 2023-04-26 01:49:33.132706 neuralprophet-0.6.0/neuralprophet/_version.py
--rw-r--r--   0        0        0      683 2023-04-15 04:16:53.704907 neuralprophet-0.6.0/neuralprophet/components/README.md
--rw-r--r--   0        0        0       46 2023-04-15 04:16:53.705091 neuralprophet-0.6.0/neuralprophet/components/__init__.py
--rw-r--r--   0        0        0      931 2023-04-15 04:16:53.706486 neuralprophet-0.6.0/neuralprophet/components/base.py
--rw-r--r--   0        0        0       49 2023-04-15 04:16:53.707158 neuralprophet-0.6.0/neuralprophet/components/future_regressors/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-15 04:16:53.707535 neuralprophet-0.6.0/neuralprophet/components/future_regressors/base.py
--rw-r--r--   0        0        0     3681 2023-04-15 04:16:53.708049 neuralprophet-0.6.0/neuralprophet/components/future_regressors/linear.py
--rw-r--r--   0        0        0     4037 2023-04-15 04:16:53.708543 neuralprophet-0.6.0/neuralprophet/components/router.py
--rw-r--r--   0        0        0       44 2023-04-15 04:16:53.708862 neuralprophet-0.6.0/neuralprophet/components/seasonality/__init__.py
--rw-r--r--   0        0        0      546 2023-04-15 04:16:53.709089 neuralprophet-0.6.0/neuralprophet/components/seasonality/base.py
--rw-r--r--   0        0        0     6233 2023-04-26 01:49:09.803435 neuralprophet-0.6.0/neuralprophet/components/seasonality/fourier.py
--rw-r--r--   0        0        0       38 2023-04-15 04:16:53.709633 neuralprophet-0.6.0/neuralprophet/components/trend/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-15 04:16:53.709985 neuralprophet-0.6.0/neuralprophet/components/trend/base.py
--rw-r--r--   0        0        0     3826 2023-04-15 04:16:53.710238 neuralprophet-0.6.0/neuralprophet/components/trend/linear.py
--rw-r--r--   0        0        0    16977 2023-04-15 04:16:53.710507 neuralprophet-0.6.0/neuralprophet/components/trend/piecewise_linear.py
--rw-r--r--   0        0        0     1198 2023-04-15 04:33:44.391908 neuralprophet-0.6.0/neuralprophet/components/trend/static.py
--rw-r--r--   0        0        0    16539 2023-04-26 01:49:09.805959 neuralprophet-0.6.0/neuralprophet/configure.py
--rw-r--r--   0        0        0     1841 2023-04-15 04:16:53.714315 neuralprophet-0.6.0/neuralprophet/custom_loss_metrics.py
--rw-r--r--   0        0        0    30579 2023-04-26 01:49:09.807945 neuralprophet-0.6.0/neuralprophet/data/process.py
--rw-r--r--   0        0        0    10167 2023-04-26 01:49:09.808816 neuralprophet-0.6.0/neuralprophet/data/split.py
--rw-r--r--   0        0        0     1066 2023-04-26 01:49:09.810275 neuralprophet-0.6.0/neuralprophet/data/transform.py
--rw-r--r--   0        0        0    64143 2023-04-26 01:49:09.812986 neuralprophet-0.6.0/neuralprophet/df_utils.py
--rw-r--r--   0        0        0   126250 2023-04-26 01:49:09.816837 neuralprophet-0.6.0/neuralprophet/forecaster.py
--rw-r--r--   0        0        0      849 2023-04-19 04:15:21.202000 neuralprophet-0.6.0/neuralprophet/hdays_utils.py
--rw-r--r--   0        0        0     2635 2023-04-15 04:16:53.722875 neuralprophet-0.6.0/neuralprophet/logger.py
--rw-r--r--   0        0        0      652 2023-04-26 01:49:09.818157 neuralprophet-0.6.0/neuralprophet/np_types.py
--rw-r--r--   0        0        0    20046 2023-04-15 04:16:53.724158 neuralprophet-0.6.0/neuralprophet/plot_forecast_matplotlib.py
--rw-r--r--   0        0        0    28933 2023-04-26 01:49:09.818912 neuralprophet-0.6.0/neuralprophet/plot_forecast_plotly.py
--rw-r--r--   0        0        0    28822 2023-04-15 04:16:53.726943 neuralprophet-0.6.0/neuralprophet/plot_model_parameters_matplotlib.py
--rw-r--r--   0        0        0    33654 2023-04-26 01:49:09.820186 neuralprophet-0.6.0/neuralprophet/plot_model_parameters_plotly.py
--rw-r--r--   0        0        0    25991 2023-04-26 01:49:09.821262 neuralprophet-0.6.0/neuralprophet/plot_utils.py
--rw-r--r--   0        0        0    32646 2023-04-26 01:49:09.822409 neuralprophet-0.6.0/neuralprophet/time_dataset.py
--rw-r--r--   0        0        0    45895 2023-04-26 01:49:09.823365 neuralprophet-0.6.0/neuralprophet/time_net.py
--rw-r--r--   0        0        0    20958 2023-04-14 18:24:09.472906 neuralprophet-0.6.0/neuralprophet/torch_prophet.py
--rw-r--r--   0        0        0    19981 2023-04-15 04:16:53.737476 neuralprophet-0.6.0/neuralprophet/uncertainty.py
--rw-r--r--   0        0        0    31338 2023-04-26 01:49:09.825013 neuralprophet-0.6.0/neuralprophet/utils.py
--rw-r--r--   0        0        0     1679 2023-04-15 04:16:53.739371 neuralprophet-0.6.0/neuralprophet/utils_metrics.py
--rw-r--r--   0        0        0     4697 2023-04-26 01:49:09.825436 neuralprophet-0.6.0/neuralprophet/utils_torch.py
--rw-r--r--   0        0        0     1770 2023-04-26 01:49:43.650974 neuralprophet-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8532 1970-01-01 00:00:00.000000 neuralprophet-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-24 05:34:19.680929 neuralprophet-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     7464 2023-04-15 04:16:53.611613 neuralprophet-0.6.0rc1/README.md
+-rw-r--r--   0        0        0     1394 2023-04-15 04:16:53.703131 neuralprophet-0.6.0rc1/neuralprophet/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-15 04:16:53.703711 neuralprophet-0.6.0rc1/neuralprophet/__main__.py
+-rw-r--r--   0        0        0       25 2023-04-15 04:17:20.775326 neuralprophet-0.6.0rc1/neuralprophet/_version.py
+-rw-r--r--   0        0        0      683 2023-04-15 04:16:53.704907 neuralprophet-0.6.0rc1/neuralprophet/components/README.md
+-rw-r--r--   0        0        0       46 2023-04-15 04:16:53.705091 neuralprophet-0.6.0rc1/neuralprophet/components/__init__.py
+-rw-r--r--   0        0        0      931 2023-04-15 04:16:53.706486 neuralprophet-0.6.0rc1/neuralprophet/components/base.py
+-rw-r--r--   0        0        0       49 2023-04-15 04:16:53.707158 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-15 04:16:53.707535 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/base.py
+-rw-r--r--   0        0        0     3681 2023-04-15 04:16:53.708049 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/linear.py
+-rw-r--r--   0        0        0     4037 2023-04-15 04:16:53.708543 neuralprophet-0.6.0rc1/neuralprophet/components/router.py
+-rw-r--r--   0        0        0       44 2023-04-15 04:16:53.708862 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/__init__.py
+-rw-r--r--   0        0        0      546 2023-04-15 04:16:53.709089 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/base.py
+-rw-r--r--   0        0        0     6220 2023-04-15 04:16:53.709368 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/fourier.py
+-rw-r--r--   0        0        0       38 2023-04-15 04:16:53.709633 neuralprophet-0.6.0rc1/neuralprophet/components/trend/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-15 04:16:53.709985 neuralprophet-0.6.0rc1/neuralprophet/components/trend/base.py
+-rw-r--r--   0        0        0     3826 2023-04-15 04:16:53.710238 neuralprophet-0.6.0rc1/neuralprophet/components/trend/linear.py
+-rw-r--r--   0        0        0    16977 2023-04-15 04:16:53.710507 neuralprophet-0.6.0rc1/neuralprophet/components/trend/piecewise_linear.py
+-rw-r--r--   0        0        0     1198 2023-04-15 04:16:53.711296 neuralprophet-0.6.0rc1/neuralprophet/components/trend/static.py
+-rw-r--r--   0        0        0    16531 2023-04-15 04:16:53.712670 neuralprophet-0.6.0rc1/neuralprophet/configure.py
+-rw-r--r--   0        0        0     1841 2023-04-15 04:16:53.714315 neuralprophet-0.6.0rc1/neuralprophet/custom_loss_metrics.py
+-rw-r--r--   0        0        0    23809 2023-04-15 04:16:53.715073 neuralprophet-0.6.0rc1/neuralprophet/data/process.py
+-rw-r--r--   0        0        0     6803 2023-04-15 04:16:53.716051 neuralprophet-0.6.0rc1/neuralprophet/data/split.py
+-rw-r--r--   0        0        0      878 2023-04-15 04:16:53.716561 neuralprophet-0.6.0rc1/neuralprophet/data/transform.py
+-rw-r--r--   0        0        0    63826 2023-04-15 04:16:53.717906 neuralprophet-0.6.0rc1/neuralprophet/df_utils.py
+-rw-r--r--   0        0        0   121126 2023-04-15 04:16:53.719900 neuralprophet-0.6.0rc1/neuralprophet/forecaster.py
+-rw-r--r--   0        0        0      849 2023-04-15 04:16:53.721434 neuralprophet-0.6.0rc1/neuralprophet/hdays_utils.py
+-rw-r--r--   0        0        0     2635 2023-04-15 04:16:53.722875 neuralprophet-0.6.0rc1/neuralprophet/logger.py
+-rw-r--r--   0        0        0      601 2023-04-14 18:24:09.467754 neuralprophet-0.6.0rc1/neuralprophet/np_types.py
+-rw-r--r--   0        0        0    20046 2023-04-15 04:16:53.724158 neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_matplotlib.py
+-rw-r--r--   0        0        0    28793 2023-04-15 04:16:53.725746 neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_plotly.py
+-rw-r--r--   0        0        0    28822 2023-04-15 04:16:53.726943 neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_matplotlib.py
+-rw-r--r--   0        0        0    33617 2023-04-15 04:16:53.728146 neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_plotly.py
+-rw-r--r--   0        0        0    25987 2023-04-15 04:16:53.729478 neuralprophet-0.6.0rc1/neuralprophet/plot_utils.py
+-rw-r--r--   0        0        0    29297 2023-04-15 04:16:53.731451 neuralprophet-0.6.0rc1/neuralprophet/time_dataset.py
+-rw-r--r--   0        0        0    42383 2023-04-15 04:16:53.734947 neuralprophet-0.6.0rc1/neuralprophet/time_net.py
+-rw-r--r--   0        0        0    20958 2023-04-14 18:24:09.472906 neuralprophet-0.6.0rc1/neuralprophet/torch_prophet.py
+-rw-r--r--   0        0        0    19981 2023-04-15 04:16:53.737476 neuralprophet-0.6.0rc1/neuralprophet/uncertainty.py
+-rw-r--r--   0        0        0    31119 2023-04-15 04:16:53.738755 neuralprophet-0.6.0rc1/neuralprophet/utils.py
+-rw-r--r--   0        0        0     1679 2023-04-15 04:16:53.739371 neuralprophet-0.6.0rc1/neuralprophet/utils_metrics.py
+-rw-r--r--   0        0        0     4542 2023-04-15 04:16:53.740338 neuralprophet-0.6.0rc1/neuralprophet/utils_torch.py
+-rw-r--r--   0        0        0     1773 2023-04-15 04:17:13.016717 neuralprophet-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     8535 1970-01-01 00:00:00.000000 neuralprophet-0.6.0rc1/PKG-INFO
```

### Comparing `neuralprophet-0.6.0/LICENSE` & `neuralprophet-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/README.md` & `neuralprophet-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/__init__.py` & `neuralprophet-0.6.0rc1/neuralprophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/README.md` & `neuralprophet-0.6.0rc1/neuralprophet/components/README.md`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/future_regressors/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/future_regressors/linear.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/router.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/router.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/seasonality/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/seasonality/fourier.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/fourier.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         Returns
         -------
             torch.Tensor
                 Forecast component of dims (batch, n_forecasts)
         """
         device = s[list(s.keys())[0]].device
         x = torch.zeros(
-            size=(s[list(s.keys())[0]].shape[0], s[list(s.keys())[0]].shape[1], len(self.quantiles)),
+            size=(s[list(s.keys())[0]].shape[0], self.n_forecasts, len(self.quantiles)),
             device=device,
         )
         for name, features in s.items():
             x = x + self.compute_fourier(features, name, meta)
         return x
```

### Comparing `neuralprophet-0.6.0/neuralprophet/components/trend/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/trend/linear.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/trend/piecewise_linear.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/components/trend/static.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/static.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/configure.py` & `neuralprophet-0.6.0rc1/neuralprophet/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from neuralprophet.custom_loss_metrics import PinballLoss
 
 log = logging.getLogger("NP.config")
 
 
 @dataclass
 class Model:
-    lagged_reg_layers: Optional[List[int]]
+    num_hidden_layers: int
+    d_hidden: Optional[int]
 
 
 @dataclass
 class Normalization:
     normalize: str
     global_normalization: bool
     global_time_normalization: bool
@@ -340,15 +341,14 @@
         self.periods[name] = Season(resolution=resolution, period=period, arg=arg, condition_name=condition_name)
 
 
 @dataclass
 class AR:
     n_lags: int
     ar_reg: Optional[float] = None
-    ar_layers: Optional[List[int]] = None
 
     def __post_init__(self):
         if self.ar_reg is not None and self.ar_reg > 0:
             if self.ar_reg < 0:
                 raise ValueError("regularization must be >= 0")
             self.reg_lambda = 0.0001 * self.ar_reg
         else:
@@ -379,15 +379,16 @@
 
 @dataclass
 class LaggedRegressor:
     reg_lambda: Optional[float]
     as_scalar: bool
     normalize: Union[bool, str]
     n_lags: int
-    lagged_reg_layers: Optional[List[int]]
+    num_hidden_layers: Optional[int]
+    d_hidden: Optional[int]
 
     def __post_init__(self):
         if self.reg_lambda is not None:
             if self.reg_lambda < 0:
                 raise ValueError("regularization must be >= 0")
```

### Comparing `neuralprophet-0.6.0/neuralprophet/custom_loss_metrics.py` & `neuralprophet-0.6.0rc1/neuralprophet/custom_loss_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/data/process.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,717 +1,650 @@
 import logging
-from typing import List, Optional
+import warnings
+from collections import OrderedDict
+from typing import Optional
 
 import numpy as np
-import pandas as pd
+import torch
 
-from neuralprophet import df_utils, time_dataset
-from neuralprophet.configure import (
-    ConfigCountryHolidays,
-    ConfigEvents,
-    ConfigFutureRegressors,
-    ConfigLaggedRegressors,
-    ConfigSeasonality,
-)
-from neuralprophet.np_types import Components
-
-log = logging.getLogger("NP.data.processing")
-
-
-def _reshape_raw_predictions_to_forecst_df(
-    df: pd.DataFrame,
-    predicted: np.ndarray,
-    components: Optional[Components],
-    prediction_frequency: Optional[dict],
-    dates: pd.Series,
-    n_forecasts: int,
-    max_lags: int,
-    freq: Optional[str],
-    quantiles: List[float],
-    config_lagged_regressors: Optional[ConfigLaggedRegressors],
-) -> pd.DataFrame:
-    """
-    Turns forecast-origin-wise predictions into forecast-target-wise predictions.
+from neuralprophet import time_dataset, utils_torch
 
-    Parameters
-    ----------
-        df : pd.DataFrame
-            input dataframe
-        predicted : np.array
-            Array containing the forecasts
-        components : dict[np.array]
-            Dictionary of components containing an array of each components' contribution to the forecast
-        prediction_frequency : str
-            Frequency of the predictions
-        dates : pd.Series
-            timestamps referring to the start of the predictions
-        n_forecasts : int
-            Number of steps ahead of prediction time step to forecast.
-        max_lags : int
-            Maximum number of lags to use
-        freq : str
-            Data step sizes. Frequency of data recording.
-        quantiles : list[float]
-            List of quantiles to include in the forecast
-        config_lagged_regressors : ConfigLaggedRegressors
-            Configuration for lagged regressors
+log = logging.getLogger("NP.plotting")
 
-    Returns
-    -------
-        pd.DataFrame
-            columns ``ds``, ``y``, ``trend`` and [``yhat<i>``]
 
-            Note
-            ----
-            where yhat<i> refers to the i-step-ahead prediction for this row's datetime.
-            e.g. yhat3 is the prediction for this datetime, predicted 3 steps ago, "3 steps old".
-    """
-    # Receives df with single ID column
-    assert len(df["ID"].unique()) == 1
-    cols = ["ds", "y", "ID"]  # cols to keep from df
-    df_forecast = pd.concat((df[cols],), axis=1)
-    # create a line for each forecast_lag
-    # 'yhat<i>' is the forecast for 'y' at 'ds' from i steps ago.
-    for j in range(len(quantiles)):
-        for forecast_lag in range(1, n_forecasts + 1):
-            forecast = predicted[:, forecast_lag - 1, j]
-            pad_before = max_lags + forecast_lag - 1
-            pad_after = n_forecasts - forecast_lag
-            yhat = np.concatenate(([np.NaN] * pad_before, forecast, [np.NaN] * pad_after))
-            if prediction_frequency is not None:
-                ds = df_forecast["ds"].iloc[pad_before : -pad_after if pad_after > 0 else None]
-                mask = df_utils.create_mask_for_prediction_frequency(
-                    prediction_frequency=prediction_frequency,
-                    ds=ds,
-                    forecast_lag=forecast_lag,
-                )
-                yhat = np.full((len(ds),), np.nan)
-                yhat[mask] = forecast
-                yhat = np.concatenate(([np.NaN] * pad_before, yhat, [np.NaN] * pad_after))
-            # 0 is the median quantile index
-            if j == 0:
-                name = f"yhat{forecast_lag}"
-            else:
-                name = f"yhat{forecast_lag} {round(quantiles[j] * 100, 1)}%"
-            df_forecast[name] = yhat
+def log_warning_deprecation_plotly(plotting_backend):
+    if plotting_backend == "matplotlib":
+        log.warning(
+            "DeprecationWarning: default plotting_backend will be changed to plotly in a future version. "
+            "Switch to plotly by calling `m.set_plotting_backend('plotly')`."
+        )
 
-    if components is None:
-        return df_forecast
 
-    # else add components
-    lagged_components = [
-        "ar",
-    ]
-    if config_lagged_regressors is not None:
-        for name in config_lagged_regressors.keys():
-            lagged_components.append(f"lagged_regressor_{name}")
-    for comp in lagged_components:
-        if comp in components:
-            for j in range(len(quantiles)):
-                for forecast_lag in range(1, n_forecasts + 1):
-                    forecast = components[comp][:, forecast_lag - 1, j]  # 0 is the median quantile
-                    pad_before = max_lags + forecast_lag - 1
-                    pad_after = n_forecasts - forecast_lag
-                    yhat = np.concatenate(([np.NaN] * pad_before, forecast, [np.NaN] * pad_after))
-                    if prediction_frequency is not None:
-                        ds = df_forecast["ds"].iloc[pad_before : -pad_after if pad_after > 0 else None]
-                        mask = df_utils.create_mask_for_prediction_frequency(
-                            prediction_frequency=prediction_frequency,
-                            ds=ds,
-                            forecast_lag=forecast_lag,
-                        )
-                        yhat = np.full((len(ds),), np.nan)
-                        yhat[mask] = forecast
-                        yhat = np.concatenate(([np.NaN] * pad_before, yhat, [np.NaN] * pad_after))
-                    if j == 0:  # temporary condition to add only the median component
-                        name = f"{comp}{forecast_lag}"
-                        df_forecast[name] = yhat
-
-    # only for non-lagged components
-    for comp in components:
-        if comp not in lagged_components:
-            for j in range(len(quantiles)):
-                forecast_0 = components[comp][0, :, j]
-                forecast_rest = components[comp][1:, n_forecasts - 1, j]
-                yhat = np.concatenate(([np.NaN] * max_lags, forecast_0, forecast_rest))
-                if prediction_frequency is not None:
-                    date_list = []
-                    for key, value in prediction_frequency.items():
-                        if key == "daily-hour":
-                            dates_comp = dates[dates.dt.hour == value]
-                        elif key == "weekly-day":
-                            dates_comp = dates[dates.dt.dayofweek == value]
-                        elif key == "monthly-day":
-                            dates_comp = dates[dates.dt.day == value]
-                        elif key == "yearly-month":
-                            dates_comp = dates[dates.dt.month == value]
-                        elif key == "hourly-minute":
-                            dates_comp = dates[dates.dt.minute == value]
-                        else:
-                            raise ValueError(f"prediction_frequency {key} not supported")
-                        date_list.append(dates_comp)
-                    # create new pd.Series only containing the dates that are in all Series in date_list
-                    dates_comp = pd.Series(date_list[0])
-                    for i in range(1, len(date_list)):
-                        dates_comp = dates_comp[dates_comp.isin(date_list[i])]
-                    ser = pd.Series(dtype="datetime64[ns]")
-                    for date in dates_comp:
-                        d = pd.date_range(date, periods=n_forecasts + 1, freq=freq)
-                        ser = pd.concat((ser, pd.Series(d).iloc[1:]))
-                    df_comp = pd.DataFrame({"ds": ser, "yhat": components[comp].flatten()}).drop_duplicates(subset="ds")
-                    df_comp, _ = df_utils.add_missing_dates_nan(df=df_comp, freq=freq)
-                    yhat = pd.merge(df_forecast.filter(["ds", "ID"]), df_comp, on="ds", how="left")["yhat"].values
-                if j == 0:  # temporary condition to add only the median component
-                    # add yhat into dataframe, using df_forecast indexing
-                    yhat_df = pd.Series(yhat, name=comp).set_axis(df_forecast.index)
-                    df_forecast = pd.concat([df_forecast, yhat_df], axis=1, ignore_index=False)
-    return df_forecast
-
-
-def _convert_raw_predictions_to_raw_df(
-    dates: pd.Series,
-    predicted: np.ndarray,
-    n_forecasts: int,
-    quantiles: List[float],
-    components: Optional[Components] = None,
-) -> pd.DataFrame:
-    """Turns forecast-origin-wise predictions into forecast-target-wise predictions.
+def log_warning_resampler_invalid_env():
+    log.warning(
+        "Warning: plotly-resampler not supported for the environment you are using. "
+        "Consider switching plotting_backend to 'plotly' or 'matplotlib "
+    )
+
+
+def log_warning_resampler_switch_to_valid_env():
+    log.warning(
+        "Warning: plotly-resampler not supported for the environment you are using. "
+        "Plotting backend automatically switched to 'plotly' without resampling "
+    )
+
+
+def set_y_as_percent(ax):
+    """Set y axis as percentage
 
     Parameters
     ----------
-        dates : pd.Series
-            timestamps referring to the start of the predictions.
-        predicted : np.array
-            Array containing the forecasts
-        n_forecasts : int
-            optional, number of steps ahead of prediction time step to forecast
-        quantiles : list[float]
-            optional, list of quantiles for quantile regression uncertainty estimate
-        components : dict[np.array]
-            Dictionary of components containing an array of each components' contribution to the forecast
+        ax : matplotlib axis
+            Respective y axis element
 
     Returns
     -------
-        pd. DataFrame
-            columns ``ds``, ``y``, and [``step<i>``]
-
-            Note
-            ----
-            where step<i> refers to the i-step-ahead prediction *made at* this row's datetime.
-            e.g. the first forecast step0 is the prediction for this timestamp,
-            the step1 is for the timestamp after, ...
-            ... step3 is the prediction for 3 steps into the future,
-            predicted using information up to (excluding) this datetime.
-    """
-    all_data = predicted
-    df_raw = pd.DataFrame()
-    df_raw.insert(0, "ds", dates.values)
-    df_raw.insert(1, "ID", "__df__")  # type: ignore
-    for forecast_lag in range(n_forecasts):
-        for quantile_idx in range(len(quantiles)):
-            # 0 is the median quantile index
-            if quantile_idx == 0:
-                step_name = f"step{forecast_lag}"
-            else:
-                step_name = f"step{forecast_lag} {quantiles[quantile_idx] * 100}%"
-            data = all_data[:, forecast_lag, quantile_idx]
-            ser = pd.Series(data=data, name=step_name)
-            df_raw = df_raw.merge(ser, left_index=True, right_index=True)
-        if components is not None:
-            for comp_name, comp_data in components.items():
-                comp_name_ = f"{comp_name}{forecast_lag}"
-                data = comp_data[:, forecast_lag, 0]  # for components the quantiles are ignored for now
-                ser = pd.Series(data=data, name=comp_name_)
-                df_raw = df_raw.merge(ser, left_index=True, right_index=True)
-    return df_raw
+        matplotlib axis
+            Manipulated axis element
+    """
+    warnings.filterwarnings(
+        action="ignore", category=UserWarning
+    )  # workaround until there is clear direction how to handle this recent matplotlib bug
+    yticks = 100 * ax.get_yticks()
+    yticklabels = [f"{y:.4g}%" for y in yticks]
+    ax.set_yticklabels(yticklabels)
+    return ax
 
 
-def _prepare_dataframe_to_predict(model, df: pd.DataFrame, max_lags: int, freq: Optional[str]) -> pd.DataFrame:
+def predict_one_season(m, quantile, name, n_steps=100, df_name="__df__"):
     """
-    Pre-processes a dataframe for prediction using the specified model.
+     Predicts the seasonal component given a number of time steps.
 
     Parameters
     ----------
-        model:
-            The NeuralProphet model
-        df: pd.DataFrame
-            dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
-        max_lags: int
-            The maximum number of lags to include in the output dataframe.
-        freq: str
-            data step sizes. Frequency of data recording,
-
-    Returns
-    ----------
-        pd.DataFrame
-            pre-processed dataframe
+         m : NeuralProphet
+             Fitted NeuralProphet model
+         quantile: float
+             The quantile for which the season is predicted
+         name: str
+             Name of seasonality component
+         n_steps: int
+             number of prediction steps related to the season frequency
+         df_name: str
+                Name of dataframe to refer to data params from original keys of train dataframes
+
+        Returns
+        -------
+            t_i: np.array
+                 time scale of predicted seasonal component
+            predicted: OrderedDict
+                 predicted seasonal component
+
+    """
+    config = m.config_seasonality.periods[name]
+    t_i = np.arange(n_steps + 1) / float(n_steps)
+    features = time_dataset.fourier_series_t(
+        t=t_i * config.period, period=config.period, series_order=config.resolution
+    )
+    features = torch.from_numpy(np.expand_dims(features, 1))
 
-    Raises
-    ----------
-        ValueError
-        If the input dataframe has already been normalized, if there is insufficient input data for prediction,
-        if only datestamps are provided but y values are needed for auto-regression.
-    """
-    # Receives df with ID column
-    df_prepared = pd.DataFrame()
-    for df_name, df_i in df.groupby("ID"):
-        df_i = df_i.copy(deep=True)
-        _ = df_utils.infer_frequency(df_i, n_lags=max_lags, freq=freq)
-        # check if received pre-processed df
-        if "y_scaled" in df_i.columns or "t" in df_i.columns:
-            raise ValueError(
-                "DataFrame has already been normalized. " "Please provide raw dataframe or future dataframe."
-            )
-        # Checks
-        if len(df_i) == 0 or len(df_i) < max_lags:
-            raise ValueError(
-                "Insufficient input data for a prediction."
-                "Please supply historic observations (number of rows) of at least max_lags (max of number of n_lags)."
-            )
-        if len(df_i.columns) == 1 and "ds" in df_i:
-            if max_lags != 0:
-                raise ValueError("only datestamps provided but y values needed for auto-regression.")
-            df_i = _check_dataframe(model, df_i, check_y=False, exogenous=False)
-        else:
-            df_i = _check_dataframe(model, df_i, check_y=model.max_lags > 0, exogenous=False)
-            # fill in missing nans except for nans at end
-            df_i = _handle_missing_data(
-                df=df_i,
-                freq=freq,
-                n_lags=model.n_lags,
-                n_forecasts=model.n_forecasts,
-                config_missing=model.config_missing,
-                config_regressors=model.config_regressors,
-                config_lagged_regressors=model.config_lagged_regressors,
-                config_events=model.config_events,
-                config_seasonality=model.config_seasonality,
-                predicting=True,
-            )
-        df_prepared = pd.concat((df_prepared, df_i.copy(deep=True).reset_index(drop=True)), ignore_index=True)
-    return df_prepared
+    if df_name == "__df__":
+        meta_name_tensor = None
+    else:
+        meta = OrderedDict()
+        meta["df_name"] = [df_name for _ in range(n_steps + 1)]
+        meta_name_tensor = torch.tensor([m.model.id_dict[i] for i in meta["df_name"]])
+
+    quantile_index = m.model.quantiles.index(quantile)
+    predicted = m.model.seasonality.compute_fourier(features=features, name=name, meta=meta_name_tensor)[
+        :, :, quantile_index
+    ]
+    predicted = predicted.squeeze().detach().numpy()
+    if m.config_seasonality.mode == "additive":
+        data_params = m.config_normalization.get_data_params(df_name)
+        scale = data_params["y"].scale
+        predicted = predicted * scale
+    return t_i, predicted
+
+
+def predict_season_from_dates(m, dates, name, quantile, df_name="__df__"):
+    """
+     Predicts the seasonal component given a date range.
+
+     Parameters
+     ----------
+         m : NeuralProphet
+             Fitted NeuralProphet model
+         dates: pd.datetime
+             date range for prediction
+         name: str
+             Name of seasonality component
+         quantile: float
+             The quantile for which the season is predicted
+         df_name: str
+             Name of dataframe to refer to data params from original keys of train dataframes
 
+    Returns
+    -------
+        predicted: OrderedDict
+             presdicted seasonal component
+    """
+    config = m.config_seasonality.periods[name]
+    features = time_dataset.fourier_series(dates=dates, period=config.period, series_order=config.resolution)
+    features = torch.from_numpy(np.expand_dims(features, 1))
+    if df_name == "__df__":
+        meta_name_tensor = None
+    else:
+        meta = OrderedDict()
+        meta["df_name"] = [df_name for _ in range(len(dates))]
+        meta_name_tensor = torch.tensor([m.model.id_dict[i] for i in meta["df_name"]])
+
+    quantile_index = m.model.quantiles.index(quantile)
+    predicted = m.model.seasonality.compute_fourier(features=features, name=name, meta=meta_name_tensor)[
+        :, :, quantile_index
+    ]
 
-def _validate_column_name(
-    name: str,
-    config_events: Optional[ConfigEvents],
-    config_country_holidays: Optional[ConfigCountryHolidays],
-    config_seasonality: Optional[ConfigSeasonality],
-    config_lagged_regressors: Optional[ConfigLaggedRegressors],
-    config_regressors: Optional[ConfigFutureRegressors],
-    events: Optional[bool] = True,
-    seasons: Optional[bool] = True,
-    regressors: Optional[bool] = True,
-    covariates: Optional[bool] = True,
-):
-    """Validates the name of a seasonality, event, or regressor.
+    predicted = predicted.squeeze().detach().numpy()
+    if m.config_seasonality.mode == "additive":
+        data_params = m.config_normalization.get_data_params(df_name)
+        scale = data_params["y"].scale
+        predicted = predicted * scale
+    predicted = {name: predicted}
+    return predicted
 
-    Parameters
-    ----------
-        name : str
-            name of seasonality, event or regressor
-        config_events : Optional[ConfigEvents]
-            Configuration options for adding events to the model.
-        config_country_holidays : Optional[ConfigCountryHolidays]
-            Configuration options for adding country holidays to the model.
-        config_seasonality : Optional[ConfigSeasonality]
-            Configuration options for adding seasonal components to the model.
-        config_lagged_regressors : Optional[ConfigLaggedRegressors]
-            Configuration options for adding lagged external regressors to the model.
-        config_regressors : Optional[ConfigFutureRegressors]
-            Configuration options for adding future regressors to the model.
-        events : bool
-            check if name already used for event
-        seasons : bool
-            check if name already used for seasonality
-        regressors : bool
-            check if name already used for regressor
-        covariates : bool
-            check if name already used for covariate
-    """
-    reserved_names = [
-        "trend",
-        "additive_terms",
-        "daily",
-        "weekly",
-        "yearly",
-        "events",
-        "holidays",
-        "zeros",
-        "extra_regressors_additive",
-        "yhat",
-        "extra_regressors_multiplicative",
-        "multiplicative_terms",
-        "ID",
-    ]
-    rn_l = [n + "_lower" for n in reserved_names]
-    rn_u = [n + "_upper" for n in reserved_names]
-    reserved_names.extend(rn_l)
-    reserved_names.extend(rn_u)
-    reserved_names.extend(["ds", "y", "cap", "floor", "y_scaled", "cap_scaled"])
-    if name in reserved_names:
-        raise ValueError(f"Name {name!r} is reserved.")
-    if events and config_events is not None:
-        if name in config_events.keys():
-            raise ValueError(f"Name {name!r} already used for an event.")
-    if events and config_country_holidays is not None:
-        if name in config_country_holidays.holiday_names:
-            raise ValueError(f"Name {name!r} is a holiday name in {config_country_holidays.country}.")
-    if seasons and config_seasonality is not None:
-        if name in config_seasonality.periods:
-            raise ValueError(f"Name {name!r} already used for a seasonality.")
-    if covariates and config_lagged_regressors is not None:
-        if name in config_lagged_regressors:
-            raise ValueError(f"Name {name!r} already used for an added covariate.")
-    if regressors and config_regressors is not None:
-        if name in config_regressors.keys():
-            raise ValueError(f"Name {name!r} already used for an added regressor.")
-
-
-def _check_dataframe(
-    model,
-    df: pd.DataFrame,
-    check_y: bool = True,
-    exogenous: bool = True,
-    future: Optional[bool] = None,
-) -> pd.DataFrame:
-    """Performs basic data sanity checks and ordering
 
-    Prepare dataframe for fitting or predicting.
+def check_if_configured(m, components, error_flag=False):  # move to utils
+    """Check if components were set in the model configuration by the user.
 
     Parameters
     ----------
-        df : pd.DataFrame
-            dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
-        check_y : bool
-            if df must have series values
+        m : NeuralProphet
+            Fitted NeuralProphet model
+        components : str or list, optional
+            name or list of names of components to check
 
-            Note
+            Options
             ----
-            set to True if training or predicting with autoregression
-        exogenous : bool
-            whether to check covariates, regressors and events column names
-        future : bool
-            whether this function is called by make_future_dataframe()
+            * ``trend``
+            * ``trend_rate_change``
+            * ``seasonality``
+            * ``autoregression``
+            * ``lagged_regressors```
+            * ``events``
+            * ``future_regressors`
+            * ``uncertainty``
+        error_flag : bool
+            Activate to raise a ValueError if component has not been configured
 
     Returns
     -------
-        pd.DataFrame
-            checked dataframe
+        components
+            list of components only including the components set in the model configuration
     """
-    if len(df) < (model.n_forecasts + model.n_lags) and not future:
+    invalid_components = []
+    if "trend_rate_change" in components and m.model.config_trend.changepoints is None:
+        components.remove("trend_rate_change")
+        invalid_components.append("trend_rate_change")
+    if "seasonality" in components and m.config_seasonality is None:
+        components.remove("seasonality")
+        invalid_components.append("seasonality")
+    if "autoregression" in components and not m.config_ar.n_lags > 0:
+        components.remove("autoregression")
+        invalid_components.append("autoregression")
+    if "lagged_regressors" in components and m.config_lagged_regressors is None:
+        components.remove("lagged_regressors")
+        invalid_components.append("lagged_regressors")
+    if "events" in components and (m.config_events and m.config_country_holidays) is None:
+        components.remove("events")
+        invalid_components.append("events")
+    if "future_regressors" in components and m.config_regressors is None:
+        components.remove("future_regressors")
+        invalid_components.append("future_regressors")
+    if "uncertainty" in components and not len(m.model.quantiles) > 1:
+        components.remove("uncertainty")
+        invalid_components.append("uncertainty")
+    if error_flag and len(invalid_components) != 0:
         raise ValueError(
-            "Dataframe has less than n_forecasts + n_lags rows. "
-            "Forecasting not possible. Please either use a larger dataset, or adjust the model parameters."
+            f" Selected component(s) {(invalid_components)} for plotting not specified in the model configuration."
         )
-    df, _, _, _ = df_utils.prep_or_copy_df(df)
-    df, regressors_to_remove, lag_regressors_to_remove = df_utils.check_dataframe(
-        df=df,
-        check_y=check_y,
-        covariates=model.config_lagged_regressors if exogenous else None,
-        regressors=model.config_regressors if exogenous else None,
-        events=model.config_events if exogenous else None,
-        seasonalities=model.config_seasonality if exogenous else None,
-        future=True if future else None,
-    )
-    if model.config_regressors is not None:
-        for reg in regressors_to_remove:
-            log.warning(f"Removing regressor {reg} because it is not present in the data.")
-            model.config_regressors.pop(reg)
-        if len(model.config_regressors) == 0:
-            model.config_regressors = None
-    if model.config_lagged_regressors is not None:
-        for reg in lag_regressors_to_remove:
-            log.warning(f"Removing lagged regressor {reg} because it is not present in the data.")
-            model.config_lagged_regressors.pop(reg)
-        if len(model.config_lagged_regressors) == 0:
-            model.config_lagged_regressors = None
-    return df
-
-
-def _handle_missing_data(
-    df: pd.DataFrame,
-    freq: Optional[str],
-    n_lags: int,
-    n_forecasts: int,
-    config_missing,
-    config_regressors: Optional[ConfigFutureRegressors],
-    config_lagged_regressors: Optional[ConfigLaggedRegressors],
-    config_events: Optional[ConfigEvents],
-    config_seasonality: Optional[ConfigSeasonality],
-    predicting: bool = False,
-) -> pd.DataFrame:
-    """
-    Checks and normalizes new data, auto-imputing missing data if `config_missing` allows it.
+    return components
+
+
+def get_valid_configuration(  # move to utils
+    m, components=None, df_name=None, valid_set=None, validator=None, forecast_in_focus=None, quantile=0.5
+):
+    """Validate and adapt the selected components to be plotted.
 
     Parameters
     ----------
-    df : pd.DataFrame
-        Dataframe containing columns 'ds', 'y', and optionally 'ID' with all data.
-    freq : str
-            data step sizes. Frequency of data recording,
+        m : NeuralProphet
+            Fitted NeuralProphet model
+        components : str or list, optional
+            name or list of names of components to validate and adapt
+        df_name: str
+            ID from time series that should be plotted
+        valid_set : str or list, optional
+            name or list of names of components that are defined as valid option
 
-            Note
+            Options
             ----
-            Any valid frequency for pd.date_range, such as ``5min``, ``D``, ``MS`` or ``auto`` (default) to automatically set frequency.
-    n_lags : int
-        Previous time series steps to include in auto-regression. Aka AR-order
-    n_forecasts : int
-        Number of steps ahead of prediction time step to forecast.
-    config_missing :
-        Configuration options for handling missing data.
-    config_regressors : Optional[ConfigFutureRegressors]
-        Configuration options for adding future regressors to the model.
-    config_lagged_regressors : Optional[ConfigLaggedRegressors]
-        Configuration options for adding lagged external regressors to the model.
-    config_events : Optional[ConfigEvents]
-        Configuration options for adding events to the model.
-    config_seasonality : Optional[ConfigSeasonality]
-        Configuration options for adding seasonal components to the model.
-    predicting : bool, default False
-        If True, allows missing values in the 'y' column for the forecast period, or missing completely.
-
-    Returns
-    -------
-    pd.DataFrame
-        The pre-processed DataFrame, including imputed missing data, if applicable.
+             * (default)``None``:  All components the user set in the model configuration are validated and adapted
+            * ``trend``
+            * ``seasonality``
+            * ``autoregression``
+            * ``lagged_regressors``
+            * ``future_regressors``
+            * ``events``
+            * ``uncertainty``
+        validator: str
+            specifies the validation purpose to customize
 
-    """
-    df, _, _, _ = df_utils.prep_or_copy_df(df)
-    df_handled_missing = pd.DataFrame()
-    for df_name, df_i in df.groupby("ID"):
-        df_handled_missing_aux = _handle_missing_data_single_id(
-            df=df_i,
-            freq=freq,
-            n_lags=n_lags,
-            n_forecasts=n_forecasts,
-            config_missing=config_missing,
-            config_regressors=config_regressors,
-            config_lagged_regressors=config_lagged_regressors,
-            config_events=config_events,
-            config_seasonality=config_seasonality,
-            predicting=predicting,
-        ).copy(deep=True)
-        df_handled_missing_aux["ID"] = df_name
-        df_handled_missing = pd.concat((df_handled_missing, df_handled_missing_aux), ignore_index=True)
-    return df_handled_missing
-
-
-def _handle_missing_data_single_id(
-    df: pd.DataFrame,
-    freq: Optional[str],
-    n_lags: int,
-    n_forecasts: int,
-    config_missing,
-    config_regressors: Optional[ConfigFutureRegressors],
-    config_lagged_regressors: Optional[ConfigLaggedRegressors],
-    config_events: Optional[ConfigEvents],
-    config_seasonality: Optional[ConfigSeasonality],
-    predicting: bool = False,
-) -> pd.DataFrame:
-    """
-    Checks and normalizes new data
-
-    Data is also auto-imputed, unless impute_missing is set to ``False``.
+            Options
+            ----
+            * ``plot_parameters``: customize for plot_parameters() function
+            * ``plot_components``: customize for plot_components() function
+        forecast_in_focus: int
+            optinal, i-th step ahead forecast to plot
 
-        Parameters
-    ----------
-    df : pd.DataFrame
-        Dataframe containing columns 'ds', 'y', and optionally 'ID' of a single ID.
-    freq : str
-            data step sizes. Frequency of data recording,
+            Note
+            ----
+            None (default): plot self.highlight_forecast_step_n by default
+        quantile: float
+            The quantile for which the model parameters are to be plotted
 
             Note
             ----
-            Any valid frequency for pd.date_range, such as ``5min``, ``D``, ``MS`` or ``auto`` (default) to automatically set frequency.
-    n_lags : int
-        Previous time series steps to include in auto-regression. Aka AR-order
-    n_forecasts : int
-        Number of steps ahead of prediction time step to forecast.
-    config_missing :
-        Configuration options for handling missing data.
-    config_regressors : Optional[ConfigFutureRegressors]
-        Configuration options for adding future regressors to the model.
-    config_lagged_regressors : Optional[ConfigLaggedRegressors]
-        Configuration options for adding lagged external regressors to the model.
-    config_events : Optional[ConfigEvents]
-        Configuration options for adding events to the model.
-    config_seasonality : Optional[ConfigSeasonality]
-        Configuration options for adding seasonal components to the model.
-    predicting : bool, default False
-        If True, allows missing values in the 'y' column for the forecast period, or missing completely.
+            0.5 (default):  Parameters will be plotted for the median quantile.
 
     Returns
     -------
-    pd.DataFrame
-        The pre-processed DataFrame, including imputed missing data, if applicable.
+        valid_configuration: dict
+            dict of validated components and values to be plotted
     """
-    # Receives df with single ID column
-    assert len(df["ID"].unique()) == 1
-    if n_lags == 0 and not predicting:
-        # we can drop rows with NA in y
-        sum_na = sum(df["y"].isna())
-        if sum_na > 0:
-            df = df[df["y"].notna()]
-            log.info(f"dropped {sum_na} NAN row in 'y'")
-
-    # add missing dates for autoregression modelling
-    if n_lags > 0:
-        df, missing_dates = df_utils.add_missing_dates_nan(df, freq=freq)
-        if missing_dates > 0:
-            if config_missing.impute_missing:
-                log.info(f"{missing_dates} missing dates added.")
-            # FIX Issue#52
-            # Comment error raising to allow missing data for autoregression flow.
-            # else:
-            #     raise ValueError(f"{missing_dates} missing dates found. Please preprocess data manually or set impute_missing to True.")
-            # END FIX
-
-    if config_regressors is not None:
-        # if future regressors, check that they are not nan at end, else drop
-        # we ignore missing events, as those will be filled in with zeros.
-        reg_nan_at_end = 0
-        for col, regressor in config_regressors.items():
-            # check for completeness of the regressor values
-            col_nan_at_end = 0
-            while len(df) > col_nan_at_end and df[col].isnull().iloc[-(1 + col_nan_at_end)]:
-                col_nan_at_end += 1
-            reg_nan_at_end = max(reg_nan_at_end, col_nan_at_end)
-        if reg_nan_at_end > 0:
-            # drop rows at end due to missing future regressors
-            df = df[:-reg_nan_at_end]
-            log.info(f"Dropped {reg_nan_at_end} rows at end due to missing future regressor values.")
-
-    df_end_to_append = None
-    nan_at_end = 0
-    while len(df) > nan_at_end and df["y"].isnull().iloc[-(1 + nan_at_end)]:
-        nan_at_end += 1
-    if nan_at_end > 0:
-        if predicting:
-            # allow nans at end - will re-add at end
-            if n_forecasts > 1 and n_forecasts < nan_at_end:
-                # check that not more than n_forecasts nans, else drop surplus
-                df = df[: -(nan_at_end - n_forecasts)]
-                # correct new length:
-                nan_at_end = n_forecasts
-                log.info(
-                    "Detected y to have more NaN values than n_forecast can predict. "
-                    f"Dropped {nan_at_end - n_forecasts} rows at end."
+    if type(valid_set) is not list:
+        valid_set = [valid_set]
+
+    if components is None:
+        components = valid_set
+        components = check_if_configured(m=m, components=components)
+    else:
+        if type(components) is not list:
+            components = [components]
+        components = [comp.lower() for comp in components]
+        for comp in components:
+            if comp not in valid_set:
+                raise ValueError(
+                    f" Selected component {comp} is either mis-spelled or not an available "
+                    f"option for this function."
                 )
-            df_end_to_append = df[-nan_at_end:]
-            df = df[:-nan_at_end]
+        components = check_if_configured(m=m, components=components, error_flag=True)
+    if validator is None:
+        raise ValueError("Specify a validator from the available options")
+    # Adapt Normalization
+    if validator == "plot_parameters":
+        # Set to True in case of local normalization and unknown_data_params is not True
+        overwriting_unknown_data_normalization = False
+        if m.config_normalization.global_normalization:
+            if df_name is None and m.id_list.__len__() == 1:
+                df_name = "__df__"
+            elif df_name is None and m.id_list.__len__() > 1:
+                df_name = m.id_list[0]
+            else:
+                log.debug("Global normalization set - ignoring given df_name for normalization")
         else:
-            # training - drop nans at end
-            df = df[:-nan_at_end]
-            log.info(
-                f"Dropped {nan_at_end} consecutive nans at end. "
-                "Training data can only be imputed up to last observation."
-            )
+            if df_name is None:
+                if m.id_list.__len__() > 1:
+                    if (
+                        m.model.config_seasonality.global_local == "local"
+                        or m.model.config_trend.trend_global_local == "local"
+                    ):
+                        df_name = m.id_list
+                        log.warning(
+                            "Glocal model set with > 1 time series in the pd.DataFrame. Plotting components of mean time series and quants. "
+                        )
+                    else:
+                        df_name = m.id_list[0]
+                        log.warning(
+                            "Local model set with > 1 time series in the pd.DataFrame. Plotting components of first time series. "
+                        )
+                else:
+                    log.warning("Local normalization set, but df_name is None. Using global data params instead.")
+                    df_name = "__df__"
+                if not m.config_normalization.unknown_data_normalization:
+                    m.config_normalization.unknown_data_normalization = True
+                    overwriting_unknown_data_normalization = True
+            elif df_name not in m.config_normalization.local_data_params:
+                log.warning(
+                    f"Local normalization set, but df_name '{df_name}' not found. Using global data params instead."
+                )
+                df_name = "__df__"
+                if not m.config_normalization.unknown_data_normalization:
+                    m.config_normalization.unknown_data_normalization = True
+                    overwriting_unknown_data_normalization = True
+            else:
+                log.debug(f"Local normalization set. Data params for {df_name} will be used to denormalize.")
 
-    # impute missing values
-    data_columns = []
-    if n_lags > 0:
-        data_columns.append("y")
-    if config_lagged_regressors is not None:
-        data_columns.extend(config_lagged_regressors.keys())
-    if config_regressors is not None:
-        data_columns.extend(config_regressors.keys())
-    if config_events is not None:
-        data_columns.extend(config_events.keys())
-    conditional_cols = []
-    if config_seasonality is not None:
-        conditional_cols = list(
-            set(
-                [
-                    value.condition_name
-                    for key, value in config_seasonality.periods.items()
-                    if value.condition_name is not None
-                ]
+    # Identify components to be plotted
+    # as dict, minimum: {plot_name}
+    plot_components = []
+    if validator == "plot_parameters":
+        quantile_index = m.model.quantiles.index(quantile)
+
+    # Plot trend
+    if "trend" in components:
+        plot_components.append({"plot_name": "Trend", "comp_name": "trend"})
+    if "trend_rate_change" in components:
+        plot_components.append({"plot_name": "Trend Rate Change"})
+
+    # Plot  seasonalities, if present
+    if "seasonality" in components:
+        for name in m.config_seasonality.periods:
+            if validator == "plot_components":
+                plot_components.append(
+                    {
+                        "plot_name": f"{name} seasonality",
+                        "comp_name": name,
+                    }
+                )
+            elif validator == "plot_parameters":
+                plot_components.append({"plot_name": "seasonality", "comp_name": name})
+
+    # AR
+    if "autoregression" in components:
+        if validator == "plot_components":
+            if forecast_in_focus is None:
+                plot_components.append(
+                    {
+                        "plot_name": "Auto-Regression",
+                        "comp_name": "ar",
+                        "num_overplot": m.n_forecasts,
+                        "bar": True,
+                    }
+                )
+            else:
+                plot_components.append(
+                    {
+                        "plot_name": f"AR ({forecast_in_focus})-ahead",
+                        "comp_name": f"ar{forecast_in_focus}",
+                    }
+                )
+        elif validator == "plot_parameters":
+            plot_components.append(
+                {
+                    "plot_name": "lagged weights",
+                    "comp_name": "AR",
+                    "weights": utils_torch.interprete_model(m.model, net="ar_net", forward_func="auto_regression")
+                    .detach()
+                    .numpy(),
+                    "focus": forecast_in_focus,
+                }
             )
-        )
-        data_columns.extend(conditional_cols)
-    for column in data_columns:
-        sum_na = sum(df[column].isnull())
-        if sum_na > 0:
-            log.warning(f"{sum_na} missing values in column {column} were detected in total. ")
-            if config_missing.impute_missing:
-                # use 0 substitution for holidays and events missing values
-                if config_events is not None and column in config_events.keys():
-                    df[column].fillna(0, inplace=True)
-                    remaining_na = 0
-                else:
-                    df.loc[:, column], remaining_na = df_utils.fill_linear_then_rolling_avg(
-                        df[column],
-                        limit_linear=config_missing.impute_linear,
-                        rolling=config_missing.impute_rolling,
+
+    # Add lagged regressors
+    lagged_scalar_regressors = []
+    if "lagged_regressors" in components:
+        if validator == "plot_components":
+            if forecast_in_focus is None:
+                for name in m.config_lagged_regressors.keys():
+                    plot_components.append(
+                        {
+                            "plot_name": f'Lagged Regressor "{name}"',
+                            "comp_name": f"lagged_regressor_{name}",
+                            "num_overplot": m.n_forecasts,
+                            "bar": True,
+                        }
                     )
-                log.info(f"{sum_na - remaining_na} NaN values in column {column} were auto-imputed.")
-                if remaining_na > 0:
-                    log.warning(
-                        f"More than {2 * config_missing.impute_linear + config_missing.impute_rolling} consecutive missing values encountered in column {column}. "
-                        f"{remaining_na} NA remain after auto-imputation. "
+            else:
+                for name in m.config_lagged_regressors.keys():
+                    plot_components.append(
+                        {
+                            "plot_name": f'Lagged Regressor "{name}" ({forecast_in_focus})-ahead',
+                            "comp_name": f"lagged_regressor_{name}{forecast_in_focus}",
+                        }
+                    )
+        elif validator == "plot_parameters":
+            for name in m.config_lagged_regressors.keys():
+                if m.config_lagged_regressors[name].as_scalar:
+                    lagged_scalar_regressors.append((name, m.model.get_covar_weights(name).detach().numpy()))
+                else:
+                    plot_components.append(
+                        {
+                            "plot_name": "lagged weights",
+                            "comp_name": f'Lagged Regressor "{name}"',
+                            "weights": m.model.get_covar_weights(name).detach().numpy(),
+                            "focus": forecast_in_focus,
+                        }
                     )
-            # FIX Issue#52
-            # Comment error raising to allow missing data for autoregression flow.
-            # else:  # fail because set to not impute missing
-            #    raise ValueError(
-            #        "Missing values found. " "Please preprocess data manually or set impute_missing to True."
-            #    )
-            # END FIX
-    if df_end_to_append is not None:
-        df = pd.concat([df, df_end_to_append])
-        if config_seasonality is not None and len(conditional_cols) > 0:
-            df[conditional_cols] = df[conditional_cols].ffill()  # type: ignore
-    return df
 
+    # Add Events
+    additive_events = []
+    multiplicative_events = []
+    if "events" in components:
+        additive_events_flag = False
+        muliplicative_events_flag = False
+        for event, configs in m.config_events.items():
+            if validator == "plot_components" and configs.mode == "additive":
+                additive_events_flag = True
+            elif validator == "plot_components" and configs.mode == "multiplicative":
+                muliplicative_events_flag = True
+            elif validator == "plot_parameters":
+                event_params = m.model.get_event_weights(event)
+                weight_list = [(key, param.detach().numpy()[quantile_index, :]) for key, param in event_params.items()]
+                if configs.mode == "additive":
+                    additive_events = additive_events + weight_list
+                elif configs.mode == "multiplicative":
+                    multiplicative_events = multiplicative_events + weight_list
+
+        for country_holiday in m.config_country_holidays.holiday_names:
+            if validator == "plot_components" and m.config_country_holidays.mode == "additive":
+                additive_events_flag = True
+            elif validator == "plot_components" and m.config_country_holidays.mode == "multiplicative":
+                muliplicative_events_flag = True
+            elif validator == "plot_parameters":
+                event_params = m.model.get_event_weights(country_holiday)
+                weight_list = [(key, param.detach().numpy()[quantile_index, :]) for key, param in event_params.items()]
+                if m.config_country_holidays.mode == "additive":
+                    additive_events = additive_events + weight_list
+                elif m.config_country_holidays.mode == "multiplicative":
+                    multiplicative_events = multiplicative_events + weight_list
+
+        if additive_events_flag:
+            plot_components.append(
+                {
+                    "plot_name": "Additive Events",
+                    "comp_name": "events_additive",
+                }
+            )
+        if muliplicative_events_flag:
+            plot_components.append(
+                {
+                    "plot_name": "Multiplicative Events",
+                    "comp_name": "events_multiplicative",
+                    "multiplicative": True,
+                }
+            )
+
+    # Add Regressors
+    additive_future_regressors = []
+    multiplicative_future_regressors = []
+    if "future_regressors" in components:
+        for regressor, configs in m.config_regressors.items():
+            if validator == "plot_components" and configs.mode == "additive":
+                plot_components.append(
+                    {
+                        "plot_name": "Additive Future Regressors",
+                        "comp_name": "future_regressors_additive",
+                    }
+                )
+            elif validator == "plot_components" and configs.mode == "multiplicative":
+                plot_components.append(
+                    {
+                        "plot_name": "Multiplicative Future Regressors",
+                        "comp_name": "future_regressors_multiplicative",
+                        "multiplicative": True,
+                    }
+                )
+            elif validator == "plot_parameters":
+                regressor_param = m.model.future_regressors.get_reg_weights(regressor)[quantile_index, :]
+                if configs.mode == "additive":
+                    additive_future_regressors.append((regressor, regressor_param.detach().numpy()))
+                elif configs.mode == "multiplicative":
+                    multiplicative_future_regressors.append((regressor, regressor_param.detach().numpy()))
+
+    # Plot  quantiles as a separate component, if present
+    # If multiple steps in the future are predicted, only plot quantiles if highlight_forecast_step_n is set
+    if (
+        "quantiles" in components
+        and validator == "plot_components"
+        and len(m.model.quantiles) > 1
+        and forecast_in_focus is None
+    ):
+        if len(m.config_train.quantiles) > 1 and (
+            m.n_forecasts > 1 or m.config_ar.n_lags > 0
+        ):  # rather query if n_forecasts >1 than n_lags>1
+            raise ValueError(
+                "Please specify step_number using the highlight_nth_step_ahead_of_each_forecast function"
+                " for quantiles plotting when autoregression enabled."
+            )
+        for i in range(1, len(m.model.quantiles)):
+            plot_components.append(
+                {
+                    "plot_name": "Uncertainty",
+                    "comp_name": f"yhat1 {round(m.model.quantiles[i] * 100, 1)}%",
+                    "fill": True,
+                }
+            )
+    elif (
+        "uncertainty" in components
+        and validator == "plot_components"
+        and len(m.model.quantiles) > 1
+        and forecast_in_focus is not None
+    ):
+        for i in range(1, len(m.model.quantiles)):
+            plot_components.append(
+                {
+                    "plot_name": "Uncertainty",
+                    "comp_name": f"yhat{forecast_in_focus} {round(m.model.quantiles[i] * 100, 1)}%",
+                    "fill": True,
+                }
+            )
+    if validator == "plot_parameters":
+        if len(additive_future_regressors) > 0:
+            plot_components.append({"plot_name": "Additive future regressor"})
+        if len(multiplicative_future_regressors) > 0:
+            plot_components.append({"plot_name": "Multiplicative future regressor"})
+        if len(lagged_scalar_regressors) > 0:
+            plot_components.append({"plot_name": "Lagged scalar regressor"})
+        if len(additive_events) > 0:
+            data_params = m.config_normalization.get_data_params(df_name)
+            scale = data_params["y"].scale
+            additive_events = [(key, weight * scale) for (key, weight) in additive_events]
+            plot_components.append({"plot_name": "Additive event"})
+        if len(multiplicative_events) > 0:
+            plot_components.append({"plot_name": "Multiplicative event"})
+
+        valid_configuration = {
+            "components_list": plot_components,
+            "additive_future_regressors": additive_future_regressors,
+            "additive_events": additive_events,
+            "multiplicative_future_regressors": multiplicative_future_regressors,
+            "multiplicative_events": multiplicative_events,
+            "lagged_scalar_regressors": lagged_scalar_regressors,
+            "overwriting_unknown_data_normalization": overwriting_unknown_data_normalization,
+            "df_name": df_name,
+        }
+    elif validator == "plot_components":
+        valid_configuration = {
+            "components_list": plot_components,
+        }
+    return valid_configuration
 
-def _create_dataset(model, df, predict_mode, prediction_frequency=None):
-    """Construct dataset from dataframe.
 
-    (Configured Hyperparameters can be overridden by explicitly supplying them.
-    Useful to predict a single model component.)
+def validate_current_env_for_resampler(auto: bool = False) -> Optional[bool]:
+    """
+    Validate the current environment to check if it is a valid environment for plotly-resampler and if invalid trigger warning message.
 
     Parameters
     ----------
-        df : pd.DataFrame
-            dataframe containing column ``ds``, ``y``, and optionally``ID`` and
-            normalized columns normalized columns ``ds``, ``y``, ``t``, ``y_scaled``
-        predict_mode : bool
-            specifies predict mode
+    auto: bool, optional
+        If True, the function will automatically switch to a valid environment if the current environment is not valid.
+        If False, the function will return None if the current environment is not valid.
+    Returns
+    -------
+    bool :
+        True if the current environment is a valid environment to run the code, False if the current environment is
+        not a valid environment to run the code. None if the current environment is not a valid environment to run
+        the code and the function did not switch to a valid environment.
+    """
 
-            Options
-                * ``False``: includes target values.
-                * ``True``: does not include targets but includes entire dataset as input
+    from IPython import get_ipython
+
+    if "google.colab" in str(get_ipython()):
+        if auto:
+            log_warning_resampler_switch_to_valid_env()
+            valid_env = False
+        else:
+            log_warning_resampler_invalid_env()
+            valid_env = None
+    else:
+        if is_notebook():
+            valid_env = True
+        else:
+            if auto:
+                log_warning_resampler_switch_to_valid_env()
+                valid_env = False
+            else:
+                log_warning_resampler_invalid_env()
+                valid_env = None
+    return valid_env
 
-        prediction_frequency: dict
-            periodic interval in which forecasts should be made.
-            Key: str
-                periodicity of the predictions to be made, e.g. 'daily-hour'.
 
-            Options
-                * ``'hourly-minute'``: forecast once per hour at a specified minute
-                * ``'daily-hour'``: forecast once per day at a specified hour
-                * ``'weekly-day'``: forecast once per week at a specified day
-                * ``'monthly-day'``: forecast once per month at a specified day
-                * ``'yearly-month'``: forecast once per year at a specified month
+def is_notebook():
+    """
+    Determine if the code is being executed in a Jupyter notebook environment.
+
+    Returns
+    -------
+    bool :
+        True if the code is being executed in a Jupyter notebook, False otherwise.
+    """
+    try:
+        from IPython import get_ipython
 
-            value: int
-                forecast origin of the predictions to be made, e.g. 7 for 7am in case of 'daily-hour'.
+        if "IPKernelApp" not in get_ipython().config:  # pragma: no cover
+            return False
+    except ImportError:
+        return False
+    except AttributeError:
+        return False
+    return True
+
+
+def select_plotting_backend(model, plotting_backend):
+    """Automatically selects the plotting backend based on the global plotting_backend and plotting_backend set by the
+    user. If the plotting backend is selected as "plotly-resampler", triggers warning message.
+
+    Parameters
+    ----------
+    model: NeuralProphet
+        The configured model.
+    plotting_backend: str
+        The plotting backend to use.
 
     Returns
     -------
-        TimeDataset
+    str
+        The new plotting backend.
     """
-    df, _, _, _ = df_utils.prep_or_copy_df(df)
-    return time_dataset.GlobalTimeDataset(
-        df,
-        predict_mode=predict_mode,
-        n_lags=model.n_lags,
-        n_forecasts=model.n_forecasts,
-        predict_steps=model.predict_steps,
-        config_seasonality=model.config_seasonality,
-        config_events=model.config_events,
-        config_country_holidays=model.config_country_holidays,
-        config_lagged_regressors=model.config_lagged_regressors,
-        config_regressors=model.config_regressors,
-        config_missing=model.config_missing,
-        prediction_frequency=prediction_frequency,
-    )
+    if hasattr(model, "plotting_backend") and plotting_backend is None:
+        plotting_backend = model.plotting_backend
+        if plotting_backend == "plotly-resampler":
+            validate_current_env_for_resampler()
+    else:
+        if plotting_backend is None:
+            if validate_current_env_for_resampler(auto=True):
+                plotting_backend = "plotly-resampler"
+            else:
+                plotting_backend = "plotly"
+        elif plotting_backend == "plotly-resampler":
+            validate_current_env_for_resampler()
+    return plotting_backend.lower()
```

### Comparing `neuralprophet-0.6.0/neuralprophet/data/transform.py` & `neuralprophet-0.6.0rc1/neuralprophet/data/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import logging
 
 import pandas as pd
 
 from neuralprophet import df_utils
-from neuralprophet.configure import Normalization
 
 log = logging.getLogger("NP.data.transforming")
 
 
-def _normalize(df: pd.DataFrame, config_normalization: Normalization) -> pd.DataFrame:
+def _normalize(model, df):
     """Apply data scales.
 
     Applies data scaling factors to df using data_params.
 
     Parameters
     ----------
         df : pd.DataFrame
             dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
-        config_normalization: Normalization
-            Normalization configuration
 
     Returns
     -------
         df: pd.DataFrame, normalized
     """
     df, _, _, _ = df_utils.prep_or_copy_df(df)
     df_norm = pd.DataFrame()
     for df_name, df_i in df.groupby("ID"):
-        data_params = config_normalization.get_data_params(df_name)
+        data_params = model.config_normalization.get_data_params(df_name)
         df_i.drop("ID", axis=1, inplace=True)
         df_aux = df_utils.normalize(df_i, data_params).copy(deep=True)
         df_aux["ID"] = df_name
         df_norm = pd.concat((df_norm, df_aux), ignore_index=True)
     return df_norm
```

### Comparing `neuralprophet-0.6.0/neuralprophet/df_utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/df_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
     df: pd.DataFrame,
     check_y: bool = True,
     covariates=None,
     regressors=None,
     events=None,
     seasonalities=None,
     future: Optional[bool] = None,
-) -> Tuple[pd.DataFrame, List, List]:
+) -> Tuple[pd.DataFrame, List]:
     """Performs basic data sanity checks and ordering,
     as well as prepare dataframe for fitting or predicting.
 
     Parameters
     ----------
         df : pd.DataFrame
             containing column ``ds``
@@ -552,42 +552,37 @@
     checked_df = pd.DataFrame()
     for df_name, df_i in df.groupby("ID"):
         df_aux = check_single_dataframe(df_i, check_y, covariates, regressors, events, seasonalities)
         df_aux = df_aux.copy(deep=True)
         df_aux["ID"] = df_name
         checked_df = pd.concat((checked_df, df_aux), ignore_index=True)
     regressors_to_remove = []
-    lag_regressors_to_remove = []
     if regressors is not None:
         for reg in regressors:
             if len(df[reg].unique()) < 2:
                 log.warning(
                     "Encountered future regressor with only unique values in training set across all IDs."
                     "Automatically removed variable."
                 )
                 regressors_to_remove.append(reg)
+    if future:
+        return checked_df, regressors_to_remove
     if covariates is not None:
         for covar in covariates:
             if len(df[covar].unique()) < 2:
                 log.warning(
                     "Encountered lagged regressor with only unique values in training set across all IDs."
                     "Automatically removed variable."
                 )
-                lag_regressors_to_remove.append(covar)
-    if future:
-        return checked_df, regressors_to_remove, lag_regressors_to_remove
+                regressors_to_remove.append(covar)
     if len(regressors_to_remove) > 0:
         regressors_to_remove = list(set(regressors_to_remove))
-        checked_df = checked_df.drop(regressors_to_remove, axis=1)
-        assert checked_df is not None
-    if len(lag_regressors_to_remove) > 0:
-        lag_regressors_to_remove = list(set(lag_regressors_to_remove))
-        checked_df = checked_df.drop(lag_regressors_to_remove, axis=1)
+        checked_df = checked_df.drop(*regressors_to_remove, axis=1)
         assert checked_df is not None
-    return checked_df, regressors_to_remove, lag_regressors_to_remove
+    return checked_df, regressors_to_remove
 
 
 def _crossvalidation_split_df(df, n_lags, n_forecasts, k, fold_pct, fold_overlap_pct=0.0):
     """Splits data in k folds for crossvalidation.
 
     Parameters
     ----------
```

### Comparing `neuralprophet-0.6.0/neuralprophet/forecaster.py` & `neuralprophet-0.6.0rc1/neuralprophet/forecaster.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,26 +164,24 @@
             how much sparsity to induce in the AR-coefficients
 
             Note
             ----
             Large values (~1-100) will limit the number of nonzero coefficients dramatically.
             Small values (~0.001-1.0) will allow more non-zero coefficients.
             default: 0 no regularization of coefficients.
-        ar_layers : list of int, optional
-            array of hidden layer dimensions of the AR-Net. Specifies number of hidden layers (number of entries)
-            and layer dimension (list entry).
 
         COMMENT
         Model Config
         COMMENT
         n_forecasts : int
             Number of steps ahead of prediction time step to forecast.
-        lagged_reg_layers : list of int, optional
-            array of hidden layer dimensions of the Covar-Net. Specifies number of hidden layers (number of entries)
-            and layer dimension (list entry).
+        num_hidden_layers : int, optional
+            number of hidden layer to include in AR-Net (defaults to 0)
+        d_hidden : int, optional
+            dimension of hidden layers of the AR-Net. Ignored if ``num_hidden_layers`` == 0.
 
         COMMENT
         Train Config
         COMMENT
         learning_rate : float
             Maximum learning rate setting for 1cycle policy scheduler.
 
@@ -342,17 +340,17 @@
         weekly_seasonality: np_types.SeasonalityArgument = "auto",
         daily_seasonality: np_types.SeasonalityArgument = "auto",
         seasonality_mode: np_types.SeasonalityMode = "additive",
         seasonality_reg: float = 0,
         season_global_local: np_types.SeasonGlobalLocalMode = "global",
         n_forecasts: int = 1,
         n_lags: int = 0,
-        ar_layers: Optional[list] = [],
+        num_hidden_layers: int = 0,
+        d_hidden: Optional[int] = None,
         ar_reg: Optional[float] = None,
-        lagged_reg_layers: Optional[list] = [],
         learning_rate: Optional[float] = None,
         epochs: Optional[int] = None,
         batch_size: Optional[int] = None,
         loss_func: Union[str, torch.nn.modules.loss._Loss, Callable] = "Huber",
         optimizer: Union[str, Type[torch.optim.Optimizer]] = "AdamW",
         newer_samples_weight: float = 2,
         newer_samples_start: float = 0.0,
@@ -412,20 +410,26 @@
                 DeprecationWarning(
                     "Providing metrics to collect via `collect_metrics` in NeuralProphet is deprecated and will be removed in a future version. The metrics are now configure in the `fit()` method via `metrics`."
                 )
             )
         self.metrics = utils_metrics.get_metrics(collect_metrics)
 
         # AR
-        self.config_ar = configure.AR(n_lags=n_lags, ar_reg=ar_reg, ar_layers=ar_layers)
+        self.config_ar = configure.AR(
+            n_lags=n_lags,
+            ar_reg=ar_reg,
+        )
         self.n_lags = self.config_ar.n_lags
         self.max_lags = self.n_lags
 
         # Model
-        self.config_model = configure.Model(lagged_reg_layers=lagged_reg_layers)
+        self.config_model = configure.Model(
+            num_hidden_layers=num_hidden_layers,
+            d_hidden=d_hidden,
+        )
 
         # Trend
         self.config_trend = configure.Trend(
             growth=growth,
             changepoints=changepoints,
             n_changepoints=n_changepoints,
             changepoints_range=changepoints_range,
@@ -472,14 +476,16 @@
         self.highlight_forecast_step_n = None
         self.true_ar_weights = None
 
     def add_lagged_regressor(
         self,
         names: Union[str, List[str]],
         n_lags: Union[int, np_types.Literal["auto", "scalar"]] = "auto",
+        num_hidden_layers: Optional[int] = None,
+        d_hidden: Optional[int] = None,
         regularization: Optional[float] = None,
         normalize: Union[bool, str] = "auto",
     ):
         """Add a covariate or list of covariate time series as additional lagged regressors to be used for fitting and predicting.
         The dataframe passed to ``fit`` and ``predict`` will have the column with the specified name to be used as
         lagged regressor. When normalize=True, the covariate will be normalized unless it is binary.
 
@@ -487,22 +493,29 @@
         ----------
             names : string or list
                 name of the regressor/list of regressors.
             n_lags : int
                 previous regressors time steps to use as input in the predictor (covar order)
                 if ``auto``, time steps will be equivalent to the AR order (default)
                 if ``scalar``, all the regressors will only use last known value as input
+            num_hidden_layers : int
+                number of hidden layers to include in Lagged-Regressor-Net (defaults to same configuration as AR-Net)
+            d_hidden : int
+                dimension of hidden layers of the Lagged-Regressor-Net. Ignored if ``num_hidden_layers`` == 0.
             regularization : float
                 optional  scale for regularization strength
             normalize : bool
                 optional, specify whether this regressor will benormalized prior to fitting.
                 if ``auto``, binary regressors will not be normalized.
         """
-        lagged_reg_layers = self.config_model.lagged_reg_layers
+        if num_hidden_layers is None:
+            num_hidden_layers = self.config_model.num_hidden_layers
 
+        if d_hidden is None:
+            d_hidden = self.config_model.d_hidden
         if n_lags == 0 or n_lags is None:
             n_lags = 0
             log.warning(
                 "Please, set n_lags to a value greater than 0 or to the options 'scalar' or 'auto'. No lags will be added to regressors when n_lags = 0 or n_lags is None"
             )
         if n_lags == "auto":
             if self.n_lags is not None and self.n_lags > 0:
@@ -520,30 +533,24 @@
             log.info("n_lags = 'scalar', number of lags for regressor is set to 1")
         only_last_value = False if n_lags > 1 else True
         if self.fitted:
             raise Exception("Regressors must be added prior to model fitting.")
         if not isinstance(names, list):
             names = [names]
         for name in names:
-            _validate_column_name(
-                name=name,
-                config_events=self.config_events,
-                config_country_holidays=self.config_country_holidays,
-                config_seasonality=self.config_seasonality,
-                config_lagged_regressors=self.config_lagged_regressors,
-                config_regressors=self.config_regressors,
-            )
+            _validate_column_name(self, name)
             if self.config_lagged_regressors is None:
                 self.config_lagged_regressors = OrderedDict()
             self.config_lagged_regressors[name] = configure.LaggedRegressor(
                 reg_lambda=regularization,
                 normalize=normalize,
                 as_scalar=only_last_value,
                 n_lags=n_lags,
-                lagged_reg_layers=lagged_reg_layers,
+                num_hidden_layers=num_hidden_layers,
+                d_hidden=d_hidden,
             )
         return self
 
     def parameters(self):
         return self.config
 
     def state_dict(self):
@@ -594,22 +601,15 @@
         if self.fitted:
             raise Exception("Regressors must be added prior to model fitting.")
         if regularization is not None:
             if regularization < 0:
                 raise ValueError("regularization must be >= 0")
             if regularization == 0:
                 regularization = None
-        _validate_column_name(
-            name=name,
-            config_events=self.config_events,
-            config_country_holidays=self.config_country_holidays,
-            config_seasonality=self.config_seasonality,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_regressors=self.config_regressors,
-        )
+        _validate_column_name(self, name)
 
         if self.config_regressors is None:
             self.config_regressors = OrderedDict()
         self.config_regressors[name] = configure.Regressor(reg_lambda=regularization, normalize=normalize, mode=mode)
         return self
 
     def add_events(
@@ -650,22 +650,15 @@
             if regularization == 0:
                 regularization = None
 
         if not isinstance(events, list):
             events = [events]
 
         for event_name in events:
-            _validate_column_name(
-                name=event_name,
-                config_events=self.config_events,
-                config_country_holidays=self.config_country_holidays,
-                config_seasonality=self.config_seasonality,
-                config_lagged_regressors=self.config_lagged_regressors,
-                config_regressors=self.config_regressors,
-            )
+            _validate_column_name(self, event_name)
             self.config_events[event_name] = configure.Event(
                 lower_window=lower_window, upper_window=upper_window, reg_lambda=regularization, mode=mode
             )
         return self
 
     def add_country_holidays(
         self,
@@ -764,32 +757,17 @@
             >>> m.add_seasonality(name="weekly_fall", period=7, fourier_order=4, condition_name="fall")
         """
         if self.fitted:
             raise Exception("Seasonality must be added prior to model fitting.")
         if name in ["daily", "weekly", "yearly"]:
             log.error("Please use inbuilt daily, weekly, or yearly seasonality or set another name.")
         # Do not Allow overwriting built-in seasonalities
-        _validate_column_name(
-            name=name,
-            config_events=self.config_events,
-            config_country_holidays=self.config_country_holidays,
-            config_seasonality=self.config_seasonality,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_regressors=self.config_regressors,
-            seasons=True,
-        )
+        _validate_column_name(self, name, seasons=True)
         if condition_name is not None:
-            _validate_column_name(
-                name=condition_name,
-                config_events=self.config_events,
-                config_country_holidays=self.config_country_holidays,
-                config_seasonality=self.config_seasonality,
-                config_lagged_regressors=self.config_lagged_regressors,
-                config_regressors=self.config_regressors,
-            )
+            _validate_column_name(self, condition_name)
         if fourier_order <= 0:
             raise ValueError("Fourier Order must be > 0")
         self.config_seasonality.append(
             name=name, period=period, resolution=fourier_order, condition_name=condition_name, arg="custom"
         )
         return self
 
@@ -908,26 +886,15 @@
             progress = None
 
         # Pre-processing
         # Copy df and save list of unique time series IDs (the latter for global-local modelling if enabled)
         df, _, _, self.id_list = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=True, exogenous=True)
         self.data_freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(
-            df=df,
-            freq=self.data_freq,
-            n_lags=self.n_lags,
-            n_forecasts=self.n_forecasts,
-            config_missing=self.config_missing,
-            config_regressors=self.config_regressors,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_events=self.config_events,
-            config_seasonality=self.config_seasonality,
-            predicting=False,
-        )
+        df = _handle_missing_data(self, df, freq=self.data_freq)
 
         # Setup for global-local modelling: If there is only a single time series, then self.id_list = ['__df__']
         self.num_trends_modelled = len(self.id_list) if self.config_trend.trend_global_local == "local" else 1
         self.num_seasonalities_modelled = len(self.id_list) if self.config_seasonality.global_local == "local" else 1
         self.meta_used_in_model = self.num_trends_modelled != 1 or self.num_seasonalities_modelled != 1
 
         if self.fitted is True and not continue_training:
@@ -950,26 +917,15 @@
                 checkpointing_enabled=checkpointing,
                 continue_training=continue_training,
                 num_workers=num_workers,
             )
         else:
             df_val, _, _, _ = df_utils.prep_or_copy_df(validation_df)
             df_val = _check_dataframe(self, df_val, check_y=False, exogenous=False)
-            df_val = _handle_missing_data(
-                df=df_val,
-                freq=self.data_freq,
-                n_lags=self.n_lags,
-                n_forecasts=self.n_forecasts,
-                config_missing=self.config_missing,
-                config_regressors=self.config_regressors,
-                config_lagged_regressors=self.config_lagged_regressors,
-                config_events=self.config_events,
-                config_seasonality=self.config_seasonality,
-                predicting=False,
-            )
+            df_val = _handle_missing_data(self, df_val, freq=self.data_freq)
             metrics_df = self._train(
                 df,
                 df_val=df_val,
                 progress_bar_enabled=bool(progress),
                 metrics_enabled=bool(self.metrics),
                 checkpointing_enabled=checkpointing,
                 continue_training=continue_training,
@@ -1029,55 +985,33 @@
         """
         if raw:
             log.warning("Raw forecasts are incompatible with plotting utilities")
         if self.fitted is False:
             raise ValueError("Model has not been fitted. Predictions will be random.")
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         # to get all forecasteable values with df given, maybe extend into future:
-        df, periods_added = _maybe_extend_df(
-            df=df,
-            n_forecasts=self.n_forecasts,
-            max_lags=self.max_lags,
-            freq=self.data_freq,
-            config_regressors=self.config_regressors,
-            config_events=self.config_events,
-        )
-        df = _prepare_dataframe_to_predict(model=self, df=df, max_lags=self.max_lags, freq=self.data_freq)
+        df, periods_added = _maybe_extend_df(self, df)
+        df = _prepare_dataframe_to_predict(self, df)
         # normalize
-        df = _normalize(df=df, config_normalization=self.config_normalization)
+        df = _normalize(self, df)
         forecast = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             dates, predicted, components = self._predict_raw(
                 df_i, df_name, include_components=decompose, prediction_frequency=self.prediction_frequency
             )
             df_i = df_utils.drop_missing_from_df(
                 df_i, self.config_missing.drop_missing, self.predict_steps, self.n_lags
             )
             if raw:
-                fcst = _convert_raw_predictions_to_raw_df(
-                    dates=dates,
-                    predicted=predicted,
-                    n_forecasts=self.n_forecasts,
-                    quantiles=self.config_train.quantiles,
-                    components=components,
-                )
+                fcst = _convert_raw_predictions_to_raw_df(self, dates, predicted, components)
                 if periods_added[df_name] > 0:
                     fcst = fcst[:-1]
             else:
                 fcst = _reshape_raw_predictions_to_forecst_df(
-                    df=df_i,
-                    predicted=predicted,
-                    components=components,
-                    prediction_frequency=self.prediction_frequency,
-                    dates=dates,
-                    n_forecasts=self.n_forecasts,
-                    max_lags=self.max_lags,
-                    freq=self.data_freq,
-                    quantiles=self.config_train.quantiles,
-                    config_lagged_regressors=self.config_lagged_regressors,
+                    self, df_i, predicted, components, self.prediction_frequency, dates
                 )
                 if periods_added[df_name] > 0:
                     fcst = fcst[: -periods_added[df_name]]
             forecast = pd.concat((forecast, fcst), ignore_index=True)
         df = df_utils.return_df_in_original_format(forecast, received_ID_col, received_single_time_series)
         self.predict_steps = self.n_forecasts
         return df
@@ -1094,27 +1028,16 @@
             pd.DataFrame
                 evaluation metrics
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
         if self.fitted is False:
             log.warning("Model has not been fitted. Test results will be random.")
         df = _check_dataframe(self, df, check_y=True, exogenous=True)
-        freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=self.data_freq)
-        df = _handle_missing_data(
-            df=df,
-            freq=freq,
-            n_lags=self.n_lags,
-            n_forecasts=self.n_forecasts,
-            config_missing=self.config_missing,
-            config_regressors=self.config_regressors,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_events=self.config_events,
-            config_seasonality=self.config_seasonality,
-            predicting=False,
-        )
+        _ = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=self.data_freq)
+        df = _handle_missing_data(self, df, freq=self.data_freq)
         loader = self._init_val_loader(df)
         # Use Lightning to calculate metrics
         val_metrics = self.trainer.test(self.model, dataloaders=loader)
         val_metrics_df = pd.DataFrame(val_metrics)
         # TODO Check whether supported by Lightning
         if not self.config_normalization.global_normalization:
             log.warning("Note that the metrics are displayed in normalized scale because of local normalization.")
@@ -1231,26 +1154,15 @@
             0	2022-12-05	7.89	data1
             1	2022-12-13	8.02	data2
             2	2022-12-13	8.30	data3
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(
-            df=df,
-            freq=freq,
-            n_lags=self.n_lags,
-            n_forecasts=self.n_forecasts,
-            config_missing=self.config_missing,
-            config_regressors=self.config_regressors,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_events=self.config_events,
-            config_seasonality=self.config_seasonality,
-            predicting=False,
-        )
+        df = _handle_missing_data(self, df, freq=freq, predicting=False)
         df_train, df_val = df_utils.split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             valid_p=valid_p,
             inputs_overbleed=True,
             local_split=local_split,
@@ -1410,26 +1322,15 @@
             0	2022-12-10	8.09	data1
             1	2022-12-10	8.25	data2
             2	2022-12-10	7.55	data3
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(
-            df=df,
-            freq=freq,
-            n_lags=self.n_lags,
-            n_forecasts=self.n_forecasts,
-            config_missing=self.config_missing,
-            config_regressors=self.config_regressors,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_events=self.config_events,
-            config_seasonality=self.config_seasonality,
-            predicting=False,
-        )
+        df = _handle_missing_data(self, df, freq=freq, predicting=False)
         folds = df_utils.crossvalidation_split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             k=k,
             fold_pct=fold_pct,
             fold_overlap_pct=fold_overlap_pct,
@@ -1473,26 +1374,15 @@
         -------
             tuple of k tuples [(folds_val, folds_test), …]
                 elements same as :meth:`crossvalidation_split_df` returns
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = _handle_missing_data(
-            df=df,
-            freq=freq,
-            n_lags=self.n_lags,
-            n_forecasts=self.n_forecasts,
-            config_missing=self.config_missing,
-            config_regressors=self.config_regressors,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_events=self.config_events,
-            config_seasonality=self.config_seasonality,
-            predicting=False,
-        )
+        df = _handle_missing_data(self, df, freq=freq, predicting=False)
         folds_val, folds_test = df_utils.double_crossvalidation_split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             k=k,
             valid_pct=valid_pct,
             test_pct=test_pct,
@@ -1598,23 +1488,20 @@
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         events_dict = df_utils.create_dict_for_events_or_regressors(df, events_df, "events")
         regressors_dict = df_utils.create_dict_for_events_or_regressors(df, regressors_df, "regressors")
 
         df_future_dataframe = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             df_aux = _make_future_dataframe(
-                model=self,
+                self,
                 df=df_i,
                 events_df=events_dict[df_name],
                 regressors_df=regressors_dict[df_name],
                 periods=periods,
                 n_historic_predictions=n_historic_predictions,
-                n_forecasts=self.n_forecasts,
-                max_lags=self.max_lags,
-                freq=self.data_freq,
             )
             df_aux["ID"] = df_name
             df_future_dataframe = pd.concat((df_future_dataframe, df_aux), ignore_index=True)
 
         df_future = df_utils.return_df_in_original_format(
             df_future_dataframe, received_ID_col, received_single_time_series
         )
@@ -1676,15 +1563,15 @@
                 trend on prediction dates.
         """
         if quantile is not None and not (0 < quantile < 1):
             raise ValueError("The quantile specified need to be a float in-between (0,1)")
 
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
-        df = _normalize(df=df, config_normalization=self.config_normalization)
+        df = _normalize(self, df)
         df_trend = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             t = torch.from_numpy(np.expand_dims(df_i["t"].values, 1))  # type: ignore
 
             # Creating and passing meta, in this case the meta['df_name'] is the ID of the dataframe
             # Note: meta is only used on the trend method if trend_global_local is not "global"
             meta = OrderedDict()
@@ -1720,15 +1607,15 @@
                 seasonal components with columns of name <seasonality component name>
         """
         if quantile is not None and not (0 < quantile < 1):
             raise ValueError("The quantile specified need to be a float in-between (0,1)")
 
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         df = _check_dataframe(self, df, check_y=False, exogenous=False)
-        df = _normalize(df=df, config_normalization=self.config_normalization)
+        df = _normalize(self, df)
         df_seasonal = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             dataset = time_dataset.TimeDataset(
                 df_i,
                 name=df_name,
                 config_seasonality=self.config_seasonality,
                 # n_lags=0,
@@ -2444,16 +2331,16 @@
             config_regressors=self.config_regressors,
             config_events=self.config_events,
             config_holidays=self.config_country_holidays,
             config_normalization=self.config_normalization,
             n_forecasts=self.n_forecasts,
             n_lags=self.n_lags,
             max_lags=self.max_lags,
-            ar_layers=self.config_ar.ar_layers,
-            lagged_reg_layers=self.config_model.lagged_reg_layers,
+            num_hidden_layers=self.config_model.num_hidden_layers,
+            d_hidden=self.config_model.d_hidden,
             metrics=self.metrics,
             id_list=self.id_list,
             num_trends_modelled=self.num_trends_modelled,
             num_seasonalities_modelled=self.num_seasonalities_modelled,
             meta_used_in_model=self.meta_used_in_model,
         )
         log.debug(self.model)
@@ -2479,20 +2366,20 @@
             df=df,
             config_lagged_regressors=self.config_lagged_regressors,
             config_regressors=self.config_regressors,
             config_events=self.config_events,
             config_seasonality=self.config_seasonality,
         )
 
-        df = _normalize(df=df, config_normalization=self.config_normalization)
+        df = _normalize(self, df)
         # if not self.fitted:
         if self.config_trend.changepoints is not None:
             # scale user-specified changepoint times
             df_aux = pd.DataFrame({"ds": pd.Series(self.config_trend.changepoints)})
-            self.config_trend.changepoints = _normalize(df=df_aux, config_normalization=self.config_normalization)["t"].values  # type: ignore # types are numpy.ArrayLike and list
+            self.config_trend.changepoints = _normalize(self, df_aux)["t"].values  # type: ignore # types are numpy.ArrayLike and list
 
         # df_merged, _ = df_utils.join_dataframes(df)
         # df_merged = df_merged.sort_values("ds")
         # df_merged.drop_duplicates(inplace=True, keep="first", subset=["ds"])
         df_merged = df_utils.merge_dataframes(df)
         self.config_seasonality = utils.set_auto_seasonalities(df_merged, config_seasonality=self.config_seasonality)
         if self.config_country_holidays is not None:
@@ -2501,20 +2388,15 @@
         dataset = _create_dataset(
             self, df, predict_mode=False, prediction_frequency=self.prediction_frequency
         )  # needs to be called after set_auto_seasonalities
 
         # Determine the max_number of epochs
         self.config_train.set_auto_batch_epoch(n_data=len(dataset))
 
-        loader = DataLoader(
-            dataset,
-            batch_size=self.config_train.batch_size,
-            shuffle=True,
-            num_workers=num_workers,
-        )
+        loader = DataLoader(dataset, batch_size=self.config_train.batch_size, shuffle=True, num_workers=num_workers)
 
         return loader
 
     def _init_val_loader(self, df):
         """Executes data preparation steps and initiates evaluation procedure.
 
         Parameters
@@ -2523,15 +2405,15 @@
                 dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
 
         Returns
         -------
             torch DataLoader
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df = _normalize(df=df, config_normalization=self.config_normalization)
+        df = _normalize(self, df)
         dataset = _create_dataset(self, df, predict_mode=False)
         loader = DataLoader(dataset, batch_size=min(1024, len(dataset)), shuffle=False, drop_last=False)
         return loader
 
     def _train(
         self,
         df: pd.DataFrame,
@@ -2735,17 +2617,15 @@
         loader = DataLoader(dataset, batch_size=min(1024, len(df)), shuffle=False, drop_last=False)
         if self.n_forecasts > 1:
             dates = df["ds"].iloc[self.max_lags : -self.n_forecasts + 1]
         else:
             dates = df["ds"].iloc[self.max_lags :]
 
         # Pass the include_components flag to the model
-        if include_components:
-            self.model.set_compute_components(include_components)
-            self.model.set_covar_weights(self.model.get_covar_weights())
+        self.model.set_compute_components(include_components)
         # Compute the predictions and components (if requested)
         result = self.trainer.predict(self.model, loader)
         # Extract the prediction and components
         predicted, component_vectors = zip(*result)
         predicted = np.concatenate(predicted)
 
         # Post-process and normalize the predictions
```

### Comparing `neuralprophet-0.6.0/neuralprophet/hdays_utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/hdays_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/logger.py` & `neuralprophet-0.6.0rc1/neuralprophet/logger.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/np_types.py` & `neuralprophet-0.6.0rc1/neuralprophet/np_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 from typing import Dict, List, Union
 
-import torch
 import torchmetrics
 
 # Ensure compatibility with python 3.7
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -18,9 +17,7 @@
 SeasonalityArgument = Union[Literal["auto"], bool, int]
 
 GrowthMode = Literal["off", "linear", "discontinuous"]
 
 CollectMetricsMode = Union[List[str], bool, Dict[str, torchmetrics.Metric]]
 
 SeasonGlobalLocalMode = Literal["global", "local"]
-
-Components = Dict[str, torch.Tensor]
```

### Comparing `neuralprophet-0.6.0/neuralprophet/plot_forecast_matplotlib.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_matplotlib.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/plot_forecast_plotly.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,14 @@
             rangeslider=dict(visible=True),
             **xaxis_args,
         ),
         yaxis=go.layout.YAxis(title=ylabel, **yaxis_args),
         **layout_args,
     )
     fig = go.Figure(data=data, layout=layout)
-    unregister_plotly_resampler()
     return fig
 
 
 def plot_components(
     m,
     fcst,
     plot_configuration,
@@ -334,15 +333,14 @@
         for trace in trace_object["traces"]:
             fig.add_trace(trace, row=j + 1, col=1)  # adapt var name to plotly-resampler
         fig.update_layout(legend={"y": 0.1, "traceorder": "reversed"})
 
     # Reset multiplicative axes labels after tight_layout adjustment
     for ax in multiplicative_axes:
         ax = set_y_as_percent(ax)
-    unregister_plotly_resampler()
     return fig
 
 
 def get_forecast_component_props(
     fcst,
     comp_name,
     plot_name=None,
@@ -812,15 +810,14 @@
             y=q_hi,
             annotation_text=f"q1_hi = {round(q_hi, 2)}",
             annotation_position="bottom left",
             line_width=1,
             line_color="red",
         )
         fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
-        unregister_plotly_resampler()
         return fig
 
 
 def plot_interval_width_per_timestep(q_hats, method, resampler_active=False):
     """Plot the nonconformity scores as well as the one-sided interval width (q).
 
     Parameters
@@ -872,9 +869,8 @@
             x="Timestep Number",
             y=["One-Sided Lower Interval Width", "One-Sided Upper Interval Width"],
             title=f"{method} One-Sided Interval Width with q per Timestep",
             width=600,
             height=400,
         )
     fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
-    unregister_plotly_resampler()
     return fig
```

### Comparing `neuralprophet-0.6.0/neuralprophet/plot_model_parameters_matplotlib.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_matplotlib.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/plot_model_parameters_plotly.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -951,9 +951,9 @@
 
         xaxis.update(trace_object["xaxis"])
         yaxis.update(trace_object["yaxis"])
         xaxis.update(**xaxis_args)
         yaxis.update(**yaxis_args)
         for trace in trace_object["traces"]:
             fig.add_trace(trace, row=i + 1, col=1)  # adapt var name to plotly-resampler
-        unregister_plotly_resampler()
+
     return fig
```

### Comparing `neuralprophet-0.6.0/neuralprophet/plot_utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/time_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,650 +1,717 @@
 import logging
-import warnings
-from collections import OrderedDict
+from collections import OrderedDict, defaultdict
+from datetime import datetime
 from typing import Optional
 
 import numpy as np
+import pandas as pd
 import torch
+from torch.utils.data.dataset import Dataset
 
-from neuralprophet import time_dataset, utils_torch
+from neuralprophet import configure, utils
+from neuralprophet.df_utils import get_max_num_lags
+from neuralprophet.hdays_utils import get_country_holidays
+
+log = logging.getLogger("NP.time_dataset")
+
+
+class GlobalTimeDataset(Dataset):
+    def __init__(self, df, **kwargs):
+        """Initialize Timedataset from time-series df.
+
+        Parameters
+        ----------
+            df : pd.DataFrame
+                dataframe containing column ``ds``, ``y``, and optionally``ID`` and
+                normalized columns normalized columns ``ds``, ``y``, ``t``, ``y_scaled``
+            **kwargs : dict
+                Identical to :meth:`tabularize_univariate_datetime`
+        """
+        self.combined_timedataset = []
+        # TODO (future): vectorize
+        self.length = 0
+        for df_name, df_i in df.groupby("ID"):
+            timedataset = TimeDataset(df_i, df_name, **kwargs)
+            self.length += timedataset.length
+            for i in range(0, len(timedataset)):
+                self.combined_timedataset.append(timedataset[i])
+
+    def __len__(self):
+        return self.length
+
+    def __getitem__(self, idx):
+        return self.combined_timedataset[idx]
+
+
+class TimeDataset(Dataset):
+    """Create a PyTorch dataset of a tabularized time-series"""
+
+    def __init__(self, df, name, **kwargs):
+        """Initialize Timedataset from time-series df.
+
+        Parameters
+        ----------
+            df : pd.DataFrame
+                Time series data
+            name : str
+                Name of time-series
+            **kwargs : dict
+                Identical to :meth:`tabularize_univariate_datetime`
+        """
+        self.name = name
+        self.length = None
+        self.inputs = OrderedDict({})
+        self.targets = None
+        self.meta = OrderedDict({})
+        self.two_level_inputs = ["seasonalities", "covariates"]
+        inputs, targets, drop_missing = tabularize_univariate_datetime(df, **kwargs)
+        self.init_after_tabularized(inputs, targets)
+        self.filter_samples_after_init(kwargs["prediction_frequency"])
+        self.drop_nan_after_init(df, kwargs["predict_steps"], drop_missing)
+
+    def drop_nan_after_init(self, df, predict_steps, drop_missing):
+        """Checks if inputs/targets contain any NaN values and drops them, if user opts to.
+
+        Parameters
+        ----------
+            drop_missing : bool
+                whether to automatically drop missing samples from the data
+        """
+        nan_idx = []
+        for i, (inputs, targets, meta) in enumerate(self):
+            for key, data in inputs.items():  # key: lags/seasonality, data: torch tensor (oder OrderedDict)
+                if key in self.two_level_inputs or key == "events" or key == "regressors":
+                    # Extract tensor out of OrderedDict to see if it contains NaNs
+                    tuple_list = list(data.items())
+                    tensor = tuple_list[0][1]
+                    if np.isnan(np.array(tensor)).any() and (i not in nan_idx):
+                        nan_idx.append(i)
+                else:
+                    # save index of the NaN-containing sample
+                    if np.isnan(np.array(data)).any() and (i not in nan_idx):
+                        nan_idx.append(i)
+            if np.isnan(np.array(targets)).any() and (i not in nan_idx):
+                if (
+                    i < len(self) - predict_steps
+                ):  # do not remove the targets that were inserted for prediction at the end
+                    nan_idx.append(i)  # nan_idx contains all indices of inputs/targets containing 1 or more NaN values
+        if drop_missing and len(nan_idx) > 0:
+            log.warning(f"{len(nan_idx)} samples with missing values were dropped from the data. ")
+            for key, data in self.inputs.items():
+                if key not in ["time", "lags"]:
+                    for name, features in data.items():
+                        self.inputs[key][name] = np.delete(self.inputs[key][name], nan_idx, 0)
+                else:
+                    self.inputs[key] = np.delete(self.inputs[key], nan_idx, 0)
+            self.targets = np.delete(self.targets, nan_idx, 0)
+            self.length = self.inputs["time"].shape[0]
+        if not drop_missing and len(nan_idx) > 0:
+            raise ValueError(
+                "Inputs/targets with missing values detected. "
+                "Please either adjust imputation parameters, or set 'drop_missing' to True to drop those samples."
+            )
 
-log = logging.getLogger("NP.plotting")
+    def init_after_tabularized(self, inputs, targets=None):
+        """Create Timedataset with data.
 
+        Parameters
+        ----------
+            inputs : ordered dict
+                Identical to returns from :meth:`tabularize_univariate_datetime`
+            targets : np.array, float
+                Identical to returns from :meth:`tabularize_univariate_datetime`
+        """
+        inputs_dtype = {
+            "time": torch.float,
+            "timestamps": np.datetime64,
+            # "changepoints": torch.bool,
+            "seasonalities": torch.float,
+            "events": torch.float,
+            "lags": torch.float,
+            "covariates": torch.float,
+            "regressors": torch.float,
+        }
+        targets_dtype = torch.float
+        self.length = inputs["time"].shape[0]
 
-def log_warning_deprecation_plotly(plotting_backend):
-    if plotting_backend == "matplotlib":
-        log.warning(
-            "DeprecationWarning: default plotting_backend will be changed to plotly in a future version. "
-            "Switch to plotly by calling `m.set_plotting_backend('plotly')`."
-        )
+        for key, data in inputs.items():
+            if key in self.two_level_inputs or key == "events" or key == "regressors":
+                self.inputs[key] = OrderedDict({})
+                for name, features in data.items():
+                    self.inputs[key][name] = torch.from_numpy(features.astype(float)).type(inputs_dtype[key])
+            else:
+                if key == "timestamps":
+                    self.inputs[key] = data
+                else:
+                    self.inputs[key] = torch.from_numpy(data).type(inputs_dtype[key])
+        self.targets = torch.from_numpy(targets).type(targets_dtype).unsqueeze(dim=2)
+        self.meta["df_name"] = self.name
+        # Pre-compute all samples for faster iteration in __getitem__
+        self.samples = []
+        for index in range(self.length):
+            sample = OrderedDict({})
+            for key, data in self.inputs.items():
+                if key in self.two_level_inputs:
+                    sample[key] = OrderedDict({})
+                    for name, period_features in self.inputs[key].items():
+                        sample[key][name] = period_features[index]
+                elif key == "events" or key == "regressors":
+                    sample[key] = OrderedDict({})
+                    for mode, features in self.inputs[key].items():
+                        sample[key][mode] = features[index, :, :]
+                else:
+                    sample[key] = data[index]
+            self.samples.append(sample)
 
+    def filter_samples_after_init(
+        self,
+        prediction_frequency=None,
+    ):
+        """Filters samples from the dataset based on the forecast frequency.
 
-def log_warning_resampler_invalid_env():
-    log.warning(
-        "Warning: plotly-resampler not supported for the environment you are using. "
-        "Consider switching plotting_backend to 'plotly' or 'matplotlib "
-    )
+        Parameters
+        ----------
+            prediction_frequency : int
+                periodic interval in which forecasts should be made.
 
+            Note
+            ----
+            E.g. if prediction_frequency=7, forecasts are only made on every 7th step (once in a week in case of daily resolution).
+        """
+        if prediction_frequency is None or prediction_frequency == 1:
+            return
+        # Only the first target timestamp is of interest for filtering
+        timestamps = pd.to_datetime([sample["timestamps"][0] for sample in self.samples])
+        masks = []
+        for key, value in prediction_frequency.items():
+            if key == "daily-hour":
+                mask = timestamps.hour == value + 1  # + 1 because prediction starts one step after origin
+            elif key == "weekly-day":
+                mask = timestamps.dayofweek == value + 1
+            elif key == "monthly-day":
+                mask = timestamps.day == value + 1
+            elif key == "yearly-month":
+                mask = timestamps.month == value + 1
+            elif key == "hourly-minute":
+                mask = timestamps.minute == value + 1
+            else:
+                raise ValueError(f"Invalid prediction frequency: {key}")
+            masks.append(mask)
+        mask = np.ones((len(timestamps),), dtype=bool)
+        for m in masks:
+            mask = mask & m
+        self.samples = [self.samples[i] for i in range(len(self.samples)) if mask[i]]
+
+        # Exact timestamps are not needed anymore
+        self.inputs.pop("timestamps")
+        for sample in self.samples:
+            sample.pop("timestamps")
+        self.length = len(self.samples)
+
+    def __getitem__(self, index):
+        """Overrides parent class method to get an item at index.
+
+        Parameters
+        ----------
+            index : int
+                Sample location in dataset
 
-def log_warning_resampler_switch_to_valid_env():
-    log.warning(
-        "Warning: plotly-resampler not supported for the environment you are using. "
-        "Plotting backend automatically switched to 'plotly' without resampling "
-    )
+        Returns
+        -------
+        OrderedDict
+            Model inputs, each of len(df) but with varying dimensions
+
+            Note
+            ----
+            Contains the following data:
 
+            Model Inputs
+                * ``time`` (np.array, float), dims: (num_samples, 1)
+                * ``seasonalities`` (OrderedDict), named seasonalities
+                each with features (np.array, float) - dims: (num_samples, n_features[name])
+                * ``lags`` (np.array, float), dims: (num_samples, n_lags)
+                * ``covariates`` (OrderedDict), named covariates,
+                each with features (np.array, float) of dims: (num_samples, n_lags)
+                * ``events`` (OrderedDict), events,
+                each with features (np.array, float) of dims: (num_samples, n_lags)
+                * ``regressors`` (OrderedDict), regressors,
+                each with features (np.array, float) of dims: (num_samples, n_lags)
+        np.array, float
+            Targets to be predicted of same length as each of the model inputs, dims: (num_samples, n_forecasts)
+        """
+        sample = self.samples[index]
+        targets = self.targets[index]
+        meta = self.meta
+        return sample, targets, meta
+
+    def __len__(self):
+        """Overrides Parent class method to get data length."""
+        return self.length
+
+
+def tabularize_univariate_datetime(
+    df,
+    predict_mode=False,
+    n_lags=0,
+    n_forecasts=1,
+    predict_steps=1,
+    config_seasonality: Optional[configure.ConfigSeasonality] = None,
+    config_events: Optional[configure.ConfigEvents] = None,
+    config_country_holidays=None,
+    config_lagged_regressors: Optional[configure.ConfigLaggedRegressors] = None,
+    config_regressors: Optional[configure.ConfigFutureRegressors] = None,
+    config_missing=None,
+    prediction_frequency=None,
+):
+    """Create a tabular dataset from univariate timeseries for supervised forecasting.
 
-def set_y_as_percent(ax):
-    """Set y axis as percentage
+    Note
+    ----
+    Data must have no gaps.
+    If data contains missing values, they are ignored for the creation of the dataset.
 
     Parameters
     ----------
-        ax : matplotlib axis
-            Respective y axis element
+        df : pd.DataFrame
+            Sequence of observations with original ``ds``, ``y`` and normalized ``t``, ``y_scaled`` columns
+        config_seasonality : configure.ConfigSeasonality
+            Configuration for seasonalities
+        n_lags : int
+            Number of lagged values of series to include as model inputs (aka AR-order)
+        n_forecasts : int
+            Number of steps to forecast into future
+        config_events : configure.ConfigEvents
+            User specified events, each with their upper, lower windows (int) and regularization
+        config_country_holidays : configure.ConfigCountryHolidays
+            Configurations (holiday_names, upper, lower windows, regularization) for country specific holidays
+        config_lagged_regressors : configure.ConfigLaggedRegressors
+            Configurations for lagged regressors
+        config_regressors : configure.ConfigFutureRegressors
+            Configuration for regressors
+        predict_mode : bool
+            Chooses the prediction mode
+
+            Options
+                * (default) ``False``: Includes target values
+                * ``True``: Does not include targets but includes entire dataset as input
 
     Returns
     -------
-        matplotlib axis
-            Manipulated axis element
-    """
-    warnings.filterwarnings(
-        action="ignore", category=UserWarning
-    )  # workaround until there is clear direction how to handle this recent matplotlib bug
-    yticks = 100 * ax.get_yticks()
-    yticklabels = [f"{y:.4g}%" for y in yticks]
-    ax.set_yticklabels(yticklabels)
-    return ax
+        OrderedDict
+            Model inputs, each of len(df) but with varying dimensions
 
+            Note
+            ----
+            Contains the following data:
 
-def predict_one_season(m, quantile, name, n_steps=100, df_name="__df__"):
-    """
-     Predicts the seasonal component given a number of time steps.
+            Model Inputs
+                * ``time`` (np.array, float), dims: (num_samples, 1)
+                * ``seasonalities`` (OrderedDict), named seasonalities
+                each with features (np.array, float) - dims: (num_samples, n_features[name])
+                * ``lags`` (np.array, float), dims: (num_samples, n_lags)
+                * ``covariates`` (OrderedDict), named covariates,
+                each with features (np.array, float) of dims: (num_samples, n_lags)
+                * ``events`` (OrderedDict), events,
+                each with features (np.array, float) of dims: (num_samples, n_lags)
+                * ``regressors`` (OrderedDict), regressors,
+                each with features (np.array, float) of dims: (num_samples, n_lags)
+        np.array, float
+            Targets to be predicted of same length as each of the model inputs, dims: (num_samples, n_forecasts)
+    """
+    max_lags = get_max_num_lags(config_lagged_regressors, n_lags)
+    n_samples = len(df) - max_lags + 1 - n_forecasts
+    # data is stored in OrderedDict
+    inputs = OrderedDict({})
+
+    def _stride_time_features_for_forecasts(x):
+        # only for case where n_lags > 0
+        if x.dtype != np.float64:
+            dtype = np.datetime64
+        else:
+            dtype = np.float64
+        return np.array([x[max_lags + i : max_lags + i + n_forecasts] for i in range(n_samples)], dtype=dtype)
 
-    Parameters
-    ----------
-         m : NeuralProphet
-             Fitted NeuralProphet model
-         quantile: float
-             The quantile for which the season is predicted
-         name: str
-             Name of seasonality component
-         n_steps: int
-             number of prediction steps related to the season frequency
-         df_name: str
-                Name of dataframe to refer to data params from original keys of train dataframes
+    # time is the time at each forecast step
+    t = df.loc[:, "t"].values
+    if max_lags == 0:
+        assert n_forecasts == 1
+        time = np.expand_dims(t, 1)
+    else:
+        time = _stride_time_features_for_forecasts(t)
+    inputs["time"] = time
 
-        Returns
-        -------
-            t_i: np.array
-                 time scale of predicted seasonal component
-            predicted: OrderedDict
-                 predicted seasonal component
+    if prediction_frequency is not None:
+        ds = df.loc[:, "ds"].values
+        if max_lags == 0:
+            timestamps = np.expand_dims(ds, 1)
+        else:
+            timestamps = _stride_time_features_for_forecasts(ds)
+        inputs["timestamps"] = timestamps
 
-    """
-    config = m.config_seasonality.periods[name]
-    t_i = np.arange(n_steps + 1) / float(n_steps)
-    features = time_dataset.fourier_series_t(
-        t=t_i * config.period, period=config.period, series_order=config.resolution
-    )
-    features = torch.from_numpy(np.expand_dims(features, 1))
+    if config_seasonality is not None:
+        seasonalities = seasonal_features_from_dates(df, config_seasonality)
+        for name, features in seasonalities.items():
+            if max_lags == 0:
+                seasonalities[name] = np.expand_dims(features, axis=1)
+            else:
+                # stride into num_forecast at dim=1 for each sample, just like we did with time
+                seasonalities[name] = _stride_time_features_for_forecasts(features)
+        inputs["seasonalities"] = seasonalities
+
+    def _stride_lagged_features(df_col_name, feature_dims):
+        # only for case where max_lags > 0
+        assert feature_dims >= 1
+        series = df.loc[:, df_col_name].values
+        # Added dtype=np.float64 to solve the problem with np.isnan for ubuntu test
+        return np.array(
+            [series[i + max_lags - feature_dims : i + max_lags] for i in range(n_samples)], dtype=np.float64
+        )
+
+    if n_lags > 0 and "y" in df.columns:
+        inputs["lags"] = _stride_lagged_features(df_col_name="y_scaled", feature_dims=n_lags)
+
+    if config_lagged_regressors is not None and max_lags > 0:
+        covariates = OrderedDict({})
+        for covar in df.columns:
+            if covar in config_lagged_regressors:
+                assert config_lagged_regressors[covar].n_lags > 0
+                window = config_lagged_regressors[covar].n_lags
+                covariates[covar] = _stride_lagged_features(df_col_name=covar, feature_dims=window)
+        inputs["covariates"] = covariates
+
+    # get the regressors features
+    if config_regressors is not None:
+        additive_regressors, multiplicative_regressors = make_regressors_features(df, config_regressors)
+
+        regressors = OrderedDict({})
+        if max_lags == 0:
+            if additive_regressors is not None:
+                regressors["additive"] = np.expand_dims(additive_regressors, axis=1)
+            if multiplicative_regressors is not None:
+                regressors["multiplicative"] = np.expand_dims(multiplicative_regressors, axis=1)
+        else:
+            if additive_regressors is not None:
+                additive_regressor_feature_windows = []
+                for i in range(0, additive_regressors.shape[1]):
+                    # stride into num_forecast at dim=1 for each sample, just like we did with time
+                    stride = _stride_time_features_for_forecasts(additive_regressors[:, i])
+                    additive_regressor_feature_windows.append(stride)
+                additive_regressors = np.dstack(additive_regressor_feature_windows)
+                regressors["additive"] = additive_regressors
+
+            if multiplicative_regressors is not None:
+                multiplicative_regressor_feature_windows = []
+                for i in range(0, multiplicative_regressors.shape[1]):
+                    # stride into num_forecast at dim=1 for each sample, just like we did with time
+                    stride = _stride_time_features_for_forecasts(multiplicative_regressors[:, i])
+                    multiplicative_regressor_feature_windows.append(stride)
+                multiplicative_regressors = np.dstack(multiplicative_regressor_feature_windows)
+                regressors["multiplicative"] = multiplicative_regressors
+
+        inputs["regressors"] = regressors
+
+    # get the events features
+    if config_events is not None or config_country_holidays is not None:
+        additive_events, multiplicative_events = make_events_features(df, config_events, config_country_holidays)
+
+        events = OrderedDict({})
+        if max_lags == 0:
+            if additive_events is not None:
+                events["additive"] = np.expand_dims(additive_events, axis=1)
+            if multiplicative_events is not None:
+                events["multiplicative"] = np.expand_dims(multiplicative_events, axis=1)
+        else:
+            if additive_events is not None:
+                additive_event_feature_windows = []
+                for i in range(0, additive_events.shape[1]):
+                    # stride into num_forecast at dim=1 for each sample, just like we did with time
+                    additive_event_feature_windows.append(_stride_time_features_for_forecasts(additive_events[:, i]))
+                additive_events = np.dstack(additive_event_feature_windows)
+                events["additive"] = additive_events
+
+            if multiplicative_events is not None:
+                multiplicative_event_feature_windows = []
+                for i in range(0, multiplicative_events.shape[1]):
+                    # stride into num_forecast at dim=1 for each sample, just like we did with time
+                    multiplicative_event_feature_windows.append(
+                        _stride_time_features_for_forecasts(multiplicative_events[:, i])
+                    )
+                multiplicative_events = np.dstack(multiplicative_event_feature_windows)
+                events["multiplicative"] = multiplicative_events
 
-    if df_name == "__df__":
-        meta_name_tensor = None
+        inputs["events"] = events
+    if predict_mode:
+        targets = np.empty_like(time)
+        targets = np.nan_to_num(targets)
     else:
-        meta = OrderedDict()
-        meta["df_name"] = [df_name for _ in range(n_steps + 1)]
-        meta_name_tensor = torch.tensor([m.model.id_dict[i] for i in meta["df_name"]])
-
-    quantile_index = m.model.quantiles.index(quantile)
-    predicted = m.model.seasonality.compute_fourier(features=features, name=name, meta=meta_name_tensor)[
-        :, :, quantile_index
-    ]
-    predicted = predicted.squeeze().detach().numpy()
-    if m.config_seasonality.mode == "additive":
-        data_params = m.config_normalization.get_data_params(df_name)
-        scale = data_params["y"].scale
-        predicted = predicted * scale
-    return t_i, predicted
-
-
-def predict_season_from_dates(m, dates, name, quantile, df_name="__df__"):
-    """
-     Predicts the seasonal component given a date range.
-
-     Parameters
-     ----------
-         m : NeuralProphet
-             Fitted NeuralProphet model
-         dates: pd.datetime
-             date range for prediction
-         name: str
-             Name of seasonality component
-         quantile: float
-             The quantile for which the season is predicted
-         df_name: str
-             Name of dataframe to refer to data params from original keys of train dataframes
+        targets = _stride_time_features_for_forecasts(df["y_scaled"].values)
+
+    tabularized_input_shapes_str = ""
+    for key, value in inputs.items():
+        if key in ["seasonalities", "covariates", "events", "regressors"]:
+            for name, period_features in value.items():
+                tabularized_input_shapes_str += f"    {name} {key} {period_features}\n"
+        else:
+            tabularized_input_shapes_str += f"    {key} {value.shape} \n"
+    log.debug(f"Tabularized inputs shapes: \n{tabularized_input_shapes_str}")
+
+    return inputs, targets, config_missing.drop_missing
+
+
+def fourier_series(dates, period, series_order):
+    """Provides Fourier series components with the specified frequency and order.
+
+    Note
+    ----
+    Identical to OG Prophet.
+
+    Parameters
+    ----------
+        dates : pd.Series
+            Containing timestamps
+        period : float
+            Number of days of the period
+        series_order : int
+            Number of fourier components
 
     Returns
     -------
-        predicted: OrderedDict
-             presdicted seasonal component
+        np.array
+            Matrix with seasonality features
     """
-    config = m.config_seasonality.periods[name]
-    features = time_dataset.fourier_series(dates=dates, period=config.period, series_order=config.resolution)
-    features = torch.from_numpy(np.expand_dims(features, 1))
-    if df_name == "__df__":
-        meta_name_tensor = None
-    else:
-        meta = OrderedDict()
-        meta["df_name"] = [df_name for _ in range(len(dates))]
-        meta_name_tensor = torch.tensor([m.model.id_dict[i] for i in meta["df_name"]])
-
-    quantile_index = m.model.quantiles.index(quantile)
-    predicted = m.model.seasonality.compute_fourier(features=features, name=name, meta=meta_name_tensor)[
-        :, :, quantile_index
-    ]
-
-    predicted = predicted.squeeze().detach().numpy()
-    if m.config_seasonality.mode == "additive":
-        data_params = m.config_normalization.get_data_params(df_name)
-        scale = data_params["y"].scale
-        predicted = predicted * scale
-    predicted = {name: predicted}
-    return predicted
+    # convert to days since epoch
+    t = np.array((dates - datetime(1970, 1, 1)).dt.total_seconds().astype(float)) / (3600 * 24.0)
+    return fourier_series_t(t, period, series_order)
+
 
+def fourier_series_t(t, period, series_order):
+    """Provides Fourier series components with the specified frequency and order.
 
-def check_if_configured(m, components, error_flag=False):  # move to utils
-    """Check if components were set in the model configuration by the user.
+    Note
+    ----
+    This function is identical to Meta AI's Prophet Library
 
     Parameters
     ----------
-        m : NeuralProphet
-            Fitted NeuralProphet model
-        components : str or list, optional
-            name or list of names of components to check
-
-            Options
-            ----
-            * ``trend``
-            * ``trend_rate_change``
-            * ``seasonality``
-            * ``autoregression``
-            * ``lagged_regressors```
-            * ``events``
-            * ``future_regressors`
-            * ``uncertainty``
-        error_flag : bool
-            Activate to raise a ValueError if component has not been configured
+        t : pd.Series, float
+            Containing time as floating point number of days
+        period : float
+            Number of days of the period
+        series_order : int
+            Number of fourier components
 
     Returns
     -------
-        components
-            list of components only including the components set in the model configuration
+        np.array
+            Matrix with seasonality features
     """
-    invalid_components = []
-    if "trend_rate_change" in components and m.model.config_trend.changepoints is None:
-        components.remove("trend_rate_change")
-        invalid_components.append("trend_rate_change")
-    if "seasonality" in components and m.config_seasonality is None:
-        components.remove("seasonality")
-        invalid_components.append("seasonality")
-    if "autoregression" in components and not m.config_ar.n_lags > 0:
-        components.remove("autoregression")
-        invalid_components.append("autoregression")
-    if "lagged_regressors" in components and m.config_lagged_regressors is None:
-        components.remove("lagged_regressors")
-        invalid_components.append("lagged_regressors")
-    if "events" in components and (m.config_events and m.config_country_holidays) is None:
-        components.remove("events")
-        invalid_components.append("events")
-    if "future_regressors" in components and m.config_regressors is None:
-        components.remove("future_regressors")
-        invalid_components.append("future_regressors")
-    if "uncertainty" in components and not len(m.model.quantiles) > 1:
-        components.remove("uncertainty")
-        invalid_components.append("uncertainty")
-    if error_flag and len(invalid_components) != 0:
-        raise ValueError(
-            f" Selected component(s) {(invalid_components)} for plotting not specified in the model configuration."
-        )
-    return components
+    features = np.column_stack(
+        [fun((2.0 * (i + 1) * np.pi * t / period)) for i in range(series_order) for fun in (np.sin, np.cos)]
+    )
+    return features
 
 
-def get_valid_configuration(  # move to utils
-    m, components=None, df_name=None, valid_set=None, validator=None, forecast_in_focus=None, quantile=0.5
-):
-    """Validate and adapt the selected components to be plotted.
+def make_country_specific_holidays_df(year_list, country):
+    """
+    Make dataframe of country specific holidays for given years and countries
 
     Parameters
     ----------
-        m : NeuralProphet
-            Fitted NeuralProphet model
-        components : str or list, optional
-            name or list of names of components to validate and adapt
-        df_name: str
-            ID from time series that should be plotted
-        valid_set : str or list, optional
-            name or list of names of components that are defined as valid option
+        year_list : list
+            List of years
+        country : str, list
+            List of country names
 
-            Options
-            ----
-             * (default)``None``:  All components the user set in the model configuration are validated and adapted
-            * ``trend``
-            * ``seasonality``
-            * ``autoregression``
-            * ``lagged_regressors``
-            * ``future_regressors``
-            * ``events``
-            * ``uncertainty``
-        validator: str
-            specifies the validation purpose to customize
+    Returns
+    -------
+        pd.DataFrame
+            Containing country specific holidays df with columns 'ds' and 'holiday'
+    """
+    # iterate over countries and get holidays for each country
+    # convert to list if not already
+    if isinstance(country, str):
+        country = [country]
+    country_specific_holidays = {}
+    for single_country in country:
+        single_country_specific_holidays = get_country_holidays(single_country, year_list)
+        # only add holiday if it is not already in the dict
+        country_specific_holidays.update(single_country_specific_holidays)
+    country_specific_holidays_dict = defaultdict(list)
+    for date, holiday in country_specific_holidays.items():
+        country_specific_holidays_dict[holiday].append(pd.to_datetime(date))
+    return country_specific_holidays_dict
 
-            Options
-            ----
-            * ``plot_parameters``: customize for plot_parameters() function
-            * ``plot_components``: customize for plot_components() function
-        forecast_in_focus: int
-            optinal, i-th step ahead forecast to plot
 
-            Note
-            ----
-            None (default): plot self.highlight_forecast_step_n by default
-        quantile: float
-            The quantile for which the model parameters are to be plotted
+def _create_event_offset_features(event, config, feature, additive_events, multiplicative_events):
+    """
+    Create event offset features for the given event, config and feature
 
-            Note
-            ----
-            0.5 (default):  Parameters will be plotted for the median quantile.
+    Parameters
+    ----------
+        event : str
+            Name of the event
+        config : configure.ConfigEvents
+            User specified events, holidays, and country specific holidays
+        feature : pd.Series
+            Feature for the event
+        additive_events : pd.DataFrame
+            Dataframe of additive events
+        multiplicative_events : pd.DataFrame
+            Dataframe of multiplicative events
 
     Returns
     -------
-        valid_configuration: dict
-            dict of validated components and values to be plotted
+        tuple
+            Tuple of additive_events and multiplicative_events
     """
-    if type(valid_set) is not list:
-        valid_set = [valid_set]
-
-    if components is None:
-        components = valid_set
-        components = check_if_configured(m=m, components=components)
-    else:
-        if type(components) is not list:
-            components = [components]
-        components = [comp.lower() for comp in components]
-        for comp in components:
-            if comp not in valid_set:
-                raise ValueError(
-                    f" Selected component {comp} is either mis-spelled or not an available "
-                    f"option for this function."
-                )
-        components = check_if_configured(m=m, components=components, error_flag=True)
-    if validator is None:
-        raise ValueError("Specify a validator from the available options")
-    # Adapt Normalization
-    if validator == "plot_parameters":
-        # Set to True in case of local normalization and unknown_data_params is not True
-        overwriting_unknown_data_normalization = False
-        if m.config_normalization.global_normalization:
-            if df_name is None and m.id_list.__len__() == 1:
-                df_name = "__df__"
-            elif df_name is None and m.id_list.__len__() > 1:
-                df_name = m.id_list[0]
-            else:
-                log.debug("Global normalization set - ignoring given df_name for normalization")
+    lw = config.lower_window
+    uw = config.upper_window
+    mode = config.mode
+    for offset in range(lw, uw + 1):
+        key = utils.create_event_names_for_offsets(event, offset)
+        offset_feature = feature.shift(periods=offset, fill_value=0.0)
+        if mode == "additive":
+            additive_events[key] = offset_feature
         else:
-            if df_name is None:
-                if m.id_list.__len__() > 1:
-                    if (
-                        m.model.config_seasonality.global_local == "local"
-                        or m.model.config_trend.trend_global_local == "local"
-                    ):
-                        df_name = m.id_list
-                        log.warning(
-                            "Glocal model set with > 1 time series in the pd.DataFrame. Plotting components of mean time series and quants. "
-                        )
-                    else:
-                        df_name = m.id_list[0]
-                        log.warning(
-                            "Local model set with > 1 time series in the pd.DataFrame. Plotting components of first time series. "
-                        )
-                else:
-                    log.warning("Local normalization set, but df_name is None. Using global data params instead.")
-                    df_name = "__df__"
-                if not m.config_normalization.unknown_data_normalization:
-                    m.config_normalization.unknown_data_normalization = True
-                    overwriting_unknown_data_normalization = True
-            elif df_name not in m.config_normalization.local_data_params:
-                log.warning(
-                    f"Local normalization set, but df_name '{df_name}' not found. Using global data params instead."
-                )
-                df_name = "__df__"
-                if not m.config_normalization.unknown_data_normalization:
-                    m.config_normalization.unknown_data_normalization = True
-                    overwriting_unknown_data_normalization = True
-            else:
-                log.debug(f"Local normalization set. Data params for {df_name} will be used to denormalize.")
+            multiplicative_events[key] = offset_feature
 
-    # Identify components to be plotted
-    # as dict, minimum: {plot_name}
-    plot_components = []
-    if validator == "plot_parameters":
-        quantile_index = m.model.quantiles.index(quantile)
-
-    # Plot trend
-    if "trend" in components:
-        plot_components.append({"plot_name": "Trend", "comp_name": "trend"})
-    if "trend_rate_change" in components:
-        plot_components.append({"plot_name": "Trend Rate Change"})
-
-    # Plot  seasonalities, if present
-    if "seasonality" in components:
-        for name in m.config_seasonality.periods:
-            if validator == "plot_components":
-                plot_components.append(
-                    {
-                        "plot_name": f"{name} seasonality",
-                        "comp_name": name,
-                    }
-                )
-            elif validator == "plot_parameters":
-                plot_components.append({"plot_name": "seasonality", "comp_name": name})
 
-    # AR
-    if "autoregression" in components:
-        if validator == "plot_components":
-            if forecast_in_focus is None:
-                plot_components.append(
-                    {
-                        "plot_name": "Auto-Regression",
-                        "comp_name": "ar",
-                        "num_overplot": m.n_forecasts,
-                        "bar": True,
-                    }
-                )
-            else:
-                plot_components.append(
-                    {
-                        "plot_name": f"AR ({forecast_in_focus})-ahead",
-                        "comp_name": f"ar{forecast_in_focus}",
-                    }
-                )
-        elif validator == "plot_parameters":
-            plot_components.append(
-                {
-                    "plot_name": "lagged weights",
-                    "comp_name": "AR",
-                    "weights": utils_torch.interprete_model(m.model, net="ar_net", forward_func="auto_regression")
-                    .detach()
-                    .numpy(),
-                    "focus": forecast_in_focus,
-                }
-            )
+def make_events_features(df, config_events: Optional[configure.ConfigEvents] = None, config_country_holidays=None):
+    """
+    Construct arrays of all event features
 
-    # Add lagged regressors
-    lagged_scalar_regressors = []
-    if "lagged_regressors" in components:
-        if validator == "plot_components":
-            if forecast_in_focus is None:
-                for name in m.config_lagged_regressors.keys():
-                    plot_components.append(
-                        {
-                            "plot_name": f'Lagged Regressor "{name}"',
-                            "comp_name": f"lagged_regressor_{name}",
-                            "num_overplot": m.n_forecasts,
-                            "bar": True,
-                        }
-                    )
-            else:
-                for name in m.config_lagged_regressors.keys():
-                    plot_components.append(
-                        {
-                            "plot_name": f'Lagged Regressor "{name}" ({forecast_in_focus})-ahead',
-                            "comp_name": f"lagged_regressor_{name}{forecast_in_focus}",
-                        }
-                    )
-        elif validator == "plot_parameters":
-            for name in m.config_lagged_regressors.keys():
-                if m.config_lagged_regressors[name].as_scalar:
-                    lagged_scalar_regressors.append((name, m.model.get_covar_weights()[name].detach().numpy()))
-                else:
-                    plot_components.append(
-                        {
-                            "plot_name": "lagged weights",
-                            "comp_name": f'Lagged Regressor "{name}"',
-                            "weights": m.model.get_covar_weights()[name].detach().numpy(),
-                            "focus": forecast_in_focus,
-                        }
-                    )
+    Parameters
+    ----------
+        df : pd.DataFrame
+            Dataframe with all values including the user specified events (provided by user)
+        config_events : configure.ConfigEvents
+            User specified events, each with their upper, lower windows (int), regularization
+        config_country_holidays : configure.ConfigCountryHolidays
+            Configurations (holiday_names, upper, lower windows, regularization) for country specific holidays
 
-    # Add Events
-    additive_events = []
-    multiplicative_events = []
-    if "events" in components:
-        additive_events_flag = False
-        muliplicative_events_flag = False
-        for event, configs in m.config_events.items():
-            if validator == "plot_components" and configs.mode == "additive":
-                additive_events_flag = True
-            elif validator == "plot_components" and configs.mode == "multiplicative":
-                muliplicative_events_flag = True
-            elif validator == "plot_parameters":
-                event_params = m.model.get_event_weights(event)
-                weight_list = [(key, param.detach().numpy()[quantile_index, :]) for key, param in event_params.items()]
-                if configs.mode == "additive":
-                    additive_events = additive_events + weight_list
-                elif configs.mode == "multiplicative":
-                    multiplicative_events = multiplicative_events + weight_list
-
-        for country_holiday in m.config_country_holidays.holiday_names:
-            if validator == "plot_components" and m.config_country_holidays.mode == "additive":
-                additive_events_flag = True
-            elif validator == "plot_components" and m.config_country_holidays.mode == "multiplicative":
-                muliplicative_events_flag = True
-            elif validator == "plot_parameters":
-                event_params = m.model.get_event_weights(country_holiday)
-                weight_list = [(key, param.detach().numpy()[quantile_index, :]) for key, param in event_params.items()]
-                if m.config_country_holidays.mode == "additive":
-                    additive_events = additive_events + weight_list
-                elif m.config_country_holidays.mode == "multiplicative":
-                    multiplicative_events = multiplicative_events + weight_list
-
-        if additive_events_flag:
-            plot_components.append(
-                {
-                    "plot_name": "Additive Events",
-                    "comp_name": "events_additive",
-                }
-            )
-        if muliplicative_events_flag:
-            plot_components.append(
-                {
-                    "plot_name": "Multiplicative Events",
-                    "comp_name": "events_multiplicative",
-                    "multiplicative": True,
-                }
+    Returns
+    -------
+        np.array
+            All additive event features (both user specified and country specific)
+        np.array
+            All multiplicative event features (both user specified and country specific)
+    """
+    df = df.reset_index(drop=True)
+    additive_events = pd.DataFrame()
+    multiplicative_events = pd.DataFrame()
+
+    # create all user specified events
+    if config_events is not None:
+        for event, configs in config_events.items():
+            if event not in df.columns:
+                df[event] = np.zeros_like(df["ds"], dtype=np.float64)
+            feature = df[event]
+            _create_event_offset_features(event, configs, feature, additive_events, multiplicative_events)
+
+    # create all country specific holidays
+    if config_country_holidays is not None:
+        year_list = list({x.year for x in df.ds})
+        country_holidays_dict = make_country_specific_holidays_df(year_list, config_country_holidays.country)
+        for holiday in config_country_holidays.holiday_names:
+            feature = pd.Series([0.0] * df.shape[0])
+            if holiday in country_holidays_dict.keys():
+                dates = country_holidays_dict[holiday]
+                feature[df.ds.isin(dates)] = 1.0
+            _create_event_offset_features(
+                holiday, config_country_holidays, feature, additive_events, multiplicative_events
             )
 
-    # Add Regressors
-    additive_future_regressors = []
-    multiplicative_future_regressors = []
-    if "future_regressors" in components:
-        for regressor, configs in m.config_regressors.items():
-            if validator == "plot_components" and configs.mode == "additive":
-                plot_components.append(
-                    {
-                        "plot_name": "Additive Future Regressors",
-                        "comp_name": "future_regressors_additive",
-                    }
-                )
-            elif validator == "plot_components" and configs.mode == "multiplicative":
-                plot_components.append(
-                    {
-                        "plot_name": "Multiplicative Future Regressors",
-                        "comp_name": "future_regressors_multiplicative",
-                        "multiplicative": True,
-                    }
-                )
-            elif validator == "plot_parameters":
-                regressor_param = m.model.future_regressors.get_reg_weights(regressor)[quantile_index, :]
-                if configs.mode == "additive":
-                    additive_future_regressors.append((regressor, regressor_param.detach().numpy()))
-                elif configs.mode == "multiplicative":
-                    multiplicative_future_regressors.append((regressor, regressor_param.detach().numpy()))
-
-    # Plot  quantiles as a separate component, if present
-    # If multiple steps in the future are predicted, only plot quantiles if highlight_forecast_step_n is set
-    if (
-        "quantiles" in components
-        and validator == "plot_components"
-        and len(m.model.quantiles) > 1
-        and forecast_in_focus is None
-    ):
-        if len(m.config_train.quantiles) > 1 and (
-            m.n_forecasts > 1 or m.config_ar.n_lags > 0
-        ):  # rather query if n_forecasts >1 than n_lags>1
-            raise ValueError(
-                "Please specify step_number using the highlight_nth_step_ahead_of_each_forecast function"
-                " for quantiles plotting when autoregression enabled."
-            )
-        for i in range(1, len(m.model.quantiles)):
-            plot_components.append(
-                {
-                    "plot_name": "Uncertainty",
-                    "comp_name": f"yhat1 {round(m.model.quantiles[i] * 100, 1)}%",
-                    "fill": True,
-                }
-            )
-    elif (
-        "uncertainty" in components
-        and validator == "plot_components"
-        and len(m.model.quantiles) > 1
-        and forecast_in_focus is not None
-    ):
-        for i in range(1, len(m.model.quantiles)):
-            plot_components.append(
-                {
-                    "plot_name": "Uncertainty",
-                    "comp_name": f"yhat{forecast_in_focus} {round(m.model.quantiles[i] * 100, 1)}%",
-                    "fill": True,
-                }
-            )
-    if validator == "plot_parameters":
-        if len(additive_future_regressors) > 0:
-            plot_components.append({"plot_name": "Additive future regressor"})
-        if len(multiplicative_future_regressors) > 0:
-            plot_components.append({"plot_name": "Multiplicative future regressor"})
-        if len(lagged_scalar_regressors) > 0:
-            plot_components.append({"plot_name": "Lagged scalar regressor"})
-        if len(additive_events) > 0:
-            data_params = m.config_normalization.get_data_params(df_name)
-            scale = data_params["y"].scale
-            additive_events = [(key, weight * scale) for (key, weight) in additive_events]
-            plot_components.append({"plot_name": "Additive event"})
-        if len(multiplicative_events) > 0:
-            plot_components.append({"plot_name": "Multiplicative event"})
-
-        valid_configuration = {
-            "components_list": plot_components,
-            "additive_future_regressors": additive_future_regressors,
-            "additive_events": additive_events,
-            "multiplicative_future_regressors": multiplicative_future_regressors,
-            "multiplicative_events": multiplicative_events,
-            "lagged_scalar_regressors": lagged_scalar_regressors,
-            "overwriting_unknown_data_normalization": overwriting_unknown_data_normalization,
-            "df_name": df_name,
-        }
-    elif validator == "plot_components":
-        valid_configuration = {
-            "components_list": plot_components,
-        }
-    return valid_configuration
+    # Make sure column order is consistent
+    if not additive_events.empty:
+        additive_events = additive_events[sorted(additive_events.columns.tolist())]
+        additive_events = additive_events.values
+    else:
+        additive_events = None
+    if not multiplicative_events.empty:
+        multiplicative_events = multiplicative_events[sorted(multiplicative_events.columns.tolist())]
+        multiplicative_events = multiplicative_events.values
+    else:
+        multiplicative_events = None
 
+    return additive_events, multiplicative_events
 
-def validate_current_env_for_resampler(auto: bool = False) -> Optional[bool]:
-    """
-    Validate the current environment to check if it is a valid environment for plotly-resampler and if invalid trigger warning message.
+
+def make_regressors_features(df, config_regressors):
+    """Construct arrays of all scalar regressor features
 
     Parameters
     ----------
-    auto: bool, optional
-        If True, the function will automatically switch to a valid environment if the current environment is not valid.
-        If False, the function will return None if the current environment is not valid.
+        df : pd.DataFrame
+            Dataframe with all values including the user specified regressors
+        config_regressors : configure.ConfigFutureRegressors
+            User specified regressors config
+
     Returns
     -------
-    bool :
-        True if the current environment is a valid environment to run the code, False if the current environment is
-        not a valid environment to run the code. None if the current environment is not a valid environment to run
-        the code and the function did not switch to a valid environment.
+        np.array
+            All additive regressor features
+        np.array
+            All multiplicative regressor features
+
     """
+    additive_regressors = pd.DataFrame()
+    multiplicative_regressors = pd.DataFrame()
+
+    for reg in df.columns:
+        if reg in config_regressors:
+            mode = config_regressors[reg].mode
+            if mode == "additive":
+                additive_regressors[reg] = df[reg]
+            else:
+                multiplicative_regressors[reg] = df[reg]
 
-    from IPython import get_ipython
-
-    if "google.colab" in str(get_ipython()):
-        if auto:
-            log_warning_resampler_switch_to_valid_env()
-            valid_env = False
-        else:
-            log_warning_resampler_invalid_env()
-            valid_env = None
+    if not additive_regressors.empty:
+        additive_regressors = additive_regressors[sorted(additive_regressors.columns.tolist())]
+        additive_regressors = additive_regressors.values
     else:
-        if is_notebook():
-            valid_env = True
-        else:
-            if auto:
-                log_warning_resampler_switch_to_valid_env()
-                valid_env = False
-            else:
-                log_warning_resampler_invalid_env()
-                valid_env = None
-    return valid_env
+        additive_regressors = None
+    if not multiplicative_regressors.empty:
+        multiplicative_regressors = multiplicative_regressors[sorted(multiplicative_regressors.columns.tolist())]
+        multiplicative_regressors = multiplicative_regressors.values
+    else:
+        multiplicative_regressors = None
 
+    return additive_regressors, multiplicative_regressors
 
-def is_notebook():
-    """
-    Determine if the code is being executed in a Jupyter notebook environment.
 
-    Returns
-    -------
-    bool :
-        True if the code is being executed in a Jupyter notebook, False otherwise.
-    """
-    try:
-        from IPython import get_ipython
+def seasonal_features_from_dates(df, config_seasonality: configure.ConfigSeasonality):
+    """Dataframe with seasonality features.
 
-        if "IPKernelApp" not in get_ipython().config:  # pragma: no cover
-            return False
-    except ImportError:
-        return False
-    except AttributeError:
-        return False
-    return True
-
-
-def select_plotting_backend(model, plotting_backend):
-    """Automatically selects the plotting backend based on the global plotting_backend and plotting_backend set by the
-    user. If the plotting backend is selected as "plotly-resampler", triggers warning message.
+    Includes seasonality features, holiday features, and added regressors.
 
     Parameters
     ----------
-    model: NeuralProphet
-        The configured model.
-    plotting_backend: str
-        The plotting backend to use.
+        df : pd.DataFrame
+            Dataframe with all values
+        config_seasonality : configure.ConfigSeasonality
+            Configuration for seasonalities
 
     Returns
     -------
-    str
-        The new plotting backend.
-    """
-    if hasattr(model, "plotting_backend") and plotting_backend is None:
-        plotting_backend = model.plotting_backend
-        if plotting_backend == "plotly-resampler":
-            validate_current_env_for_resampler()
-    else:
-        if plotting_backend is None:
-            if validate_current_env_for_resampler(auto=True):
-                plotting_backend = "plotly-resampler"
+        OrderedDict
+            Dictionary with keys for each period name containing an np.array
+            with the respective regression features. each with dims: (len(dates), 2*fourier_order)
+    """
+    dates = df["ds"]
+    assert len(dates.shape) == 1
+    seasonalities = OrderedDict({})
+    # Seasonality features
+    for name, period in config_seasonality.periods.items():
+        if period.resolution > 0:
+            if config_seasonality.computation == "fourier":
+                features = fourier_series(
+                    dates=dates,
+                    period=period.period,
+                    series_order=period.resolution,
+                )
             else:
-                plotting_backend = "plotly"
-        elif plotting_backend == "plotly-resampler":
-            validate_current_env_for_resampler()
-    return plotting_backend.lower()
+                raise NotImplementedError
+            if period.condition_name is not None:
+                features = features * df[period.condition_name].values[:, np.newaxis]
+            seasonalities[name] = features
+    return seasonalities
```

### Comparing `neuralprophet-0.6.0/neuralprophet/time_net.py` & `neuralprophet-0.6.0rc1/neuralprophet/time_net.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 import logging
 import math
 from collections import OrderedDict
-from functools import reduce
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 import torchmetrics
 
-from neuralprophet import configure, np_types
+from neuralprophet import configure, np_types, utils
 from neuralprophet.components.router import get_future_regressors, get_seasonality, get_trend
-from neuralprophet.utils import (
-    check_for_regularization,
-    config_events_to_model_dims,
-    reg_func_events,
-    reg_func_regressors,
-    reg_func_season,
-    reg_func_trend,
-)
-from neuralprophet.utils_torch import init_parameter, interprete_model
+from neuralprophet.utils_torch import init_parameter
 
 log = logging.getLogger("NP.time_net")
 
 
 class TimeNet(pl.LightningModule):
     """Linear time regression fun and some not so linear fun.
+
     A modular model that models classic time-series components
         * trend
         * seasonality
         * auto-regression (as AR-Net)
         * covariates (as AR-Net)
         * apriori regressors
         * events and holidays
@@ -48,97 +40,124 @@
         config_lagged_regressors: Optional[configure.ConfigLaggedRegressors] = None,
         config_regressors: Optional[configure.ConfigFutureRegressors] = None,
         config_events: Optional[configure.ConfigEvents] = None,
         config_holidays: Optional[configure.ConfigCountryHolidays] = None,
         n_forecasts: int = 1,
         n_lags: int = 0,
         max_lags: int = 0,
-        ar_layers: Optional[List[int]] = [],
-        lagged_reg_layers: Optional[List[int]] = [],
+        num_hidden_layers: int = 0,
+        d_hidden: Optional[int] = None,
         compute_components_flag: bool = False,
         metrics: Optional[np_types.CollectMetricsMode] = {},
         id_list: List[str] = ["__df__"],
         num_trends_modelled: int = 1,
         num_seasonalities_modelled: int = 1,
         meta_used_in_model: bool = False,
     ):
         """
         Parameters
         ----------
             quantiles : list
                 the set of quantiles estimated
+
             config_train : configure.Train
+
             config_trend : configure.Trend
+
             config_seasonality : configure.ConfigSeasonality
+
             config_ar : configure.AR
+
             config_lagged_regressors : configure.ConfigLaggedRegressors
                 Configurations for lagged regressors
             config_regressors : configure.ConfigFutureRegressors
                 Configs of regressors with mode and index.
             config_events : configure.ConfigEvents
+
             config_holidays : OrderedDict
+
             config_normalization: OrderedDict
+
             n_forecasts : int
                 number of steps to forecast. Aka number of model outputs
             n_lags : int
                 number of previous steps of time series used as input (aka AR-order)
+
                 Note
                 ----
                 The default value is ``0``, which initializes no auto-regression.
+            num_hidden_layers : int
+                Number of hidden layers (for AR-Net)
+
+                Note
+                ----
+                The default value is ``0``, which initializes no hidden layers (classic Auto-Regression).
 
             max_lags : int
                 Number of max. previous steps of time series used as input (aka AR-order).
 
-            ar_layers : list
-                List of hidden layers (for AR-Net).
+            num_hidden_layers : int
+                Number of hidden layers (for AR-Net).
+
+            d_hidden : int
+                Dimensionality of hidden layers  (for AR-Net).
 
                 Note
                 ----
-                The default value is ``[]``, which initializes no hidden layers.
-
-            lagged_reg_layers : list
-                List of hidden layers (for covariate-Net).
+                This parameter is ignored if no hidden layers are specified.
 
                 Note
                 ----
-                The default value is ``[]``, which initializes no hidden layers.
-
+                The default value is set to ``None``, which sets to ``n_lags + n_forecasts``.
 
             compute_components_flag : bool
                 Flag whether to compute the components of the model or not.
+
             metrics : dict
                 Dictionary of torchmetrics to be used during training and for evaluation.
+
             id_list : list
                 List of different time series IDs, used for global-local modelling (if enabled)
+
                 Note
                 ----
                 This parameter is set to  ``['__df__']`` if only one time series is input.
+
             num_trends_modelled : int
                 Number of different trends modelled.
+
                 Note
                 ----
                 If only 1 time series is modelled, it will be always 1.
+
                 Note
                 ----
                 For multiple time series. If trend is modelled globally the value is set
                 to 1, otherwise it is set to the number of time series modelled.
+
             num_seasonalities_modelled : int
                 Number of different seasonalities modelled.
+
                 Note
                 ----
                 If only 1 time series is modelled, it will be always 1.
+
                 Note
                 ----
                 For multiple time series. If seasonality is modelled globally the value is set
                 to 1, otherwise it is set to the number of time series modelled.
+
             meta_used_in_model : boolean
                 Whether we need to know the time series ID when we interact with the Model.
+
                 Note
                 ----
                 Will be set to ``True`` if more than one component is modelled locally.
+
+
         """
         super().__init__()
 
         # Store hyerparameters in model checkpoint
         # TODO: causes a RuntimeError under certain conditions, investigate and handle better
         try:
             self.save_hyperparameters()
@@ -178,15 +197,15 @@
         self.id_list = id_list
         self.id_dict = dict((key, i) for i, key in enumerate(id_list))
         self.num_trends_modelled = num_trends_modelled
         self.num_seasonalities_modelled = num_seasonalities_modelled
         self.meta_used_in_model = meta_used_in_model
 
         # Regularization
-        self.reg_enabled = check_for_regularization(
+        self.reg_enabled = utils.check_for_regularization(
             [
                 config_seasonality,
                 config_regressors,
                 config_lagged_regressors,
                 config_ar,
                 config_events,
                 config_trend,
@@ -225,15 +244,15 @@
                 n_forecasts=n_forecasts,
                 device=self.device,
             )
 
         # Events
         self.config_events = config_events
         self.config_holidays = config_holidays
-        self.events_dims = config_events_to_model_dims(self.config_events, self.config_holidays)
+        self.events_dims = utils.config_events_to_model_dims(self.config_events, self.config_holidays)
         if self.events_dims is not None:
             n_additive_event_params = 0
             n_multiplicative_event_params = 0
             for event, configs in self.events_dims.items():
                 if configs["mode"] not in ["additive", "multiplicative"]:
                     log.error("Event Mode {} not implemented. Defaulting to 'additive'.".format(configs["mode"]))
                     self.events_dims[event]["mode"] = "additive"
@@ -255,39 +274,56 @@
         else:
             self.config_events = None
             self.config_holidays = None
 
         # Autoregression
         self.config_ar = config_ar
         self.n_lags = n_lags
-        self.ar_layers = ar_layers
         self.max_lags = max_lags
+        self.num_hidden_layers = num_hidden_layers
+        self.d_hidden = (
+            max(4, round((n_lags + n_forecasts) / (2.0 * (num_hidden_layers + 1)))) if d_hidden is None else d_hidden
+        )
         if self.n_lags > 0:
             self.ar_net = nn.ModuleList()
             d_inputs = self.n_lags
-            for d_hidden_i in self.ar_layers:
-                self.ar_net.append(nn.Linear(d_inputs, d_hidden_i, bias=True))
-                d_inputs = d_hidden_i
+            for i in range(self.num_hidden_layers):
+                self.ar_net.append(nn.Linear(d_inputs, self.d_hidden, bias=True))
+                d_inputs = self.d_hidden
             # final layer has input size d_inputs and output size equal to no. of forecasts * no. of quantiles
             self.ar_net.append(nn.Linear(d_inputs, self.n_forecasts * len(self.quantiles), bias=False))
             for lay in self.ar_net:
                 nn.init.kaiming_normal_(lay.weight, mode="fan_in")
 
         # Lagged regressors
-        self.lagged_reg_layers = lagged_reg_layers
         self.config_lagged_regressors = config_lagged_regressors
         if self.config_lagged_regressors is not None:
-            self.covar_net = nn.ModuleList()
-            d_inputs = sum([covar.n_lags for _, covar in self.config_lagged_regressors.items()])
-            for d_hidden_i in self.lagged_reg_layers:
-                self.covar_net.append(nn.Linear(d_inputs, d_hidden_i, bias=True))
-                d_inputs = d_hidden_i
-            self.covar_net.append(nn.Linear(d_inputs, self.n_forecasts * len(self.quantiles), bias=False))
-            for lay in self.covar_net:
-                nn.init.kaiming_normal_(lay.weight, mode="fan_in")
+            self.covar_nets = nn.ModuleDict({})
+            for covar in self.config_lagged_regressors.keys():
+                covar_net = nn.ModuleList()
+                d_inputs = self.config_lagged_regressors[covar].n_lags
+                for i in range(self.config_lagged_regressors[covar].num_hidden_layers):
+                    d_hidden = (
+                        max(
+                            4,
+                            round(
+                                (self.config_lagged_regressors[covar].n_lags + n_forecasts)
+                                / (2.0 * (self.config_lagged_regressors[covar].num_hidden_layers + 1))
+                            ),
+                        )
+                        if self.config_lagged_regressors[covar].d_hidden is None
+                        else self.config_lagged_regressors[covar].d_hidden
+                    )
+                    covar_net.append(nn.Linear(d_inputs, d_hidden, bias=True))
+                    d_inputs = d_hidden
+                # final layer has input size d_inputs and output size equal to no. of forecasts * no. of quantiles
+                covar_net.append(nn.Linear(d_inputs, self.n_forecasts * len(self.quantiles), bias=False))
+                for lay in covar_net:
+                    nn.init.kaiming_normal_(lay.weight, mode="fan_in")
+                self.covar_nets[covar] = covar_net
 
         # Regressors
         self.config_regressors = config_regressors
         if self.config_regressors is not None:
             # Initialize future_regressors
             self.future_regressors = get_future_regressors(
                 config=config_regressors,
@@ -299,64 +335,29 @@
             )
         else:
             self.config_regressors = None
 
     @property
     def ar_weights(self) -> torch.Tensor:
         """sets property auto-regression weights for regularization. Update if AR is modelled differently"""
-        # TODO: this is wrong for deep networks, use utils_torch.interprete_model
         return self.ar_net[0].weight
 
-    def get_covar_weights(self, covar_input=None) -> torch.Tensor:
-        """
-        Get attributions of covariates network w.r.t. the model input.
-        """
-        if self.config_lagged_regressors is not None:
-            # Accumulate the lags of the covariates
-            covar_splits = np.add.accumulate(
-                [covar.n_lags for _, covar in self.config_lagged_regressors.items()][:-1]
-            ).tolist()
-            # If actual covariates are provided, use them to compute the attributions
-            if covar_input is not None:
-                covar_input = torch.cat([covar for _, covar in covar_input.items()], axis=1)
-            # Calculate the attributions w.r.t. the inputs
-            if self.lagged_reg_layers == []:
-                attributions = self.covar_net[0].weight
-            else:
-                attributions = interprete_model(self, "covar_net", "forward_covar_net", covar_input)
-            # Split the attributions into the different covariates
-            attributions_split = torch.tensor_split(
-                attributions,
-                covar_splits,
-                axis=1,
-            )
-            # Combine attributions and covariate name
-            covar_attributions = dict(zip(self.config_lagged_regressors.keys(), attributions_split))
-        else:
-            covar_attributions = None
-        return covar_attributions
-
-    def set_covar_weights(self, covar_weights: torch.Tensor):
-        """
-        Function to set the covariate weights for later interpretation in compute_components.
-        This function is needed since the gradient information is not available during the predict_step
-        method and attributions cannot be calculated in compute_components.
-
-        :param covar_weights: _description_
-        :type covar_weights: torch.Tensor
-        """
-        self.covar_weights = covar_weights
+    def get_covar_weights(self, name: str) -> torch.Tensor:
+        """sets property auto-regression weights for regularization. Update if AR is modelled differently"""
+        return self.covar_nets[name][0].weight
 
     def get_event_weights(self, name: str) -> Dict[str, torch.Tensor]:
         """
         Retrieve the weights of event features given the name
+
         Parameters
         ----------
             name : str
                 Event name
+
         Returns
         -------
             OrderedDict
                 Dict of the weights of all offsets corresponding to a particular event
         """
 
         event_dims = self.events_dims[name]
@@ -372,21 +373,23 @@
         for event_delim, indices in zip(event_dims["event_delim"], event_dims["event_indices"]):
             event_param_dict[event_delim] = event_params[:, indices : (indices + 1)]
         return event_param_dict
 
     def _compute_quantile_forecasts_from_diffs(self, diffs: torch.Tensor, predict_mode: bool = False) -> torch.Tensor:
         """
         Computes the actual quantile forecasts from quantile differences estimated from the model
+
         Args:
             diffs : torch.Tensor
                 tensor of dims (batch, n_forecasts, no_quantiles) which
                 contains the median quantile forecasts as well as the diffs of other quantiles
                 from the median quantile
             predict_mode : bool
                 boolean variable indicating whether the model is in prediction mode
+
         Returns:
             dim (batch, n_forecasts, no_quantiles)
                 final forecasts
         """
         if len(self.quantiles) > 1:
             # generate the actual quantile forecasts from predicted differences
             if any(quantile > 0.5 for quantile in self.quantiles):
@@ -431,14 +434,15 @@
         else:
             out = diffs
         return out
 
     def scalar_features_effects(self, features: torch.Tensor, params: nn.Parameter, indices=None) -> torch.Tensor:
         """
         Computes events component of the model
+
         Parameters
         ----------
             features : torch.Tensor, float
                 Features (either additive or multiplicative) related to event component dims (batch, n_forecasts, n_features)
             params : nn.Parameter
                 Params (either additive or multiplicative) related to events
             indices : list of int
@@ -452,123 +456,153 @@
             features = features[:, :, indices]
             params = params[:, indices]
 
         return torch.sum(features.unsqueeze(dim=2) * params.unsqueeze(dim=0).unsqueeze(dim=0), dim=-1)
 
     def auto_regression(self, lags: Union[torch.Tensor, float]) -> torch.Tensor:
         """Computes auto-regessive model component AR-Net.
+
         Parameters
         ----------
             lags  : torch.Tensor, float
                 Previous times series values, dims: (batch, n_lags)
+
         Returns
         -------
             torch.Tensor
                 Forecast component of dims: (batch, n_forecasts)
         """
         x = lags
-        for i in range(len(self.ar_layers) + 1):
+        for i in range(self.num_hidden_layers + 1):
             if i > 0:
                 x = nn.functional.relu(x)
             x = self.ar_net[i](x)
 
         # segment the last dimension to match the quantiles
         x = x.reshape(x.shape[0], self.n_forecasts, len(self.quantiles))
         return x
 
-    def forward_covar_net(self, covariates):
-        """Compute all covariate components.
+    def covariate(self, lags: Union[torch.Tensor, float], name: str) -> torch.Tensor:
+        """Compute single covariate component.
+
         Parameters
         ----------
-            covariates : dict(torch.Tensor, float)
-                dict of named covariates (keys) with their features (values)
-                dims of each dict value: (batch, n_lags)
+            lags : torch.Tensor, float
+                Lagged values of covariate, dims: (batch, n_lags)
+            nam : str
+                Mame of covariate, for attribution to corresponding model weights
+
         Returns
         -------
             torch.Tensor
-                Forecast component of dims (batch, n_forecasts, quantiles)
+                Forecast component of dims (batch, n_forecasts)
         """
-        # Concat covariates into one tensor)
-        if isinstance(covariates, dict):
-            x = torch.cat([covar for _, covar in covariates.items()], axis=1)
-        else:
-            x = covariates
-        for i in range(len(self.lagged_reg_layers) + 1):
+        x = lags
+        for i in range(self.config_lagged_regressors[name].num_hidden_layers + 1):
             if i > 0:
                 x = nn.functional.relu(x)
-            x = self.covar_net[i](x)
+            x = self.covar_nets[name][i](x)
 
         # segment the last dimension to match the quantiles
         x = x.reshape(x.shape[0], self.n_forecasts, len(self.quantiles))
         return x
 
-    def _forward(self, inputs: Dict, meta: Dict = None, non_stationary_only: bool = False) -> torch.Tensor:
+    def all_covariates(self, covariates: Dict[str, Union[torch.Tensor, float]]) -> torch.Tensor:
+        """Compute all covariate components.
+
+        Parameters
+        ----------
+            covariates : dict(torch.Tensor, float)
+                dict of named covariates (keys) with their features (values)
+                dims of each dict value: (batch, n_lags)
+
+        Returns
+        -------
+            torch.Tensor
+                Forecast component of dims (batch, n_forecasts)
+        """
+        for i, name in enumerate(covariates.keys()):
+            if i == 0:
+                x = self.covariate(lags=covariates[name], name=name)
+            if i > 0:
+                x = x + self.covariate(lags=covariates[name], name=name)
+        return x
+
+    def forward(self, inputs: Dict, meta: Dict = None) -> torch.Tensor:
         """This method defines the model forward pass.
+
         Note
         ----
+
         Time input is required. Minimum model setup is a linear trend.
+
         Parameters
         ----------
             inputs : dict
                 Model inputs, each of len(df) but with varying dimensions
+
                 Note
                 ----
+
                 Contains the following data:
+
                 Model Inputs
                     * ``time`` (torch.Tensor , loat), normalized time, dims: (batch, n_forecasts)
                     * ``lags`` (torch.Tensor, float), dims: (batch, n_lags)
                     * ``seasonalities`` (torch.Tensor, float), dict of named seasonalities (keys) with their features (values), dims of each dict value (batch, n_forecasts, n_features)
                     * ``covariates`` (torch.Tensor, float), dict of named covariates (keys) with their features (values), dims of each dict value: (batch, n_lags)
                     * ``events`` (torch.Tensor, float), all event features, dims (batch, n_forecasts, n_features)
                     * ``regressors``(torch.Tensor, float), all regressor features, dims (batch, n_forecasts, n_features)
                     * ``predict_mode`` (bool), optional and only passed during prediction
+
             meta : dict, default=None
                 Metadata about the all the samples of the model input batch.
+
                 Contains the following:
+
                 Model Meta:
                     * ``df_name`` (list, str), time series ID corresponding to each sample of the input batch.
+
                 Note
                 ----
                 The meta is sorted in the same way the inputs are sorted.
+
                 Note
                 ----
                 The default None value allows the forward method to be used without providing the meta argument.
                 This was designed to avoid issues with the library `lr_finder` https://github.com/davidtvs/pytorch-lr-finder
                 while having  ``config_trend.trend_global_local="local"``.
                 The turnaround consists on passing the same meta (dummy ID) to all the samples of the batch.
                 Internally, this is equivalent to use ``config_trend.trend_global_local="global"`` to find the optimal learning rate.
-            non_stationary_only : bool, default=False
-                If True, only non-stationary components are returned.
 
         Returns
         -------
             torch.Tensor
                 Forecast of dims (batch, n_forecasts, no_quantiles)
         """
         # Turnaround to avoid issues when the meta argument is None and meta_used_in_model
         if meta is None and self.meta_used_in_model:
             name_id_dummy = self.id_list[0]
             meta = OrderedDict()
             meta["df_name"] = [name_id_dummy for _ in range(inputs["time"].shape[0])]
             meta = torch.tensor([self.id_dict[i] for i in meta["df_name"]], device=self.device)
 
         additive_components = torch.zeros(
-            size=(inputs["time"].shape[0], inputs["time"].shape[1], len(self.quantiles)), device=self.device
+            size=(inputs["time"].shape[0], self.n_forecasts, len(self.quantiles)), device=self.device
         )
         multiplicative_components = torch.zeros(
-            size=(inputs["time"].shape[0], inputs["time"].shape[1], len(self.quantiles)), device=self.device
+            size=(inputs["time"].shape[0], self.n_forecasts, len(self.quantiles)), device=self.device
         )
 
-        if not non_stationary_only:
-            if "lags" in inputs:
-                additive_components += self.auto_regression(lags=inputs["lags"])
-            # else: assert self.n_lags == 0
+        if "lags" in inputs:
+            additive_components += self.auto_regression(lags=inputs["lags"])
+        # else: assert self.n_lags == 0
 
-            if "covariates" in inputs:
-                additive_components += self.forward_covar_net(covariates=inputs["covariates"])
+        if "covariates" in inputs:
+            additive_components += self.all_covariates(covariates=inputs["covariates"])
 
         if "seasonalities" in inputs:
             s = self.seasonality(s=inputs["seasonalities"], meta=meta)
             if self.config_seasonality.mode == "additive":
                 additive_components += s
             elif self.config_seasonality.mode == "multiplicative":
                 multiplicative_components += s
@@ -596,115 +630,64 @@
             trend
             + additive_components
             + trend.detach() * multiplicative_components
             # 0 is the median quantile index
             # all multiplicative components are multiplied by the median quantile trend (uncomment line below to apply)
             # trend + additive_components + trend.detach()[:, :, 0].unsqueeze(dim=2) * multiplicative_components
         )  # dimensions - [batch, n_forecasts, no_quantiles]
-        return out
-
-    def forward(self, inputs: Dict, meta: Dict = None) -> Dict:
-        """
-        Forward pass of the model to compute predictions based on the provided inputs and meta data.
-        This method fits non-stationary components first, substracts them from the present "lags" and in a
-        second step fits the residuals.
-        It also computes quantile forecasts from the differences in predictions.
-
-        Parameters
-        ----------
-        inputs : Dict
-            Dictionary containing input data for the forward pass. The dictionary may include keys such as
-            "lags", "time", "time_lagged", "seasonalities", "seasonalities_lagged", "events", "events_lagged",
-            "regressors", "regressors_lagged", and "predict_mode".
-        meta : Dict, optional
-            Dictionary containing additional meta data for the forward pass, by default None.
-
-        Returns
-        -------
-        Dict
-            Dictionary containing the prediction results with quantiles.
-        """
-        if "lags" in inputs:
-            _inputs = inputs.copy()
-            _inputs["time"] = _inputs["time_lagged"]
-            if "seasonalities_lagged" in _inputs:
-                _inputs["seasonalities"] = _inputs["seasonalities_lagged"]
-            if "events_lagged" in _inputs:
-                _inputs["events"] = _inputs["events_lagged"]
-            if "regressors_lagged" in _inputs:
-                _inputs["regressors"] = _inputs["regressors_lagged"]
-
-            non_stationary_components = self._forward(_inputs, meta, non_stationary_only=True)
-            corrected_inputs = inputs.copy()
-            corrected_inputs["lags"] = (
-                corrected_inputs["lags"] - non_stationary_components[:, :, 0]
-            )  # only median quantile
-            prediction = self._forward(corrected_inputs, meta, non_stationary_only=False)
-        else:
-            prediction = self._forward(inputs, meta)
 
         # check for crossing quantiles and correct them here
         if "predict_mode" in inputs.keys() and inputs["predict_mode"]:
             predict_mode = True
         else:
             predict_mode = False
-        prediction_with_quantiles = self._compute_quantile_forecasts_from_diffs(prediction, predict_mode)
-        return prediction_with_quantiles
+        out = self._compute_quantile_forecasts_from_diffs(out, predict_mode)
+        return out
 
     def compute_components(self, inputs: Dict, meta: Dict) -> Dict:
         """This method returns the values of each model component.
+
         Note
         ----
+
         Time input is required. Minimum model setup is a linear trend.
+
         Parameters
         ----------
             inputs : dict
                 Model inputs, each of len(df) but with varying dimensions
+
                 Note
                 ----
+
                 Contains the following data:
+
                 Model Inputs
                     * ``time`` (torch.Tensor , loat), normalized time, dims: (batch, n_forecasts)
                     * ``lags`` (torch.Tensor, float), dims: (batch, n_lags)
                     * ``seasonalities`` (torch.Tensor, float), dict of named seasonalities (keys) with their features (values), dims of each dict value (batch, n_forecasts, n_features)
                     * ``covariates`` (torch.Tensor, float), dict of named covariates (keys) with their features (values), dims of each dict value: (batch, n_lags)
                     * ``events`` (torch.Tensor, float), all event features, dims (batch, n_forecasts, n_features)
                     * ``regressors``(torch.Tensor, float), all regressor features, dims (batch, n_forecasts, n_features)
+
         Returns
         -------
             dict
                 Containing forecast coomponents with elements of dims (batch, n_forecasts)
         """
         components = {}
         components["trend"] = self.trend(t=inputs["time"], meta=meta)
         if self.config_trend is not None and "seasonalities" in inputs:
             for name, features in inputs["seasonalities"].items():
                 components[f"season_{name}"] = self.seasonality.compute_fourier(features=features, name=name, meta=meta)
         if self.n_lags > 0 and "lags" in inputs:
             components["ar"] = self.auto_regression(lags=inputs["lags"])
         if self.config_lagged_regressors is not None and "covariates" in inputs:
-            # Combined forward pass
-            all_covariates = self.forward_covar_net(inputs["covariates"])
-            # Calculate the contribution of each covariate on each forecast
-            covar_attributions = self.covar_weights
-            # Sum the contributions of all covariates
-            covar_attribution_sum_per_forecast = reduce(
-                torch.add, [torch.sum(covar, axis=1) for _, covar in covar_attributions.items()]
-            ).to(all_covariates.device)
-            for name in inputs["covariates"].keys():
-                # Distribute the contribution of the current covariate to the combined forward pass
-                # 1. Calculate the relative share of each covariate on the total attributions
-                # 2. Multiply the relative share with the combined forward pass
-                components[f"lagged_regressor_{name}"] = torch.multiply(
-                    all_covariates,
-                    torch.divide(
-                        torch.sum(covar_attributions[name], axis=1).to(all_covariates.device),
-                        covar_attribution_sum_per_forecast,
-                    ).reshape(self.n_forecasts, len(self.quantiles)),
-                )
+            for name, lags in inputs["covariates"].items():
+                components[f"lagged_regressor_{name}"] = self.covariate(lags=lags, name=name)
         if (self.config_events is not None or self.config_holidays is not None) and "events" in inputs:
             if "additive" in inputs["events"].keys():
                 components["events_additive"] = self.scalar_features_effects(
                     features=inputs["events"]["additive"], params=self.event_params["additive"]
                 )
             if "multiplicative" in inputs["events"].keys():
                 components["events_multiplicative"] = self.scalar_features_effects(
@@ -821,17 +804,14 @@
             meta_name_tensor = None
         # Run forward calculation
         predicted = self.forward(inputs, meta_name_tensor)
         # Calculate loss
         loss, reg_loss = self.loss_func(inputs, predicted, targets)
         # Metrics
         if self.metrics_enabled:
-            predicted_denorm = self.denormalize(predicted[:, :, 0])
-            target_denorm = self.denormalize(targets.squeeze(dim=2))
-            self.log_dict(self.metrics_val(predicted_denorm, target_denorm), **self.log_args)
             self.log("Loss_test", loss, **self.log_args)
             self.log("RegLoss_test", reg_loss, **self.log_args)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         inputs, _, meta = batch
         # Global-local
         if self.meta_used_in_model:
@@ -876,22 +856,24 @@
             # scales end to be end weight times bigger than start weight
             # with end weight being 1.0
             weight = (1.0 + time * (end_w - 1.0)) / end_w
         return weight.unsqueeze(dim=2)  # add an extra dimension for the quantiles
 
     def _add_batch_regularizations(self, loss, epoch, progress):
         """Add regularization terms to loss, if applicable
+
         Parameters
         ----------
             loss : torch.Tensor, scalar
                 current batch loss
             epoch : int
                 current epoch number
             progress : float
                 progress within the epoch, between 0 and 1
+
         Returns
         -------
             loss, reg_loss
         """
         delay_weight = self.config_train.get_reg_delay_weight(epoch, progress)
 
         reg_loss = torch.zeros(1, dtype=torch.float, requires_grad=False, device=self.device)
@@ -901,49 +883,51 @@
                 reg_ar = self.config_ar.regularize(self.ar_weights)
                 reg_ar = torch.sum(reg_ar).squeeze() / self.n_forecasts
                 reg_loss += self.config_ar.reg_lambda * reg_ar
 
             # Regularize trend to be smoother/sparse
             l_trend = self.config_trend.trend_reg
             if self.config_trend.n_changepoints > 0 and l_trend is not None and l_trend > 0:
-                reg_trend = reg_func_trend(
+                reg_trend = utils.reg_func_trend(
                     weights=self.trend.get_trend_deltas,
                     threshold=self.config_train.trend_reg_threshold,
                 )
                 reg_loss += l_trend * reg_trend
 
             # Regularize seasonality: sparsify fourier term coefficients
             if self.config_seasonality:
                 l_season = self.config_seasonality.reg_lambda
                 if self.seasonality.season_dims is not None and l_season is not None and l_season > 0:
                     for name in self.seasonality.season_params.keys():
-                        reg_season = reg_func_season(self.seasonality.season_params[name])
+                        reg_season = utils.reg_func_season(self.seasonality.season_params[name])
                         reg_loss += l_season * reg_season
 
             # Regularize events: sparsify events features coefficients
             if self.config_events is not None or self.config_holidays is not None:
-                reg_events_loss = reg_func_events(self.config_events, self.config_holidays, self)
+                reg_events_loss = utils.reg_func_events(self.config_events, self.config_holidays, self)
                 reg_loss += reg_events_loss
 
             # Regularize regressors: sparsify regressor features coefficients
             if self.config_regressors is not None:
-                reg_regressor_loss = reg_func_regressors(self.config_regressors, self)
+                reg_regressor_loss = utils.reg_func_regressors(self.config_regressors, self)
                 reg_loss += reg_regressor_loss
 
         reg_loss = delay_weight * reg_loss
         loss = loss + reg_loss
         return loss, reg_loss
 
     def denormalize(self, ts):
         """
         Denormalize timeseries
+
         Parameters
         ----------
             target : torch.Tensor
                 ts tensor
+
         Returns
         -------
             denormalized timeseries
         """
         if self.config_normalization.global_normalization:
             shift_y = (
                 self.config_normalization.global_data_params["y"].shift
@@ -981,21 +965,21 @@
 
 
 class DeepNet(nn.Module):
     """
     A simple, general purpose, fully connected network
     """
 
-    def __init__(self, d_inputs, d_outputs, lagged_reg_layers=[]):
+    def __init__(self, d_inputs, d_outputs, d_hidden=32, num_hidden_layers=0):
         # Perform initialization of the pytorch superclass
         super(DeepNet, self).__init__()
         self.layers = nn.ModuleList()
-        for d_hidden_i in lagged_reg_layers:
-            self.layers.append(nn.Linear(d_inputs, d_hidden_i, bias=True))
-            d_inputs = d_hidden_i
+        for i in range(num_hidden_layers):
+            self.layers.append(nn.Linear(d_inputs, d_hidden, bias=True))
+            d_inputs = d_hidden
         self.layers.append(nn.Linear(d_inputs, d_outputs, bias=True))
         for lay in self.layers:
             nn.init.kaiming_normal_(lay.weight, mode="fan_in")
 
     def forward(self, x):
         """
         This method defines the network layering and activation functions
```

### Comparing `neuralprophet-0.6.0/neuralprophet/torch_prophet.py` & `neuralprophet-0.6.0rc1/neuralprophet/torch_prophet.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/uncertainty.py` & `neuralprophet-0.6.0rc1/neuralprophet/uncertainty.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,19 +181,19 @@
 
     Returns
     -------
         scalar
             Regularization loss
     """
     reg_covariate_loss = 0.0
-    weights = model.get_covar_weights()
     for covariate, configs in config_lagged_regressors.items():
         reg_lambda = configs.reg_lambda
         if reg_lambda is not None:
-            loss = torch.mean(utils_torch.penalize_nonzero(weights[covariate])).squeeze()
+            weights = model.get_covar_weights(covariate)
+            loss = torch.mean(utils_torch.penalize_nonzero(weights)).squeeze()
             reg_covariate_loss += reg_lambda * loss
 
     return reg_covariate_loss
 
 
 def reg_func_regressors(config_regressors, model):
     """
@@ -645,18 +645,14 @@
     seed : numeric
         Seed value for random number generator
 
     Note
     ----
     This needs to be set each time before fitting the model.
 
-    Example
-    -------
-    >>> from neuralprophet import set_random_seed
-    >>> set_random_seed(seed=42)
     """
     np.random.seed(seed)
     torch.manual_seed(seed)
 
 
 def set_logger_level(logger, log_level, include_handlers=False):
     if log_level is None:
@@ -682,19 +678,14 @@
     ----------
         log_level : str
             The log level of the logger objects used for printing procedure status
             updates for debugging/monitoring. Should be one of ``NOTSET``, ``DEBUG``, ``INFO``, ``WARNING``,
             ``ERROR`` or ``CRITICAL``
         include_handlers : bool
             Include any specified file/stream handlers
-
-    Example
-    -------
-    >>> from neuralprophet import set_log_level
-    >>> set_log_level("ERROR")
     """
     set_logger_level(logging.getLogger("NP"), log_level, include_handlers)
 
 
 def smooth_loss_and_suggest(lr_finder_results, window=10):
     """
     Smooth loss using a Hamming filter.
@@ -735,15 +726,14 @@
     try:
         # Find the steepest gradient and the minimum loss after that
         suggestion = lr[np.argmin(np.gradient(loss))]
     except ValueError:
         log.error(
             f"The number of loss values ({len(loss)}) is too small to estimate a learning rate. Increase the number of samples or manually set the learning rate."
         )
-        raise
     return (loss, lr, suggestion)
 
 
 def _smooth_loss(loss, beta=0.9):
     smoothed_loss = np.zeros_like(loss)
     smoothed_loss[0] = loss[0]
     for i in range(1, len(loss)):
```

### Comparing `neuralprophet-0.6.0/neuralprophet/utils_metrics.py` & `neuralprophet-0.6.0rc1/neuralprophet/utils_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.6.0/neuralprophet/utils_torch.py` & `neuralprophet-0.6.0rc1/neuralprophet/utils_torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,32 +70,29 @@
     elif inspect.isclass(optimizer_name) and issubclass(optimizer_name, torch.optim.Optimizer):
         optimizer = optimizer_name
     else:
         raise ValueError("The provided optimizer is not supported.")
     return optimizer, optimizer_args
 
 
-def interprete_model(target_model: pl.LightningModule, net: str, forward_func: str, _input: torch.Tensor = None):
+def interprete_model(target_model: pl.LightningModule, net: str, forward_func: str):
     """
     Returns model input attributions for a given network and forward function.
 
     Parameters
     ----------
         target_model : pl.LightningModule
             The model for which input attributions are to be computed.
 
         net : str
             Name of the network for which input attributions are to be computed.
 
         forward_func : str
             Name of the forward function for which input attributions are to be computed.
 
-        _input : torch.Tensor
-            Input for which the attributions are to be computed.
-
     Returns
     -------
         torch.Tensor
             Input attributions for the given network and forward function.
     """
     # Load the respective forward function from the model and init model interpreter
     forward = getattr(target_model, forward_func)
@@ -106,15 +103,15 @@
     # Number of input features to the net (aka n_lags)
     num_in_features = getattr(target_model, net)[0].in_features
     # Number of output features from the net (aka n_forecasts)
     num_out_features = getattr(target_model, net)[-1].out_features
     num_out_features_without_quantiles = int(num_out_features / num_quantiles)
 
     # Create a tensor of ones as model input
-    model_input = torch.ones(1, num_in_features, requires_grad=True) if _input is None else _input
+    model_input = torch.ones(1, num_in_features, requires_grad=True)
 
     # Iterate through each output feature and compute the model attribution wrt. the input
     attributions = torch.empty((0, num_in_features))
     for output_feature in range(num_out_features_without_quantiles):
         for quantile in range(num_quantiles):
             target_attribution = saliency.attribute(model_input, target=[(output_feature, quantile)], abs=False)
             attributions = torch.cat((attributions, target_attribution), 0)
```

### Comparing `neuralprophet-0.6.0/pyproject.toml` & `neuralprophet-0.6.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuralprophet"
-version = "0.6.0"
+version = "0.6.0rc1"
 description = "NeuralProphet is an easy to learn framework for interpretable time series forecasting."
 authors = ["Oskar Triebe <triebe@stanford.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
```

### Comparing `neuralprophet-0.6.0/PKG-INFO` & `neuralprophet-0.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralprophet
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: NeuralProphet is an easy to learn framework for interpretable time series forecasting.
 License: MIT
 Author: Oskar Triebe
 Author-email: triebe@stanford.edu
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

