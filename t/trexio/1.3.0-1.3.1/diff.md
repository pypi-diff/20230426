# Comparing `tmp/trexio-1.3.0.tar.gz` & `tmp/trexio-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trexio-1.3.0.tar", last modified: Mon Apr  3 19:45:23 2023, max compression
+gzip compressed data, was "trexio-1.3.1.tar", last modified: Wed Apr 26 08:25:43 2023, max compression
```

## Comparing `trexio-1.3.0.tar` & `trexio-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 19:45:23.845466 trexio-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-03 19:43:42.000000 trexio-1.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-04-03 19:43:42.000000 trexio-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-04-03 19:41:27.000000 trexio-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-04-03 19:45:23.845466 trexio-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-04-03 19:41:27.000000 trexio-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-03 19:41:27.000000 trexio-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 19:45:23.833466 trexio-1.3.0/pytrexio/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-03 19:41:27.000000 trexio-1.3.0/pytrexio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-03 19:41:27.000000 trexio-1.3.0/pytrexio/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)   264868 2023-04-03 19:43:42.000000 trexio-1.3.0/pytrexio/pytrexio.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-03 19:41:27.000000 trexio-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-03 19:45:23.845466 trexio-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-04-03 19:41:27.000000 trexio-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 19:45:23.841466 trexio-1.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)  2216321 2023-04-03 19:43:42.000000 trexio-1.3.0/src/pytrexio_wrap.c
--rw-r--r--   0 runner    (1001) docker     (122)  1344758 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio.c
--rw-r--r--   0 runner    (1001) docker     (122)   163581 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio.h
--rw-r--r--   0 runner    (1001) docker     (122)   658349 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio_hdf5.c
--rw-r--r--   0 runner    (1001) docker     (122)    62512 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio_hdf5.h
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio_private.h
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio_s.h
--rw-r--r--   0 runner    (1001) docker     (122)   840930 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio_text.c
--rw-r--r--   0 runner    (1001) docker     (122)    79312 2023-04-03 19:43:42.000000 trexio-1.3.0/src/trexio_text.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 19:45:23.845466 trexio-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-03 19:41:27.000000 trexio-1.3.0/test/benzene_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12197 2023-04-03 19:41:27.000000 trexio-1.3.0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-04-03 19:41:27.000000 trexio-1.3.0/test/test_pytrexio.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 19:45:23.845466 trexio-1.3.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (122)      106 2023-04-03 19:41:27.000000 trexio-1.3.0/tools/set_NUMPY_INCLUDEDIR.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 19:45:23.845466 trexio-1.3.0/trexio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-04-03 19:45:23.000000 trexio-1.3.0/trexio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-04-03 19:45:23.000000 trexio-1.3.0/trexio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-03 19:45:23.000000 trexio-1.3.0/trexio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-03 19:45:23.000000 trexio-1.3.0/trexio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-03 19:45:23.000000 trexio-1.3.0/trexio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-03 19:45:23.000000 trexio-1.3.0/trexio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)   750503 2023-04-03 19:43:42.000000 trexio-1.3.0/trexio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-26 08:24:16.000000 trexio-1.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-04-26 08:24:16.000000 trexio-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-04-26 08:21:35.000000 trexio-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-04-26 08:25:43.967239 trexio-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-04-26 08:21:35.000000 trexio-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-26 08:21:35.000000 trexio-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.959238 trexio-1.3.1/pytrexio/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-26 08:21:35.000000 trexio-1.3.1/pytrexio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-26 08:21:35.000000 trexio-1.3.1/pytrexio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)   264868 2023-04-26 08:24:16.000000 trexio-1.3.1/pytrexio/pytrexio.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-26 08:21:35.000000 trexio-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-26 08:25:43.967239 trexio-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-04-26 08:21:35.000000 trexio-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)  2216321 2023-04-26 08:24:16.000000 trexio-1.3.1/src/pytrexio_wrap.c
+-rw-r--r--   0 runner    (1001) docker     (122)  1344758 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio.c
+-rw-r--r--   0 runner    (1001) docker     (122)   163581 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio.h
+-rw-r--r--   0 runner    (1001) docker     (122)   658349 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_hdf5.c
+-rw-r--r--   0 runner    (1001) docker     (122)    62512 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_hdf5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_private.h
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_s.h
+-rw-r--r--   0 runner    (1001) docker     (122)   841272 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_text.c
+-rw-r--r--   0 runner    (1001) docker     (122)    79312 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_text.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-26 08:21:35.000000 trexio-1.3.1/test/benzene_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12197 2023-04-26 08:21:35.000000 trexio-1.3.1/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-04-26 08:21:35.000000 trexio-1.3.1/test/test_pytrexio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      106 2023-04-26 08:21:35.000000 trexio-1.3.1/tools/set_NUMPY_INCLUDEDIR.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/trexio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   750503 2023-04-26 08:24:16.000000 trexio-1.3.1/trexio.py
```

### Comparing `trexio-1.3.0/LICENSE` & `trexio-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/PKG-INFO` & `trexio-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trexio
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API of the TREXIO library
 Home-page: https://github.com/TREX-CoE/trexio
 Author: TREX-CoE
 Author-email: posenitskiy@irsamc.ups-tlse.fr
 License: BSD
 Project-URL: Bug Tracker, https://github.com/TREX-CoE/trexio/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `trexio-1.3.0/README.md` & `trexio-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/pyproject.toml` & `trexio-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/pytrexio/pytrexio.py` & `trexio-1.3.1/pytrexio/pytrexio.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/setup.py` & `trexio-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/src/pytrexio_wrap.c` & `trexio-1.3.1/src/pytrexio_wrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -61960,19 +61960,19 @@
   
   
   import_array();
   
   SWIG_Python_SetConstant(d, "TREXIO_DELIM",SWIG_FromCharPtr("\n"));
   SWIG_Python_SetConstant(d, "TREXIO_ORBITAL_SHIFT",SWIG_From_int((int)(1)));
   SWIG_Python_SetConstant(d, "TREXIO_INT_SIZE",SWIG_From_int((int)(64)));
-  SWIG_Python_SetConstant(d, "TREXIO_PACKAGE_VERSION",SWIG_FromCharPtr("2.3.0"));
+  SWIG_Python_SetConstant(d, "TREXIO_PACKAGE_VERSION",SWIG_FromCharPtr("2.3.1"));
   SWIG_Python_SetConstant(d, "TREXIO_VERSION_MAJOR",SWIG_From_int((int)(2)));
   SWIG_Python_SetConstant(d, "TREXIO_VERSION_MINOR",SWIG_From_int((int)(3)));
-  SWIG_Python_SetConstant(d, "TREXIO_VERSION_PATCH",SWIG_From_int((int)(0)));
-  SWIG_Python_SetConstant(d, "TREXIO_GIT_HASH",SWIG_FromCharPtr("f4b409c501d6f2b22a4394cd097faa932d27cff1"));
+  SWIG_Python_SetConstant(d, "TREXIO_VERSION_PATCH",SWIG_From_int((int)(1)));
+  SWIG_Python_SetConstant(d, "TREXIO_GIT_HASH",SWIG_FromCharPtr("13567fceb89aaafff9e38952bd2bd486611243b8"));
 #if PY_VERSION_HEX >= 0x03000000
   return m;
 #else
   return;
 #endif
 }
```

### Comparing `trexio-1.3.0/src/trexio.c` & `trexio-1.3.1/src/trexio.c`

 * *Files 0% similar despite different names*

```diff
@@ -23937,16 +23937,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_ao_2e_int_eri_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_ao_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_2e_int_eri_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -24034,16 +24034,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_ao_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_ao_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -24420,16 +24420,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_mo_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -25863,16 +25863,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -25960,16 +25960,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_rdm_2e_dndn_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_rdm_2e_dndn_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -47012,16 +47012,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_ao_2e_int_eri_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_ao_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_2e_int_eri_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -47141,16 +47141,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_ao_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_ao_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_ao_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -47655,16 +47655,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_mo_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_2e_int_eri_lr_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -49578,16 +49578,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -49707,16 +49707,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_rdm_2e_dndn_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_rdm_2e_dndn_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
```

### Comparing `trexio-1.3.0/src/trexio.h` & `trexio-1.3.1/src/trexio.h`

 * *Files 0% similar despite different names*

```diff
@@ -102,19 +102,19 @@
 
 trexio_exit_code trexio_to_orbital_list (const int32_t N_int, const bitfield_t* d1, int32_t* const list, int32_t* const occupied_num);
 trexio_exit_code trexio_to_orbital_list_up_dn (const int32_t N_int, const bitfield_t* d1, int32_t* const list_up, int32_t* const list_dn, int32_t* const occ_num_up, int32_t* const occ_num_dn);
 trexio_exit_code trexio_safe_to_orbital_list (const int32_t N_int, const bitfield_t* dset_in, const int64_t dim_in, int32_t* const dset_out, const int64_t dim_out, int32_t* const num);
 trexio_exit_code trexio_safe_to_orbital_list_up_dn (const int32_t N_int, const bitfield_t* dset_in, const int64_t dim_in, int32_t* const dset_up_out, const int64_t dim_up_out, int32_t* const dset_dn_out, const int64_t dim_dn_out, int32_t* const num_up, int32_t* const num_dn);
 trexio_exit_code trexio_to_bitfield_list (const int32_t* orb_list, const int32_t occupied_num, bitfield_t* const bit_list, const int32_t N_int);
 
-#define TREXIO_PACKAGE_VERSION "2.3.0"
+#define TREXIO_PACKAGE_VERSION "2.3.1"
 #define TREXIO_VERSION_MAJOR 2
 #define TREXIO_VERSION_MINOR 3
-#define TREXIO_VERSION_PATCH 0
-#define TREXIO_GIT_HASH "f4b409c501d6f2b22a4394cd097faa932d27cff1"
+#define TREXIO_VERSION_PATCH 1
+#define TREXIO_GIT_HASH "13567fceb89aaafff9e38952bd2bd486611243b8"
 
 trexio_exit_code trexio_delete_metadata(trexio_t* const file);
 
 trexio_exit_code trexio_delete_nucleus(trexio_t* const file);
 
 trexio_exit_code trexio_delete_cell(trexio_t* const file);
```

### Comparing `trexio-1.3.0/src/trexio_hdf5.c` & `trexio-1.3.1/src/trexio_hdf5.c`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/src/trexio_hdf5.h` & `trexio-1.3.1/src/trexio_hdf5.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/src/trexio_private.h` & `trexio-1.3.1/src/trexio_private.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/src/trexio_s.h` & `trexio-1.3.1/src/trexio_s.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/src/trexio_text.c` & `trexio-1.3.1/src/trexio_text.c`

 * *Files 0% similar despite different names*

```diff
@@ -27,30 +27,48 @@
   int rc = stat(file_name, &st);
 
   bool file_exists = rc == 0;
 
   if (file_exists) {
 
     bool is_a_directory = false;
-#ifdef S_IFDIR
+#if defined(S_IFDIR)
     is_a_directory = st.st_mode & S_IFDIR;
-#elif S_ISDIR
-    is_a_directory = S_ISDIR(s.st_mode);
+#elif defined(S_ISDIR)
+    is_a_directory = S_ISDIR(st.st_mode);
 #else
     printf("Some important macros are missing for directory handling.\n");
     return TREXIO_FAILURE;
 #endif
     if (!is_a_directory) return TREXIO_FILE_ERROR;
 
     return TREXIO_SUCCESS;
   } else {
     return TREXIO_FAILURE;
   }
 }
 
+#if defined _POSIX_C_SOURCE && (_POSIX_C_SOURCE - 0) >= 200809L
+#else
+
+char* mkdtemp(char* template) {
+    char* dir = NULL;
+    dir = tmpnam(dir);
+    if (dir == NULL) return NULL;
+
+    if (mkdir(dir, S_IRWXU | S_IRWXG | S_IRWXO) != 0) {
+        return NULL;
+    }
+
+    strcpy(template, dir);
+    return template;
+}
+
+#endif
+
 trexio_exit_code
 trexio_text_init (trexio_t* const file)
 {
 
   if (file == NULL) return TREXIO_INVALID_ARG_1;
 
   trexio_text_t* const f = (trexio_text_t*) file;
```

### Comparing `trexio-1.3.0/src/trexio_text.h` & `trexio-1.3.1/src/trexio_text.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/test/benzene_data.py` & `trexio-1.3.1/test/benzene_data.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/test/test_api.py` & `trexio-1.3.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/test/test_pytrexio.py` & `trexio-1.3.1/test/test_pytrexio.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/trexio.egg-info/PKG-INFO` & `trexio-1.3.1/trexio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trexio
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API of the TREXIO library
 Home-page: https://github.com/TREX-CoE/trexio
 Author: TREX-CoE
 Author-email: posenitskiy@irsamc.ups-tlse.fr
 License: BSD
 Project-URL: Bug Tracker, https://github.com/TREX-CoE/trexio/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `trexio-1.3.0/trexio.egg-info/SOURCES.txt` & `trexio-1.3.1/trexio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trexio-1.3.0/trexio.py` & `trexio-1.3.1/trexio.py`

 * *Files identical despite different names*

