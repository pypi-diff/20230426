# Comparing `tmp/spectralib-0.0.6.tar.gz` & `tmp/spectralib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralib-0.0.6.tar", last modified: Wed Apr 26 19:40:08 2023, max compression
+gzip compressed data, was "spectralib-0.0.7.tar", last modified: Wed Apr 26 19:49:45 2023, max compression
```

## Comparing `spectralib-0.0.6.tar` & `spectralib-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:08.285123 spectralib-0.0.6/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:40:08.280700 spectralib-0.0.6/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1611 2023-04-26 19:07:37.000000 spectralib-0.0.6/README.md
--rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 19:40:08.286134 spectralib-0.0.6/setup.cfg
--rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 19:39:56.000000 spectralib-0.0.6/setup.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:07.742779 spectralib-0.0.6/src/
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:07.927101 spectralib-0.0.6/src/spectralib/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.6/src/spectralib/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.6/src/spectralib/filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.6/src/spectralib/frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3690 2023-04-26 19:36:51.000000 spectralib-0.0.6/src/spectralib/pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.6/src/spectralib/rfi.py
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:08.051683 spectralib-0.0.6/src/spectralib.egg-info/
--rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/PKG-INFO
--rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/SOURCES.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/dependency_links.txt
--rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 19:40:07.000000 spectralib-0.0.6/src/spectralib.egg-info/top_level.txt
-drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:40:08.244521 spectralib-0.0.6/src/tests/
--rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.6/src/tests/__init__.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.6/src/tests/benchmark.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.6/src/tests/test_filterbank.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.6/src/tests/test_frb.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     2087 2023-04-26 10:38:51.000000 spectralib-0.0.6/src/tests/test_pulsar.py
--rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.6/src/tests/test_rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:49:45.073123 spectralib-0.0.7/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:49:45.067871 spectralib-0.0.7/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1611 2023-04-26 19:07:37.000000 spectralib-0.0.7/README.md
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       38 2023-04-26 19:49:45.074121 spectralib-0.0.7/setup.cfg
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      744 2023-04-26 19:49:39.000000 spectralib-0.0.7/setup.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:49:44.481132 spectralib-0.0.7/src/
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:49:44.685847 spectralib-0.0.7/src/spectralib/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:14.000000 spectralib-0.0.7/src/spectralib/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     6921 2023-04-26 11:05:26.000000 spectralib-0.0.7/src/spectralib/filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3098 2023-04-26 13:08:36.000000 spectralib-0.0.7/src/spectralib/frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3690 2023-04-26 19:46:00.000000 spectralib-0.0.7/src/spectralib/pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     4892 2023-04-26 10:33:46.000000 spectralib-0.0.7/src/spectralib/rfi.py
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:49:44.830019 spectralib-0.0.7/src/spectralib.egg-info/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      580 2023-04-26 19:49:44.000000 spectralib-0.0.7/src/spectralib.egg-info/PKG-INFO
+-rwxrwxrwx   0 jack      (1000) jack      (1000)      438 2023-04-26 19:49:44.000000 spectralib-0.0.7/src/spectralib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        1 2023-04-26 19:49:44.000000 spectralib-0.0.7/src/spectralib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jack      (1000) jack      (1000)       17 2023-04-26 19:49:44.000000 spectralib-0.0.7/src/spectralib.egg-info/top_level.txt
+drwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 19:49:45.029910 spectralib-0.0.7/src/tests/
+-rwxrwxrwx   0 jack      (1000) jack      (1000)        0 2023-04-26 11:50:43.000000 spectralib-0.0.7/src/tests/__init__.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     3942 2023-04-26 10:33:55.000000 spectralib-0.0.7/src/tests/benchmark.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2520 2023-04-26 10:38:37.000000 spectralib-0.0.7/src/tests/test_filterbank.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1161 2023-04-26 10:38:42.000000 spectralib-0.0.7/src/tests/test_frb.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     2103 2023-04-26 19:48:19.000000 spectralib-0.0.7/src/tests/test_pulsar.py
+-rwxrwxrwx   0 jack      (1000) jack      (1000)     1218 2023-04-26 10:38:58.000000 spectralib-0.0.7/src/tests/test_rfi.py
```

### Comparing `spectralib-0.0.6/PKG-INFO` & `spectralib-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.6/README.md` & `spectralib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/setup.py` & `spectralib-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="spectralib",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     classifiers=[
         "Development Status :: 1 - Planning",
     ],
     author="Jack White",
     author_email="jack.white@eng.ox.ac.uk",
```

### Comparing `spectralib-0.0.6/src/spectralib/filterbank.py` & `spectralib-0.0.7/src/spectralib/filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/spectralib/frb.py` & `spectralib-0.0.7/src/spectralib/frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/spectralib/pulsar.py` & `spectralib-0.0.7/src/spectralib/pulsar.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/spectralib/rfi.py` & `spectralib-0.0.7/src/spectralib/rfi.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/spectralib.egg-info/PKG-INFO` & `spectralib-0.0.7/src/spectralib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Synthetic Pulsar Emission, Contamination and Transients Radio Astronomy Library (SPECTRALib)
 Home-page: https://github.com/jack-white1/spectralib
 Author: Jack White
 Author-email: jack.white@eng.ox.ac.uk
 License: UNKNOWN
 Description: A python library for creating synthetic filterbank files (pulsars, FRBs, RFI) for radio astronomy. Integrate functions in your code or use standalone to generate custom datasets.
 Platform: UNKNOWN
```

### Comparing `spectralib-0.0.6/src/tests/benchmark.py` & `spectralib-0.0.7/src/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/tests/test_filterbank.py` & `spectralib-0.0.7/src/tests/test_filterbank.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/tests/test_frb.py` & `spectralib-0.0.7/src/tests/test_frb.py`

 * *Files identical despite different names*

### Comparing `spectralib-0.0.6/src/tests/test_pulsar.py` & `spectralib-0.0.7/src/tests/test_pulsar.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,64 +3,64 @@
 from spectralib.frb import generate_frb, calculate_dispersion_offsets
 from spectralib.pulsar import generate_binary_pulsar, generate_solitary_pulsar, apparent_pulse_period
 
 class TestPulsar(unittest.TestCase):
 
     def test_apparent_pulse_period(self):
         binary_params = {
+            'rest_period': 1,
             'inclination': 0.5,
             'orbital_period': 3600,
             'start_phase': 0,
             'companion_mass': 1.0,
             'pulsar_mass': 1.4,
             'eccentricity': 0.1,
             'omega': 0.3
         }
-        p_rest = 1
         time = 1000
-        p_apparent = apparent_pulse_period(binary_params, p_rest, time)
+        p_apparent = apparent_pulse_period(binary_params, time)
         self.assertIsNotNone(p_apparent)
 
     def test_generate_binary_pulsar(self):
         data = np.zeros((64, 1024), dtype=np.uint8)
         DM = 100
         tsamp = 0.000064
         foff = -0.09765625
         fch1 = 1500
-        p_rest = 100
         binary_params = {
+            'rest_period': 100,
             'inclination': 0.5,
             'orbital_period': 3600,
             'start_phase': 0,
             'companion_mass': 1.0,
             'pulsar_mass': 1.4,
             'eccentricity': 0.1,
             'omega': 0.3
         }
         frb_params = {
             'frb_duration': 10,
             'frb_amplitude': 50
         }
 
-        data_with_pulsar = generate_binary_pulsar(data, DM, tsamp, foff, fch1, p_rest, binary_params, **frb_params)
+        data_with_pulsar = generate_binary_pulsar(data, DM, tsamp, foff, fch1, binary_params, **frb_params)
 
         self.assertIsNotNone(data_with_pulsar)
         self.assertEqual(data_with_pulsar.shape, data.shape)
 
     def test_generate_solitary_pulsar(self):
         data = np.zeros((64, 1024), dtype=np.uint8)
         DM = 100
         tsamp = 0.000064
         foff = -0.09765625
         fch1 = 1500
-        p_rest = 100
+        rest_period = 100
         frb_params = {
             'frb_amplitude': 50
         }
 
-        data_with_pulsar = generate_solitary_pulsar(data, DM, tsamp, foff, fch1, p_rest, **frb_params)
+        data_with_pulsar = generate_solitary_pulsar(data, DM, tsamp, foff, fch1, rest_period, **frb_params)
 
         self.assertIsNotNone(data_with_pulsar)
         self.assertEqual(data_with_pulsar.shape, data.shape)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `spectralib-0.0.6/src/tests/test_rfi.py` & `spectralib-0.0.7/src/tests/test_rfi.py`

 * *Files identical despite different names*

