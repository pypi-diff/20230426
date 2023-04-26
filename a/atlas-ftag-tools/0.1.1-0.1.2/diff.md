# Comparing `tmp/atlas-ftag-tools-0.1.1.tar.gz` & `tmp/atlas-ftag-tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-ftag-tools-0.1.1.tar", last modified: Mon Apr 24 14:27:37 2023, max compression
+gzip compressed data, was "atlas-ftag-tools-0.1.2.tar", last modified: Wed Apr 26 11:03:09 2023, max compression
```

## Comparing `atlas-ftag-tools-0.1.1.tar` & `atlas-ftag-tools-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.902977 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/ftag/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/flavour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/flavours.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/ftag/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/h5reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/h5utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/h5writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/vds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/ftag/wps/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/wps/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/wps/working_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.649164 atlas-ftag-tools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-26 11:03:09.649164 atlas-ftag-tools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 11:03:09.000000 atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/ftag/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/flavour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/flavours.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/ftag/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/h5reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/h5utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/hdf5/h5writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/vds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:09.645164 atlas-ftag-tools-0.1.2/ftag/wps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/wps/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/ftag/wps/working_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-26 11:02:50.000000 atlas-ftag-tools-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:03:09.649164 atlas-ftag-tools-0.1.2/setup.cfg
```

### Comparing `atlas-ftag-tools-0.1.1/PKG-INFO` & `atlas-ftag-tools-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -71,14 +71,16 @@
 ```
 
 Both the `--tagger` and `--fx` options accept a list if you want to get the WPs for multiple taggers.
 
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
+If instead of defining the working points for a series of signal efficiencies, you wish to calculate a WP corresponding to a specific background rejection, the `--rejection` option can be given along with the desired background.
+
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
 Use `--help` for more options and information.
 
 
 ## Tests
```

### Comparing `atlas-ftag-tools-0.1.1/README.md` & `atlas-ftag-tools-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 ```
 
 Both the `--tagger` and `--fx` options accept a list if you want to get the WPs for multiple taggers.
 
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
+If instead of defining the working points for a series of signal efficiencies, you wish to calculate a WP corresponding to a specific background rejection, the `--rejection` option can be given along with the desired background.
+
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
 Use `--help` for more options and information.
 
 
 ## Tests
```

### Comparing `atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/PKG-INFO` & `atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -71,14 +71,16 @@
 ```
 
 Both the `--tagger` and `--fx` options accept a list if you want to get the WPs for multiple taggers.
 
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
+If instead of defining the working points for a series of signal efficiencies, you wish to calculate a WP corresponding to a specific background rejection, the `--rejection` option can be given along with the desired background.
+
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
 Use `--help` for more options and information.
 
 
 ## Tests
```

### Comparing `atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/SOURCES.txt` & `atlas-ftag-tools-0.1.2/atlas_ftag_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/__init__.py` & `atlas-ftag-tools-0.1.2/ftag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """atlas-ftag-tools - Common tools for ATLAS flavour tagging software."""
 
 
-__version__ = "v0.1.1"
+__version__ = "v0.1.2"
 
 
 import ftag.hdf5 as hdf5
 from ftag.cuts import Cuts
 from ftag.flavour import Flavour, Flavours
 from ftag.mock import get_mock_file
 from ftag.sample import Sample
```

### Comparing `atlas-ftag-tools-0.1.1/ftag/cuts.py` & `atlas-ftag-tools-0.1.2/ftag/cuts.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/flavour.py` & `atlas-ftag-tools-0.1.2/ftag/flavour.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/flavours.yaml` & `atlas-ftag-tools-0.1.2/ftag/flavours.yaml`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/hdf5/h5reader.py` & `atlas-ftag-tools-0.1.2/ftag/hdf5/h5reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,16 +212,17 @@
                     samples.append(next(stream))
                 except StopIteration:
                     return
 
             # combine samples and shuffle
             data = {name: np.concatenate([s[name] for s in samples]) for name in variables}
             if self.shuffle:
-                for name in variables:
-                    rng.shuffle(data[name])
+                idx = np.arange(len(data[self.jets_name]))
+                rng.shuffle(idx)
+                data = {name: array[idx] for name, array in data.items()}
 
             # select
             yield data
 
     def load(
         self, variables: dict | None = None, num_jets: int | None = None, cuts: Cuts | None = None
     ) -> dict:
```

### Comparing `atlas-ftag-tools-0.1.1/ftag/hdf5/h5utils.py` & `atlas-ftag-tools-0.1.2/ftag/hdf5/h5utils.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/hdf5/h5writer.py` & `atlas-ftag-tools-0.1.2/ftag/hdf5/h5writer.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/mock.py` & `atlas-ftag-tools-0.1.2/ftag/mock.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/sample.py` & `atlas-ftag-tools-0.1.2/ftag/sample.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/vds.py` & `atlas-ftag-tools-0.1.2/ftag/vds.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.1/ftag/wps/discriminant.py` & `atlas-ftag-tools-0.1.2/ftag/wps/discriminant.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def ctag_discriminant(pb, pc, pu, fb=0.2, epsilon=1e-10):
     return np.log((pc + epsilon) / ((1.0 - fb) * pu + fb * pb + epsilon))
 
 
 def get_discriminant(
-    jets: np.ndarray, tagger: str, signal: Flavour, fx: float, epsilon: float = 1e-10
+    jets: np.ndarray, tagger: str, signal: Flavour | str, fx: float, epsilon: float = 1e-10
 ):
     """Calculate the b-tag or c-tag discriminant for a given tagger.
 
     Parameters
     ----------
     jets : np.ndarray
         Structured array of jets containing tagger outputs
```

### Comparing `atlas-ftag-tools-0.1.1/ftag/wps/working_points.py` & `atlas-ftag-tools-0.1.2/ftag/wps/working_points.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         help="path to zprime (supports globbing). WPs from ttbar will be reused for zprime",
     )
     parser.add_argument(
         "-e",
         "--effs",
         nargs="+",
         type=float,
-        help="efficiency working point(s)",
+        help="efficiency working point(s). If -r is specified, values should be 1/efficiency",
         default=[60, 70, 77, 85],
     )
     parser.add_argument(
         "-t",
         "--tagger",
         nargs="+",
         required=True,
@@ -57,14 +57,21 @@
         "--signal",
         default="bjets",
         choices=["bjets", "cjets"],
         type=str,
         help='signal flavour ("bjets" or "cjets")',
     )
     parser.add_argument(
+        "-r",
+        "--rejection",
+        default=None,
+        choices=["ujets", "cjets", "bjets"],
+        help="use rejection of specified background class to determine working points",
+    )
+    parser.add_argument(
         "-n",
         "--num_jets",
         default=1_000_000,
         type=int,
         help="use this many jets (post selection)",
     )
     parser.add_argument(
@@ -125,23 +132,27 @@
 
     # loop over taggers
     out = {}
     for tagger, fx in zip(args.tagger, args.fx):
         out[tagger] = {"signal": args.signal, "fx": fx}
 
         # calculate discriminant
-        disc = get_discriminant(jets, tagger, Flavours[args.signal], fx)
-        sig_disc = disc[flavs[args.signal].cuts(jets).idx]
+        disc = get_discriminant(jets, tagger, args.signal, fx)
 
         # loop over efficiency working points
         for eff in args.effs:
             d = out[tagger][f"{eff:.0f}"] = {}
 
-            # calculate working point
-            wp = d["cut_value"] = round(float(np.percentile(sig_disc, 100 - eff)), 3)
+            wp_flavour = args.signal
+            if args.rejection:
+                eff = 100 / eff
+                wp_flavour = args.rejection
+
+            wp_disc = disc[flavs[wp_flavour].cuts(jets).idx]
+            wp = d["cut_value"] = round(float(np.percentile(wp_disc, 100 - eff)), 3)
 
             # calculate eff and rej for each flavour
             d["ttbar"] = get_eff_rej(jets, disc, wp, flavs)
 
             # calculate for zprime
             if args.zprime:
                 zp_disc = get_discriminant(zp_jets, tagger, Flavours[args.signal], fx)
```

### Comparing `atlas-ftag-tools-0.1.1/pyproject.toml` & `atlas-ftag-tools-0.1.2/pyproject.toml`

 * *Files identical despite different names*

