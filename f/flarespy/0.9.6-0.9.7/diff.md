# Comparing `tmp/flarespy-0.9.6.tar.gz` & `tmp/flarespy-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.9.6.tar", max compression
+gzip compressed data, was "flarespy-0.9.7.tar", max compression
```

## Comparing `flarespy-0.9.6.tar` & `flarespy-0.9.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.6/LICENSE
--rw-r--r--   0        0        0      428 2023-04-25 16:47:51.276523 flarespy-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.6/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.6/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.6/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    34997 2023-04-25 16:48:46.724403 flarespy-0.9.6/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4674 2023-04-25 16:16:25.193202 flarespy-0.9.6/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-25 16:47:51.274527 flarespy-0.9.6/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.7/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-25 23:11:23.194116 flarespy-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.7/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.7/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.7/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    34997 2023-04-25 23:10:54.809941 flarespy-0.9.7/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4674 2023-04-25 16:16:25.193202 flarespy-0.9.7/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-25 23:11:23.188897 flarespy-0.9.7/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.7/PKG-INFO
```

### Comparing `flarespy-0.9.6/LICENSE` & `flarespy-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.6/src/flarespy/Flare_model.py` & `flarespy-0.9.7/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.6/src/flarespy/data/model.dat` & `flarespy-0.9.7/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.6/src/flarespy/flarefinder.py` & `flarespy-0.9.7/src/flarespy/flarefinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,17 +501,17 @@
                         )
                         with warnings.catch_warnings():
                             warnings.filterwarnings("ignore", category=ErfaWarning)
                             coords = coords_j2000.apply_space_motion(new_obstime=Time("J2016"))
                     else:
                         coords = SkyCoord(ra, dec, frame="icrs")
                     radius = u.Quantity(1, u.arcmin)
-                    gaia_result = Gaia.cone_search_async(coords, radius, columns=["source_id"]).get_results()[0]
+                    gaia_result = Gaia.cone_search_async(coords, radius, columns=["source_id"]).get_results()
                     if (gaia_result["dist"] < (3 / 3600)).any():
-                        gaia_dr3_source_id = str(gaia_result["source_id"])
+                        gaia_dr3_source_id = str(gaia_result[0]["source_id"])
 
         self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_source_id
 
     def _query_object_type(self):
         """
         Query object info from SIMBAD
         """
```

### Comparing `flarespy-0.9.6/src/flarespy/utils.py` & `flarespy-0.9.7/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.6/PKG-INFO` & `flarespy-0.9.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.9.6
+Version: 0.9.7
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

