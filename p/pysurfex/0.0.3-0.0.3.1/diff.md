# Comparing `tmp/pysurfex-0.0.3.tar.gz` & `tmp/pysurfex-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfex-0.0.3.tar", max compression
+gzip compressed data, was "pysurfex-0.0.3.1.tar", max compression
```

## Comparing `pysurfex-0.0.3.tar` & `pysurfex-0.0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2532 2023-04-25 14:46:17.108126 pysurfex-0.0.3/README.rst
--rw-r--r--   0        0        0     5177 2023-04-25 17:56:18.103745 pysurfex-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      142 2023-03-31 12:11:48.374345 pysurfex-0.0.3/pysurfex/__init__.py
--rw-r--r--   0        0        0    30965 2023-04-17 19:19:49.756387 pysurfex-0.0.3/pysurfex/binary_input.py
--rw-r--r--   0        0        0    18837 2023-04-11 16:19:27.906442 pysurfex-0.0.3/pysurfex/bufr.py
--rw-r--r--   0        0        0    10460 2023-04-11 16:19:16.982458 pysurfex-0.0.3/pysurfex/cache.py
--rw-r--r--   0        0        0    19335 2023-03-31 08:57:44.837420 pysurfex-0.0.3/pysurfex/cfg/config.yml
--rw-r--r--   0        0        0     8985 2023-03-31 08:57:44.837420 pysurfex-0.0.3/pysurfex/cfg/config_exp_surfex.toml
--rw-r--r--   0        0        0      135 2023-03-31 08:54:13.421958 pysurfex-0.0.3/pysurfex/cfg/default_thredds.cfg
--rw-r--r--   0        0        0     5253 2023-03-31 08:54:13.421958 pysurfex-0.0.3/pysurfex/cfg/first_guess.yml
--rw-r--r--   0        0        0      192 2023-03-31 08:54:13.421958 pysurfex-0.0.3/pysurfex/cfg/qc_codes.json
--rw-r--r--   0        0        0      370 2023-03-31 08:54:13.421958 pysurfex-0.0.3/pysurfex/cfg/user.yml
--rw-r--r--   0        0        0    62279 2023-04-18 15:50:09.017659 pysurfex-0.0.3/pysurfex/cli.py
--rw-r--r--   0        0        0    61762 2023-04-18 15:50:09.013659 pysurfex-0.0.3/pysurfex/cmd_parsing.py
--rw-r--r--   0        0        0    32663 2023-04-17 20:41:42.891563 pysurfex-0.0.3/pysurfex/configuration.py
--rw-r--r--   0        0        0     1291 2023-04-17 20:48:42.738319 pysurfex-0.0.3/pysurfex/datetime_utils.py
--rw-r--r--   0        0        0     8511 2023-04-11 13:03:13.949437 pysurfex-0.0.3/pysurfex/ecoclimap.py
--rw-r--r--   0        0        0     3891 2023-04-17 20:35:08.520837 pysurfex-0.0.3/pysurfex/fa.py
--rw-r--r--   0        0        0    58096 2023-04-17 20:48:43.446317 pysurfex-0.0.3/pysurfex/file.py
--rw-r--r--   0        0        0    35668 2023-04-11 12:43:07.897621 pysurfex-0.0.3/pysurfex/forcing.py
--rw-r--r--   0        0        0    33675 2023-04-11 11:15:45.811149 pysurfex-0.0.3/pysurfex/geo.py
--rw-r--r--   0        0        0    22471 2023-04-17 20:16:06.418276 pysurfex-0.0.3/pysurfex/grib.py
--rw-r--r--   0        0        0    14928 2023-04-18 15:50:08.465659 pysurfex-0.0.3/pysurfex/input_methods.py
--rw-r--r--   0        0        0    18924 2023-04-17 20:48:42.986318 pysurfex-0.0.3/pysurfex/interpolation.py
--rw-r--r--   0        0        0   100050 2023-04-17 20:37:11.304424 pysurfex-0.0.3/pysurfex/namelist.py
--rw-r--r--   0        0        0    34770 2023-04-17 19:19:49.760387 pysurfex-0.0.3/pysurfex/netcdf.py
--rw-r--r--   0        0        0    37729 2023-04-17 19:19:49.764387 pysurfex-0.0.3/pysurfex/obs.py
--rw-r--r--   0        0        0     4483 2023-04-11 10:39:28.527316 pysurfex-0.0.3/pysurfex/observation.py
--rw-r--r--   0        0        0    12016 2023-04-11 16:19:16.906458 pysurfex-0.0.3/pysurfex/obsmon.py
--rw-r--r--   0        0        0     6415 2023-04-17 20:48:42.802318 pysurfex-0.0.3/pysurfex/obsoul.py
--rw-r--r--   0        0        0    16227 2023-04-17 20:48:37.366334 pysurfex-0.0.3/pysurfex/platform.py
--rw-r--r--   0        0        0       20 2023-04-17 19:19:49.764387 pysurfex-0.0.3/pysurfex/plot.py
--rw-r--r--   0        0        0    17168 2023-04-17 20:40:07.519858 pysurfex-0.0.3/pysurfex/read.py
--rw-r--r--   0        0        0    11682 2023-04-11 16:19:28.082442 pysurfex-0.0.3/pysurfex/run.py
--rw-r--r--   0        0        0     2254 2023-03-31 08:54:13.425958 pysurfex-0.0.3/pysurfex/settings/assimilation.json
--rw-r--r--   0        0        0        0 2023-03-31 08:54:13.425958 pysurfex-0.0.3/pysurfex/settings/filetype.json
--rw-r--r--   0        0        0     1075 2023-03-31 08:54:13.425958 pysurfex-0.0.3/pysurfex/settings/forecast.json
--rw-r--r--   0        0        0     1305 2023-03-31 08:54:13.425958 pysurfex-0.0.3/pysurfex/settings/pgd.json
--rw-r--r--   0        0        0      952 2023-03-31 08:54:13.425958 pysurfex-0.0.3/pysurfex/settings/prep.json
--rw-r--r--   0        0        0     3499 2023-04-17 20:48:42.778319 pysurfex-0.0.3/pysurfex/timeseries.py
--rw-r--r--   0        0        0    67688 2023-04-17 20:48:37.326334 pysurfex-0.0.3/pysurfex/titan.py
--rw-r--r--   0        0        0     3463 2023-04-11 12:37:02.630242 pysurfex-0.0.3/pysurfex/util.py
--rw-r--r--   0        0        0    19977 2023-04-17 19:19:49.764387 pysurfex-0.0.3/pysurfex/variable.py
--rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 pysurfex-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2532 2023-04-26 06:09:39.281463 pysurfex-0.0.3.1/README.rst
+-rw-r--r--   0        0        0     5233 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/__init__.py
+-rw-r--r--   0        0        0    30965 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/binary_input.py
+-rw-r--r--   0        0        0    18837 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/bufr.py
+-rw-r--r--   0        0        0    10460 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cache.py
+-rw-r--r--   0        0        0    19335 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/config.yml
+-rw-r--r--   0        0        0     8985 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/config_exp_surfex.toml
+-rw-r--r--   0        0        0      135 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/default_thredds.cfg
+-rw-r--r--   0        0        0     5253 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/first_guess.yml
+-rw-r--r--   0        0        0      192 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/qc_codes.json
+-rw-r--r--   0        0        0      370 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/user.yml
+-rw-r--r--   0        0        0    62279 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/cli.py
+-rw-r--r--   0        0        0    61762 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/cmd_parsing.py
+-rw-r--r--   0        0        0    32663 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/configuration.py
+-rw-r--r--   0        0        0     1291 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/datetime_utils.py
+-rw-r--r--   0        0        0     8511 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/ecoclimap.py
+-rw-r--r--   0        0        0     3891 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/fa.py
+-rw-r--r--   0        0        0    58096 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/file.py
+-rw-r--r--   0        0        0    35668 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/forcing.py
+-rw-r--r--   0        0        0    33675 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/geo.py
+-rw-r--r--   0        0        0    22471 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/grib.py
+-rw-r--r--   0        0        0    14928 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/input_methods.py
+-rw-r--r--   0        0        0    18924 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/interpolation.py
+-rw-r--r--   0        0        0   100050 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/namelist.py
+-rw-r--r--   0        0        0    34770 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/netcdf.py
+-rw-r--r--   0        0        0    37729 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/obs.py
+-rw-r--r--   0        0        0     4483 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/observation.py
+-rw-r--r--   0        0        0    12016 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/obsmon.py
+-rw-r--r--   0        0        0     6415 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/obsoul.py
+-rw-r--r--   0        0        0    16227 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/platform.py
+-rw-r--r--   0        0        0       20 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/plot.py
+-rw-r--r--   0        0        0    17168 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/read.py
+-rw-r--r--   0        0        0    11682 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/run.py
+-rw-r--r--   0        0        0     2254 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/assimilation.json
+-rw-r--r--   0        0        0        0 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/filetype.json
+-rw-r--r--   0        0        0     1075 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/forecast.json
+-rw-r--r--   0        0        0     1305 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/pgd.json
+-rw-r--r--   0        0        0      952 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/prep.json
+-rw-r--r--   0        0        0     3499 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/timeseries.py
+-rw-r--r--   0        0        0    67688 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/titan.py
+-rw-r--r--   0        0        0     3463 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/util.py
+-rw-r--r--   0        0        0    19977 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/variable.py
+-rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 pysurfex-0.0.3.1/PKG-INFO
```

### Comparing `pysurfex-0.0.3/README.rst` & `pysurfex-0.0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pyproject.toml` & `pysurfex-0.0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [tool.poetry]
     name = "pysurfex"
-    version = "0.0.3"
+    version = "0.0.3.1"
     description = "Python API to SURFEX"
     authors = ["Trygve Aspelien"]
     license = "MIT"
     readme = "README.rst"
     repository = "https://github.com/metno/pysurfex"
     documentation = "https://metno.github.io/pysurfex/"
 
 [tool.poetry.scripts]
-    bufr2json = "surfex.cli:bufr2json"
-    create_forcing = "surfex.cli:create_forcing"
-    create_lsm_file = "surfex.cli:create_lsm_file_assim"
-    create_namelist = "surfex.cli:create_namelist"
-    cryoclim_pseudoobs = "surfex.cli:cryoclim_pseudoobs"
-    FirstGuess4gridpp = "surfex.cli:first_guess_for_oi"
-    dump_environ = "surfex.cli:dump_environ"
-    gridpp = "surfex.cli:gridpp"
-    hm2pysurfex = "surfex.cli:hm2pysurfex"
-    masterodb = "surfex.cli:masterodb"
-    merge_qc_data = "surfex.cli:cli_merge_qc_data"
-    modify_forcing = "surfex.cli:cli_modify_forcing"
-    obs2json = "surfex.cli:obs2json"
-    oi2soda = "surfex.cli:cli_oi2soda"
-    offline = "surfex.cli:offline"
-    perturbed_offline = "surfex.cli:perturbed_offline"
-    pgd = "surfex.cli:pgd"
-    plot_points = "surfex.cli:plot_points"
-    prep = "surfex.cli:prep"
-    qc2obsmon = "surfex.cli:qc2obsmon"
-    sentinel_obs = "surfex.cli:sentinel_obs"
-    set_domain = "surfex.cli:cli_set_domain"
-    set_geo_from_obs_set = "surfex.cli:cli_set_geo_from_obs_set"
-    set_geo_from_stationlist = "surfex.cli:set_geo_from_stationlist"
-    shape2ign = "surfex.cli:cli_shape2ign"
-    soda = "surfex.cli:soda"
-    titan = "surfex.cli:titan"
+    bufr2json = "pysurfex.cli:bufr2json"
+    create_forcing = "pysurfex.cli:create_forcing"
+    create_lsm_file = "pysurfex.cli:create_lsm_file_assim"
+    create_namelist = "pysurfex.cli:create_namelist"
+    cryoclim_pseudoobs = "pysurfex.cli:cryoclim_pseudoobs"
+    FirstGuess4gridpp = "pysurfex.cli:first_guess_for_oi"
+    dump_environ = "pysurfex.cli:dump_environ"
+    gridpp = "pysurfex.cli:gridpp"
+    hm2pysurfex = "pysurfex.cli:hm2pysurfex"
+    masterodb = "pysurfex.cli:masterodb"
+    merge_qc_data = "pysurfex.cli:cli_merge_qc_data"
+    modify_forcing = "pysurfex.cli:cli_modify_forcing"
+    obs2json = "pysurfex.cli:obs2json"
+    oi2soda = "pysurfex.cli:cli_oi2soda"
+    offline = "pysurfex.cli:offline"
+    perturbed_offline = "pysurfex.cli:perturbed_offline"
+    pgd = "pysurfex.cli:pgd"
+    plot_points = "pysurfex.cli:plot_points"
+    prep = "pysurfex.cli:prep"
+    qc2obsmon = "pysurfex.cli:qc2obsmon"
+    sentinel_obs = "pysurfex.cli:sentinel_obs"
+    set_domain = "pysurfex.cli:cli_set_domain"
+    set_geo_from_obs_set = "pysurfex.cli:cli_set_geo_from_obs_set"
+    set_geo_from_stationlist = "pysurfex.cli:set_geo_from_stationlist"
+    shape2ign = "pysurfex.cli:cli_shape2ign"
+    soda = "pysurfex.cli:soda"
+    titan = "pysurfex.cli:titan"
 
 [build-system]
     build-backend = "poetry.core.masonry.api"
     requires = ["poetry-core > 1.2.0"]
 
 [tool.poetry.dependencies]
     python = "^3.8"
```

### Comparing `pysurfex-0.0.3/pysurfex/binary_input.py` & `pysurfex-0.0.3.1/pysurfex/binary_input.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/bufr.py` & `pysurfex-0.0.3.1/pysurfex/bufr.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/cache.py` & `pysurfex-0.0.3.1/pysurfex/cache.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/cfg/config.yml` & `pysurfex-0.0.3.1/pysurfex/cfg/config.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/cfg/config_exp_surfex.toml` & `pysurfex-0.0.3.1/pysurfex/cfg/config_exp_surfex.toml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/cfg/first_guess.yml` & `pysurfex-0.0.3.1/pysurfex/cfg/first_guess.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/cli.py` & `pysurfex-0.0.3.1/pysurfex/cli.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/cmd_parsing.py` & `pysurfex-0.0.3.1/pysurfex/cmd_parsing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/configuration.py` & `pysurfex-0.0.3.1/pysurfex/configuration.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/datetime_utils.py` & `pysurfex-0.0.3.1/pysurfex/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/ecoclimap.py` & `pysurfex-0.0.3.1/pysurfex/ecoclimap.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/fa.py` & `pysurfex-0.0.3.1/pysurfex/fa.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/file.py` & `pysurfex-0.0.3.1/pysurfex/file.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/forcing.py` & `pysurfex-0.0.3.1/pysurfex/forcing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/geo.py` & `pysurfex-0.0.3.1/pysurfex/geo.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/grib.py` & `pysurfex-0.0.3.1/pysurfex/grib.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/input_methods.py` & `pysurfex-0.0.3.1/pysurfex/input_methods.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/interpolation.py` & `pysurfex-0.0.3.1/pysurfex/interpolation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/namelist.py` & `pysurfex-0.0.3.1/pysurfex/namelist.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/netcdf.py` & `pysurfex-0.0.3.1/pysurfex/netcdf.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/obs.py` & `pysurfex-0.0.3.1/pysurfex/obs.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/observation.py` & `pysurfex-0.0.3.1/pysurfex/observation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/obsmon.py` & `pysurfex-0.0.3.1/pysurfex/obsmon.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/obsoul.py` & `pysurfex-0.0.3.1/pysurfex/obsoul.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/platform.py` & `pysurfex-0.0.3.1/pysurfex/platform.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/read.py` & `pysurfex-0.0.3.1/pysurfex/read.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/run.py` & `pysurfex-0.0.3.1/pysurfex/run.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/settings/assimilation.json` & `pysurfex-0.0.3.1/pysurfex/settings/assimilation.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/settings/forecast.json` & `pysurfex-0.0.3.1/pysurfex/settings/forecast.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/settings/pgd.json` & `pysurfex-0.0.3.1/pysurfex/settings/pgd.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/settings/prep.json` & `pysurfex-0.0.3.1/pysurfex/settings/prep.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/timeseries.py` & `pysurfex-0.0.3.1/pysurfex/timeseries.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/titan.py` & `pysurfex-0.0.3.1/pysurfex/titan.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/util.py` & `pysurfex-0.0.3.1/pysurfex/util.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/pysurfex/variable.py` & `pysurfex-0.0.3.1/pysurfex/variable.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3/PKG-INFO` & `pysurfex-0.0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfex
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Python API to SURFEX
 Home-page: https://github.com/metno/pysurfex
 License: MIT
 Author: Trygve Aspelien
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

