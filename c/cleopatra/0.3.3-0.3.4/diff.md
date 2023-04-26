# Comparing `tmp/cleopatra-0.3.3.tar.gz` & `tmp/cleopatra-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleopatra-0.3.3.tar", last modified: Tue Apr 25 21:09:40 2023, max compression
+gzip compressed data, was "cleopatra-0.3.4.tar", last modified: Wed Apr 26 21:35:44 2023, max compression
```

## Comparing `cleopatra-0.3.3.tar` & `cleopatra-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.537488 cleopatra-0.3.3/
--rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.3/AUTHORS.rst
--rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.3/LICENSE.md
--rw-rw-rw-   0        0        0     7040 2023-04-25 21:09:40.537488 cleopatra-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5081 2023-04-25 20:03:44.000000 cleopatra-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.514440 cleopatra-0.3.3/cleopatra/
--rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.3/cleopatra/__init__.py
--rw-rw-rw-   0        0        0    37348 2023-04-23 09:44:18.000000 cleopatra-0.3.3/cleopatra/array.py
--rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.3/cleopatra/statistics.py
--rw-rw-rw-   0        0        0     6386 2023-04-25 20:03:44.000000 cleopatra-0.3.3/cleopatra/styles.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.526490 cleopatra-0.3.3/cleopatra.egg-info/
--rw-rw-rw-   0        0        0     7040 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 21:09:40.538663 cleopatra-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1679 2023-04-25 20:39:25.000000 cleopatra-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.534490 cleopatra-0.3.3/tests/
--rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.3/tests/test_plot_array.py
--rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.3/tests/test_statistics.py
--rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.3/tests/test_styles.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:35:44.765971 cleopatra-0.3.4/
+-rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.4/LICENSE.md
+-rw-rw-rw-   0        0        0     7179 2023-04-26 21:35:44.764971 cleopatra-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5081 2023-04-26 21:28:12.000000 cleopatra-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 21:35:44.741757 cleopatra-0.3.4/cleopatra/
+-rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.4/cleopatra/__init__.py
+-rw-rw-rw-   0        0        0    37539 2023-04-26 21:28:12.000000 cleopatra-0.3.4/cleopatra/array.py
+-rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.4/cleopatra/statistics.py
+-rw-rw-rw-   0        0        0     6386 2023-04-25 20:03:44.000000 cleopatra-0.3.4/cleopatra/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:35:44.753459 cleopatra-0.3.4/cleopatra.egg-info/
+-rw-rw-rw-   0        0        0     7179 2023-04-26 21:35:44.000000 cleopatra-0.3.4/cleopatra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-04-26 21:35:44.000000 cleopatra-0.3.4/cleopatra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 21:35:44.000000 cleopatra-0.3.4/cleopatra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-25 21:09:40.000000 cleopatra-0.3.4/cleopatra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2023-04-26 21:35:44.000000 cleopatra-0.3.4/cleopatra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 21:35:44.000000 cleopatra-0.3.4/cleopatra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 21:35:44.765971 cleopatra-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-04-26 21:28:12.000000 cleopatra-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 21:35:44.761971 cleopatra-0.3.4/tests/
+-rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.4/tests/test_plot_array.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.4/tests/test_statistics.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.4/tests/test_styles.py
```

### Comparing `cleopatra-0.3.3/LICENSE.md` & `cleopatra-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.3/PKG-INFO` & `cleopatra-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.3
+Version: 0.3.4
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
 Keywords: matplotlib,visualization
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.3
+pip install cleopatra==0.3.4
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -130,7 +130,11 @@
 0.3.2 (2023-04-23)
 ------------------
 * bump up hpc version
 
 0.3.3 (2023-04-25)
 ------------------
 * change the default value for the color bar label.
+
+0.3.4 (2023-04-26)
+------------------
+* pass the plot kwargs to the init of the array to scale the color bar using the vmin and vmax.
```

### Comparing `cleopatra-0.3.3/README.md` & `cleopatra-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.3
+pip install cleopatra==0.3.4
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
```

### Comparing `cleopatra-0.3.3/cleopatra/__init__.py` & `cleopatra-0.3.4/cleopatra/__init__.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.3/cleopatra/array.py` & `cleopatra-0.3.4/cleopatra/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def __init__(
         self,
         array: np.ndarray,
         exclude_value: List = np.nan,
         rgb: List[int] = None,
         surface_reflectance: int = 10000,
         cutoff: List = None,
+        **kwargs,
     ):
         """Plot array.
 
         Parameters
         ----------
         array: [numpy array]
             array.
@@ -87,29 +88,35 @@
                     surface_reflectance=surface_reflectance,
                     cutoff=cutoff,
                 )
         else:
             self.rgb = False
 
         self._exclude_value = exclude_value
-        self._vmin = np.nanmin(array)
-        self._vmax = np.nanmax(array)
+
+        self._vmax = (
+            np.nanmax(array) if kwargs.get("vmax") is None else kwargs.get("vmax")
+        )
+        self._vmin = (
+            np.nanmin(array) if kwargs.get("vmin") is None else kwargs.get("vmin")
+        )
+
         self.arr = array
         # get the tick spacing that have 10 ticks only
         self.ticks_spacing = (self._vmax - self._vmin) / 10
         shape = array.shape
         if len(shape) == 3:
             no_elem = np.size(array[0, :, :]) - np.count_nonzero(
                 (array[0, np.isnan(array[0, :, :])])
             )
         else:
             no_elem = np.size(array[:, :]) - np.count_nonzero((array[np.isnan(array)]))
 
         self.no_elem = no_elem
-        self._default_options = DEFAULT_OPTIONS
+        self._default_options = DEFAULT_OPTIONS.copy()
 
     def _prepare_rgb(
         self,
         array: np.ndarray,
         rgb: List[int] = None,
         surface_reflectance: int = 10000,
         cutoff: List = None,
@@ -187,15 +194,15 @@
             ticks = np.arange(vmin, vmax + ticks_spacing, ticks_spacing)
         else:
             try:
                 ticks = np.arange(vmin, vmax, ticks_spacing)
             except ValueError:
                 raise ValueError(
                     "The number of ticks exceeded the max allowed size, possible errors"
-                    f"is the value of the NodataValue you entered-{self.exclude_value}"
+                    f" is the value of the NodataValue you entered-{self.exclude_value}"
                 )
             ticks = np.append(
                 ticks,
                 [int(vmax / ticks_spacing) * ticks_spacing + ticks_spacing],
             )
         return ticks
```

### Comparing `cleopatra-0.3.3/cleopatra/statistics.py` & `cleopatra-0.3.4/cleopatra/statistics.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.3/cleopatra/styles.py` & `cleopatra-0.3.4/cleopatra/styles.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.3/cleopatra.egg-info/PKG-INFO` & `cleopatra-0.3.4/cleopatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.3
+Version: 0.3.4
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
 Keywords: matplotlib,visualization
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.3
+pip install cleopatra==0.3.4
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -130,7 +130,11 @@
 0.3.2 (2023-04-23)
 ------------------
 * bump up hpc version
 
 0.3.3 (2023-04-25)
 ------------------
 * change the default value for the color bar label.
+
+0.3.4 (2023-04-26)
+------------------
+* pass the plot kwargs to the init of the array to scale the color bar using the vmin and vmax.
```

### Comparing `cleopatra-0.3.3/setup.py` & `cleopatra-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     history = history_file.read()
 
 requirements = [line.strip() for line in open("requirements.txt").readlines()]
 requirements_dev = [line.strip() for line in open("requirements-dev.txt").readlines()]
 
 setup(
     name="cleopatra",
-    version="0.3.3",
+    version="0.3.4",
     description="visualization package",
     author="Mostafa Farrag",
     author_email="moah.farag@gmail.come",
     url="https://github.com/MAfarrag/cleopatra",
     keywords=["matplotlib", "visualization"],
     long_description=readme + "\n\n" + history,
     repository="https://github.com/MAfarrag/celopatra",
```

### Comparing `cleopatra-0.3.3/tests/test_plot_array.py` & `cleopatra-0.3.4/tests/test_plot_array.py`

 * *Files identical despite different names*

