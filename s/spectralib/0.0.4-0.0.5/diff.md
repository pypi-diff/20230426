# Comparing `tmp/spectralib-0.0.4.tar.gz` & `tmp/spectralib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralib-0.0.4.tar", last modified: Wed Apr 26 11:51:05 2023, max compression
+gzip compressed data, was "spectralib-0.0.5.tar", last modified: Wed Apr 26 13:30:18 2023, max compression
```

## Comparing `spectralib-0.0.4.tar` & `spectralib-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.877972 spectralib-0.0.4/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 11:51:05.873434 spectralib-0.0.4/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1087 2023-04-26 11:24:27.000000 spectralib-0.0.4/README.md
--rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 11:51:05.879487 spectralib-0.0.4/setup.cfg
--rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 11:51:01.000000 spectralib-0.0.4/setup.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.289531 spectralib-0.0.4/src/
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.507487 spectralib-0.0.4/src/spectralib/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.4/src/spectralib/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.4/src/spectralib/filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1398 2023-04-26 10:33:13.000000 spectralib-0.0.4/src/spectralib/frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 10:33:24.000000 spectralib-0.0.4/src/spectralib/main.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3683 2023-04-26 10:33:33.000000 spectralib-0.0.4/src/spectralib/pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.4/src/spectralib/rfi.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.645349 spectralib-0.0.4/src/spectralib.egg-info/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)      461 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/SOURCES.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/dependency_links.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 11:51:05.000000 spectralib-0.0.4/src/spectralib.egg-info/top_level.txt
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:51:05.839183 spectralib-0.0.4/src/tests/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.4/src/tests/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.4/src/tests/benchmark.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.4/src/tests/test_filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.4/src/tests/test_frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2087 2023-04-26 10:38:51.000000 spectralib-0.0.4/src/tests/test_pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.4/src/tests/test_rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:58.281542 spectralib-0.0.5/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 15:23:58.277542 spectralib-0.0.5/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1307 2023-04-26 15:22:41.000000 spectralib-0.0.5/README.md
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 15:23:58.282545 spectralib-0.0.5/setup.cfg
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 12:14:25.000000 spectralib-0.0.5/setup.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:57.705672 spectralib-0.0.5/src/
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:57.895167 spectralib-0.0.5/src/spectralib/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.5/src/spectralib/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.5/src/spectralib/filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.5/src/spectralib/frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3683 2023-04-26 10:33:33.000000 spectralib-0.0.5/src/spectralib/pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.5/src/spectralib/rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:58.030655 spectralib-0.0.5/src/spectralib.egg-info/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/top_level.txt
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:58.238531 spectralib-0.0.5/src/tests/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.5/src/tests/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.5/src/tests/benchmark.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.5/src/tests/test_filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.5/src/tests/test_frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2087 2023-04-26 10:38:51.000000 spectralib-0.0.5/src/tests/test_pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.5/src/tests/test_rfi.py
```

### Comparing `spectralib-0.0.4/PKG-INFO` & `spectralib-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.4/README.md` & `spectralib-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 SPECTRALib is a 100% python library with minimal dependencies (`numpy` and `matplotlib`) for handling filterbank files and generating synthetic transients such as pulsars and FRBs, mixed with RFI and other effects.
 
 SPECTRALib stands for Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library.
 
 ### Feel free to use the code however you wish:
  - You can `import spectralib` and use the functions in your code
- - You can modify the **example scripts** to generate files that fit your requirement
+ - You can modify the [**example scripts**](https://github.com/jack-white1/SPECTRALib_examples) to generate files that fit your requirement
  - The functions should be modular enough to **copy and paste** into your own code
 
 ### Citation
 If you use SPECTRALib to contribute to a publication, please cite:
 ___Paper that you can cite___
 
 # Installation
@@ -18,9 +18,15 @@
 `pip install spectralib`
 
 # Usage
 Once you have installed SPECTRALib with `pip install spectralib`, please test the installation with the built-in tests:
 
 Now you have confirmed the installation is functional, run the example scripts:
 
-# Examples
-![Animation showing RFI creation process](/images/rfi.gif)
+# RFI Example
+![Animation showing RFI creation process](/images/rfi.gif)
+
+# FRB Example
+![Example of FRB created with spectralib](/images/frb.png)
+
+# Pulsar Example
+![Example of pulsar created with spectralib](/images/pulsar.png)
```

### Comparing `spectralib-0.0.4/setup.py` & `spectralib-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="spectralib",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     classifiers=[
         "Development Status :: 1 - Planning",
     ],
     author="Jack White",
     author_email="jack.white@eng.ox.ac.uk",
```

### Comparing `spectralib-0.0.4/src/spectralib/filterbank.py` & `spectralib-0.0.5/src/spectralib/filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/spectralib/frb.py` & `spectralib-0.0.5/src/spectralib/frb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,43 @@
 import numpy as np
 
+def generate_high_res_frb(data, DM, tsamp, foff, fch1, freq_upsample_factor, **frb_params):
+    frb_start_index = frb_params.get('frb_start_index', 0)
+    frb_duration = frb_params.get('frb_duration', 100)
+    frb_amplitude = frb_params.get('frb_amplitude', 200)
+    time_profile = frb_params.get('time_profile', None)
+    freq_profile = frb_params.get('freq_profile', None)
+
+    nchans, nsamp = data.shape
+
+    if time_profile is None:
+        time_profile = np.ones(frb_duration)
+    if freq_profile is None:
+        freq_profile = np.ones(nchans)
+
+    # Interpolate time and frequency profiles
+    time_profile_hr = np.interp(np.linspace(0, frb_duration - 1, frb_duration * freq_upsample_factor),
+                                np.arange(frb_duration), time_profile)
+    freq_profile_hr = np.interp(np.linspace(0, nchans - 1, nchans * freq_upsample_factor),
+                                np.arange(nchans), freq_profile)
+
+    # Calculate high-resolution dispersion offsets
+    foff_hr = foff / freq_upsample_factor
+    fch1_hr = np.array([fch1 + i * foff for i in range(nchans * freq_upsample_factor)])
+    sub_band_offsets = calculate_dispersion_offsets(DM, fch1_hr, foff_hr, nchans * freq_upsample_factor, tsamp)
+
+    for i in range(nchans * freq_upsample_factor):
+        for j in range(frb_duration * freq_upsample_factor):
+            time_index = round((frb_start_index * freq_upsample_factor) + j + sub_band_offsets[i])
+            if 0 <= time_index < nsamp * freq_upsample_factor:
+                data[i // freq_upsample_factor, time_index] += frb_amplitude * time_profile_hr[j] * freq_profile_hr[i]
+
+    data = np.clip(data, 0, 255)
+    return data
+
 def generate_frb(data, DM, tsamp, foff, fch1, **frb_params):
     frb_start_index = frb_params.get('frb_start_index', 0)
     frb_duration = frb_params.get('frb_duration', 100)
     frb_amplitude = frb_params.get('frb_amplitude', 200)
     time_profile = frb_params.get('time_profile', None)
     freq_profile = frb_params.get('freq_profile', None)
```

### Comparing `spectralib-0.0.4/src/spectralib/pulsar.py` & `spectralib-0.0.5/src/spectralib/pulsar.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/spectralib/rfi.py` & `spectralib-0.0.5/src/spectralib/rfi.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/spectralib.egg-info/PKG-INFO` & `spectralib-0.0.5/src/spectralib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.4/src/tests/benchmark.py` & `spectralib-0.0.5/src/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/tests/test_filterbank.py` & `spectralib-0.0.5/src/tests/test_filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/tests/test_frb.py` & `spectralib-0.0.5/src/tests/test_frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/tests/test_pulsar.py` & `spectralib-0.0.5/src/tests/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.4/src/tests/test_rfi.py` & `spectralib-0.0.5/src/tests/test_rfi.py`

 * *Files identical despite different names*

