# Comparing `tmp/pyseistr-0.0.4.3.tar.gz` & `tmp/pyseistr-0.0.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyseistr-0.0.4.3.tar", last modified: Sun Apr 23 22:01:58 2023, max compression
+gzip compressed data, was "pyseistr-0.0.4.3.1.tar", last modified: Wed Apr 26 02:58:08 2023, max compression
```

## Comparing `pyseistr-0.0.4.3.tar` & `pyseistr-0.0.4.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.872939 pyseistr-0.0.4.3/
--rw-r--r--   0 chenyk     (501) staff       (20)    35149 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/LICENSE
--rw-r--r--   0 chenyk     (501) staff       (20)     1165 2023-04-23 22:01:58.872546 pyseistr-0.0.4.3/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     5858 2023-04-23 22:01:30.000000 pyseistr-0.0.4.3/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.862369 pyseistr-0.0.4.3/pyseistr/
--rw-r--r--   0 chenyk     (501) staff       (20)     1893 2023-04-22 20:38:05.000000 pyseistr-0.0.4.3/pyseistr/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     5563 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/bp.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4852 2023-04-23 20:41:03.000000 pyseistr-0.0.4.3/pyseistr/dip2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6636 2023-04-23 20:41:11.000000 pyseistr-0.0.4.3/pyseistr/dip3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     7494 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/divne.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1044 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/fk.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/mf.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4557 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/operators.py
--rw-r--r--   0 chenyk     (501) staff       (20)      696 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/plot.py
--rw-r--r--   0 chenyk     (501) staff       (20)     6801 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/pwspray2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     9410 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/pwspray3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)      657 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/ricker.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1990 2023-04-23 18:14:53.000000 pyseistr-0.0.4.3/pyseistr/soint2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2300 2023-04-22 20:42:00.000000 pyseistr-0.0.4.3/pyseistr/soint3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     7771 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/solvers.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1263 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somean2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1496 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somean3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2823 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somf2d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2932 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somf3d.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.871936 pyseistr-0.0.4.3/pyseistr/src/
--rw-r--r--   0 chenyk     (501) staff       (20)    14513 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/src/bp_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    42528 2023-04-23 21:14:48.000000 pyseistr-0.0.4.3/pyseistr/src/dip_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    35389 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/src/sof3d_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    34464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/src/sof_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    49126 2023-04-23 18:43:05.000000 pyseistr-0.0.4.3/pyseistr/src/soint2d_cfuns.c
--rw-r--r--   0 chenyk     (501) staff       (20)    31152 2023-04-22 19:39:19.000000 pyseistr-0.0.4.3/pyseistr/src/soint3d_cfuns.c
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.866471 pyseistr-0.0.4.3/pyseistr.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1165 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      737 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-22 19:39:47.000000 pyseistr-0.0.4.3/pyseistr.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       66 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-04-23 22:01:58.873088 pyseistr-0.0.4.3/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     2666 2023-04-23 22:01:45.000000 pyseistr-0.0.4.3/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.825459 pyseistr-0.0.4.3.1/
+-rw-r--r--   0 chenyk     (501) staff       (20)    35149 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/LICENSE
+-rw-r--r--   0 chenyk     (501) staff       (20)     1167 2023-04-26 02:58:08.825071 pyseistr-0.0.4.3.1/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     6520 2023-04-23 23:19:43.000000 pyseistr-0.0.4.3.1/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.812730 pyseistr-0.0.4.3.1/pyseistr/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1893 2023-04-22 20:38:05.000000 pyseistr-0.0.4.3.1/pyseistr/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     5563 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/bp.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4852 2023-04-26 02:53:38.000000 pyseistr-0.0.4.3.1/pyseistr/dip2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6636 2023-04-26 02:54:03.000000 pyseistr-0.0.4.3.1/pyseistr/dip3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7494 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/divne.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1044 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/fk.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/mf.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4557 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/operators.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      696 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/plot.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6801 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/pwspray2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9410 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/pwspray3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      657 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/ricker.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1990 2023-04-23 18:14:53.000000 pyseistr-0.0.4.3.1/pyseistr/soint2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2300 2023-04-22 20:42:00.000000 pyseistr-0.0.4.3.1/pyseistr/soint3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7771 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/solvers.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1263 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somean2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1496 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somean3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2823 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somf2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2932 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/somf3d.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.823427 pyseistr-0.0.4.3.1/pyseistr/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)    14513 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/src/bp_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    42528 2023-04-23 21:14:48.000000 pyseistr-0.0.4.3.1/pyseistr/src/dip_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    35389 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/src/sof3d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    34464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3.1/pyseistr/src/sof_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    49126 2023-04-23 18:43:05.000000 pyseistr-0.0.4.3.1/pyseistr/src/soint2d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    31152 2023-04-22 19:39:19.000000 pyseistr-0.0.4.3.1/pyseistr/src/soint3d_cfuns.c
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-26 02:58:08.816476 pyseistr-0.0.4.3.1/pyseistr.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1167 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      737 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-22 19:39:47.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       66 2023-04-26 02:58:08.000000 pyseistr-0.0.4.3.1/pyseistr.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-04-26 02:58:08.825597 pyseistr-0.0.4.3.1/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     2668 2023-04-26 02:57:52.000000 pyseistr-0.0.4.3.1/setup.py
```

### Comparing `pyseistr-0.0.4.3/LICENSE` & `pyseistr-0.0.4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/PKG-INFO` & `pyseistr-0.0.4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyseistr
-Version: 0.0.4.3
+Version: 0.0.4.3.1
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr
 Author: pyseistr developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyseistr-0.0.4.3/README.md` & `pyseistr-0.0.4.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -83,55 +83,55 @@
     Regarding any questions, bugs, developments, collaborations, please contact  
     Yangkang Chen
     chenyk2016@gmail.com
 
 -----------
 ## Examples
 # Example 1 (2D structure-oriented mean/smoothing filter) 
-Produced by demos/test_pyseistr_somean2d.py
+Generated by [demos/test_pyseistr_somean2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somean2d.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somean2d.png' alt='Slicing' width=960/>
 
 # Example 2 (3D structure-oriented mean/smoothing filter) 
-Produced by demos/test_pyseistr_somean3d.py
+Generated by [demos/test_pyseistr_somean3d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somean3d.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somean3d.png' alt='Slicing' width=960/>
 
 # Example 3 (2D structure-oriented median filter) 
-Produced by demos/test_pyseistr_somf2d.py
+Generated by [demos/test_pyseistr_somf2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somf2d.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somf2d.png' alt='Slicing' width=960/>
 
 # Example 4 (3D structure-oriented median filter) 
-Produced by demos/test_pyseistr_somf3d.py
+Generated by [demos/test_pyseistr_somf3d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_somf3d.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_somf3d.png' alt='Slicing' width=960/>
 
 # Example 5 (3D structure-oriented interpolation) 
-Produced by demos/test_pyseistr_passive_recon3d.py
+Generated by [demos/test_pyseistr_passive_recon3d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_passive_recon3d.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_passive_recon3d.png' alt='Slicing' width=960/>
 
 # Example 6 (SS precursor data enhancement) 
-Produced by demos/test_pyseistr_ssprecursor.py
+Generated by [demos/test_pyseistr_ssprecursor.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_ssprecursor.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_ssprecursor.png' alt='Slicing' width=960/>
 
 # Example 7 (receiver function data enhancement) 
-Produced by demos/test_pyseistr_rf.py
+Generated by [demos/test_pyseistr_rf.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_rf.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_rf.png' alt='Slicing' width=960/>
 
 # Example 8 (structure-oriented distributed acoustic sensing (DAS) data processing) 
-Produced by demos/test_pyseistr_das.py
+Generated by [demos/test_pyseistr_das.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_das.py)
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_das.png' alt='Slicing' width=960/>
 
-# Below are New Examples in addition to the results in the original paper
+# Below are new examples in addition to the results in the original paper
 
-# Below is a paper for 2D structure-oriented interpolation of a multi-channel synthetic seismic data
-Generated by [demos/test_pyseistr_soint2d.m](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d.m)
+# Below is an example for 2D structure-oriented interpolation of a multi-channel synthetic seismic data
+Generated by [demos/test_pyseistr_soint2d.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d.py)
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2d.png' alt='comp' width=960/>
 
-# Below is a paper for 2D structure-oriented interpolation of a seafloor dataset
-Generated by [demos/test_pyseistr_soint2d.m](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d_seafloor.m)
+# Below is an example for 2D structure-oriented interpolation of a seafloor dataset
+Generated by [demos/test_pyseistr_soint2d_seafloor.py](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d_seafloor.py)
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2d_seafloor.png' alt='comp' width=960/>
```

### Comparing `pyseistr-0.0.4.3/pyseistr/__init__.py` & `pyseistr-0.0.4.3.1/pyseistr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/bp.py` & `pyseistr-0.0.4.3.1/pyseistr/bp.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/dip2d.py` & `pyseistr-0.0.4.3.1/pyseistr/dip2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 		"""corresponding to the eq.21 in the paper  (Wang et al., 2022)"""
 		[u1,u2] = conv_allpass(din,dip,order); 
 		ratio = divne(-u2, u1, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
 		dip=dip+ratio;
 
 	return dip
 
-def dip2dc(din,mask=None,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1):
+def dip2dc(din,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1,mask=None):
 	'''
 	dip2dc: dip estimation based on shaping regularized PWD algorithm 
 	(C implementation)
 	
 	INPUT
 	din: input data (nt*nx)
 	niter: number of nonlinear iterations
```

### Comparing `pyseistr-0.0.4.3/pyseistr/dip3d.py` & `pyseistr-0.0.4.3.1/pyseistr/dip3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 		ratio_x  = divne(-u2_x, u1_x, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
 	
 		dip_i=dip_i+ratio_i;
 		dip_x=dip_x+ratio_x;
 
 	return dip_i,dip_x
 
-def dip3dc(din,mask=None,niter=5,liter=10,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[5,5,5],verb=1,runc=1):
+def dip3dc(din,niter=5,liter=10,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[5,5,5],verb=1,runc=1,mask=None):
 	'''
 	dip3dc: 3D dip estimation based on shaping regularized PWD algorithm
 	(C implementation)
 	
 	Ported to Python by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
 	
 	INPUT
```

### Comparing `pyseistr-0.0.4.3/pyseistr/divne.py` & `pyseistr-0.0.4.3.1/pyseistr/divne.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/fk.py` & `pyseistr-0.0.4.3.1/pyseistr/fk.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/mf.py` & `pyseistr-0.0.4.3.1/pyseistr/mf.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/operators.py` & `pyseistr-0.0.4.3.1/pyseistr/operators.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/plot.py` & `pyseistr-0.0.4.3.1/pyseistr/plot.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/pwspray2d.py` & `pyseistr-0.0.4.3.1/pyseistr/pwspray2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/pwspray3d.py` & `pyseistr-0.0.4.3.1/pyseistr/pwspray3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/ricker.py` & `pyseistr-0.0.4.3.1/pyseistr/ricker.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/soint2d.py` & `pyseistr-0.0.4.3.1/pyseistr/soint2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/soint3d.py` & `pyseistr-0.0.4.3.1/pyseistr/soint3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/solvers.py` & `pyseistr-0.0.4.3.1/pyseistr/solvers.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/somean2d.py` & `pyseistr-0.0.4.3.1/pyseistr/somean2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/somean3d.py` & `pyseistr-0.0.4.3.1/pyseistr/somean3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/somf2d.py` & `pyseistr-0.0.4.3.1/pyseistr/somf2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/somf3d.py` & `pyseistr-0.0.4.3.1/pyseistr/somf3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/src/bp_cfuns.c` & `pyseistr-0.0.4.3.1/pyseistr/src/bp_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/src/dip_cfuns.c` & `pyseistr-0.0.4.3.1/pyseistr/src/dip_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/src/sof3d_cfuns.c` & `pyseistr-0.0.4.3.1/pyseistr/src/sof3d_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/src/sof_cfuns.c` & `pyseistr-0.0.4.3.1/pyseistr/src/sof_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/src/soint2d_cfuns.c` & `pyseistr-0.0.4.3.1/pyseistr/src/soint2d_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr/src/soint3d_cfuns.c` & `pyseistr-0.0.4.3.1/pyseistr/src/soint3d_cfuns.c`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/pyseistr.egg-info/PKG-INFO` & `pyseistr-0.0.4.3.1/pyseistr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyseistr
-Version: 0.0.4.3
+Version: 0.0.4.3.1
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr
 Author: pyseistr developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyseistr-0.0.4.3/pyseistr.egg-info/SOURCES.txt` & `pyseistr-0.0.4.3.1/pyseistr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.3/setup.py` & `pyseistr-0.0.4.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 sointc2d_module = Extension('soint2dcfun', sources=['pyseistr/src/soint2d_cfuns.c'], 
 										include_dirs=[numpy.get_include()])
 bpc_module = Extension('bpcfun', sources=['pyseistr/src/bp_cfuns.c'], 
 										include_dirs=[numpy.get_include()])
 
 setup(
     name="pyseistr",
-    version="0.0.4.3",
+    version="0.0.4.3.1",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="A python package for structural denoising and interpolation of multi-channel seismic data",
     long_description=long_description,
     author="pyseistr developing team",
     author_email="chenyk2016@gmail.com",
     url="https://github.com/aaspip/pyseistr",
     ext_modules=[dipc_module,sofc_module,sofc3d_module,sointc2d_module,sointc3d_module,bpc_module],
```

