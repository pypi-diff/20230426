# Comparing `tmp/cleopatra-0.3.2.tar.gz` & `tmp/cleopatra-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleopatra-0.3.2.tar", last modified: Sun Apr 23 03:15:41 2023, max compression
+gzip compressed data, was "cleopatra-0.3.3.tar", last modified: Tue Apr 25 21:09:40 2023, max compression
```

## Comparing `cleopatra-0.3.2.tar` & `cleopatra-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.521115 cleopatra-0.3.2/
--rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.2/AUTHORS.rst
--rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.2/LICENSE.md
--rw-rw-rw-   0        0        0     6952 2023-04-23 03:15:41.520114 cleopatra-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5081 2023-04-23 03:09:51.000000 cleopatra-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.502096 cleopatra-0.3.2/cleopatra/
--rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.2/cleopatra/__init__.py
--rw-rw-rw-   0        0        0    37348 2023-04-23 03:09:51.000000 cleopatra-0.3.2/cleopatra/array.py
--rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.2/cleopatra/statistics.py
--rw-rw-rw-   0        0        0     6398 2023-04-17 03:25:28.000000 cleopatra-0.3.2/cleopatra/styles.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.511605 cleopatra-0.3.2/cleopatra.egg-info/
--rw-rw-rw-   0        0        0     6952 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 03:15:41.000000 cleopatra-0.3.2/cleopatra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 03:15:41.521115 cleopatra-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1689 2023-04-23 03:09:51.000000 cleopatra-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:15:41.518114 cleopatra-0.3.2/tests/
--rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.2/tests/test_plot_array.py
--rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.2/tests/test_statistics.py
--rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.2/tests/test_styles.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.537488 cleopatra-0.3.3/
+-rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.3/LICENSE.md
+-rw-rw-rw-   0        0        0     7040 2023-04-25 21:09:40.537488 cleopatra-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5081 2023-04-25 20:03:44.000000 cleopatra-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.514440 cleopatra-0.3.3/cleopatra/
+-rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.3/cleopatra/__init__.py
+-rw-rw-rw-   0        0        0    37348 2023-04-23 09:44:18.000000 cleopatra-0.3.3/cleopatra/array.py
+-rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.3/cleopatra/statistics.py
+-rw-rw-rw-   0        0        0     6386 2023-04-25 20:03:44.000000 cleopatra-0.3.3/cleopatra/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.526490 cleopatra-0.3.3/cleopatra.egg-info/
+-rw-rw-rw-   0        0        0     7040 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 21:09:40.000000 cleopatra-0.3.3/cleopatra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 21:09:40.538663 cleopatra-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-04-25 20:39:25.000000 cleopatra-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:09:40.534490 cleopatra-0.3.3/tests/
+-rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.3/tests/test_plot_array.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.3/tests/test_statistics.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.3/tests/test_styles.py
```

### Comparing `cleopatra-0.3.2/LICENSE.md` & `cleopatra-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.2/PKG-INFO` & `cleopatra-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.2
+Version: 0.3.3
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
-Keywords: matplotlib,arrays,visualization
+Keywords: matplotlib,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.2
+pip install cleopatra==0.3.3
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -126,7 +126,11 @@
 0.3.1 (2023-04-17)
 ------------------
 * plot RGB plots
 
 0.3.2 (2023-04-23)
 ------------------
 * bump up hpc version
+
+0.3.3 (2023-04-25)
+------------------
+* change the default value for the color bar label.
```

### Comparing `cleopatra-0.3.2/README.md` & `cleopatra-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.2
+pip install cleopatra==0.3.3
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
```

### Comparing `cleopatra-0.3.2/cleopatra/__init__.py` & `cleopatra-0.3.3/cleopatra/__init__.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.2/cleopatra/array.py` & `cleopatra-0.3.3/cleopatra/array.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.2/cleopatra/statistics.py` & `cleopatra-0.3.3/cleopatra/statistics.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.2/cleopatra/styles.py` & `cleopatra-0.3.3/cleopatra/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     color_1="#3D59AB",
     color_2="#DC143C",
     line_width=3,
     cbar_length=0.75,
     orientation="vertical",
     cmap="coolwarm_r",
     cbar_label_size=12,
-    cbar_label="Color bar label",
+    cbar_label=None,
     rotation=-90,
     ticks_spacing=5,
     color_scale=1,
     gamma=0.5,
     line_scale=0.001,
     line_threshold=0.0001,
     bounds=None,
@@ -136,15 +136,15 @@
         Parameters
         ----------
         minval
         maxval
 
         Returns
         -------
-        """
+        #"""
 
         def scalar(val):
             """scalar.
 
                 scalar
 
             Parameters
```

### Comparing `cleopatra-0.3.2/cleopatra.egg-info/PKG-INFO` & `cleopatra-0.3.3/cleopatra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.2
+Version: 0.3.3
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
-Keywords: matplotlib,arrays,visualization
+Keywords: matplotlib,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.2
+pip install cleopatra==0.3.3
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -126,7 +126,11 @@
 0.3.1 (2023-04-17)
 ------------------
 * plot RGB plots
 
 0.3.2 (2023-04-23)
 ------------------
 * bump up hpc version
+
+0.3.3 (2023-04-25)
+------------------
+* change the default value for the color bar label.
```

### Comparing `cleopatra-0.3.2/setup.py` & `cleopatra-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     history = history_file.read()
 
 requirements = [line.strip() for line in open("requirements.txt").readlines()]
 requirements_dev = [line.strip() for line in open("requirements-dev.txt").readlines()]
 
 setup(
     name="cleopatra",
-    version="0.3.2",
+    version="0.3.3",
     description="visualization package",
     author="Mostafa Farrag",
     author_email="moah.farag@gmail.come",
     url="https://github.com/MAfarrag/cleopatra",
-    keywords=["matplotlib", "arrays", "visualization"],
+    keywords=["matplotlib", "visualization"],
     long_description=readme + "\n\n" + history,
     repository="https://github.com/MAfarrag/celopatra",
     documentation="https://celopatra.readthedocs.io/",
     long_description_content_type="text/markdown",
     license="GNU General Public License v3",
     zip_safe=False,
     packages=find_packages(include=["cleopatra", "cleopatra.*"]),
```

### Comparing `cleopatra-0.3.2/tests/test_plot_array.py` & `cleopatra-0.3.3/tests/test_plot_array.py`

 * *Files identical despite different names*

