# Comparing `tmp/spectralib-0.0.5.tar.gz` & `tmp/spectralib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralib-0.0.5.tar", last modified: Wed Apr 26 13:30:18 2023, max compression
+gzip compressed data, was "spectralib-0.0.6.tar", last modified: Wed Apr 26 19:40:08 2023, max compression
```

## Comparing `spectralib-0.0.5.tar` & `spectralib-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:58.281542 spectralib-0.0.5/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 15:23:58.277542 spectralib-0.0.5/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1307 2023-04-26 15:22:41.000000 spectralib-0.0.5/README.md
--rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 15:23:58.282545 spectralib-0.0.5/setup.cfg
--rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 12:14:25.000000 spectralib-0.0.5/setup.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:57.705672 spectralib-0.0.5/src/
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:57.895167 spectralib-0.0.5/src/spectralib/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.5/src/spectralib/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.5/src/spectralib/filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.5/src/spectralib/frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3683 2023-04-26 10:33:33.000000 spectralib-0.0.5/src/spectralib/pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.5/src/spectralib/rfi.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:58.030655 spectralib-0.0.5/src/spectralib.egg-info/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/SOURCES.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/dependency_links.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 15:23:57.000000 spectralib-0.0.5/src/spectralib.egg-info/top_level.txt
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 15:23:58.238531 spectralib-0.0.5/src/tests/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.5/src/tests/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.5/src/tests/benchmark.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.5/src/tests/test_filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.5/src/tests/test_frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2087 2023-04-26 10:38:51.000000 spectralib-0.0.5/src/tests/test_pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.5/src/tests/test_rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:08.285123 spectralib-0.0.6/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:40:08.280700 spectralib-0.0.6/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1611 2023-04-26 19:07:37.000000 spectralib-0.0.6/README.md
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 19:40:08.286134 spectralib-0.0.6/setup.cfg
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 19:39:56.000000 spectralib-0.0.6/setup.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:07.742779 spectralib-0.0.6/src/
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:07.927101 spectralib-0.0.6/src/spectralib/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.6/src/spectralib/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.6/src/spectralib/filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.6/src/spectralib/frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3690 2023-04-26 19:36:51.000000 spectralib-0.0.6/src/spectralib/pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.6/src/spectralib/rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:08.051683 spectralib-0.0.6/src/spectralib.egg-info/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/top_level.txt
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:08.244521 spectralib-0.0.6/src/tests/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.6/src/tests/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.6/src/tests/benchmark.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.6/src/tests/test_filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.6/src/tests/test_frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2087 2023-04-26 10:38:51.000000 spectralib-0.0.6/src/tests/test_pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.6/src/tests/test_rfi.py
```

### Comparing `spectralib-0.0.5/PKG-INFO` & `spectralib-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.5/README.md` & `spectralib-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 
 SPECTRALib is a 100% python library with minimal dependencies (`numpy` and `matplotlib`) for handling filterbank files and generating synthetic transients such as pulsars and FRBs, mixed with RFI and other effects.
 
 SPECTRALib stands for Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library.
 
 ### Feel free to use the code however you wish:
  - You can `import spectralib` and use the functions in your code
- - You can modify the [**example scripts**](https://github.com/jack-white1/SPECTRALib_examples) to generate files that fit your requirement
+ - You can modify the [**example scripts**](https://github.com/jack-white1/SPECTRALib/examples) to generate files that fit your requirement
  - The functions should be modular enough to **copy and paste** into your own code
 
 ### Citation
 If you use SPECTRALib to contribute to a publication, please cite:
 ___Paper that you can cite___
 
 # Installation
 
 `pip install spectralib`
 
-# Usage
-Once you have installed SPECTRALib with `pip install spectralib`, please test the installation with the built-in tests:
-
-Now you have confirmed the installation is functional, run the example scripts:
-
 # RFI Example
 ![Animation showing RFI creation process](/images/rfi.gif)
 
 # FRB Example
 ![Example of FRB created with spectralib](/images/frb.png)
 
 # Pulsar Example
-![Example of pulsar created with spectralib](/images/pulsar.png)
+![Example of pulsar created with spectralib](/images/pulsar.png)
+
+# Usage
+Once you have installed SPECTRALib with `pip install spectralib`, you can import the library into your python code with `import spectralib`.
+
+To test the library, download and run the examples by cloning this git repo.
+
+ - `git clone https://github.com/jack-white1/SPECTRALib`
+ - `cd SPECTRALib/examples`
+ - `python example_rfi.py` or `python3 example_rfi.py`
+ - `python example_frb.py` or `python3 example_frb.py`
+ - `python example_pulsar.py` or `python3 example_pulsar.py`
+
+ # Documentation
+
```

### Comparing `spectralib-0.0.5/setup.py` & `spectralib-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="spectralib",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     classifiers=[
         "Development Status :: 1 - Planning",
     ],
     author="Jack White",
     author_email="jack.white@eng.ox.ac.uk",
```

### Comparing `spectralib-0.0.5/src/spectralib/filterbank.py` & `spectralib-0.0.6/src/spectralib/filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/spectralib/frb.py` & `spectralib-0.0.6/src/spectralib/frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/spectralib/pulsar.py` & `spectralib-0.0.6/src/spectralib/pulsar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from spectralib.frb import generate_frb, calculate_dispersion_offsets
 import numpy as np
 
-def apparent_pulse_period(binary_params, p_rest, time):
+def apparent_pulse_period(binary_params, time):
     # heavily influenced by sigproc's fake, Duncan Lorimer, and Mike Keith's implementation in C
     G = 6.67430e-11
     M_SUN = 1.9885e30
     SPEED_OF_LIGHT = 299792458
 
+    rest_period = binary_params["rest_period"]
     inclination = binary_params["inclination"]
     orbital_period = binary_params["orbital_period"]
     start_phase = binary_params["start_phase"]
     mass_companion = binary_params["companion_mass"]
     mass_pulsar = binary_params["pulsar_mass"]
     eccentricity = binary_params["eccentricity"]
     omega = binary_params["omega"]
@@ -27,53 +28,52 @@
         e_next = eccentric_anomaly - (eccentric_anomaly - eccentricity * np.sin(eccentric_anomaly) - mean_anomaly) / (1 - eccentricity * np.cos(eccentric_anomaly))
         if abs(e_next - eccentric_anomaly) < 1e-10:
             break
         eccentric_anomaly = e_next
 
     true_anomaly = 2 * np.arctan(np.sqrt((1 + eccentricity) / (1 - eccentricity)) * np.tan(eccentric_anomaly / 2))
     velocity = omega_b * asini / np.sqrt(1 - eccentricity**2) * (np.cos(omega + true_anomaly) + eccentricity * np.cos(omega))
-    p_apparent = p_rest * (1 + velocity / SPEED_OF_LIGHT)
+    p_apparent = rest_period * (1 + velocity / SPEED_OF_LIGHT)
 
     return p_apparent
 
-def generate_binary_pulsar(data, DM, tsamp, foff, fch1, p_rest, binary_params, **frb_params):
+def generate_binary_pulsar(data, DM, tsamp, foff, fch1, binary_params, **frb_params):
     nchans, nsamp = data.shape
-    pulse_duration = frb_params.get("frb_duration", 100)
-
+    
     # Use calculate_dispersion_offsets from frb.py to calculate the maximum offset, and subtract it from 0 to get the start index
     # this ensures the pulsar signal is present in the entire data array
     offsets = calculate_dispersion_offsets(DM, fch1, foff, nchans, tsamp)
     start_index = -max(offsets)
 
     pulse = 0
     pulse_start_time = start_index*tsamp
     while pulse_start_time < nsamp*tsamp:
-        pulse_start_time = start_index*tsamp + pulse * p_rest
-        app_pulse_period = apparent_pulse_period(binary_params, p_rest, pulse_start_time)
+        pulse_start_time = start_index*tsamp + pulse * binary_params["rest_period"]
+        app_pulse_period = apparent_pulse_period(binary_params, pulse_start_time)
         print("At time : ",pulse_start_time," apparent pulse period: ", app_pulse_period)
         frb_start_time = pulse_start_time + app_pulse_period
         frb_start_index = int(frb_start_time / tsamp)
 
         data = generate_frb(data, DM, tsamp, foff, fch1, frb_start_index=frb_start_index, **frb_params)
         pulse+=1
 
     return data
 
-def generate_solitary_pulsar(data, DM, tsamp, foff, fch1, p_rest, **frb_params):
+def generate_solitary_pulsar(data, DM, tsamp, foff, fch1, rest_period, **frb_params):
     nchans, nsamp = data.shape
     pulse_duration = frb_params.get("frb_duration", 100)
 
 
     # Use calculate_dispersion_offsets from frb.py to calculate the maximum offset, and subtract it from 0 to get the start index
     # this ensures the pulsar signal is present in the entire data array, rather than missing from the bottom left corner
     offsets = calculate_dispersion_offsets(DM, fch1, foff, nchans, tsamp)
     start_index = -max(offsets)
     pulse = 0
     pulse_start_time = start_index*tsamp
     while pulse_start_time < nsamp*tsamp:
-        pulse_start_time = start_index*tsamp + pulse * p_rest
+        pulse_start_time = start_index*tsamp + pulse * rest_period
         frb_start_index = int(pulse_start_time / tsamp)
 
         data = generate_frb(data, DM, tsamp, foff, fch1, frb_start_index=frb_start_index, frb_duration=pulse_duration, **frb_params)
         pulse+=1
 
     return data
```

### Comparing `spectralib-0.0.5/src/spectralib/rfi.py` & `spectralib-0.0.6/src/spectralib/rfi.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/spectralib.egg-info/PKG-INFO` & `spectralib-0.0.6/src/spectralib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.5/src/tests/benchmark.py` & `spectralib-0.0.6/src/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/tests/test_filterbank.py` & `spectralib-0.0.6/src/tests/test_filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/tests/test_frb.py` & `spectralib-0.0.6/src/tests/test_frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/tests/test_pulsar.py` & `spectralib-0.0.6/src/tests/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.5/src/tests/test_rfi.py` & `spectralib-0.0.6/src/tests/test_rfi.py`

 * *Files identical despite different names*

