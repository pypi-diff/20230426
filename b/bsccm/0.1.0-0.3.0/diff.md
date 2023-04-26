# Comparing `tmp/bsccm-0.1.0.tar.gz` & `tmp/bsccm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsccm-0.1.0.tar", last modified: Thu Mar 31 18:28:49 2022, max compression
+gzip compressed data, was "bsccm-0.3.0.tar", last modified: Wed Apr 26 18:00:08 2023, max compression
```

## Comparing `bsccm-0.1.0.tar` & `bsccm-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hpinkard_waller  (1002) hpinkard_waller  (1002)        0 2022-03-31 18:28:49.923201 bsccm-0.1.0/
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)     1507 2022-03-31 17:31:22.000000 bsccm-0.1.0/LICENSE
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)      696 2022-03-31 18:28:49.919201 bsccm-0.1.0/PKG-INFO
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)        0 2022-03-31 17:59:38.000000 bsccm-0.1.0/README.md
-drwxrwxr-x   0 hpinkard_waller  (1002) hpinkard_waller  (1002)        0 2022-03-31 18:28:49.919201 bsccm-0.1.0/bsccm/
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)      129 2022-03-31 17:31:22.000000 bsccm-0.1.0/bsccm/__init__.py
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)       71 2022-03-31 18:26:24.000000 bsccm-0.1.0/bsccm/_version.py
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)     6437 2022-03-31 18:21:02.000000 bsccm-0.1.0/bsccm/bsccm.py
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)     6091 2021-08-27 17:05:19.000000 bsccm-0.1.0/bsccm/led_array_calibration.py
-drwxrwxr-x   0 hpinkard_waller  (1002) hpinkard_waller  (1002)        0 2022-03-31 18:28:49.919201 bsccm-0.1.0/bsccm.egg-info/
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)      696 2022-03-31 18:28:49.000000 bsccm-0.1.0/bsccm.egg-info/PKG-INFO
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)      252 2022-03-31 18:28:49.000000 bsccm-0.1.0/bsccm.egg-info/SOURCES.txt
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)        1 2022-03-31 18:28:49.000000 bsccm-0.1.0/bsccm.egg-info/dependency_links.txt
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)       18 2022-03-31 18:28:49.000000 bsccm-0.1.0/bsccm.egg-info/requires.txt
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)        6 2022-03-31 18:28:49.000000 bsccm-0.1.0/bsccm.egg-info/top_level.txt
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)       38 2022-03-31 18:28:49.923201 bsccm-0.1.0/setup.cfg
--rw-rw-r--   0 hpinkard_waller  (1002) hpinkard_waller  (1002)     1175 2022-03-31 18:27:37.000000 bsccm-0.1.0/setup.py
+drwxr-xr-x   0 henrypinkard   (501) staff       (20)        0 2023-04-26 18:00:08.217596 bsccm-0.3.0/
+-rw-------   0 henrypinkard   (501) staff       (20)     1507 2022-04-08 16:52:16.000000 bsccm-0.3.0/LICENSE
+-rw-r--r--   0 henrypinkard   (501) staff       (20)      657 2023-04-26 18:00:08.217392 bsccm-0.3.0/PKG-INFO
+-rw-------   0 henrypinkard   (501) staff       (20)        5 2022-04-08 16:52:14.000000 bsccm-0.3.0/README.md
+drwxr-xr-x   0 henrypinkard   (501) staff       (20)        0 2023-04-26 18:00:08.216648 bsccm-0.3.0/bsccm/
+-rw-------   0 henrypinkard   (501) staff       (20)      272 2022-04-08 16:51:38.000000 bsccm-0.3.0/bsccm/__init__.py
+-rw-r--r--   0 henrypinkard   (501) staff       (20)       72 2023-04-25 20:31:03.000000 bsccm-0.3.0/bsccm/_version.py
+-rw-r--r--   0 henrypinkard   (501) staff       (20)     9467 2023-04-25 20:31:03.000000 bsccm-0.3.0/bsccm/bsccm.py
+-rw-r--r--   0 henrypinkard   (501) staff       (20)     6633 2023-04-25 20:31:03.000000 bsccm-0.3.0/bsccm/led_array_calibration.py
+drwxr-xr-x   0 henrypinkard   (501) staff       (20)        0 2023-04-26 18:00:08.217212 bsccm-0.3.0/bsccm.egg-info/
+-rw-------   0 henrypinkard   (501) staff       (20)      657 2023-04-26 18:00:08.000000 bsccm-0.3.0/bsccm.egg-info/PKG-INFO
+-rw-------   0 henrypinkard   (501) staff       (20)      252 2023-04-26 18:00:08.000000 bsccm-0.3.0/bsccm.egg-info/SOURCES.txt
+-rw-------   0 henrypinkard   (501) staff       (20)        1 2023-04-26 18:00:08.000000 bsccm-0.3.0/bsccm.egg-info/dependency_links.txt
+-rw-------   0 henrypinkard   (501) staff       (20)       27 2023-04-26 18:00:08.000000 bsccm-0.3.0/bsccm.egg-info/requires.txt
+-rw-------   0 henrypinkard   (501) staff       (20)        6 2023-04-26 18:00:08.000000 bsccm-0.3.0/bsccm.egg-info/top_level.txt
+-rw-r--r--   0 henrypinkard   (501) staff       (20)       38 2023-04-26 18:00:08.217640 bsccm-0.3.0/setup.cfg
+-rw-------   0 henrypinkard   (501) staff       (20)     1195 2022-04-08 16:51:43.000000 bsccm-0.3.0/setup.py
```

### Comparing `bsccm-0.1.0/LICENSE` & `bsccm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsccm-0.1.0/bsccm/led_array_calibration.py` & `bsccm-0.3.0/bsccm/led_array_calibration.py`

 * *Files 14% similar despite different names*

```diff
@@ -81,41 +81,51 @@
 
 def get_led_angle(led_index):
     source_list_na, source_list_cart = load_led_positions_from_json(os.path.dirname(__file__) + '/quasi_dome_design.json')
     angles_xy = np.arcsin(np.abs(source_list_na))
     angle = np.arctan(np.sqrt(np.tan(angles_xy[:, 0])**2 + np.tan(angles_xy[:, 1])**2 ))
     return angle[led_index - 1] / (2*3.14) *360
 
-def plot_led_pattern(led_indices=None, channel_name=None, ax=None, legend=True, size=20):
+def plot_led_pattern(led_indices=None, channel_name=None, ax=None, legend=True, shorten_na_labels=False):
     """
     Make a plot of the the illumination pattern in NA space
     """
+    def normalize_marker_sizes(ax, marker_size):
+        bbox = ax.get_window_extent().transformed(ax.figure.dpi_scale_trans.inverted())
+        width, height = bbox.width, bbox.height
+        scaling_factor = (width * height)
+        return marker_size * scaling_factor
+    
+    size = normalize_marker_sizes(ax, 2.3)
+
     if channel_name is None and led_indices is None:
         raise Exception('Must supply either channel_name or led_indices')
     if channel_name is not None and led_indices is not None:
         raise Exception('Must supply only channel_name or led_indices')
     if channel_name is not None:
         led_indices = illumination_to_led_indices(channel_name)
 
     if ax is None:
         ax = plt.gca()
     all_led_list = np.array([get_led_na_xy(led) for led in range(1, 582)])
-    ax.scatter(all_led_list[:,0], all_led_list[:,1], size, marker=',', color=[0.15,0.15,0.15], 
-                facecolor=None,edgecolor=None, edgecolors=None)
+    ax.scatter(all_led_list[:,0], all_led_list[:,1], size, marker='o', color=[0.15,0.15,0.15], 
+                facecolor=None,edgecolor=None, edgecolors=None, label='Off')
     ax.set_facecolor([0,0,0])
     
     for led_index in led_indices:
         nax, nay = get_led_na_xy(led_index) 
-        ax.scatter(nax, nay, size, marker='s', color=[0,1.0,0], 
-                    facecolor=None, edgecolor=None, edgecolors=None)
-    ax.add_patch(plt.Circle((0, 0), 0.5, alpha=0.25))
-    ax.set_xlabel('Numerical aperture (x)')
-    ax.set_ylabel('Numerical aperture (y)')
+        ax.scatter(nax, nay, size, marker='o', color=[0,1.0,0], 
+                    facecolor=None, edgecolor=None, edgecolors=None, label='On' if led_index == led_indices[0] else None)
+    ax.add_patch(plt.Circle((0, 0), 0.5, alpha=0.25, label='Brightfield LEDs'))
+    ax.set_xlabel('Numerical aperture (x)' if not shorten_na_labels else 'NA (x)')
+    ax.set_ylabel('Numerical aperture (y)' if not shorten_na_labels else 'NA (y)')
+    ax.set(xticks=[-1, 0, 1], yticks=[-1, 0, 1])
+    ax.set_aspect('equal')
     if legend:
-        plt.legend(['Brightfield LEDs','LED off','LED on'])
+        ax.legend()
 
 
 def illumination_to_led_indices(channel):
     """
     Compute a channel name to a list of LED indices. LED indices are 1-based
     """
     if channel == 'LED119':
```

### Comparing `bsccm-0.1.0/setup.py` & `bsccm-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henrypinkard/BSCCM",
     packages=setuptools.find_packages(),
     install_requires=[
         "numpy",
         "pandas",
-        "zarr"
+        "zarr",
+        "requests"
     ],
     python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

