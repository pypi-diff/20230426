# Comparing `tmp/ensembleperturbation-1.1.2.tar.gz` & `tmp/ensembleperturbation-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembleperturbation-1.1.2.tar", max compression
+gzip compressed data, was "ensembleperturbation-1.2.0.tar", max compression
```

## Comparing `ensembleperturbation-1.1.2.tar` & `ensembleperturbation-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     7048 2022-11-29 15:40:17.772294 ensembleperturbation-1.1.2/LICENSE
--rw-r--r--   0        0        0     1554 2022-11-29 15:40:17.772294 ensembleperturbation-1.1.2/README.md
--rw-r--r--   0        0        0        3 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/client/__init__.py
--rw-r--r--   0        0        0     3803 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/client/combine_results.py
--rw-r--r--   0        0        0     1952 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/client/make_storm_ensemble.py
--rw-r--r--   0        0        0     5792 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/client/perturb_tracks.py
--rw-r--r--   0        0        0     2566 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/client/plot_results.py
--rw-r--r--   0        0        0        0 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/parsing/__init__.py
--rw-r--r--   0        0        0    32710 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/parsing/adcirc.py
--rw-r--r--   0        0        0    24828 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/parsing/comparison.py
--rw-r--r--   0        0        0    46660 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/parsing/schism.py
--rw-r--r--   0        0        0      545 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/parsing/utilities.py
--rw-r--r--   0        0        0        0 2022-11-29 15:40:17.780295 ensembleperturbation-1.1.2/ensembleperturbation/perturbation/__init__.py
--rw-r--r--   0        0        0    68923 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/perturbation/atcf.py
--rw-r--r--   0        0        0        0 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/__init__.py
--rw-r--r--   0        0        0    10510 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/gdal_dataset.py
--rw-r--r--   0        0        0     5453 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/geometry.py
--rw-r--r--   0        0        0     1590 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/map.py
--rw-r--r--   0        0        0     8938 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/nodes.py
--rw-r--r--   0        0        0     9729 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/perturbation.py
--rw-r--r--   0        0        0    20101 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/surrogate.py
--rw-r--r--   0        0        0     4623 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/taylor_diagram.py
--rw-r--r--   0        0        0      908 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/plotting/utilities.py
--rw-r--r--   0        0        0        0 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/__init__.py
--rw-r--r--   0        0        0     2663 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/ensemble_array.py
--rw-r--r--   0        0        0    10684 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
--rw-r--r--   0        0        0     5332 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
--rw-r--r--   0        0        0    23410 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/surrogate.py
--rw-r--r--   0        0        0     5066 2022-11-29 15:40:17.784294 ensembleperturbation-1.1.2/ensembleperturbation/utilities.py
--rw-r--r--   0        0        0     2310 2022-11-29 15:40:23.668315 ensembleperturbation-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3723 2022-11-29 15:40:24.464550 ensembleperturbation-1.1.2/setup.py
--rw-r--r--   0        0        0     3731 2022-11-29 15:40:24.465075 ensembleperturbation-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-04-26 19:18:20.650799 ensembleperturbation-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1554 2023-04-26 19:18:20.650799 ensembleperturbation-1.2.0/README.md
+-rw-r--r--   0        0        0        3 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/__init__.py
+-rw-r--r--   0        0        0     3803 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/combine_results.py
+-rw-r--r--   0        0        0     1952 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/make_storm_ensemble.py
+-rw-r--r--   0        0        0     5792 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/perturb_tracks.py
+-rw-r--r--   0        0        0     2566 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/plot_results.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/__init__.py
+-rw-r--r--   0        0        0    32929 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/adcirc.py
+-rw-r--r--   0        0        0    24828 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/comparison.py
+-rw-r--r--   0        0        0    46714 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/schism.py
+-rw-r--r--   0        0        0      545 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/utilities.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/perturbation/__init__.py
+-rw-r--r--   0        0        0    74453 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/perturbation/atcf.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/__init__.py
+-rw-r--r--   0        0        0    10510 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/gdal_dataset.py
+-rw-r--r--   0        0        0     5453 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/geometry.py
+-rw-r--r--   0        0        0     1590 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/map.py
+-rw-r--r--   0        0        0     9135 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/nodes.py
+-rw-r--r--   0        0        0    13796 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/perturbation.py
+-rw-r--r--   0        0        0    20101 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/surrogate.py
+-rw-r--r--   0        0        0     4623 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/taylor_diagram.py
+-rw-r--r--   0        0        0      908 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/utilities.py
+-rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/ensemble_array.py
+-rw-r--r--   0        0        0    11112 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
+-rw-r--r--   0        0        0     5332 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
+-rw-r--r--   0        0        0    23410 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/surrogate.py
+-rw-r--r--   0        0        0     5066 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/utilities.py
+-rw-r--r--   0        0        0     2310 2023-04-26 19:18:27.026868 ensembleperturbation-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3723 2023-04-26 19:18:27.933598 ensembleperturbation-1.2.0/setup.py
+-rw-r--r--   0        0        0     3731 2023-04-26 19:18:27.934111 ensembleperturbation-1.2.0/PKG-INFO
```

### Comparing `ensembleperturbation-1.1.2/LICENSE` & `ensembleperturbation-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/README.md` & `ensembleperturbation-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/client/combine_results.py` & `ensembleperturbation-1.2.0/ensembleperturbation/client/combine_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/client/make_storm_ensemble.py` & `ensembleperturbation-1.2.0/ensembleperturbation/client/make_storm_ensemble.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/client/perturb_tracks.py` & `ensembleperturbation-1.2.0/ensembleperturbation/client/perturb_tracks.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/client/plot_results.py` & `ensembleperturbation-1.2.0/ensembleperturbation/client/plot_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/parsing/adcirc.py` & `ensembleperturbation-1.2.0/ensembleperturbation/parsing/adcirc.py`

 * *Files 1% similar despite different names*

```diff
@@ -854,14 +854,15 @@
     da: DataArray,
     k_neighbors: int = 1,
     idw_order: int = 1,
     compute_headloss: bool = False,
     mann_coef: float = 0.05,
     u_ref: float = 0.4,
     d_ref: float = 1.0,
+    min_depth: float = 0.0,
 ):
     # return a deep copy of original datarrary on output
     da_adjusted = da.copy(deep=True)
 
     # Get coordinates in conformal projection (e.g,, Mercator)
     # for determining closest distance
     crs_from = 'EPSG:4326'  # WGS84
@@ -882,24 +883,27 @@
         friction_factor = 0.0
 
     # inverse distance weighting of order `idw_order` with `k_nearest` neighbors
     for run in range(da.sizes['run']):
         null = numpy.isnan(da[run, :])
         tree = KDTree(projected_coordinates[~null])
         dd, nn = tree.query(projected_coordinates[null], k=k_neighbors)
+        max_allowable_values = da['depth'][null].values + min_depth - numpy.finfo(float).eps
         if k_neighbors == 1:
             headloss = dd * friction_factor  # hydraulic friction loss
-            da_adjusted[run, null] = da[run, nodes[~null][nn]].values - headloss
+            da_adjusted[run, null] = numpy.fmin(
+                da[run, nodes[~null][nn]].values - headloss, max_allowable_values
+            )
         else:
             for kk in range(k_neighbors):
                 weights = dd[:, kk] ** (-idw_order)
                 headloss = dd[:, kk] * friction_factor  # hydraulic friction loss
                 total_head = da[run, nodes[~null][nn[:, kk]]].values - headloss
                 if kk == 0:
                     idw_sum = total_head * weights
                     weight_sum = weights
                 else:
                     idw_sum += total_head * weights
                     weight_sum += weights
-            da_adjusted[run, null] = idw_sum / weight_sum
+            da_adjusted[run, null] = numpy.fmin(idw_sum / weight_sum, max_allowable_values)
 
     return da_adjusted
```

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/parsing/comparison.py` & `ensembleperturbation-1.2.0/ensembleperturbation/parsing/comparison.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/parsing/schism.py` & `ensembleperturbation-1.2.0/ensembleperturbation/parsing/schism.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,19 +499,19 @@
                             lock=False,
                         ).expand_dims({'run': [run_dir.name]}),
                     ],
                     concat_dim='run',
                 )
 
         # Drop run dimension for variables fixed across runs
+        # `SCHISM_hgrid_node_x` and `SCHISM_hgrid_node_y` are
+        # coordinates and are not expanded in `run` dimension
         fixed_vars = [
             'node',
             'depth',
-            'SCHISM_hgrid_node_x',
-            'SCHISM_hgrid_node_y',
         ]
         for var in fixed_vars:
             if var not in dataset:
                 continue
             dataset = dataset.assign({var: dataset[var].isel(run=0)})
 
         # Add element table
```

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/parsing/utilities.py` & `ensembleperturbation-1.2.0/ensembleperturbation/parsing/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/perturbation/atcf.py` & `ensembleperturbation-1.2.0/ensembleperturbation/perturbation/atcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
 warnings.simplefilter(action='ignore', category=UnitStrippedWarning)
 
 AIR_DENSITY = 1.15 * units.kilogram / units.meters ** 3
 
 E1 = exp(1.0)  # e
 
+BLAdj = 0.9  # adjustment factor from 10-m height to top of boundary layer
+
 # Index of absolute errors (forecast times [hrs)]
 HISTORICAL_ERROR_HOURS = [0, 12, 24, 36, 48, 60, 72, 96, 120]  # has 60-hr data (for Rmax)
 HISTORICAL_ERROR_HOURS_NO_60H = (
     HISTORICAL_ERROR_HOURS[:5] + HISTORICAL_ERROR_HOURS[6:]
 )  # no 60-hr data
 
 
@@ -100,14 +102,15 @@
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(lower_bound={repr(self.lower_bound)}, upper_bound={repr(self.upper_bound)}, historical_forecast_errors={repr(self.historical_forecast_errors)}, default={repr(self.default)}, unit={repr(self.unit)})'
 
 
 class CentralPressure(VortexVariable):
     name = 'central_pressure'
+    unit = units.millibar
 
 
 class BackgroundPressure(VortexVariable):
     name = 'background_pressure'
 
     def __init__(self):
         super().__init__(
@@ -240,44 +243,51 @@
 
         variable_values = vortex_dataframe[self.name].values
         if (
             not isinstance(variable_values, PintArray)
             or variable_values.units == variable_values.units._REGISTRY.dimensionless
         ):
             variable_values *= self.unit
+        if isinstance(variable_values, PintArray):
+            variable_values = variable_values.quantity
         if (
             not isinstance(values, Quantity)
             or values.units == values.units._REGISTRY.dimensionless
         ):
             values *= self.unit
 
         all_values = variable_values - values
+        # ensure that we don't change zero values
+        all_values[variable_values.magnitude < 1] = 0 * all_values.units
         vortex_dataframe[self.name] = [
             min(self.upper_bound, max(value, self.lower_bound)).magnitude
+            if value.magnitude >= 1
+            else 0
             for value in all_values
         ] * self.unit
 
         return vortex_dataframe
 
-    def storm_errors(self, data_frame: DataFrame) -> DataFrame:
+    def storm_errors(self, data_frame: DataFrame, loc_index: int = 0) -> DataFrame:
         """
         Historical forecast errors of the given storm, based on initial intensity.
 
         :param data_frame: storm data frame
+        :param loc_index: index to classify the errors at (0 by default for initial)
         :return: errors based on intensity classification
         """
 
-        intial_intensity = data_frame[MaximumSustainedWindSpeed.name].iloc[0]
+        initial_intensity = data_frame[MaximumSustainedWindSpeed.name].iloc[loc_index]
 
-        if not isinstance(intial_intensity, Quantity):
-            intial_intensity *= units.knot
+        if not isinstance(initial_intensity, Quantity):
+            initial_intensity *= units.knot
 
-        if intial_intensity < 50 * units.knot:
+        if initial_intensity < 50 * units.knot:
             storm_classification = '<50kt'  # weak
-        elif intial_intensity <= 95 * units.knot:
+        elif initial_intensity <= 95 * units.knot:
             storm_classification = '50-95kt'  # medium
         else:
             storm_classification = '>95kt'  # strong
 
         LOGGER.debug(f'storm classification: {storm_classification}')
         return self.historical_forecast_errors[storm_classification]
 
@@ -287,28 +297,31 @@
     ``max_sustained_wind_speed`` (``Vmax``) represents the maximum wind speed sustained by the storm.
     It is perturbed along a random gaussian distribution (``0`` - ``1``), scaled to the mean of absolute historical errors.
     ``central_pressure`` (``pc``) is then changed proportionally based on the Holland B parameter.
     """
 
     name = 'max_sustained_wind_speed'
     perturbation_type = PerturbationType.GAUSSIAN
+    unit = units.knot
 
     # Reference - 2019_Psurge_Error_Update_FINAL.docx
     # Table 12: Adjusted intensity errors [kt] for 2015-2019
     def __init__(self):
         super().__init__(
             lower_bound=15,
             upper_bound=175,
             historical_forecast_errors={
                 '<50kt': DataFrame(
                     {'mean error [kt]': [1.45, 4.01, 6.17, 8.42, 10.46, 14.28, 18.26, 19.91]},
+                    dtype=PintType(units.knot),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
                 '50-95kt': DataFrame(
                     {'mean error [kt]': [2.26, 5.75, 8.54, 9.97, 11.28, 13.11, 13.46, 12.62]},
+                    dtype=PintType(units.knot),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
                 '>95kt': DataFrame(
                     {
                         'mean error [kt]': [
                             2.80,
                             7.94,
@@ -316,61 +329,63 @@
                             13.27,
                             12.66,
                             13.41,
                             13.46,
                             13.55,
                         ]
                     },
+                    dtype=PintType(units.knot),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
             },
             unit=units.knot,
         )
 
 
 class RadiusOfMaximumWinds(VortexPerturbedVariable):
     """
     ``radius_of_maximum_winds`` (``Rmax``)
-    It is perturbed along a uniform distribution on [-1,1] between the 15th and 85th percentile CDFs of NHC historical forecast errors.
+    It is perturbed along a uniform distribution on [-1,1] between the 0th and 100th percentile CDFs of NHC historical forecast errors.
+    0th and 100th percentiles are calculated based on extrapolation from the provided 15th, 50th, and 85th percentiles.
     """
 
     name = 'radius_of_maximum_winds'
     perturbation_type = PerturbationType.UNIFORM
 
     def __init__(self):
         super().__init__(
             lower_bound=5,
             upper_bound=200,
             historical_forecast_errors={
                 '<15sm': DataFrame(
                     {
                         '15th percentile error': [
-                            0.0,
+                            2 * -13.82 - -19.67,
                             -13.82,
                             -19.67,
                             -21.37,
                             -26.31,
                             -32.71,
                             -39.12,
                             -46.80,
                             -52.68,
                         ],
                         '50th percentile error': [
-                            0.0,
+                            2 * -2.72 - -6.74,
                             -2.72,
                             -6.74,
                             -9.59,
                             -12.12,
                             -15.64,
                             -19.16,
                             -18.60,
                             -24.07,
                         ],
                         '85th percentile error': [
-                            0.0,
+                            2 * 1.27 - 0.22,
                             1.27,
                             0.22,
                             1.02,
                             0.00,
                             -2.59,
                             -5.18,
                             -7.15,
@@ -379,37 +394,37 @@
                     },
                     dtype=PintType(units.us_statute_mile),
                     index=HISTORICAL_ERROR_HOURS,
                 ),
                 '15-25sm': DataFrame(
                     {
                         '15th percentile error': [
-                            0.0,
+                            2 * -10.47 - -14.54,
                             -10.47,
                             -14.54,
                             -20.35,
                             -23.88,
                             -21.78,
                             -19.68,
                             -24.24,
                             -28.30,
                         ],
                         '50th percentile error': [
-                            0.0,
+                            2 * -1.07 - -2.48,
                             -1.07,
                             -2.48,
                             -4.25,
                             -4.33,
                             -3.55,
                             -2.77,
                             -6.02,
                             -4.44,
                         ],
                         '85th percentile error': [
-                            0.0,
+                            2 * 4.17 - 6.70,
                             4.17,
                             6.70,
                             6.13,
                             6.54,
                             6.93,
                             7.32,
                             9.33,
@@ -418,37 +433,37 @@
                     },
                     dtype=PintType(units.us_statute_mile),
                     index=HISTORICAL_ERROR_HOURS,
                 ),
                 '25-35sm': DataFrame(
                     {
                         '15th percentile error': [
-                            0.0,
+                            2 * -8.57 - -13.41,
                             -8.57,
                             -13.41,
                             -10.87,
                             -9.26,
                             -9.34,
                             -9.42,
                             -7.41,
                             -7.40,
                         ],
                         '50th percentile error': [
-                            0.0,
+                            2 * 0.39 - 1.66,
                             0.39,
                             1.66,
                             2.49,
                             4.42,
                             5.20,
                             5.98,
                             5.98,
                             6.96,
                         ],
                         '85th percentile error': [
-                            0.0,
+                            2 * 8.21 - 10.62,
                             8.21,
                             10.62,
                             13.93,
                             15.62,
                             16.04,
                             16.46,
                             16.51,
@@ -457,37 +472,37 @@
                     },
                     dtype=PintType(units.us_statute_mile),
                     index=HISTORICAL_ERROR_HOURS,
                 ),
                 '35-45sm': DataFrame(
                     {
                         '15th percentile error': [
-                            0.0,
+                            2 * -10.66 - -7.64,
                             -10.66,
                             -7.64,
                             -5.68,
                             -3.25,
                             -1.72,
                             -0.19,
                             3.65,
                             2.59,
                         ],
                         '50th percentile error': [
-                            0.0,
+                            2 * 3.22 - 7.32,
                             3.22,
                             7.32,
                             12.67,
                             14.14,
                             13.72,
                             13.31,
                             14.60,
                             14.01,
                         ],
                         '85th percentile error': [
-                            0.0,
+                            2 * 14.77 - 17.85,
                             14.77,
                             17.85,
                             22.07,
                             27.60,
                             27.08,
                             26.56,
                             26.80,
@@ -496,37 +511,37 @@
                     },
                     dtype=PintType(units.us_statute_mile),
                     index=HISTORICAL_ERROR_HOURS,
                 ),
                 '>45sm': DataFrame(
                     {
                         '15th percentile error': [
-                            0.0,
+                            2 * -15.36 - -10.37,
                             -15.36,
                             -10.37,
                             3.14,
                             12.10,
                             12.21,
                             12.33,
                             6.66,
                             7.19,
                         ],
                         '50th percentile error': [
-                            0.0,
+                            2 * 8.11 - 15.19,
                             8.11,
                             15.19,
                             17.21,
                             24.25,
                             25.63,
                             27.00,
                             20.56,
                             20.51,
                         ],
                         '85th percentile error': [
-                            0.0,
+                            2 * 21.43 - 29.96,
                             21.43,
                             29.96,
                             37.22,
                             39.27,
                             39.10,
                             38.93,
                             34.40,
@@ -536,23 +551,24 @@
                     dtype=PintType(units.us_statute_mile),
                     index=HISTORICAL_ERROR_HOURS,
                 ),
             },
             unit=units.nautical_mile,
         )
 
-    def storm_errors(self, data_frame: DataFrame) -> DataFrame:
+    def storm_errors(self, data_frame: DataFrame, loc_index: int = 0) -> DataFrame:
         """
         Historical forecast errors of the given storm, based on initial size.
 
         :param data_frame: storm data frame
+        :param loc_index: index to classify the errors at (0 by default for initial)
         :return: errors based on size classification
         """
 
-        initial_radius = data_frame[self.name].iloc[0]
+        initial_radius = data_frame[self.name].iloc[loc_index]
 
         if not isinstance(initial_radius, Quantity):
             initial_radius *= units.nautical_mile
 
         if initial_radius < 15 * units.us_statute_mile:
             storm_classification = '<15sm'  # very small
         elif initial_radius < 25 * units.us_statute_mile:
@@ -564,14 +580,83 @@
         else:
             storm_classification = '>45sm'  # very large
 
         LOGGER.debug(f'storm classification: {storm_classification}')
         return self.historical_forecast_errors[storm_classification]
 
 
+# Rmax-dependent radius variables
+class IsotachRadiusSWQ(VortexPerturbedVariable):
+    """
+    ``isotach_radius_for_SWQ`
+    """
+
+    name = 'isotach_radius_for_SWQ'
+    perturbation_type = PerturbationType.UNIFORM
+
+    def __init__(self):
+        super().__init__(
+            lower_bound=5,
+            upper_bound=400,
+            historical_forecast_errors={},
+            unit=units.nautical_mile,
+        )
+
+
+class IsotachRadiusSEQ(VortexPerturbedVariable):
+    """
+    ``isotach_radius_for_SEQ`
+    """
+
+    name = 'isotach_radius_for_SEQ'
+    perturbation_type = PerturbationType.UNIFORM
+
+    def __init__(self):
+        super().__init__(
+            lower_bound=5,
+            upper_bound=400,
+            historical_forecast_errors={},
+            unit=units.nautical_mile,
+        )
+
+
+class IsotachRadiusNWQ(VortexPerturbedVariable):
+    """
+    ``isotach_radius_for_NWQ`
+    """
+
+    name = 'isotach_radius_for_NWQ'
+    perturbation_type = PerturbationType.UNIFORM
+
+    def __init__(self):
+        super().__init__(
+            lower_bound=5,
+            upper_bound=400,
+            historical_forecast_errors={},
+            unit=units.nautical_mile,
+        )
+
+
+class IsotachRadiusNEQ(VortexPerturbedVariable):
+    """
+    ``isotach_radius_for_NEQ`
+    """
+
+    name = 'isotach_radius_for_NEQ'
+    perturbation_type = PerturbationType.UNIFORM
+
+    def __init__(self):
+        super().__init__(
+            lower_bound=5,
+            upper_bound=400,
+            historical_forecast_errors={},
+            unit=units.nautical_mile,
+        )
+
+
 class CrossTrack(VortexPerturbedVariable):
     """
     ``cross_track``  represents a perpendicular offset of the tropical cyclone center track, accomplished by moving each forecast time left or right perpedicular to the track line.
     It is perturbed along a random gaussian distribution (``0`` - ``1``), scaled to the mean of absolute historical errors.
     """
 
     name = 'cross_track'
@@ -593,14 +678,15 @@
                             28.95,
                             38.03,
                             56.88,
                             92.95,
                             119.67,
                         ]
                     },
+                    dtype=PintType(units.nautical_mile),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
                 '50-95kt': DataFrame(
                     {
                         'mean error [nm]': [
                             2.89,
                             11.58,
@@ -608,14 +694,15 @@
                             21.10,
                             27.76,
                             47.51,
                             68.61,
                             103.45,
                         ]
                     },
+                    dtype=PintType(units.nautical_mile),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
                 '>95kt': DataFrame(
                     {
                         'mean error [nm]': [
                             1.85,
                             7.79,
@@ -623,14 +710,15 @@
                             17.92,
                             25.01,
                             40.48,
                             60.69,
                             79.98,
                         ]
                     },
+                    dtype=PintType(units.nautical_mile),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
             },
             unit=units.nautical_mile,
         )
 
     def perturb(
@@ -760,14 +848,15 @@
                             37.75,
                             51.07,
                             69.22,
                             108.59,
                             125.01,
                         ]
                     },
+                    dtype=PintType(units.nautical_mile),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
                 '50-95kt': DataFrame(
                     {
                         'mean error [nm]': [
                             3.68,
                             12.74,
@@ -775,14 +864,15 @@
                             27.51,
                             37.28,
                             57.82,
                             80.15,
                             108.07,
                         ]
                     },
+                    dtype=PintType(units.nautical_mile),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
                 '>95kt': DataFrame(
                     {
                         'mean error [nm]': [
                             2.35,
                             8.57,
@@ -790,14 +880,15 @@
                             23.36,
                             33.59,
                             49.26,
                             70.90,
                             83.55,
                         ]
                     },
+                    dtype=PintType(units.nautical_mile),
                     index=HISTORICAL_ERROR_HOURS_NO_60H,
                 ),
             },
             unit=units.nautical_mile,
         )
 
     def perturb(
@@ -962,16 +1053,16 @@
         file_deck: ATCF_FileDeck = None,
         advisories: List[str] = None,
     ):
         """
         :param storm: NHC storm code, for instance `al062018`
         :param start_date: start time of ensemble
         :param end_date: end time of ensemble
-        :param file_deck: letter of file deck, one of `a`, `b`
-        :param advisories: record types (i.e. `BEST`, `OFCL`)
+        :param file_deck: ATCF file deck; one of `a`, `b`, `f`
+        :param advisories: ATCF advisory type; one of ``BEST``, ``OFCL``, ``OFCP``, ``HMON``, ``CARQ``, ``HWRF``
         """
 
         self.__start_date = None
         self.__end_date = None
         self.__file_deck = None
         self.__track = None
         self.__previous_configuration = None
@@ -982,25 +1073,38 @@
         self.file_deck = file_deck
         self.advisories = advisories
 
         self.__filename = None
 
     @classmethod
     def from_file(
-        cls, filename: PathLike, start_date: datetime = None, end_date: datetime = None
+        cls,
+        filename: PathLike,
+        start_date: datetime = None,
+        end_date: datetime = None,
+        file_deck: ATCF_FileDeck = None,
+        advisories: List[str] = None,
     ) -> 'VortexPerturber':
         """
         build storm perturber from an existing `fort.22` or ATCF file
 
         :param filename: file path to `fort.22` / ATCF file
         :param start_date: start time of ensemble
         :param end_date: end time of ensemble
+        :param file_deck: ATCF file deck; one of `a`, `b`, `f`
+        :param advisories: ATCF advisory type; one of ``BEST``, ``OFCL``, ``OFCP``, ``HMON``, ``CARQ``, ``HWRF``
         """
 
-        track = VortexTrack.from_file(filename, start_date=start_date, end_date=end_date)
+        track = VortexTrack.from_file(
+            filename,
+            start_date=start_date,
+            end_date=end_date,
+            file_deck=file_deck,
+            advisories=advisories,
+        )
         instance = VortexPerturber.from_track(track)
         instance.__filename = filename
         return instance
 
     @classmethod
     def from_track(cls, track: VortexTrack) -> 'VortexPerturber':
         """
@@ -1190,27 +1294,33 @@
                         perturbation_array.append(variable_perturbation)
                     perturbation = perturbation_array
                 else:
                     perturbation = numpy.full((len(variables),), fill_value=numpy.nan)
                 perturbations_array.append(perturbation)
             perturbations = numpy.array(perturbations_array)
 
+        if sample_from_distribution:
+            filetype_string = f'{sample_rule}'
+        else:
+            filetype_string = 'perturbation'
         if continue_numbering:
             # TODO: figure out how to continue perturbations by-variable (i.e. keep track of multiple series with different variables but the same total number of variables)
-            existing_filenames = glob(str(directory / f'vortex_*_variable_{sample_rule}_*.22'))
+            existing_filenames = glob(
+                str(directory / f'vortex_{len(variables)}_variable_{filetype_string}_*.22')
+            )
             if len(existing_filenames) > 0:
                 existing_filenames = sorted(existing_filenames)
                 last_index = int(existing_filenames[-1][-4])
             else:
                 last_index = 0
         else:
             last_index = 0
 
         run_names = [
-            f'vortex_{len(variables)}_variable_{sample_rule}_{index + 1}'
+            f'vortex_{len(variables)}_variable_{filetype_string}_{index + 1}'
             for index in range(last_index, last_index + num_perturbations)
         ]
 
         perturbations = [
             xarray.DataArray(
                 perturbations,
                 coords={'run': run_names, 'variable': variable_names},
@@ -1413,32 +1523,45 @@
 
             if alpha is None or abs(alpha) > 1.0e-3:
                 # Make the random pertubations based on the historical forecast errors
                 # Interpolate from the given VT to the storm_VT
 
                 # Get the historical forecasting errors from initial storm state (intensity or size)
                 historical_forecast_errors = variable.storm_errors(self.track.data)
-                try:
-                    # need to dequantify dataframe from pint units to run `interp`, then requantify resulting dataframe
-                    historical_forecast_errors = historical_forecast_errors.pint.dequantify()
-                except:
-                    pass
 
                 validation_hours = self.validation_times / timedelta(hours=1)
-                validation_time_errors = DataFrame(
-                    data={
-                        column: interp(
-                            x=validation_hours,
-                            xp=historical_forecast_errors.index,
-                            fp=historical_forecast_errors.loc[:, column],
-                        )
-                        for column in historical_forecast_errors.columns
-                    },
-                    index=validation_hours,
-                )
+
+                if self.file_deck.value == 'b':
+                    # hindcast errors based on the 0-hr historical averages
+                    data_dict = {}
+                    for column in historical_forecast_errors.columns:
+                        column_error = []
+                        for rdx, row in enumerate(validation_hours):
+                            column_error.append(
+                                variable.storm_errors(self.track.data, rdx)
+                                .loc[0, column]
+                                .magnitude
+                            )
+                        data_dict[column] = column_error
+                    validation_time_errors = DataFrame(data=data_dict, index=validation_hours,)
+                else:
+                    # forecast errors than grow with time based on initial intensity
+                    validation_time_errors = DataFrame(
+                        data={
+                            column: interp(
+                                x=validation_hours,
+                                xp=historical_forecast_errors.index,
+                                fp=historical_forecast_errors.loc[
+                                    :, column
+                                ].values.quantity.magnitude,
+                            )
+                            for column in historical_forecast_errors.columns
+                        },
+                        index=validation_hours,
+                    )
 
                 # get the random perturbation sample
                 if variable.perturbation_type == PerturbationType.GAUSSIAN:
                     if alpha is None:
                         alpha = gauss(0, 1)
                         perturbation[variable.name] = alpha
 
@@ -1473,19 +1596,21 @@
                     max_validation_time_errors = (
                         1.3 * validation_time_errors.loc[:, '85th percentile error']
                         - 0.3 * validation_time_errors.loc[:, '50th percentile error']
                     )
                     ## if just choose 15th/85th percentile...
                     # min_validation_time_errors = validation_time_errors.loc[:, '15th percentile error']
                     # max_validation_time_errors = validation_time_errors.loc[:, '85th percentile error']
-                    perturbed_values = 0.5 * (
-                        min_validation_time_errors * (1 - alpha)
-                        + max_validation_time_errors * (1 + alpha)
+                    perturbed_values = (
+                        0.5
+                        * (
+                            min_validation_time_errors * (1 - alpha)
+                            + max_validation_time_errors * (1 + alpha)
+                        ).values
                     )
-                    perturbed_values = perturbed_values.iloc[:, 0].values
                     if variable.unit is not None and variable.unit != units.dimensionless:
                         perturbed_values *= variable.unit
 
                     # subtract the error from the variable with physical constraint bounds
                     dataframe = variable.perturb(
                         dataframe,
                         values=perturbed_values,
@@ -1494,16 +1619,31 @@
                     )
                 else:
                     raise NotImplementedError(
                         f'perturbation type "{variable.perturbation_type}" is not recognized'
                     )
 
                 if isinstance(variable, MaximumSustainedWindSpeed):
-                    # In case of Vmax need to change the central pressure incongruence with it (obeying Holland B relationship)
+                    # In case of Vmax need to change the central pressure in accordance with Holland B relationship
                     dataframe[CentralPressure.name] = self.compute_pc_from_Vmax(dataframe)
+                elif isinstance(variable, RadiusOfMaximumWinds):
+                    # In case of Rmax need to change the r34/50,64 radii at all quadrants in the same way
+                    quadrants = [
+                        IsotachRadiusNEQ(),
+                        IsotachRadiusSEQ(),
+                        IsotachRadiusSWQ(),
+                        IsotachRadiusNWQ(),
+                    ]
+                    for quadrant in quadrants:
+                        dataframe = quadrant.perturb(
+                            vortex_dataframe=dataframe,
+                            values=perturbed_values,
+                            times=self.validation_times,
+                            inplace=True,
+                        )
 
         # remove units from data frame
         for column in dataframe:
             if isinstance(dataframe[column].dtype, PintType):
                 dataframe[column] = dataframe[column].pint.magnitude
 
         # write out the modified `fort.22`
@@ -1525,25 +1665,30 @@
         """ get the validation time of storm """
         return self.track.data['datetime'] - self.track.start_date
 
     @property
     def holland_B(self) -> float:
         """ Compute Holland B at each time snap """
         dataframe = self.track.data
-        Vmax = dataframe[MaximumSustainedWindSpeed.name]
+        # get Vmax after subtracting speed and adjusting to boundary layer
+        Vmax = (dataframe[MaximumSustainedWindSpeed.name] - dataframe['speed']) / BLAdj
+        Vmax = Vmax.values * MaximumSustainedWindSpeed.unit
         DelP = dataframe[BackgroundPressure.name] - dataframe[CentralPressure.name]
+        DelP = DelP.values * CentralPressure.unit
         B = Vmax * Vmax * AIR_DENSITY * E1 / DelP
         return B
 
     def compute_pc_from_Vmax(self, dataframe: DataFrame) -> float:
         """ Compute central pressure from Vmax based on Holland B """
-        Vmax = dataframe[MaximumSustainedWindSpeed.name]
-        DelP = Vmax ** 2 * AIR_DENSITY * E1 / self.holland_B
-        pc = dataframe[BackgroundPressure.name] - DelP
-        return pc
+        # get Vmax after subtracting speed and adjusting to boundary layer height
+        Vmax = (dataframe[MaximumSustainedWindSpeed.name] - dataframe['speed']) / BLAdj
+        Vmax = Vmax.values * MaximumSustainedWindSpeed.unit
+        DelP = Vmax * Vmax * AIR_DENSITY * E1 / self.holland_B
+        pc = dataframe[BackgroundPressure.name].values * CentralPressure.unit - DelP
+        return pc.magnitude
 
 
 def distribution_from_variables(variables: List[VortexPerturbedVariable]) -> Distribution:
     """
     :param variables: names of perturbed variables
     :return: chaospy joint distribution encompassing variables
     """
```

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/gdal_dataset.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/geometry.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/geometry.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/map.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/map.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/nodes.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,14 +215,18 @@
         float(nodes.coords['y'].min().values),
         float(nodes.coords['x'].max().values),
         float(nodes.coords['y'].max().values),
     ]
 
     countries = geopandas.read_file(geopandas.datasets.get_path('naturalearth_lowres'))
     countries.plot(color='lightgrey', ax=map_axis)
+    coast = cartopy.feature.NaturalEarthFeature(
+        category='physical', scale='50m', facecolor='none', name='coastline'
+    )
+    map_axis.add_feature(coast, edgecolor='grey', linewidth=0.5)
 
     if storm is not None:
         if not isinstance(storm, VortexTrack):
             try:
                 storm = VortexTrack.from_file(storm)
             except FileNotFoundError:
                 storm = VortexTrack(storm)
```

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/surrogate.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/taylor_diagram.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/taylor_diagram.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/plotting/utilities.py` & `ensembleperturbation-1.2.0/ensembleperturbation/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/ensemble_array.py` & `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/ensemble_array.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py` & `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from os import PathLike
 from pathlib import Path
 import pickle
 from typing import Union
 
+import cartopy
 import geopandas
+import cmocean
 from matplotlib import pyplot
 import numpy as np
 from sklearn.decomposition import PCA
 
 from ensembleperturbation.plotting.geometry import plot_points, plot_surface
 from ensembleperturbation.utilities import get_logger
 
@@ -205,29 +207,34 @@
                 actual_values['x'].max(),
                 actual_values['y'].max(),
             ]
         )
         vmax = np.round_(actual_values.quantile(0.98), decimals=1)
         vmin = min(0.0, np.round_(actual_values.quantile(0.02), decimals=1))
         sources = {'actual': actual_values, 'reconstructed': kl_prediction}
+        map_crs = cartopy.crs.PlateCarree()
         for example in ensembles_to_plot:
             figure = pyplot.figure()
             figure.set_size_inches(10, 10 / 1.61803398875)
             figure.suptitle(f'KL reconstruction comparison, ensemble #{example}')
             index = 0
             for source, value in sources.items():
                 index += 1
-                map_axis = figure.add_subplot(2, len(sources), index)
+                map_axis = figure.add_subplot(2, len(sources), index, projection=map_crs)
                 map_axis.title.set_text(f'{source}')
                 countries = geopandas.read_file(
                     geopandas.datasets.get_path('naturalearth_lowres')
                 )
+                countries.plot(color='lightgrey', ax=map_axis)
+                coast = cartopy.feature.NaturalEarthFeature(
+                    category='physical', scale='50m', facecolor='none', name='coastline'
+                )
+                map_axis.add_feature(coast, edgecolor='grey', linewidth=0.5)
                 map_axis.set_xlim((bounds[0], bounds[2]))
                 map_axis.set_ylim((bounds[1], bounds[3]))
-                countries.plot(color='lightgrey', ax=map_axis)
 
                 if element_table is None:
                     im = plot_points(
                         np.vstack(
                             (actual_values['x'], actual_values['y'], value[example, :])
                         ).T,
                         axis=map_axis,
@@ -243,14 +250,15 @@
                             (actual_values['x'], actual_values['y'], value[example, :])
                         ).T,
                         element_table=element_table.values,
                         axis=map_axis,
                         add_colorbar=False,
                         levels=np.linspace(vmin, vmax, 25 + 1),
                         extend='both',
+                        cmap=cmocean.tools.crop(cmocean.cm.diff_r, vmin, vmax, pivot=0),
                     )
 
             pyplot.subplots_adjust(wspace=0.02, right=0.96)
             cax = pyplot.axes([0.95, 0.55, 0.015, 0.3])
             cbar = figure.colorbar(im, extend='both', cax=cax)
 
             figure.savefig(
```

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py` & `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/uncertainty_quantification/surrogate.py` & `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/ensembleperturbation/utilities.py` & `ensembleperturbation-1.2.0/ensembleperturbation/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.1.2/pyproject.toml` & `ensembleperturbation-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'ensembleperturbation'
-version = "1.1.2"
+version = "1.2.0"
 description = 'perturbation of coupled model input over a space of input variables'
 authors = ['Zach Burnett <zachary.burnett@noaa.gov>']
 license = 'CC0-1.0'
 readme = 'README.md'
 repository = 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git'
 documentation = 'https://ensembleperturbation.readthedocs.io'
 
@@ -16,15 +16,15 @@
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry-dynamic-versioning]
 enable = true
 
 [tool.poetry.dependencies]
 python = '^3.8'
-adcircpy = '>=1.1.0'
+adcircpy = '>=1.2.3'
 appdirs = '*'
 beautifulsoup4 = '*'
 cartopy = { version = '*', optional = true }
 chaospy = '*'
 cmocean = { version = '*', optional = true }
 coupledmodeldriver = '>=1.5'
 dask = '*'
@@ -40,15 +40,15 @@
 pyproj = '>=2.6'
 tables = '*'
 typepigeon = '*'
 python-dateutil = '*'
 requests = '*'
 shapely = '*'
 scikit-learn = '*'
-stormevents = '>=1.4.1'
+stormevents = '>=2.1.4'
 isort = { version = '*', optional = true }
 oitnb = { version = '*', optional = true }
 pytest = { version = '*', optional = true }
 pytest-cov = { version = '*', optional = true }
 pytest-xdist = { version = '*', optional = true }
 wget = { version = '*', optional = true }
 m2r2 = { version = '*', optional = true }
```

### Comparing `ensembleperturbation-1.1.2/setup.py` & `ensembleperturbation-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  'ensembleperturbation.plotting',
  'ensembleperturbation.uncertainty_quantification']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['adcircpy>=1.1.0',
+['adcircpy>=1.2.3',
  'appdirs',
  'beautifulsoup4',
  'chaospy',
  'coupledmodeldriver>=1.5',
  'dask',
  'f90nml',
  'fiona',
@@ -28,15 +28,15 @@
  'pint-pandas',
  'pint<0.20',
  'pyproj>=2.6',
  'python-dateutil',
  'requests',
  'scikit-learn',
  'shapely',
- 'stormevents>=1.4.1',
+ 'stormevents>=2.1.4',
  'tables',
  'typepigeon']
 
 extras_require = \
 {'development': ['isort', 'oitnb'],
  'documentation': ['m2r2',
                    'sphinx',
@@ -54,15 +54,15 @@
                      'perturb_tracks = '
                      'ensembleperturbation.client.perturb_tracks:main',
                      'plot_results = '
                      'ensembleperturbation.client.plot_results:main']}
 
 setup_kwargs = {
     'name': 'ensembleperturbation',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'perturbation of coupled model input over a space of input variables',
     'long_description': '# Ensemble Perturbation\n\n[![tests](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/tests/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Atests)\n[![codecov](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation/branch/main/graph/badge.svg?token=4DwZePHp18)](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation)\n[![build](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/build/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Abuild)\n[![version](https://img.shields.io/pypi/v/EnsemblePerturbation)](https://pypi.org/project/EnsemblePerturbation)\n[![license](https://img.shields.io/github/license/noaa-ocs-modeling/EnsemblePerturbation)](https://creativecommons.org/share-your-work/public-domain/cc0)\n[![style](https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw)](https://sourceforge.net/p/oitnb/code)\n[![documentation](https://readthedocs.org/projects/ensembleperturbation/badge/?version=latest)](https://ensembleperturbation.readthedocs.io/en/latest/?badge=latest)\n\nPython library for perturbing coupled model inputs into ensemble runs. Provides\nperturbation and results comparison.\n\n```bash\npip install ensembleperturbation\n```\n\nDocumentation can be found at https://ensembleperturbation.readthedocs.io\n\n## Command-line interface\n\n`ensembleperturbation` exposes the following CLI commands:\n\n- `make_storm_ensemble`\n- `perturb_tracks`\n- `combine_results`\n- `plot_results`\n',
     'author': 'Zach Burnett',
     'author_email': 'zachary.burnett@noaa.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git',
```

### Comparing `ensembleperturbation-1.1.2/PKG-INFO` & `ensembleperturbation-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembleperturbation
-Version: 1.1.2
+Version: 1.2.0
 Summary: perturbation of coupled model input over a space of input variables
 Home-page: https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 License: CC0-1.0
 Author: Zach Burnett
 Author-email: zachary.burnett@noaa.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: development
 Provides-Extra: documentation
 Provides-Extra: plotting
 Provides-Extra: testing
-Requires-Dist: adcircpy (>=1.1.0)
+Requires-Dist: adcircpy (>=1.2.3)
 Requires-Dist: appdirs
 Requires-Dist: beautifulsoup4
 Requires-Dist: cartopy; extra == "plotting"
 Requires-Dist: chaospy
 Requires-Dist: cmocean; extra == "plotting"
 Requires-Dist: coupledmodeldriver (>=1.5)
 Requires-Dist: dask
@@ -44,15 +44,15 @@
 Requires-Dist: requests
 Requires-Dist: scikit-learn
 Requires-Dist: shapely
 Requires-Dist: sphinx-rtd-theme; extra == "documentation"
 Requires-Dist: sphinx; extra == "documentation"
 Requires-Dist: sphinxcontrib-bibtex; extra == "documentation"
 Requires-Dist: sphinxcontrib-programoutput; extra == "documentation"
-Requires-Dist: stormevents (>=1.4.1)
+Requires-Dist: stormevents (>=2.1.4)
 Requires-Dist: tables
 Requires-Dist: typepigeon
 Requires-Dist: wget; extra == "testing"
 Project-URL: Documentation, https://ensembleperturbation.readthedocs.io
 Project-URL: Repository, https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 Description-Content-Type: text/markdown
```

