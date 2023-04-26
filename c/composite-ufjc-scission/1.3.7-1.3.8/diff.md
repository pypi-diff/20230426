# Comparing `tmp/composite_ufjc_scission-1.3.7.tar.gz` & `tmp/composite_ufjc_scission-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composite_ufjc_scission-1.3.7.tar", last modified: Thu Mar  9 20:01:46 2023, max compression
+gzip compressed data, was "composite_ufjc_scission-1.3.8.tar", last modified: Tue Apr 25 16:03:02 2023, max compression
```

## Comparing `composite_ufjc_scission-1.3.7.tar` & `composite_ufjc_scission-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-03-09 20:01:46.978286 composite_ufjc_scission-1.3.7/
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      735 2022-11-09 17:27:23.000000 composite_ufjc_scission-1.3.7/LICENSE
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4028 2023-03-09 20:01:46.978286 composite_ufjc_scission-1.3.7/PKG-INFO
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     2661 2023-03-09 19:42:00.000000 composite_ufjc_scission-1.3.7/README.rst
-drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-03-09 20:01:46.978286 composite_ufjc_scission-1.3.7/composite_ufjc_scission/
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      260 2023-03-09 19:30:22.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/__init__.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1644 2022-12-12 18:37:58.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/characterizer.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     8695 2022-12-14 23:10:43.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/composite_ufjc.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    24036 2022-12-14 17:27:44.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/core.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     5601 2022-12-12 18:37:58.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/default_parameters.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    11865 2023-03-09 19:02:37.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/rate_dependence_scission.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    96459 2023-03-09 19:24:52.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/scission_model.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     3438 2022-12-12 18:37:58.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission/utility.py
-drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-03-09 20:01:46.978286 composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4028 2023-03-09 20:01:46.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/PKG-INFO
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      612 2023-03-09 20:01:46.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/SOURCES.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        1 2023-03-09 20:01:46.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/dependency_links.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       35 2023-03-09 20:01:46.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/requires.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       24 2023-03-09 20:01:46.000000 composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/top_level.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       80 2022-11-17 16:55:00.000000 composite_ufjc_scission-1.3.7/pyproject.toml
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1535 2023-03-09 20:01:46.978286 composite_ufjc_scission-1.3.7/setup.cfg
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       68 2022-11-17 18:05:25.000000 composite_ufjc_scission-1.3.7/setup.py
+drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-04-25 16:03:02.937683 composite_ufjc_scission-1.3.8/
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      735 2022-11-09 17:27:23.000000 composite_ufjc_scission-1.3.8/LICENSE
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4028 2023-04-25 16:03:02.937683 composite_ufjc_scission-1.3.8/PKG-INFO
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     2661 2023-03-09 19:42:00.000000 composite_ufjc_scission-1.3.8/README.rst
+drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-04-25 16:03:02.933683 composite_ufjc_scission-1.3.8/composite_ufjc_scission/
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      260 2023-04-24 13:40:01.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/__init__.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1644 2022-12-12 18:37:58.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/characterizer.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     8695 2022-12-14 23:10:43.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/composite_ufjc.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    24101 2023-04-24 20:51:13.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/core.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     5601 2022-12-12 18:37:58.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/default_parameters.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    11865 2023-03-09 19:02:37.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/rate_dependence_scission.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)   147636 2023-04-25 15:54:50.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/scission_model.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     3438 2022-12-12 18:37:58.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission/utility.py
+drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-04-25 16:03:02.937683 composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4028 2023-04-25 16:03:02.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/PKG-INFO
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      612 2023-04-25 16:03:02.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        1 2023-04-25 16:03:02.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       35 2023-04-25 16:03:02.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/requires.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       24 2023-04-25 16:03:02.000000 composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/top_level.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       80 2022-11-17 16:55:00.000000 composite_ufjc_scission-1.3.8/pyproject.toml
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1535 2023-04-25 16:03:02.937683 composite_ufjc_scission-1.3.8/setup.cfg
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       68 2022-11-17 18:05:25.000000 composite_ufjc_scission-1.3.8/setup.py
```

### Comparing `composite_ufjc_scission-1.3.7/LICENSE` & `composite_ufjc_scission-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/PKG-INFO` & `composite_ufjc_scission-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composite_ufjc_scission
-Version: 1.3.7
+Version: 1.3.8
 Summary: The Python package for the composite uFJC model with scission.
 Home-page: https://github.com/jasonmulderrig/composite-uFJC-scission
 Author: Jason Mulderrig, Brandon Talamini, Nikolaos Bouklas
 Author-email: jpm445@cornell.edu, talamini1@llnl.gov, nb589@cornell.edu
 Maintainer: Jason Mulderrig
 Maintainer-email: jpm445@cornell.edu, mulderrig.jason@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `composite_ufjc_scission-1.3.7/README.rst` & `composite_ufjc_scission-1.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission/characterizer.py` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission/characterizer.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission/composite_ufjc.py` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission/composite_ufjc.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission/core.py` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,17 @@
             np.argmin(np.abs(lmbda_nu_padeapprx-lmbda_nu_bergapprx))
         )
         lmbda_nu_pade2berg_crit = (
             min([lmbda_nu_bergapprx[pade2berg_crit_indx],
                 lmbda_nu_padeapprx[pade2berg_crit_indx]])
         )
         lmbda_c_eq_pade2berg_crit = lmbda_c_eq[pade2berg_crit_indx]
+
+        del lmbda_c_eq, lmbda_nu_bergapprx, lmbda_nu_padeapprx
+
         return lmbda_nu_pade2berg_crit, lmbda_c_eq_pade2berg_crit
     
     def lmbda_c_eq_pade2berg_crit_func(self):
         """Pade-to-Bergstrom (P2B) critical equilibrium chain stretch.
         
         This function returns Pade-to-Bergstrom (P2B) critical 
         equilibrium chain stretch as determined via a scipy optimize
```

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission/default_parameters.py` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission/default_parameters.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission/rate_dependence_scission.py` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission/rate_dependence_scission.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission/utility.py` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission/utility.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/PKG-INFO` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composite-ufjc-scission
-Version: 1.3.7
+Version: 1.3.8
 Summary: The Python package for the composite uFJC model with scission.
 Home-page: https://github.com/jasonmulderrig/composite-uFJC-scission
 Author: Jason Mulderrig, Brandon Talamini, Nikolaos Bouklas
 Author-email: jpm445@cornell.edu, talamini1@llnl.gov, nb589@cornell.edu
 Maintainer: Jason Mulderrig
 Maintainer-email: jpm445@cornell.edu, mulderrig.jason@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `composite_ufjc_scission-1.3.7/composite_ufjc_scission.egg-info/SOURCES.txt` & `composite_ufjc_scission-1.3.8/composite_ufjc_scission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission-1.3.7/setup.cfg` & `composite_ufjc_scission-1.3.8/setup.cfg`

 * *Files identical despite different names*

