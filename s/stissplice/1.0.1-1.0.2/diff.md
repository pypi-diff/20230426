# Comparing `tmp/stissplice-1.0.1.tar.gz` & `tmp/stissplice-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stissplice-1.0.1.tar", last modified: Tue Apr 25 14:10:32 2023, max compression
+gzip compressed data, was "stissplice-1.0.2.tar", last modified: Tue Apr 25 14:43:44 2023, max compression
```

## Comparing `stissplice-1.0.1.tar` & `stissplice-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:10:32.486074 stissplice-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-25 14:10:20.000000 stissplice-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:10:32.486074 stissplice-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 14:10:20.000000 stissplice-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:10:32.486074 stissplice-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-25 14:10:20.000000 stissplice-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:10:32.486074 stissplice-1.0.1/stissplice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:10:20.000000 stissplice-1.0.1/stissplice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32262 2023-04-25 14:10:20.000000 stissplice-1.0.1/stissplice/splicer.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 14:10:20.000000 stissplice-1.0.1/stissplice/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:10:32.486074 stissplice-1.0.1/stissplice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:10:32.000000 stissplice-1.0.1/stissplice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 14:10:32.000000 stissplice-1.0.1/stissplice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:10:32.000000 stissplice-1.0.1/stissplice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:10:32.000000 stissplice-1.0.1/stissplice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 14:10:32.000000 stissplice-1.0.1/stissplice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:44.699745 stissplice-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-25 14:43:33.000000 stissplice-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:43:44.699745 stissplice-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 14:43:33.000000 stissplice-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:43:44.699745 stissplice-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-25 14:43:33.000000 stissplice-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:44.699745 stissplice-1.0.2/stissplice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:33.000000 stissplice-1.0.2/stissplice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32299 2023-04-25 14:43:33.000000 stissplice-1.0.2/stissplice/splicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 14:43:33.000000 stissplice-1.0.2/stissplice/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:44.699745 stissplice-1.0.2/stissplice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/top_level.txt
```

### Comparing `stissplice-1.0.1/LICENSE` & `stissplice-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.1/PKG-INFO` & `stissplice-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stissplice
-Version: 1.0.1
+Version: 1.0.2
 Summary: Splicer of STIS Echelle Spectra from Hubble Space Telescope
 Home-page: https://github.com/ladsantos/stissplice
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stissplice-1.0.1/README.md` & `stissplice-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.1/setup.py` & `stissplice-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist upload")
     sys.exit()
 
 setup(
     name="stissplice",
-    version="1.0.1",
+    version="1.0.2",
     author="Leonardo dos Santos",
     author_email="ldsantos@stsci.edu",
     packages=["stissplice"],
     url="https://github.com/ladsantos/stissplice",
     license="MIT",
     description="Splicer of STIS Echelle Spectra from Hubble Space Telescope",
     install_requires=[line.strip() for line in
```

### Comparing `stissplice-1.0.1/stissplice/splicer.py` & `stissplice-1.0.2/stissplice/splicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,22 +515,22 @@
     -------
     overlap_merged (``dict``):
         Dictionary containing the merged overlapping spectrum.
     """
     n_overlaps = len(overlap_sections)
     bitwise_or_acceptable_dq_flags = reduce(np.bitwise_or, acceptable_dq_flags)
 
-    # First we need to determine which spectrum has a higher SNR
-    avg_snr = np.array([np.mean(ok['flux'] / ok['uncertainty'])
-                        for ok in overlap_sections])
+    # First we need to determine which spectrum has a higher sensitivity
+    avg_sensitivity = np.array([np.nanmean(ok['net'] / ok['flux'])
+                                for ok in overlap_sections])
 
     # We interpolate the lower-SNR spectra to the wavelength bins of the higher
     # SNR spectrum.
-    min_snr_idx = np.where(avg_snr == max(avg_snr))[0][0]
-    overlap_ref = overlap_sections.pop(min_snr_idx)
+    max_sens_idx = np.where(avg_sensitivity == max(avg_sensitivity))[0][0]
+    overlap_ref = overlap_sections.pop(max_sens_idx)
 
     f_interp = []
     err_interp = []
     net_interp = []
     for i in range(n_overlaps - 1):
         # Since we cannot really interpolate DQ flags, before we do the
         # interpolation, we need to identify the pixels where
```

### Comparing `stissplice-1.0.1/stissplice/tools.py` & `stissplice-1.0.2/stissplice/tools.py`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.1/stissplice.egg-info/PKG-INFO` & `stissplice-1.0.2/stissplice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stissplice
-Version: 1.0.1
+Version: 1.0.2
 Summary: Splicer of STIS Echelle Spectra from Hubble Space Telescope
 Home-page: https://github.com/ladsantos/stissplice
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

