# Comparing `tmp/nembem-0.1.tar.gz` & `tmp/nembem-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nembem-0.1.tar", last modified: Tue Apr 25 13:27:03 2023, max compression
+gzip compressed data, was "nembem-0.2.tar", last modified: Tue Apr 25 14:29:38 2023, max compression
```

## Comparing `nembem-0.1.tar` & `nembem-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:27:03.596090 nembem-0.1/
--rw-rw-rw-   0        0        0     1111 2023-03-14 13:19:32.000000 nembem-0.1/LICENSE
--rw-rw-rw-   0        0        0      168 2023-04-25 13:27:03.595091 nembem-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3189 2023-04-25 13:07:52.000000 nembem-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 13:27:03.571089 nembem-0.1/nembem/
--rw-rw-rw-   0        0        0        0 2023-03-21 10:34:30.000000 nembem-0.1/nembem/__init__.py
--rw-rw-rw-   0        0        0    34080 2023-04-25 13:07:52.000000 nembem-0.1/nembem/dtu_10_mw_class.py
--rw-rw-rw-   0        0        0     3301 2023-04-25 11:38:01.000000 nembem-0.1/nembem/test_turbulence.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:27:03.593091 nembem-0.1/nembem.egg-info/
--rw-rw-rw-   0        0        0      168 2023-04-25 13:27:02.000000 nembem-0.1/nembem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-25 13:27:03.000000 nembem-0.1/nembem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:27:02.000000 nembem-0.1/nembem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-25 13:27:02.000000 nembem-0.1/nembem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 13:27:03.596090 nembem-0.1/setup.cfg
--rw-rw-rw-   0        0        0      428 2023-04-25 13:25:39.000000 nembem-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:29:38.974222 nembem-0.2/
+-rw-rw-rw-   0        0        0     1111 2023-03-14 13:19:32.000000 nembem-0.2/LICENSE
+-rw-rw-rw-   0        0        0      168 2023-04-25 14:29:38.973222 nembem-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3189 2023-04-25 13:07:52.000000 nembem-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 14:29:38.963325 nembem-0.2/nembem/
+-rw-rw-rw-   0        0        0        0 2023-03-21 10:34:30.000000 nembem-0.2/nembem/__init__.py
+-rw-rw-rw-   0        0        0    34039 2023-04-25 14:27:40.000000 nembem-0.2/nembem/dtu_10_mw_class.py
+-rw-rw-rw-   0        0        0     3301 2023-04-25 11:38:01.000000 nembem-0.2/nembem/test_turbulence.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:29:38.972294 nembem-0.2/nembem.egg-info/
+-rw-rw-rw-   0        0        0      168 2023-04-25 14:29:38.000000 nembem-0.2/nembem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-25 14:29:38.000000 nembem-0.2/nembem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 14:29:38.000000 nembem-0.2/nembem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 14:29:38.000000 nembem-0.2/nembem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 14:29:38.975228 nembem-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-04-25 14:29:31.000000 nembem-0.2/setup.py
```

### Comparing `nembem-0.1/LICENSE` & `nembem-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nembem-0.1/README.md` & `nembem-0.2/README.md`

 * *Files identical despite different names*

### Comparing `nembem-0.1/nembem/dtu_10_mw_class.py` & `nembem-0.2/nembem/dtu_10_mw_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,33 +155,33 @@
         theta_tilt = 0 # rad
         lam_opt = 8 # Optimal tip speed ratio
         C_p_opt = 0.47 # Optimal power coefficient
         rho = 1.225 # kg/m^3
         k_dwf = 0.6 # Dynamic wake filter constant
         
         # Roughness length
-        z_0 = 0.9 # m
+        z_0 = 0.5 # m
         # z_0 = 0 # m
         
         # If the roughness length is larger than zero,
         # turbulence is included in the calculations.
         if z_0 > 0:
             # Defining dimensions of the turbulence box
             n1, n2, n3 = 4096, 32, 32
             Lx, Ly, Lz = 6142.5, 180, 180
             
             # Writing turbulence input file
             write_mann_input(n1, n2, n3, Lx, Ly, Lz, self.H, z_0, V_0)
             
             # Run turbulence simulation
-            subprocess.run(['input/turbulence/windsimu.exe',
-                             'input/turbulence/inputEx3.INP'])
+            subprocess.run(['turbulence/windsimu.exe',
+                             'turbulence/input.INP'])
             
             # Load turbulence data
-            turb = load_turb_box('input/turbulence/sim1.bin')
+            turb = load_turb_box('sim1.bin')
             
             # Reshape turbulence data to fit the relevant dimensions
             turb = np.reshape(turb, (n1, n2, n3))
             
             print(turb[0, 0, 0:10])
             
             # Defining the delta values (spacing between points)
@@ -810,15 +810,15 @@
             '0', # Spectrum type
             '-5', # Seed
             'sim1.bin', # Wind speed fluctuations in flow [m/s]
             'sim2.bin', # Wind speed fluctuations in horizontal [m/s]
             'sim3.bin'] # Wind speed fluctuations [m/s]
 
     # Write input parameters to file
-    with open('input/turbulence/inputEx3.INP', 'w') as f:
+    with open('turbulence/input.INP', 'w') as f:
         f.write('\n'.join(lines))
     
     return
     
 
 
 def load_turb_box(filename, N=(32, 32)):
```

### Comparing `nembem-0.1/nembem/test_turbulence.py` & `nembem-0.2/nembem/test_turbulence.py`

 * *Files identical despite different names*

