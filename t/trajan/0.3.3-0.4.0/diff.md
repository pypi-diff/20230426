# Comparing `tmp/trajan-0.3.3.tar.gz` & `tmp/trajan-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajan-0.3.3.tar", max compression
+gzip compressed data, was "trajan-0.4.0.tar", max compression
```

## Comparing `trajan-0.3.3.tar` & `trajan-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0    18092 2023-03-23 11:58:59.122729 trajan-0.3.3/LICENSE
--rw-r--r--   0        0        0     1819 2023-03-23 11:58:59.122729 trajan-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7875 2023-03-23 11:58:59.130729 trajan-0.3.3/trajan/__init__.py
--rw-r--r--   0        0        0     1385 2023-03-23 11:58:59.130729 trajan-0.3.3/trajan/animation/__init__.py
--rw-r--r--   0        0        0     6390 2023-03-23 11:58:59.130729 trajan-0.3.3/trajan/plot/__init__.py
--rw-r--r--   0        0        0     2204 2023-03-23 11:58:59.130729 trajan-0.3.3/trajan/plot/land.py
--rw-r--r--   0        0        0     2016 2023-03-23 11:58:59.130729 trajan-0.3.3/trajan/scripts/trajanshow.py
--rw-r--r--   0        0        0     1317 2023-03-23 11:58:59.134729 trajan-0.3.3/trajan/skill/__init__.py
--rw-r--r--   0        0        0    12204 2023-03-23 11:58:59.134729 trajan-0.3.3/trajan/traj.py
--rw-r--r--   0        0        0     6382 2023-03-23 11:58:59.134729 trajan-0.3.3/trajan/traj1d.py
--rw-r--r--   0        0        0     4035 2023-03-23 11:58:59.134729 trajan-0.3.3/trajan/traj2d.py
--rw-r--r--   0        0        0     2244 2023-03-23 11:58:59.134729 trajan-0.3.3/trajan/trajectory_accessor.py
--rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 trajan-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-04-26 08:17:50.990474 trajan-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1836 2023-04-26 08:17:50.994474 trajan-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9058 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/animation/__init__.py
+-rw-r--r--   0        0        0     6390 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/plot/__init__.py
+-rw-r--r--   0        0        0     2204 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/plot/land.py
+-rw-r--r--   0        0        0        0 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/readers/__init__.py
+-rw-r--r--   0        0        0    17799 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/readers/omb.py
+-rwxr-xr-x   0        0        0    27653 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/readers/omb_decoder.py
+-rw-r--r--   0        0        0     2016 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/scripts/trajanshow.py
+-rw-r--r--   0        0        0     1317 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/skill/__init__.py
+-rw-r--r--   0        0        0    12159 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/traj.py
+-rw-r--r--   0        0        0     7251 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/traj1d.py
+-rw-r--r--   0        0        0     5382 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/traj2d.py
+-rw-r--r--   0        0        0     2278 2023-04-26 08:17:51.002474 trajan-0.4.0/trajan/trajectory_accessor.py
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 trajan-0.4.0/PKG-INFO
```

### Comparing `trajan-0.3.3/LICENSE` & `trajan-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trajan-0.3.3/pyproject.toml` & `trajan-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajan"
-version = "0.3.3"
+version = "0.4.0"
 description = "Trajectory analysis package for simulated and observed trajectories"
 authors = ["Gaute Hope <gauteh@met.no>", "Knut-Frode Dagestad <knutfd@met.no>"]
 license = "GPLv2"
 
 [tool.poetry.scripts]
 trajanshow = "trajan.scripts.trajanshow:main"
 
@@ -12,14 +12,15 @@
 python = "^3.8"
 matplotlib = ">=3.5"
 numpy = ">=1.23"
 scipy = ">=1.9"
 netCDF4 = ">=1.6"
 pyproj = ">=2.3"
 xarray = ">=2022.6.0"
+pandas = ">=2.0"
 cartopy = ">=0.21"
 click = "^8.1.3"
 cf_xarray = ">=0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-benchmark = "^3"
```

### Comparing `trajan-0.3.3/trajan/__init__.py` & `trajan-0.4.0/trajan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         `time`: name of column containing timestamps (parsable by pandas).
 
         `name`: name of column to be used for drifter names.
 
     Returns:
 
-        `ds`: a CF-compliant trajaectory `xarray.Dataset`.
+        `ds`: a CF-compliant trajectory `xarray.Dataset`.
 
 
     Constructing a dataset from arrays of postions and time:
     --------------------------------------------------------
 
     .. testcode::
 
@@ -59,74 +59,108 @@
         ds = pd.DataFrame({'lon': lon, 'lat': lat, 'time': time, 'temp': temp, 'name': 'My drifter'})
         ds = ta.from_dataframe(ds, name='name')
         print(ds)
 
     .. testoutput::
 
         <xarray.Dataset>
-        Dimensions:        (trajectory: 1, obs: 50)
+        Dimensions:     (trajectory: 1, obs: 50)
         Coordinates:
-          * trajectory     (trajectory) int64 0
-          * obs            (obs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
+          * trajectory  (trajectory) <U10 'My drifter'
+          * obs         (obs) int64 0 1 2 3 4 5 6 7 8 9 ... 41 42 43 44 45 46 47 48 49
         Data variables:
-            lon            (trajectory, obs) float64 5.0 5.102 5.204 ... 9.898 10.0
-            lat            (trajectory, obs) float64 60.0 60.2 60.41 ... 69.59 69.8 70.0
-            time           (trajectory, obs) datetime64[ns] 2023-01-01 ... 2023-01-14
-            temp           (trajectory, obs) float64 10.0 10.1 10.2 ... 14.8 14.9 15.0
-            drifter_names  (trajectory) object 'My drifter'
+            lon         (trajectory, obs) float64 5.0 5.102 5.204 ... 9.796 9.898 10.0
+            lat         (trajectory, obs) float64 60.0 60.2 60.41 ... 69.59 69.8 70.0
+            time        (trajectory, obs) datetime64[ns] 2023-01-01 ... 2023-01-14
+            temp        (trajectory, obs) float64 10.0 10.1 10.2 ... 14.8 14.9 15.0
+        Attributes:
+            Conventions:          CF-1.10
+            featureType:          trajectory
+            geospatial_lat_min:   60.0
+            geospatial_lat_max:   70.0
+            geospatial_lon_min:   5.0
+            geospatial_lon_max:   10.0
+            time_coverage_start:  2023-01-01T00:00:00
+            time_coverage_end:    2023-01-14T00:00:00
 
     Often you might want to add some attributes:
 
     .. testcode::
 
         ds = ds.assign_attrs({'Author': 'Albus Dumbledore'})
         print(ds)
 
     .. testoutput::
 
         <xarray.Dataset>
-        Dimensions:        (trajectory: 1, obs: 50)
+        Dimensions:     (trajectory: 1, obs: 50)
         Coordinates:
-          * trajectory     (trajectory) int64 0
-          * obs            (obs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
+          * trajectory  (trajectory) <U10 'My drifter'
+          * obs         (obs) int64 0 1 2 3 4 5 6 7 8 9 ... 41 42 43 44 45 46 47 48 49
         Data variables:
-            lon            (trajectory, obs) float64 5.0 5.102 5.204 ... 9.898 10.0
-            lat            (trajectory, obs) float64 60.0 60.2 60.41 ... 69.59 69.8 70.0
-            time           (trajectory, obs) datetime64[ns] 2023-01-01 ... 2023-01-14
-            temp           (trajectory, obs) float64 10.0 10.1 10.2 ... 14.8 14.9 15.0
-            drifter_names  (trajectory) object 'My drifter'
+            lon         (trajectory, obs) float64 5.0 5.102 5.204 ... 9.796 9.898 10.0
+            lat         (trajectory, obs) float64 60.0 60.2 60.41 ... 69.59 69.8 70.0
+            time        (trajectory, obs) datetime64[ns] 2023-01-01 ... 2023-01-14
+            temp        (trajectory, obs) float64 10.0 10.1 10.2 ... 14.8 14.9 15.0
         Attributes:
-            Author:   Albus Dumbledore
+            Conventions:          CF-1.10
+            featureType:          trajectory
+            geospatial_lat_min:   60.0
+            geospatial_lat_max:   70.0
+            geospatial_lon_min:   5.0
+            geospatial_lon_max:   10.0
+            time_coverage_start:  2023-01-01T00:00:00
+            time_coverage_end:    2023-01-14T00:00:00
+            Author:               Albus Dumbledore
 
     """
     df = df.copy()
     df.index.names = ['obs']
-    df[time] = pd.to_datetime(df[time])
+    df[time] = pd.to_datetime(df[time], format='mixed')
 
     df = df.rename(columns={lat: 'lat', lon: 'lon', time: 'time'})
 
     if name is not None:
-        df = df.rename(columns={name: 'drifter_names'})
+        df = df.rename(columns={name: 'trajectory'})
     else:
-        df['drifter_names'] = 'Drifter 1'
+        df['trajectory'] = 'Drifter 1'
 
     # Convert to UTC and remove tz-info. Xarray does not support tz-aware
     # datetimes.
     if df['time'].dt.tz is not None:
         df['time'] = df['time'].dt.tz_convert(None)
 
-    # Classify trajectories based on drifter_names.
-    df['trajectory'] = df.groupby('drifter_names').ngroup()
+    # Classify trajectories based on drifter names.
     df = df.set_index(['trajectory', df.index])
     df = df.to_xarray()
+    df['trajectory'] = df['trajectory'].astype(str)
+    df['trajectory'].attrs = { 'cf_role': 'trajectory_id', 'long_name' : 'trajectory name' }
 
-    # Simplify the drifter_names variable: It is only dependent on the trajectory dimension.
-    df['drifter_names'] = df.drifter_names.isel(obs=0)
-
-    # df = df.dropna(dim='obs', how='all')
+    df = df.assign_attrs({
+        'Conventions':
+        'CF-1.10',
+        'featureType':
+        'trajectory',
+        'geospatial_lat_min':
+        np.nanmin(df.lat),
+        'geospatial_lat_max':
+        np.nanmax(df.lat),
+        'geospatial_lon_min':
+        np.nanmin(df.lon),
+        'geospatial_lon_max':
+        np.nanmax(df.lon),
+        'time_coverage_start':
+        pd.to_datetime(
+            np.nanmin(df.time.values[
+                df.time.values != np.datetime64('NaT')])).isoformat(),
+        'time_coverage_end':
+        pd.to_datetime(
+            np.nanmax(df.time.values[
+                df.time.values != np.datetime64('NaT')])).isoformat(),
+    })
 
     return df
 
 
 def trajectory_dict_to_dataset(trajectory_dict,
                                variable_attributes=None,
                                global_attributes=None):
```

### Comparing `trajan-0.3.3/trajan/animation/__init__.py` & `trajan-0.4.0/trajan/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `trajan-0.3.3/trajan/plot/__init__.py` & `trajan-0.4.0/trajan/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `trajan-0.3.3/trajan/plot/land.py` & `trajan-0.4.0/trajan/plot/land.py`

 * *Files identical despite different names*

### Comparing `trajan-0.3.3/trajan/scripts/trajanshow.py` & `trajan-0.4.0/trajan/scripts/trajanshow.py`

 * *Files identical despite different names*

### Comparing `trajan-0.3.3/trajan/skill/__init__.py` & `trajan-0.4.0/trajan/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `trajan-0.3.3/trajan/traj.py` & `trajan-0.4.0/trajan/traj.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,51 @@
+from abc import abstractmethod
 import pyproj
 import numpy as np
 import xarray as xr
 import cf_xarray as _
 import logging
 
 logger = logging.getLogger(__name__)
 
 
+def __require_obsdim__(f):
+    """
+    This decorator is for methods of Traj that require a time or obs dimension to work.
+    """
+
+    def wrapper(*args, **kwargs):
+        if args[0].obsdim is None:
+            raise ValueError(f'{f} requires an obs or time dimension')
+        return f(*args, **kwargs)
+
+    return wrapper
+
+
 class Traj:
     ds: xr.Dataset
+
     __gcrs__: pyproj.CRS
+
     obsdim: str
+    """
+    Name of the dimension along which observations are taken. Usually either `obs` or `time`.
+    """
 
     def __init__(self, ds):
         self.ds = ds
         self.__gcrs__ = pyproj.CRS.from_epsg(4326)
 
         if 'obs' in self.ds.dims:
             self.obsdim = 'obs'
         elif 'time' in self.ds.dims:
             self.obsdim = 'time'
         else:
-            raise ValueError('No time or obs dimension')
+            logger.warning('No time or obs dimension detected.')
+            self.obsdim = None
 
     @property
     def tx(self):
         """
         Trajectory x coordinates (usually longitude).
 
         .. see-also:
@@ -72,15 +92,15 @@
             return self.tx
         else:
             if self.crs is None:
                 return self.tx
             else:
                 x, _ = self.transform(self.__gcrs__, self.tx, self.ty)
                 X = self.tx.copy(deep=False,
-                                   data=x)  # TODO: remove grid-mapping.
+                                 data=x)  # TODO: remove grid-mapping.
                 return X
 
     @property
     def tlat(self):
         """
         Retrieve the trajectories in geographic coordinates (latitudes).
         """
@@ -88,15 +108,15 @@
             return self.ty
         else:
             if self.crs is None:
                 return self.ty
             else:
                 _, y = self.transform(self.__gcrs__, self.tx, self.ty)
                 Y = self.ty.copy(deep=False,
-                                   data=y)  # TODO: remove grid-mapping.
+                                 data=y)  # TODO: remove grid-mapping.
                 return Y
 
     def transform(self, to_crs, x, y):
         """
         Transform coordinates in this datasets coordinate system to `to_crs` coordinate system.
 
         Args:
@@ -205,14 +225,43 @@
         """Returns the speed [m/s] along trajectories"""
 
         distance = self.distance_to_next()
         timedelta_seconds = self.time_to_next() / np.timedelta64(1, 's')
 
         return distance / timedelta_seconds
 
+    def distance_to(self, other):
+        """
+        Distance between trajectories or a single point.
+        """
+
+        other = other.broadcast_like(self.ds)
+        geod = pyproj.Geod(ellps='WGS84')
+        az_fwd, a2, distance = geod.inv(self.ds.traj.tlon, self.ds.traj.tlat,
+                                        other.traj.tlon, other.traj.tlat)
+
+        ds = xr.Dataset()
+        ds['distance'] = xr.DataArray(distance,
+                                      name='distance',
+                                      coords=self.ds.traj.tlon.coords,
+                                      attrs={'unit': 'm'})
+
+        ds['az_fwd'] = xr.DataArray(az_fwd,
+                                    name='forward azimuth',
+                                    coords=self.ds.traj.tlon.coords,
+                                    attrs={'unit': 'degrees'})
+
+        ds['az_bwd'] = xr.DataArray(a2,
+                                    name='back azimuth',
+                                    coords=self.ds.traj.tlon.coords,
+                                    attrs={'unit': 'degrees'})
+
+        return ds
+
+    @__require_obsdim__
     def distance_to_next(self):
         """Returns distance in m from one position to the next
 
            Last time is repeated for last position (which has no next position)
         """
 
         lon = self.ds.lon
@@ -227,14 +276,15 @@
                                                  latto)
 
         distance = xr.DataArray(distance, coords=lonfrom.coords, dims=lon.dims)
         distance = xr.concat((distance, distance.isel({self.obsdim: -1})),
                              dim=self.obsdim)  # repeating last time step to
         return distance
 
+    @__require_obsdim__
     def azimuth_to_next(self):
         """Returns azimution travel direction in degrees from one position to the next
 
            Last time is repeated for last position (which has no next position)
         """
 
         # TODO: method is almost duplicate of "distance_to_next" above
@@ -299,66 +349,21 @@
             fin = np.isfinite(x + y)
             points = np.vstack((y.T, x.T)).T
             hull = ConvexHull(points)
             area.append(hull.volume)  # volume=area for 2D as here
 
         return np.array(area)
 
+    @abstractmethod
     def gridtime(self, times):
-        """Interpolate dataset to regular time interval
-
-        times:
-            - an array of times, or
-            - a string "freq" specifying a Pandas daterange (e.g. 'h', '6h, 'D'...)
-
-        Note that the resulting DataSet will have "time" as a dimension coordinate.
-        """
-
-        from scipy.interpolate import interp1d
-        import pandas as pd
-
-        if isinstance(times, str):  # Make time series with given interval
-            freq = times
-            start_time = np.nanmin(np.asarray(self.ds.time))
-            # start_time = pd.to_datetime(start_time).strftime('%Y-%m-%d')
-            end_time = np.nanmax(np.asarray(self.ds.time))
-            # end_time = pd.to_datetime(end_time).strftime('%Y-%m-%d')
-            times = pd.date_range(start_time, end_time, freq=freq, inclusive='both')
-
-        # Why not..
-        if not isinstance(times, np.ndarray):
-            times = times.to_numpy()
-
-        # Create empty dataset to hold interpolated values
-        d = xr.Dataset(coords={
-            'trajectory': self.ds['trajectory'],
-            'time': (["time"], times)
-        },
-                       attrs=self.ds.attrs)
-
-        for varname, var in self.ds.variables.items():
-            if varname in ('time', 'obs'):
-                continue
-            if 'obs' not in var.dims:
-                d[varname] = var
-                continue
+        """Interpolate dataset to a regular time interval or a different grid.
 
-            # Create empty dataarray to hold interpolated values for given variable
-            da = xr.DataArray(data=np.zeros(
-                tuple(d.dims[di] for di in ['trajectory', 'time'])) * np.nan,
-                              dims=d.dims,
-                              coords=d.coords,
-                              attrs=var.attrs)
-
-            origtimes = self.ds['time'].ffill(dim='obs').astype(np.float64)
-
-            for t in range(
-                    self.ds.dims['trajectory']):  # loop over trajectories
-                # Make interpolator
-                f = interp1d(origtimes.isel(trajectory=t), var.isel(trajectory=t), bounds_error=False)
-                # Interpolate onto given times
-                da.loc[{'trajectory': t}] = f(times.astype(np.float64))
+        Args:
 
-            d[varname] = da
+            `times`: Target time interval, can be either:
+                - an array of times, or
+                - a string "freq" specifying a Pandas daterange (e.g. 'h', '6h, 'D'...) suitable for `pd.date_range`.
 
-        return d
+        Returns:
 
+            A new dataset interpolated to the target times. The dataset will be 1D (i.e. gridded) and the time dimension will be named `time`.
+        """
```

### Comparing `trajan-0.3.3/trajan/traj1d.py` & `trajan-0.4.0/trajan/traj1d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import xarray as xr
 import numpy as np
-from .traj import Traj
+from .traj import Traj, __require_obsdim__
 from . import skill
 
 
 class Traj1d(Traj):
     """
     A structured dataset, where each trajectory is always given at the same times. Typically the output from a model or from a gridded dataset.
     """
@@ -71,14 +71,15 @@
         puv, quv, cw, ccw, F = rotary_spectra(u, v)
         print(puv)
         import matplotlib.pyplot as plt
         plt.plot(1 / F, cw)
         plt.xlim([0, 30])
         plt.show()
 
+    @__require_obsdim__
     def skill(self, other, method='liu-weissberg', **kwargs):
         """
         Compare the skill score between this trajectory and `other`.
 
         Args:
 
             other: Another trajectory dataset.
@@ -192,7 +193,31 @@
             else:
                 raise ValueError(f"Unknown skill-score method: {method}.")
 
         return xr.DataArray(s,
                             name='Skill-score',
                             coords={'trajectory': self.ds.trajectory},
                             attrs={'method': method})
+
+    @__require_obsdim__
+    def gridtime(self, times):
+        if isinstance(times, str):  # Make time series with given interval
+            import pandas as pd
+            start_time = np.nanmin(np.asarray(self.ds.time))
+            end_time = np.nanmax(np.asarray(self.ds.time))
+            times = pd.date_range(start_time,
+                                  end_time,
+                                  freq=times,
+                                  inclusive='both')
+
+        if not isinstance(times, np.ndarray):
+            times = times.to_numpy()
+
+        ds = self.ds.interp({self.obsdim: times})
+
+        if self.obsdim != 'time':
+            ds = ds.rename({self.obsdim: 'time'}).set_index({'time': 'time'})
+
+        if not 'trajectory' in ds.dims:
+            ds = ds.expand_dims('trajectory')
+
+        return ds
```

### Comparing `trajan-0.3.3/trajan/traj2d.py` & `trajan-0.4.0/trajan/traj2d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import xarray as xr
 import numpy as np
 
-from .traj import Traj
+from .traj import Traj, __require_obsdim__
+
 
 class Traj2d(Traj):
     """
     A unstructured dataset, where each trajectory may have observations at different times. Typically from a collection of drifters.
     """
 
     def __init__(self, ds):
         super().__init__(ds)
 
-
     def timestep(self, average=np.nanmedian):
         """
         Return median time step between observations in seconds.
         """
         td = np.diff(self.ds.time, axis=1) / np.timedelta64(1, 's')
         td = average(td)
         return td
@@ -41,15 +41,16 @@
         num_inserts = condition.sum(dim='obs')
         max_obs = (index_of_last + num_inserts).max().values
 
         # Create new empty dataset with extended obs dimension
         trajcoord = range(self.ds.dims['trajectory'])
         nd = xr.Dataset(
             coords={
-                'trajectory': (["trajectory"], range(self.ds.dims['trajectory'])),
+                'trajectory':
+                (["trajectory"], range(self.ds.dims['trajectory'])),
                 'obs': (['obs'], range(max_obs))  # Longest trajectory
             },
             attrs=self.ds.attrs)
 
         # Add extended variables
         for varname, var in self.ds.data_vars.items():
             if 'obs' not in var.dims:
@@ -106,7 +107,46 @@
         trajs = [
             t.pad(pad_width={'obs': (0, newlen - t.dims['obs'])})
             for t in trajs
         ]
 
         return xr.concat(trajs, dim='trajectory')
 
+    @__require_obsdim__
+    def gridtime(self, times):
+        if isinstance(times, str):  # Make time series with given interval
+            import pandas as pd
+            start_time = np.nanmin(np.asarray(self.ds.time))
+            end_time = np.nanmax(np.asarray(self.ds.time))
+            times = pd.date_range(start_time,
+                                  end_time,
+                                  freq=times,
+                                  inclusive='both')
+
+        if not isinstance(times, np.ndarray):
+            times = times.to_numpy()
+
+        d = None
+
+        for t in range(self.ds.dims['trajectory']):
+            dt = self.ds.isel(trajectory=t) \
+                        .dropna(self.obsdim, how='all')
+
+            dt = dt.assign_coords({self.obsdim : dt.time.values }) \
+                   .drop_vars('time') \
+                   .rename({self.obsdim : 'time'}) \
+                   .set_index({'time': 'time'})
+
+            _, ui = np.unique(dt.time, return_index=True)
+            dt = dt.isel(time=ui)
+
+            dt = dt.interp({'time': times})
+
+            if d is None:
+                d = dt.expand_dims('trajectory')
+            else:
+                d = xr.concat((d, dt), "trajectory")
+
+        d = d.assign_coords({'trajectory' : self.ds['trajectory']})
+
+        return d
+
```

### Comparing `trajan-0.3.3/trajan/trajectory_accessor.py` & `trajan-0.4.0/trajan/trajectory_accessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """
 Extending xarray Dataset with functionality specific to trajectory datasets.
 
 Presently supporting Cf convention H.4.1
 https://cfconventions.org/Data/cf-conventions/cf-conventions-1.10/cf-conventions.html#_multidimensional_array_representation_of_trajectories.
 """
 
-import numpy as np
-import pandas as pd
 import xarray as xr
-import pyproj
 import logging
 
 from .plot import Plot
 from .animation import Animation
 from .traj import Traj
 from .traj1d import Traj1d
 from .traj2d import Traj2d
@@ -36,15 +33,17 @@
             logger.info(
                 'Normalizing dimension name from "traj" to "trajectory".')
             self._ds = self._ds.rename({'traj': 'trajectory'})
 
         if 'trajectory' not in self.ds.dims:  # Add empty trajectory dimension, if single trajectory
             self._ds = self._ds.expand_dims({'trajectory': 1})
 
-        if len(self.ds['time'].shape) <= 1:
+        if 'time' not in self.ds.variables:
+            self.inner = Traj1d(self.ds)
+        elif len(self.ds['time'].shape) <= 1:
             logger.debug('Detected structured (1D) trajectory dataset')
             self.inner = Traj1d(self._ds)
         elif len(self.ds['time'].shape) == 2:
             logger.debug('Detected un-structured (2D) trajectory dataset')
             self.inner = Traj2d(self._ds)
         else:
             raise ValueError(f'Time dimension has shape greater than 2: {self.ds["time"].shape}')
```

### Comparing `trajan-0.3.3/PKG-INFO` & `trajan-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajan
-Version: 0.3.3
+Version: 0.4.0
 Summary: Trajectory analysis package for simulated and observed trajectories
 License: GPLv2
 Author: Gaute Hope
 Author-email: gauteh@met.no
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,10 +14,11 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cartopy (>=0.21)
 Requires-Dist: cf_xarray (>=0.8.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: matplotlib (>=3.5)
 Requires-Dist: netCDF4 (>=1.6)
 Requires-Dist: numpy (>=1.23)
+Requires-Dist: pandas (>=2.0)
 Requires-Dist: pyproj (>=2.3)
 Requires-Dist: scipy (>=1.9)
 Requires-Dist: xarray (>=2022.6.0)
```

