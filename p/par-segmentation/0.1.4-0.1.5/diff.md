# Comparing `tmp/par_segmentation-0.1.4.tar.gz` & `tmp/par_segmentation-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "par_segmentation-0.1.4.tar", last modified: Tue Jan 31 12:24:08 2023, max compression
+gzip compressed data, was "par_segmentation-0.1.5.tar", last modified: Wed Apr 26 14:28:37 2023, max compression
```

## Comparing `par_segmentation-0.1.4.tar` & `par_segmentation-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-31 12:24:08.493999 par_segmentation-0.1.4/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 par_segmentation-0.1.4/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     5185 2023-01-31 12:24:08.494497 par_segmentation-0.1.4/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     4260 2023-01-31 12:20:30.000000 par_segmentation-0.1.4/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-31 12:24:08.277327 par_segmentation-0.1.4/par_segmentation/
--rw-r--r--   0 blandt   (743162876) 1934034978      136 2023-01-18 17:11:30.000000 par_segmentation-0.1.4/par_segmentation/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978    18880 2023-01-25 15:05:51.000000 par_segmentation-0.1.4/par_segmentation/funcs.py
--rw-r--r--   0 blandt   (743162876) 1934034978    15490 2023-01-31 11:47:21.000000 par_segmentation-0.1.4/par_segmentation/interactive.py
--rw-r--r--   0 blandt   (743162876) 1934034978    15993 2023-01-18 17:11:30.000000 par_segmentation-0.1.4/par_segmentation/legacy.py
--rw-r--r--   0 blandt   (743162876) 1934034978    16693 2023-01-27 22:47:32.000000 par_segmentation-0.1.4/par_segmentation/model.py
--rw-r--r--   0 blandt   (743162876) 1934034978    10511 2023-01-31 12:14:21.000000 par_segmentation-0.1.4/par_segmentation/quantifier.py
--rw-r--r--   0 blandt   (743162876) 1934034978    14337 2023-01-18 17:11:30.000000 par_segmentation-0.1.4/par_segmentation/roi.py
--rw-r--r--   0 blandt   (743162876) 1934034978    16402 2023-01-18 17:11:30.000000 par_segmentation-0.1.4/par_segmentation/tgf_interpolate.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-31 12:24:08.289258 par_segmentation-0.1.4/par_segmentation.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     5185 2023-01-31 12:24:04.000000 par_segmentation-0.1.4/par_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      590 2023-01-31 12:24:05.000000 par_segmentation-0.1.4/par_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-01-31 12:24:04.000000 par_segmentation-0.1.4/par_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      114 2023-01-31 12:24:04.000000 par_segmentation-0.1.4/par_segmentation.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       23 2023-01-31 12:24:05.000000 par_segmentation-0.1.4/par_segmentation.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-01-31 12:24:08.498097 par_segmentation-0.1.4/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      935 2023-01-31 12:22:24.000000 par_segmentation-0.1.4/setup.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-31 12:24:08.492395 par_segmentation-0.1.4/tests/
--rw-r--r--   0 blandt   (743162876) 1934034978        0 2023-01-18 12:19:25.000000 par_segmentation-0.1.4/tests/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978      784 2023-01-27 22:07:48.000000 par_segmentation-0.1.4/tests/test_de_completion.py
--rw-r--r--   0 blandt   (743162876) 1934034978     1230 2023-01-27 15:24:33.000000 par_segmentation-0.1.4/tests/test_de_correct.py
--rw-r--r--   0 blandt   (743162876) 1934034978     2355 2023-01-27 22:07:48.000000 par_segmentation-0.1.4/tests/test_gd_completion.py
--rw-r--r--   0 blandt   (743162876) 1934034978     1147 2023-01-27 15:24:33.000000 par_segmentation-0.1.4/tests/test_gd_correct.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.631277 par_segmentation-0.1.5/
+-rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 par_segmentation-0.1.5/LICENSE
+-rw-r--r--   0 blandt   (743162876) 1934034978     5380 2023-04-26 14:28:37.631569 par_segmentation-0.1.5/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978     4352 2023-02-01 14:17:05.000000 par_segmentation-0.1.5/README.md
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.466907 par_segmentation-0.1.5/par_segmentation/
+-rw-r--r--   0 blandt   (743162876) 1934034978      136 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    18880 2023-01-25 15:05:51.000000 par_segmentation-0.1.5/par_segmentation/funcs.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    15490 2023-01-31 11:47:21.000000 par_segmentation-0.1.5/par_segmentation/interactive.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    15993 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/legacy.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    16693 2023-01-27 22:47:32.000000 par_segmentation-0.1.5/par_segmentation/model.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    10511 2023-01-31 12:14:21.000000 par_segmentation-0.1.5/par_segmentation/quantifier.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    14337 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/roi.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    16402 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/tgf_interpolate.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.480894 par_segmentation-0.1.5/par_segmentation.egg-info/
+-rw-r--r--   0 blandt   (743162876) 1934034978     5380 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      590 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978      114 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/requires.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       23 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/top_level.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:28:37.634613 par_segmentation-0.1.5/setup.cfg
+-rw-r--r--   0 blandt   (743162876) 1934034978     1032 2023-04-26 14:28:08.000000 par_segmentation-0.1.5/setup.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.630017 par_segmentation-0.1.5/tests/
+-rw-r--r--   0 blandt   (743162876) 1934034978        0 2023-01-18 12:19:25.000000 par_segmentation-0.1.5/tests/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978      774 2023-01-31 12:24:18.000000 par_segmentation-0.1.5/tests/test_de_completion.py
+-rw-r--r--   0 blandt   (743162876) 1934034978     1230 2023-01-27 15:24:33.000000 par_segmentation-0.1.5/tests/test_de_correct.py
+-rw-r--r--   0 blandt   (743162876) 1934034978     2355 2023-01-27 22:07:48.000000 par_segmentation-0.1.5/tests/test_gd_completion.py
+-rw-r--r--   0 blandt   (743162876) 1934034978     1147 2023-01-27 15:24:33.000000 par_segmentation-0.1.5/tests/test_gd_correct.py
```

### Comparing `par_segmentation-0.1.4/LICENSE` & `par_segmentation-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/PKG-INFO` & `par_segmentation-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: par_segmentation
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cell cortex segmentation in C. elegans PAR protein images
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
 Description: # PAR Segmentation
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
         [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
         
@@ -26,30 +27,34 @@
         The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
         In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/docs/model schematic.png" width="100%" height="100%"/>
         </p>
         
-        Cortex positions are modelled as a spline with a user specified number of knots which are optimised by gradient descent:
+        Cortex positions are modelled as a spline with a user-specified number of evenly spaced knots which are optimised by gradient descent:
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/spline.png" width="80%" height="80%"/>
         </p>
         
-        The program additionally outputs parameters related to cytoplasmic and membrane concentrations, so can serve as a quantification tool as well as a segmentation tool:
+        Cross-cortex intensity profiles at each position around the cortex are modelled as the sum of distinct cytoplasmic and membrane signal components:
+        an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension:
         
         <p align="center">
-            <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
+            <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/profiles.png" width="100%" height="100%"/>
         </p>
         
-        The differentiable simulation is built on the assumption that cross-cortex intensity profiles at each position around the cortex are the sum of distinct cytoplasmic and membrane signal components.
-        Here, we model these two components as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension.
-        This is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours, but is a close enough approximation for many purposes. 
+        The program learns the amplitude of these two components at each position around the cortex, so can serve as a quantification tool as well as a segmentation tool:
+        
+        <p align="center">
+            <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
+        </p>
         
+        The model is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex 3D light-scattering behaviours, but is a close enough approximation for many purposes. 
         Nevertheless, we can relax these assumptions if higher quantification accuracy is required. 
         See [here](https://github.com/tsmbland/discco) for an extension of the method designed for more accurate quantification.
         
         ## Installation
         
             pip install par-segmentation
```

### Comparing `par_segmentation-0.1.4/README.md` & `par_segmentation-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,34 @@
 The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
 In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/docs/model schematic.png" width="100%" height="100%"/>
 </p>
 
-Cortex positions are modelled as a spline with a user specified number of knots which are optimised by gradient descent:
+Cortex positions are modelled as a spline with a user-specified number of evenly spaced knots which are optimised by gradient descent:
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/spline.png" width="80%" height="80%"/>
 </p>
 
-The program additionally outputs parameters related to cytoplasmic and membrane concentrations, so can serve as a quantification tool as well as a segmentation tool:
+Cross-cortex intensity profiles at each position around the cortex are modelled as the sum of distinct cytoplasmic and membrane signal components:
+an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
+    <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/profiles.png" width="100%" height="100%"/>
 </p>
 
-The differentiable simulation is built on the assumption that cross-cortex intensity profiles at each position around the cortex are the sum of distinct cytoplasmic and membrane signal components.
-Here, we model these two components as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension.
-This is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours, but is a close enough approximation for many purposes. 
+The program learns the amplitude of these two components at each position around the cortex, so can serve as a quantification tool as well as a segmentation tool:
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
+</p>
 
+The model is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex 3D light-scattering behaviours, but is a close enough approximation for many purposes. 
 Nevertheless, we can relax these assumptions if higher quantification accuracy is required. 
 See [here](https://github.com/tsmbland/discco) for an extension of the method designed for more accurate quantification.
 
 ## Installation
 
     pip install par-segmentation
```

### Comparing `par_segmentation-0.1.4/par_segmentation/funcs.py` & `par_segmentation-0.1.5/par_segmentation/funcs.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation/interactive.py` & `par_segmentation-0.1.5/par_segmentation/interactive.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation/legacy.py` & `par_segmentation-0.1.5/par_segmentation/legacy.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation/model.py` & `par_segmentation-0.1.5/par_segmentation/model.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation/quantifier.py` & `par_segmentation-0.1.5/par_segmentation/quantifier.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation/roi.py` & `par_segmentation-0.1.5/par_segmentation/roi.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation/tgf_interpolate.py` & `par_segmentation-0.1.5/par_segmentation/tgf_interpolate.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/par_segmentation.egg-info/PKG-INFO` & `par_segmentation-0.1.5/par_segmentation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: par-segmentation
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cell cortex segmentation in C. elegans PAR protein images
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
 Description: # PAR Segmentation
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
         [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
         
@@ -26,30 +27,34 @@
         The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
         In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/docs/model schematic.png" width="100%" height="100%"/>
         </p>
         
-        Cortex positions are modelled as a spline with a user specified number of knots which are optimised by gradient descent:
+        Cortex positions are modelled as a spline with a user-specified number of evenly spaced knots which are optimised by gradient descent:
         
         <p align="center">
             <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/spline.png" width="80%" height="80%"/>
         </p>
         
-        The program additionally outputs parameters related to cytoplasmic and membrane concentrations, so can serve as a quantification tool as well as a segmentation tool:
+        Cross-cortex intensity profiles at each position around the cortex are modelled as the sum of distinct cytoplasmic and membrane signal components:
+        an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension:
         
         <p align="center">
-            <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
+            <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/profiles.png" width="100%" height="100%"/>
         </p>
         
-        The differentiable simulation is built on the assumption that cross-cortex intensity profiles at each position around the cortex are the sum of distinct cytoplasmic and membrane signal components.
-        Here, we model these two components as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension.
-        This is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours, but is a close enough approximation for many purposes. 
+        The program learns the amplitude of these two components at each position around the cortex, so can serve as a quantification tool as well as a segmentation tool:
+        
+        <p align="center">
+            <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
+        </p>
         
+        The model is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex 3D light-scattering behaviours, but is a close enough approximation for many purposes. 
         Nevertheless, we can relax these assumptions if higher quantification accuracy is required. 
         See [here](https://github.com/tsmbland/discco) for an extension of the method designed for more accurate quantification.
         
         ## Installation
         
             pip install par-segmentation
```

### Comparing `par_segmentation-0.1.4/par_segmentation.egg-info/SOURCES.txt` & `par_segmentation-0.1.5/par_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/setup.py` & `par_segmentation-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='par_segmentation',
-    version='0.1.4',
+    version='0.1.5',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'scipy',
@@ -21,9 +21,12 @@
                       'joblib',
                       'tensorflow>=2.9.1',
                       'tqdm',
                       'pandas',
                       'absl-py'],
     description='Cell cortex segmentation in C. elegans PAR protein images',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+        "Source Code": "https://github.com/tsmbland/par-segmentation",
+    }
 )
```

### Comparing `par_segmentation-0.1.4/tests/test_de_completion.py` & `par_segmentation-0.1.5/tests/test_de_completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     @classmethod
     def setUpClass(cls):
         path = os.path.dirname(os.path.abspath(__file__)) + '/../data/dataset2_par2_neon'
         paths = direcslist(path)[:2]
         cls.imgs = [load_image(p + '/af_corrected.tif') for p in paths]
         cls.rois = [np.loadtxt(p + '/ROI.txt') for p in paths]
 
-    # def test1(self):
-    #     # Testing that it runs to completion with default parameters
-    #     iq = ImageQuant(img=self.imgs, roi=self.rois, method='DE', verbose=False, parallel=False)
-    #     iq.run()
-    #     res = iq.compile_res()
+    def test1(self):
+        # Testing that it runs to completion with default parameters
+        iq = ImageQuant(img=self.imgs, roi=self.rois, method='DE', verbose=False, parallel=False)
+        iq.run()
+        res = iq.compile_res()
```

### Comparing `par_segmentation-0.1.4/tests/test_de_correct.py` & `par_segmentation-0.1.5/tests/test_de_correct.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/tests/test_gd_completion.py` & `par_segmentation-0.1.5/tests/test_gd_completion.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.4/tests/test_gd_correct.py` & `par_segmentation-0.1.5/tests/test_gd_correct.py`

 * *Files identical despite different names*

