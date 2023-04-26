# Comparing `tmp/bw2speedups-3.0.tar.gz` & `tmp/bw2speedups-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2speedups-3.0.tar", last modified: Wed Apr 26 12:12:34 2023, max compression
+gzip compressed data, was "bw2speedups-3.1.tar", last modified: Wed Apr 26 12:23:13 2023, max compression
```

## Comparing `bw2speedups-3.0.tar` & `bw2speedups-3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:12:34.292337 bw2speedups-3.0/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:12:34.285854 bw2speedups-3.0/.github/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:12:34.287219 bw2speedups-3.0/.github/workflows/
--rw-r--r--   0 chrismutel   (501) staff       (20)      691 2022-11-02 16:16:58.000000 bw2speedups-3.0/.github/workflows/build_wheels.yaml
--rw-r--r--   0 chrismutel   (501) staff       (20)      227 2023-04-26 12:11:37.000000 bw2speedups-3.0/CHANGES.md
--rw-r--r--   0 chrismutel   (501) staff       (20)     1474 2022-11-02 07:56:36.000000 bw2speedups-3.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       53 2022-11-02 07:56:36.000000 bw2speedups-3.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     1941 2023-04-26 12:12:34.292216 bw2speedups-3.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1302 2022-11-02 07:56:36.000000 bw2speedups-3.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:12:34.290648 bw2speedups-3.0/bw2speedups/
--rw-r--r--   0 chrismutel   (501) staff       (20)      126 2023-04-26 12:11:42.000000 bw2speedups-3.0/bw2speedups/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)   363434 2022-11-02 08:00:12.000000 bw2speedups-3.0/bw2speedups/_consolidate.c
--rw-r--r--   0 chrismutel   (501) staff       (20)     1811 2023-04-26 12:07:21.000000 bw2speedups-3.0/bw2speedups/_consolidate.pyx
--rw-r--r--   0 chrismutel   (501) staff       (20)   355353 2022-11-02 08:00:12.000000 bw2speedups-3.0/bw2speedups/_find_first.c
--rw-r--r--   0 chrismutel   (501) staff       (20)      629 2022-11-02 08:00:04.000000 bw2speedups-3.0/bw2speedups/_find_first.pyx
--rw-r--r--   0 chrismutel   (501) staff       (20)   348181 2022-11-02 08:00:12.000000 bw2speedups-3.0/bw2speedups/_indexer.c
--rw-r--r--   0 chrismutel   (501) staff       (20)      688 2022-11-02 08:00:08.000000 bw2speedups-3.0/bw2speedups/_indexer.pyx
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:12:34.291933 bw2speedups-3.0/bw2speedups/test/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2022-11-02 07:56:36.000000 bw2speedups-3.0/bw2speedups/test/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1545 2022-11-02 07:56:36.000000 bw2speedups-3.0/bw2speedups/test/test_consolidate.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1360 2022-11-02 07:56:36.000000 bw2speedups-3.0/bw2speedups/test/test_indexer.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:12:34.291490 bw2speedups-3.0/bw2speedups.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1941 2023-04-26 12:12:34.000000 bw2speedups-3.0/bw2speedups.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      585 2023-04-26 12:12:34.000000 bw2speedups-3.0/bw2speedups.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 12:12:34.000000 bw2speedups-3.0/bw2speedups.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 12:12:34.000000 bw2speedups-3.0/bw2speedups.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-26 12:12:34.000000 bw2speedups-3.0/bw2speedups.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-26 12:12:34.000000 bw2speedups-3.0/bw2speedups.egg-info/top_level.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       46 2022-11-02 07:56:36.000000 bw2speedups-3.0/pytest.ini
--rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-26 12:12:34.292371 bw2speedups-3.0/setup.cfg
--rw-r--r--   0 chrismutel   (501) staff       (20)     1725 2023-04-26 12:10:58.000000 bw2speedups-3.0/setup.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:23:13.385580 bw2speedups-3.1/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:23:13.378684 bw2speedups-3.1/.github/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:23:13.380115 bw2speedups-3.1/.github/workflows/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      691 2022-11-02 16:16:58.000000 bw2speedups-3.1/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 chrismutel   (501) staff       (20)      227 2023-04-26 12:11:37.000000 bw2speedups-3.1/CHANGES.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1474 2022-11-02 07:56:36.000000 bw2speedups-3.1/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       53 2022-11-02 07:56:36.000000 bw2speedups-3.1/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1941 2023-04-26 12:23:13.385441 bw2speedups-3.1/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1302 2022-11-02 07:56:36.000000 bw2speedups-3.1/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:23:13.383768 bw2speedups-3.1/bw2speedups/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      126 2023-04-26 12:22:36.000000 bw2speedups-3.1/bw2speedups/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)   286220 2023-04-26 12:21:12.000000 bw2speedups-3.1/bw2speedups/_consolidate.c
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1811 2023-04-26 12:07:21.000000 bw2speedups-3.1/bw2speedups/_consolidate.pyx
+-rw-r--r--   0 chrismutel   (501) staff       (20)   355353 2022-11-02 08:00:12.000000 bw2speedups-3.1/bw2speedups/_find_first.c
+-rw-r--r--   0 chrismutel   (501) staff       (20)      629 2022-11-02 08:00:04.000000 bw2speedups-3.1/bw2speedups/_find_first.pyx
+-rw-r--r--   0 chrismutel   (501) staff       (20)   348181 2022-11-02 08:00:12.000000 bw2speedups-3.1/bw2speedups/_indexer.c
+-rw-r--r--   0 chrismutel   (501) staff       (20)      688 2022-11-02 08:00:08.000000 bw2speedups-3.1/bw2speedups/_indexer.pyx
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:23:13.385136 bw2speedups-3.1/bw2speedups/test/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2022-11-02 07:56:36.000000 bw2speedups-3.1/bw2speedups/test/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1462 2023-04-26 12:14:24.000000 bw2speedups-3.1/bw2speedups/test/test_consolidate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1360 2022-11-02 07:56:36.000000 bw2speedups-3.1/bw2speedups/test/test_indexer.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-26 12:23:13.384650 bw2speedups-3.1/bw2speedups.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1941 2023-04-26 12:23:13.000000 bw2speedups-3.1/bw2speedups.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      585 2023-04-26 12:23:13.000000 bw2speedups-3.1/bw2speedups.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 12:23:13.000000 bw2speedups-3.1/bw2speedups.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 12:12:34.000000 bw2speedups-3.1/bw2speedups.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-26 12:23:13.000000 bw2speedups-3.1/bw2speedups.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-26 12:23:13.000000 bw2speedups-3.1/bw2speedups.egg-info/top_level.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       46 2022-11-02 07:56:36.000000 bw2speedups-3.1/pytest.ini
+-rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-26 12:23:13.385680 bw2speedups-3.1/setup.cfg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1725 2023-04-26 12:22:30.000000 bw2speedups-3.1/setup.py
```

### Comparing `bw2speedups-3.0/.github/workflows/build_wheels.yaml` & `bw2speedups-3.1/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/LICENSE` & `bw2speedups-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/PKG-INFO` & `bw2speedups-3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2speedups
-Version: 3.0
+Version: 3.1
 Summary: Cython functions to speed up Brightway2 LCA calculations
 Home-page: https://github.com/brightway-lca/brightway2-speedups
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bw2speedups-3.0/README.md` & `bw2speedups-3.1/README.md`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/bw2speedups/_consolidate.c` & `bw2speedups-3.1/bw2speedups/_indexer.c`

 * *Files 2% similar despite different names*

```diff
@@ -734,16 +734,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__bw2speedups___consolidate
-#define __PYX_HAVE_API__bw2speedups___consolidate
+#define __PYX_HAVE__bw2speedups___indexer
+#define __PYX_HAVE_API__bw2speedups___indexer
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
 #include "numpy/ufuncobject.h"
 #ifdef _OPENMP
 #include <omp.h>
@@ -972,15 +972,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "bw2speedups/_consolidate.pyx",
+  "bw2speedups/_indexer.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
@@ -1202,31 +1202,22 @@
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 
-/* "bw2speedups/_consolidate.pyx":10
- * VTYPE = np.float64
+/* "bw2speedups/_indexer.pyx":8
  * 
- * ctypedef np.int64_t TTYPE_t             # <<<<<<<<<<<<<<
- * ctypedef np.float64_t VTYPE_t
- * 
- */
-typedef __pyx_t_5numpy_int64_t __pyx_t_11bw2speedups_12_consolidate_TTYPE_t;
-
-/* "bw2speedups/_consolidate.pyx":11
- * 
- * ctypedef np.int64_t TTYPE_t
- * ctypedef np.float64_t VTYPE_t             # <<<<<<<<<<<<<<
+ * DTYPE = np.uint32
+ * ctypedef np.uint32_t DTYPE_t             # <<<<<<<<<<<<<<
  * 
  * try:
  */
-typedef __pyx_t_5numpy_float64_t __pyx_t_11bw2speedups_12_consolidate_VTYPE_t;
+typedef __pyx_t_5numpy_uint32_t __pyx_t_11bw2speedups_8_indexer_DTYPE_t;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
@@ -1498,21 +1489,14 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1527,17 +1511,14 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
@@ -1596,14 +1577,17 @@
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
 /* RaiseNoneIterError.proto */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
 
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1795,24 +1779,27 @@
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_uint32(npy_uint32 value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
@@ -1860,162 +1847,140 @@
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'cython' */
 
-/* Module declarations from 'bw2speedups._consolidate' */
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_TTYPE_t = { "TTYPE_t", NULL, sizeof(__pyx_t_11bw2speedups_12_consolidate_TTYPE_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_11bw2speedups_12_consolidate_TTYPE_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_11bw2speedups_12_consolidate_TTYPE_t), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_VTYPE_t = { "VTYPE_t", NULL, sizeof(__pyx_t_11bw2speedups_12_consolidate_VTYPE_t), { 0 }, 0, 'R', 0, 0 };
-#define __Pyx_MODULE_NAME "bw2speedups._consolidate"
-extern int __pyx_module_is_main_bw2speedups___consolidate;
-int __pyx_module_is_main_bw2speedups___consolidate = 0;
+/* Module declarations from 'bw2speedups._indexer' */
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_11bw2speedups_8_indexer_DTYPE_t = { "DTYPE_t", NULL, sizeof(__pyx_t_11bw2speedups_8_indexer_DTYPE_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_11bw2speedups_8_indexer_DTYPE_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_11bw2speedups_8_indexer_DTYPE_t), 0 };
+#define __Pyx_MODULE_NAME "bw2speedups._indexer"
+extern int __pyx_module_is_main_bw2speedups___indexer;
+int __pyx_module_is_main_bw2speedups___indexer = 0;
 
-/* Implementation of 'bw2speedups._consolidate' */
+/* Implementation of 'bw2speedups._indexer' */
 static PyObject *__pyx_builtin_xrange;
 static PyObject *__pyx_builtin_NameError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
-static const char __pyx_k_c[] = "c";
-static const char __pyx_k_d[] = "d";
+static const char __pyx_k_x[] = "x";
 static const char __pyx_k_np[] = "np";
-static const char __pyx_k_sum[] = "sum";
+static const char __pyx_k_get[] = "get";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
-static const char __pyx_k_sort[] = "sort";
-static const char __pyx_k_take[] = "take";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_view[] = "view";
-static const char __pyx_k_TTYPE[] = "TTYPE";
-static const char __pyx_k_VTYPE[] = "VTYPE";
-static const char __pyx_k_dtype[] = "dtype";
-static const char __pyx_k_index[] = "index";
-static const char __pyx_k_int64[] = "int64";
+static const char __pyx_k_DTYPE[] = "DTYPE";
+static const char __pyx_k_b_max[] = "b_max";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
-static const char __pyx_k_shape[] = "shape";
-static const char __pyx_k_where[] = "where";
-static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_import[] = "__import__";
-static const char __pyx_k_unique[] = "unique";
+static const char __pyx_k_uint32[] = "uint32";
 static const char __pyx_k_xrange[] = "xrange";
-static const char __pyx_k_float64[] = "float64";
+static const char __pyx_k_indexer[] = "indexer";
+static const char __pyx_k_mapping[] = "mapping";
 static const char __pyx_k_range_2[] = "_range";
 static const char __pyx_k_NameError[] = "NameError";
-static const char __pyx_k_new_shape[] = "new_shape";
+static const char __pyx_k_MAX_INT_32[] = "MAX_INT_32";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_ImportError[] = "ImportError";
-static const char __pyx_k_consolidate[] = "consolidate";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
-static const char __pyx_k_index_values[] = "index_values";
-static const char __pyx_k_timedelta64_s[] = "timedelta64[s]";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_bw2speedups__consolidate[] = "bw2speedups._consolidate";
+static const char __pyx_k_bw2speedups__indexer[] = "bw2speedups._indexer";
+static const char __pyx_k_bw2speedups__indexer_pyx[] = "bw2speedups/_indexer.pyx";
 static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
-static const char __pyx_k_bw2speedups__consolidate_pyx[] = "bw2speedups/_consolidate.pyx";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
 static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
 static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
 static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
+static PyObject *__pyx_n_s_DTYPE;
 static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
 static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_n_s_ImportError;
+static PyObject *__pyx_n_s_MAX_INT_32;
 static PyObject *__pyx_n_s_NameError;
 static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
 static PyObject *__pyx_n_s_RuntimeError;
-static PyObject *__pyx_n_s_TTYPE;
-static PyObject *__pyx_n_s_VTYPE;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_b;
-static PyObject *__pyx_n_s_bw2speedups__consolidate;
-static PyObject *__pyx_kp_s_bw2speedups__consolidate_pyx;
-static PyObject *__pyx_n_s_c;
+static PyObject *__pyx_n_s_b_max;
+static PyObject *__pyx_n_s_bw2speedups__indexer;
+static PyObject *__pyx_kp_s_bw2speedups__indexer_pyx;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_consolidate;
-static PyObject *__pyx_n_s_d;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_float64;
+static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_index;
-static PyObject *__pyx_n_s_index_values;
-static PyObject *__pyx_n_s_int64;
+static PyObject *__pyx_n_s_indexer;
 static PyObject *__pyx_n_s_main;
+static PyObject *__pyx_n_s_mapping;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
 static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
-static PyObject *__pyx_n_s_new_shape;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_range_2;
-static PyObject *__pyx_n_s_shape;
-static PyObject *__pyx_n_s_sort;
-static PyObject *__pyx_n_s_sum;
-static PyObject *__pyx_n_s_take;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_kp_u_timedelta64_s;
-static PyObject *__pyx_n_s_unique;
+static PyObject *__pyx_n_s_uint32;
 static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
-static PyObject *__pyx_n_s_view;
-static PyObject *__pyx_n_s_where;
+static PyObject *__pyx_n_s_x;
 static PyObject *__pyx_n_s_xrange;
-static PyObject *__pyx_n_s_zeros;
-static PyObject *__pyx_pf_11bw2speedups_12_consolidate_consolidate(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b); /* proto */
+static PyObject *__pyx_pf_11bw2speedups_8_indexer_indexer(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b, PyObject *__pyx_v_mapping); /* proto */
 static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_codeobj__9;
 /* Late includes */
 
-/* "bw2speedups/_consolidate.pyx":19
+/* "bw2speedups/_indexer.pyx":17
  * 
  * @cython.boundscheck(False)
- * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
- *                 np.ndarray[VTYPE_t, ndim=1] b):
- *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
+ * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
+ *             mapping):
+ *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11bw2speedups_12_consolidate_1consolidate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_11bw2speedups_12_consolidate_consolidate[] = "Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.\n\n    For example:\n\n    .. code-block:: python\n\n        import numpy as np\n        a = np.array((0.5, 1, 2, 2, -1, -1)).astype('timedelta64[s]')\n        b = np.arange(6).astype(float)\n\n    Would return:\n\n    .. code-block:: python\n\n        np.array([-1, 0.5, 1, 2], dtype='timedelta64[s]'),\n        np.array((9, 0, 1, 5))\n\n    ``a``, the index array, must by one-dimensional NumPy arrays with dtype ``timedelta64[s]`` and ``b``, the value array, must by one-dimensional NumPy arrays with dtype ``float64``.\n\n    Returns:\n        Consolidated sorted index array and consolidated values array.\n\n    ";
-static PyMethodDef __pyx_mdef_11bw2speedups_12_consolidate_1consolidate = {"consolidate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11bw2speedups_12_consolidate_1consolidate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11bw2speedups_12_consolidate_consolidate};
-static PyObject *__pyx_pw_11bw2speedups_12_consolidate_1consolidate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_11bw2speedups_8_indexer_1indexer(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_11bw2speedups_8_indexer_indexer[] = "Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.\n\n    Modifies numpy arrays in place.\n\n    Much faster than plain python because of direct access without conversion to Numpy array.";
+static PyMethodDef __pyx_mdef_11bw2speedups_8_indexer_1indexer = {"indexer", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11bw2speedups_8_indexer_1indexer, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11bw2speedups_8_indexer_indexer};
+static PyObject *__pyx_pw_11bw2speedups_8_indexer_1indexer(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_a = 0;
   PyArrayObject *__pyx_v_b = 0;
+  PyObject *__pyx_v_mapping = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("consolidate (wrapper)", 0);
+  __Pyx_RefNannySetupContext("indexer (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_a,&__pyx_n_s_b,0};
-    PyObject* values[2] = {0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_a,&__pyx_n_s_b,&__pyx_n_s_mapping,0};
+    PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -2024,524 +1989,305 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("consolidate", 1, 2, 2, 1); __PYX_ERR(0, 19, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("indexer", 1, 3, 3, 1); __PYX_ERR(0, 17, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mapping)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("indexer", 1, 3, 3, 2); __PYX_ERR(0, 17, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "consolidate") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "indexer") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_a = ((PyArrayObject *)values[0]);
     __pyx_v_b = ((PyArrayObject *)values[1]);
+    __pyx_v_mapping = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("consolidate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("indexer", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 17, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("bw2speedups._consolidate.consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bw2speedups._indexer.indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 19, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_5numpy_ndarray, 1, "b", 0))) __PYX_ERR(0, 20, __pyx_L1_error)
-  __pyx_r = __pyx_pf_11bw2speedups_12_consolidate_consolidate(__pyx_self, __pyx_v_a, __pyx_v_b);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_5numpy_ndarray, 1, "b", 0))) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_r = __pyx_pf_11bw2speedups_8_indexer_indexer(__pyx_self, __pyx_v_a, __pyx_v_b, __pyx_v_mapping);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11bw2speedups_12_consolidate_consolidate(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b) {
-  PyObject *__pyx_v_index_values = NULL;
-  int __pyx_v_new_shape;
-  PyArrayObject *__pyx_v_c = 0;
-  PyArrayObject *__pyx_v_d = 0;
-  PyObject *__pyx_v_index = NULL;
+static PyObject *__pyx_pf_11bw2speedups_8_indexer_indexer(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b, PyObject *__pyx_v_mapping) {
+  __pyx_t_11bw2speedups_8_indexer_DTYPE_t __pyx_v_MAX_INT_32;
+  int __pyx_v_b_max;
+  PyObject *__pyx_v_x = NULL;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_a;
   __Pyx_Buffer __pyx_pybuffer_a;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_b;
   __Pyx_Buffer __pyx_pybuffer_b;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_c;
-  __Pyx_Buffer __pyx_pybuffer_c;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_d;
-  __Pyx_Buffer __pyx_pybuffer_d;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyArrayObject *__pyx_t_6 = NULL;
-  PyArrayObject *__pyx_t_7 = NULL;
-  Py_ssize_t __pyx_t_8;
-  PyObject *(*__pyx_t_9)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  Py_ssize_t __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
-  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("consolidate", 0);
-  __pyx_pybuffer_c.pybuffer.buf = NULL;
-  __pyx_pybuffer_c.refcount = 0;
-  __pyx_pybuffernd_c.data = NULL;
-  __pyx_pybuffernd_c.rcbuffer = &__pyx_pybuffer_c;
-  __pyx_pybuffer_d.pybuffer.buf = NULL;
-  __pyx_pybuffer_d.refcount = 0;
-  __pyx_pybuffernd_d.data = NULL;
-  __pyx_pybuffernd_d.rcbuffer = &__pyx_pybuffer_d;
+  __Pyx_RefNannySetupContext("indexer", 0);
   __pyx_pybuffer_a.pybuffer.buf = NULL;
   __pyx_pybuffer_a.refcount = 0;
   __pyx_pybuffernd_a.data = NULL;
   __pyx_pybuffernd_a.rcbuffer = &__pyx_pybuffer_a;
   __pyx_pybuffer_b.pybuffer.buf = NULL;
   __pyx_pybuffer_b.refcount = 0;
   __pyx_pybuffernd_b.data = NULL;
   __pyx_pybuffernd_b.rcbuffer = &__pyx_pybuffer_b;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_TTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 19, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_8_indexer_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 17, __pyx_L1_error)
   }
   __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b.rcbuffer->pybuffer, (PyObject*)__pyx_v_b, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_VTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 19, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b.rcbuffer->pybuffer, (PyObject*)__pyx_v_b, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_8_indexer_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 17, __pyx_L1_error)
   }
   __pyx_pybuffernd_b.diminfo[0].strides = __pyx_pybuffernd_b.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_b.diminfo[0].shape = __pyx_pybuffernd_b.rcbuffer->pybuffer.shape[0];
 
-  /* "bw2speedups/_consolidate.pyx":46
- *     #integration of timedelta based on http://stackoverflow.com/questions/33522626/using-datetime-and-bool-in-cython
- *     #it works with view so `times.view('int64')` has to be passed to consolidate instead of `times`
- *     assert a.shape[0] == b.shape[0]             # <<<<<<<<<<<<<<
- *     index_values = np.unique(a)
- *     index_values.sort()
- */
-  #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!(((__pyx_v_a->dimensions[0]) == (__pyx_v_b->dimensions[0])) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 46, __pyx_L1_error)
-    }
-  }
-  #endif
-
-  /* "bw2speedups/_consolidate.pyx":47
- *     #it works with view so `times.view('int64')` has to be passed to consolidate instead of `times`
- *     assert a.shape[0] == b.shape[0]
- *     index_values = np.unique(a)             # <<<<<<<<<<<<<<
- *     index_values.sort()
- *     cdef int new_shape = index_values.shape[0]
+  /* "bw2speedups/_indexer.pyx":24
+ * 
+ *     Much faster than plain python because of direct access without conversion to Numpy array."""
+ *     cdef DTYPE_t MAX_INT_32 = 4294967295             # <<<<<<<<<<<<<<
+ *     cdef int b_max = b.shape[0]
+ *     for x in _range(b_max):
+ */
+  __pyx_v_MAX_INT_32 = 0xFFFFFFFF;
+
+  /* "bw2speedups/_indexer.pyx":25
+ *     Much faster than plain python because of direct access without conversion to Numpy array."""
+ *     cdef DTYPE_t MAX_INT_32 = 4294967295
+ *     cdef int b_max = b.shape[0]             # <<<<<<<<<<<<<<
+ *     for x in _range(b_max):
+ *         b[x] = mapping.get(a[x], MAX_INT_32)
+ */
+  __pyx_v_b_max = (__pyx_v_b->dimensions[0]);
+
+  /* "bw2speedups/_indexer.pyx":26
+ *     cdef DTYPE_t MAX_INT_32 = 4294967295
+ *     cdef int b_max = b.shape[0]
+ *     for x in _range(b_max):             # <<<<<<<<<<<<<<
+ *         b[x] = mapping.get(a[x], MAX_INT_32)
+ *     return True
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_range_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_unique); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_b_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, ((PyObject *)__pyx_v_a)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_a));
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_index_values = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  /* "bw2speedups/_consolidate.pyx":48
- *     assert a.shape[0] == b.shape[0]
- *     index_values = np.unique(a)
- *     index_values.sort()             # <<<<<<<<<<<<<<
- *     cdef int new_shape = index_values.shape[0]
- *     cdef np.ndarray[TTYPE_t, ndim=1] c = \
- */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_values, __pyx_n_s_sort); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "bw2speedups/_consolidate.pyx":49
- *     index_values = np.unique(a)
- *     index_values.sort()
- *     cdef int new_shape = index_values.shape[0]             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[TTYPE_t, ndim=1] c = \
- *             np.zeros(new_shape, dtype=TTYPE)
- */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_values, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_new_shape = __pyx_t_4;
-
-  /* "bw2speedups/_consolidate.pyx":51
- *     cdef int new_shape = index_values.shape[0]
- *     cdef np.ndarray[TTYPE_t, ndim=1] c = \
- *             np.zeros(new_shape, dtype=TTYPE)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[VTYPE_t, ndim=1] d = \
- *             np.zeros(new_shape, dtype=VTYPE)
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_new_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_TTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_TTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-      __pyx_v_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_c.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 50, __pyx_L1_error)
-    } else {__pyx_pybuffernd_c.diminfo[0].strides = __pyx_pybuffernd_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_c.diminfo[0].shape = __pyx_pybuffernd_c.rcbuffer->pybuffer.shape[0];
-    }
-  }
-  __pyx_t_6 = 0;
-  __pyx_v_c = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
-
-  /* "bw2speedups/_consolidate.pyx":53
- *             np.zeros(new_shape, dtype=TTYPE)
- *     cdef np.ndarray[VTYPE_t, ndim=1] d = \
- *             np.zeros(new_shape, dtype=VTYPE)             # <<<<<<<<<<<<<<
- * 
- *     for index in _range(new_shape):
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_new_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
-  __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_VTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 53, __pyx_L1_error)
-  __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_d.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_VTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-      __pyx_v_d = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_d.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 52, __pyx_L1_error)
-    } else {__pyx_pybuffernd_d.diminfo[0].strides = __pyx_pybuffernd_d.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_d.diminfo[0].shape = __pyx_pybuffernd_d.rcbuffer->pybuffer.shape[0];
-    }
-  }
-  __pyx_t_7 = 0;
-  __pyx_v_d = ((PyArrayObject *)__pyx_t_1);
-  __pyx_t_1 = 0;
-
-  /* "bw2speedups/_consolidate.pyx":55
- *             np.zeros(new_shape, dtype=VTYPE)
- * 
- *     for index in _range(new_shape):             # <<<<<<<<<<<<<<
- *         c[index] = index_values[index]
- *         d[index] = b.take(np.where(a == index_values[index])).sum()
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_range_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_new_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-    __pyx_t_5 = __pyx_t_1; __Pyx_INCREF(__pyx_t_5); __pyx_t_8 = 0;
-    __pyx_t_9 = NULL;
+    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
+    __pyx_t_6 = NULL;
   } else {
-    __pyx_t_8 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 55, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 26, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
-    if (likely(!__pyx_t_9)) {
-      if (likely(PyList_CheckExact(__pyx_t_5))) {
-        if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_5)) break;
+    if (likely(!__pyx_t_6)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 26, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
-        if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 26, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
-      __pyx_t_1 = __pyx_t_9(__pyx_t_5);
+      __pyx_t_1 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 55, __pyx_L1_error)
+          else __PYX_ERR(0, 26, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
-    __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_1);
+    __Pyx_XDECREF_SET(__pyx_v_x, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "bw2speedups/_consolidate.pyx":56
- * 
- *     for index in _range(new_shape):
- *         c[index] = index_values[index]             # <<<<<<<<<<<<<<
- *         d[index] = b.take(np.where(a == index_values[index])).sum()
- *     #c.view need to be reconverted to 'timedelta64[s]' in __mul__ and __add__
- */
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_index_values, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_c), __pyx_v_index, __pyx_t_1) < 0)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-    /* "bw2speedups/_consolidate.pyx":57
- *     for index in _range(new_shape):
- *         c[index] = index_values[index]
- *         d[index] = b.take(np.where(a == index_values[index])).sum()             # <<<<<<<<<<<<<<
- *     #c.view need to be reconverted to 'timedelta64[s]' in __mul__ and __add__
- *     return c.view('timedelta64[s]'), d
+    /* "bw2speedups/_indexer.pyx":27
+ *     cdef int b_max = b.shape[0]
+ *     for x in _range(b_max):
+ *         b[x] = mapping.get(a[x], MAX_INT_32)             # <<<<<<<<<<<<<<
+ *     return True
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_take); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_mapping, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_where); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_v_index_values, __pyx_v_index); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_13 = PyObject_RichCompare(((PyObject *)__pyx_v_a), __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
-      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_12);
-      if (likely(__pyx_t_11)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-        __Pyx_INCREF(__pyx_t_11);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_12, function);
-      }
-    }
-    __pyx_t_10 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_11, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_13);
-    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = NULL;
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_a), __pyx_v_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_7 = __Pyx_PyInt_From_npy_uint32(__pyx_v_MAX_INT_32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_8 = NULL;
+    __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_12)) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_12);
+        __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_9 = 1;
       }
     }
-    __pyx_t_2 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_12, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_10);
-    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_2);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_3)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_7};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_7};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      if (__pyx_t_8) {
+        __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
+      __Pyx_GIVEREF(__pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_4);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_7);
+      __pyx_t_4 = 0;
+      __pyx_t_7 = 0;
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
-    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_d), __pyx_v_index, __pyx_t_1) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_b), __pyx_v_x, __pyx_t_1) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bw2speedups/_consolidate.pyx":55
- *             np.zeros(new_shape, dtype=VTYPE)
- * 
- *     for index in _range(new_shape):             # <<<<<<<<<<<<<<
- *         c[index] = index_values[index]
- *         d[index] = b.take(np.where(a == index_values[index])).sum()
+    /* "bw2speedups/_indexer.pyx":26
+ *     cdef DTYPE_t MAX_INT_32 = 4294967295
+ *     cdef int b_max = b.shape[0]
+ *     for x in _range(b_max):             # <<<<<<<<<<<<<<
+ *         b[x] = mapping.get(a[x], MAX_INT_32)
+ *     return True
  */
   }
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bw2speedups/_consolidate.pyx":59
- *         d[index] = b.take(np.where(a == index_values[index])).sum()
- *     #c.view need to be reconverted to 'timedelta64[s]' in __mul__ and __add__
- *     return c.view('timedelta64[s]'), d             # <<<<<<<<<<<<<<
+  /* "bw2speedups/_indexer.pyx":28
+ *     for x in _range(b_max):
+ *         b[x] = mapping.get(a[x], MAX_INT_32)
+ *     return True             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_c), __pyx_n_s_view); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
-    }
-  }
-  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_u_timedelta64_s) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_timedelta64_s);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
-  __Pyx_INCREF(((PyObject *)__pyx_v_d));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_d));
-  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_d));
-  __pyx_t_5 = 0;
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __Pyx_INCREF(Py_True);
+  __pyx_r = Py_True;
   goto __pyx_L0;
 
-  /* "bw2speedups/_consolidate.pyx":19
+  /* "bw2speedups/_indexer.pyx":17
  * 
  * @cython.boundscheck(False)
- * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
- *                 np.ndarray[VTYPE_t, ndim=1] b):
- *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
+ * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
+ *             mapping):
+ *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_13);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_c.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_d.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("bw2speedups._consolidate.consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bw2speedups._indexer.indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_c.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_d.rcbuffer->pybuffer);
   __pyx_L2:;
-  __Pyx_XDECREF(__pyx_v_index_values);
-  __Pyx_XDECREF((PyObject *)__pyx_v_c);
-  __Pyx_XDECREF((PyObject *)__pyx_v_d);
-  __Pyx_XDECREF(__pyx_v_index);
+  __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":258
  *         # experimental exception made for __getbuffer__ and __releasebuffer__
@@ -4994,25 +4740,25 @@
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec__consolidate(PyObject* module); /*proto*/
+static int __pyx_pymod_exec__indexer(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec__consolidate},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__indexer},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "_consolidate",
+    "_indexer",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -5033,70 +4779,58 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_n_s_DTYPE, __pyx_k_DTYPE, sizeof(__pyx_k_DTYPE), 0, 0, 1, 1},
   {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
   {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+  {&__pyx_n_s_MAX_INT_32, __pyx_k_MAX_INT_32, sizeof(__pyx_k_MAX_INT_32), 0, 0, 1, 1},
   {&__pyx_n_s_NameError, __pyx_k_NameError, sizeof(__pyx_k_NameError), 0, 0, 1, 1},
   {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
-  {&__pyx_n_s_TTYPE, __pyx_k_TTYPE, sizeof(__pyx_k_TTYPE), 0, 0, 1, 1},
-  {&__pyx_n_s_VTYPE, __pyx_k_VTYPE, sizeof(__pyx_k_VTYPE), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
-  {&__pyx_n_s_bw2speedups__consolidate, __pyx_k_bw2speedups__consolidate, sizeof(__pyx_k_bw2speedups__consolidate), 0, 0, 1, 1},
-  {&__pyx_kp_s_bw2speedups__consolidate_pyx, __pyx_k_bw2speedups__consolidate_pyx, sizeof(__pyx_k_bw2speedups__consolidate_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
+  {&__pyx_n_s_b_max, __pyx_k_b_max, sizeof(__pyx_k_b_max), 0, 0, 1, 1},
+  {&__pyx_n_s_bw2speedups__indexer, __pyx_k_bw2speedups__indexer, sizeof(__pyx_k_bw2speedups__indexer), 0, 0, 1, 1},
+  {&__pyx_kp_s_bw2speedups__indexer_pyx, __pyx_k_bw2speedups__indexer_pyx, sizeof(__pyx_k_bw2speedups__indexer_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_consolidate, __pyx_k_consolidate, sizeof(__pyx_k_consolidate), 0, 0, 1, 1},
-  {&__pyx_n_s_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
+  {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
-  {&__pyx_n_s_index_values, __pyx_k_index_values, sizeof(__pyx_k_index_values), 0, 0, 1, 1},
-  {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
+  {&__pyx_n_s_indexer, __pyx_k_indexer, sizeof(__pyx_k_indexer), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+  {&__pyx_n_s_mapping, __pyx_k_mapping, sizeof(__pyx_k_mapping), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
   {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
-  {&__pyx_n_s_new_shape, __pyx_k_new_shape, sizeof(__pyx_k_new_shape), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_range_2, __pyx_k_range_2, sizeof(__pyx_k_range_2), 0, 0, 1, 1},
-  {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
-  {&__pyx_n_s_sort, __pyx_k_sort, sizeof(__pyx_k_sort), 0, 0, 1, 1},
-  {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
-  {&__pyx_n_s_take, __pyx_k_take, sizeof(__pyx_k_take), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_kp_u_timedelta64_s, __pyx_k_timedelta64_s, sizeof(__pyx_k_timedelta64_s), 0, 1, 0, 0},
-  {&__pyx_n_s_unique, __pyx_k_unique, sizeof(__pyx_k_unique), 0, 0, 1, 1},
+  {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
   {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
-  {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
-  {&__pyx_n_s_where, __pyx_k_where, sizeof(__pyx_k_where), 0, 0, 1, 1},
+  {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {&__pyx_n_s_xrange, __pyx_k_xrange, sizeof(__pyx_k_xrange), 0, 0, 1, 1},
-  {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   #if PY_MAJOR_VERSION >= 3
-  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_xrange) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_xrange) __PYX_ERR(0, 11, __pyx_L1_error)
   #else
-  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 11, __pyx_L1_error)
   #endif
-  __pyx_builtin_NameError = __Pyx_GetBuiltinName(__pyx_n_s_NameError); if (!__pyx_builtin_NameError) __PYX_ERR(0, 15, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_builtin_NameError = __Pyx_GetBuiltinName(__pyx_n_s_NameError); if (!__pyx_builtin_NameError) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 13, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 272, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 855, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1037, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -5178,25 +4912,25 @@
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1043, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "bw2speedups/_consolidate.pyx":19
+  /* "bw2speedups/_indexer.pyx":17
  * 
  * @cython.boundscheck(False)
- * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
- *                 np.ndarray[VTYPE_t, ndim=1] b):
- *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
+ * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
+ *             mapping):
+ *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
  */
-  __pyx_tuple__8 = PyTuple_Pack(7, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_index_values, __pyx_n_s_new_shape, __pyx_n_s_c, __pyx_n_s_d, __pyx_n_s_index); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(6, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_mapping, __pyx_n_s_MAX_INT_32, __pyx_n_s_b_max, __pyx_n_s_x); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bw2speedups__consolidate_pyx, __pyx_n_s_consolidate, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bw2speedups__indexer_pyx, __pyx_n_s_indexer, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5318,19 +5052,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC init_consolidate(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC init_consolidate(void)
+__Pyx_PyMODINIT_FUNC init_indexer(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC init_indexer(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit__consolidate(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit__consolidate(void)
+__Pyx_PyMODINIT_FUNC PyInit__indexer(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit__indexer(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -5389,15 +5123,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec__consolidate(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec__indexer(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -5407,30 +5141,30 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module '_consolidate' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module '_indexer' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__consolidate(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__indexer(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5459,15 +5193,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("_consolidate", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("_indexer", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -5477,22 +5211,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_bw2speedups___consolidate) {
+  if (__pyx_module_is_main_bw2speedups___indexer) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "bw2speedups._consolidate")) {
-      if (unlikely(PyDict_SetItemString(modules, "bw2speedups._consolidate", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "bw2speedups._indexer")) {
+      if (unlikely(PyDict_SetItemString(modules, "bw2speedups._indexer", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5505,130 +5239,115 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bw2speedups/_consolidate.pyx":3
+  /* "bw2speedups/_indexer.pyx":3
  * #cython: language_level=3
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * cimport cython
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bw2speedups/_consolidate.pyx":7
+  /* "bw2speedups/_indexer.pyx":7
  * cimport cython
  * 
- * TTYPE= np.int64             # <<<<<<<<<<<<<<
- * VTYPE = np.float64
+ * DTYPE = np.uint32             # <<<<<<<<<<<<<<
+ * ctypedef np.uint32_t DTYPE_t
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TTYPE, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bw2speedups/_consolidate.pyx":8
- * 
- * TTYPE= np.int64
- * VTYPE = np.float64             # <<<<<<<<<<<<<<
- * 
- * ctypedef np.int64_t TTYPE_t
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DTYPE, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_VTYPE, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bw2speedups/_consolidate.pyx":13
- * ctypedef np.float64_t VTYPE_t
+  /* "bw2speedups/_indexer.pyx":10
+ * ctypedef np.uint32_t DTYPE_t
  * 
  * try:             # <<<<<<<<<<<<<<
  *     _range = xrange
  * except NameError:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "bw2speedups/_consolidate.pyx":14
+      /* "bw2speedups/_indexer.pyx":11
  * 
  * try:
  *     _range = xrange             # <<<<<<<<<<<<<<
  * except NameError:
  *     _range = range
  */
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_xrange) < 0) __PYX_ERR(0, 14, __pyx_L2_error)
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_xrange) < 0) __PYX_ERR(0, 11, __pyx_L2_error)
 
-      /* "bw2speedups/_consolidate.pyx":13
- * ctypedef np.float64_t VTYPE_t
+      /* "bw2speedups/_indexer.pyx":10
+ * ctypedef np.uint32_t DTYPE_t
  * 
  * try:             # <<<<<<<<<<<<<<
  *     _range = xrange
  * except NameError:
  */
     }
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L7_try_end;
     __pyx_L2_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bw2speedups/_consolidate.pyx":15
+    /* "bw2speedups/_indexer.pyx":12
  * try:
  *     _range = xrange
  * except NameError:             # <<<<<<<<<<<<<<
  *     _range = range
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_NameError);
     if (__pyx_t_6) {
-      __Pyx_AddTraceback("bw2speedups._consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_7) < 0) __PYX_ERR(0, 15, __pyx_L4_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_AddTraceback("bw2speedups._indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_7) < 0) __PYX_ERR(0, 12, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "bw2speedups/_consolidate.pyx":16
+      /* "bw2speedups/_indexer.pyx":13
  *     _range = xrange
  * except NameError:
  *     _range = range             # <<<<<<<<<<<<<<
  * 
- * @cython.boundscheck(False)
+ * 
  */
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_range) < 0) __PYX_ERR(0, 16, __pyx_L4_except_error)
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_range) < 0) __PYX_ERR(0, 13, __pyx_L4_except_error)
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L3_exception_handled;
     }
     goto __pyx_L4_except_error;
     __pyx_L4_except_error:;
 
-    /* "bw2speedups/_consolidate.pyx":13
- * ctypedef np.float64_t VTYPE_t
+    /* "bw2speedups/_indexer.pyx":10
+ * ctypedef np.uint32_t DTYPE_t
  * 
  * try:             # <<<<<<<<<<<<<<
  *     _range = xrange
  * except NameError:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
@@ -5639,27 +5358,27 @@
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     __pyx_L7_try_end:;
   }
 
-  /* "bw2speedups/_consolidate.pyx":19
+  /* "bw2speedups/_indexer.pyx":17
  * 
  * @cython.boundscheck(False)
- * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
- *                 np.ndarray[VTYPE_t, ndim=1] b):
- *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
+ * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
+ *             mapping):
+ *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
  */
-  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_11bw2speedups_12_consolidate_1consolidate, NULL, __pyx_n_s_bw2speedups__consolidate); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_11bw2speedups_8_indexer_1indexer, NULL, __pyx_n_s_bw2speedups__indexer); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_consolidate, __pyx_t_7) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_indexer, __pyx_t_7) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "bw2speedups/_consolidate.pyx":1
+  /* "bw2speedups/_indexer.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * import numpy as np
  */
   __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5678,19 +5397,19 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init bw2speedups._consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init bw2speedups._indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init bw2speedups._consolidate");
+    PyErr_SetString(PyExc_ImportError, "init bw2speedups._indexer");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -6776,36 +6495,14 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
 /* GetItemInt */
   static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -6885,27 +6582,14 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
-/* ExtTypeTest */
-  static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* ObjectGetItem */
   #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
     PyObject *runerr;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
@@ -7152,14 +6836,27 @@
 }
 
 /* RaiseNoneIterError */
   static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
+/* ExtTypeTest */
+  static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -7684,37 +7381,15 @@
         else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
-  /* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
-/* Declarations */
+  /* Declarations */
   #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
@@ -8014,48 +7689,108 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
+/* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
+        if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(long) <= sizeof(long)) {
+        if (sizeof(int) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_uint32(npy_uint32 value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const npy_uint32 neg_one = (npy_uint32) -1, const_zero = (npy_uint32) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(npy_uint32) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(npy_uint32) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(npy_uint32) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(npy_uint32) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(npy_uint32) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(npy_uint32),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
@@ -8249,85 +7984,85 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `bw2speedups-3.0/bw2speedups/_consolidate.pyx` & `bw2speedups-3.1/bw2speedups/_consolidate.pyx`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/bw2speedups/_find_first.c` & `bw2speedups-3.1/bw2speedups/_find_first.c`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/bw2speedups/_find_first.pyx` & `bw2speedups-3.1/bw2speedups/_find_first.pyx`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/bw2speedups/_indexer.c` & `bw2speedups-3.1/bw2speedups/_consolidate.c`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,15 +83,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -548,35 +548,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -734,21 +734,27 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__bw2speedups___indexer
-#define __PYX_HAVE_API__bw2speedups___indexer
+#define __PYX_HAVE__bw2speedups___consolidate
+#define __PYX_HAVE_API__bw2speedups___consolidate
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
+
+    /* NumPy API declarations from "numpy/__init__.pxd" */
+    
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -972,15 +978,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "bw2speedups/_indexer.pyx",
+  "bw2speedups/_consolidate.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
@@ -1013,211 +1019,220 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":775
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":776
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":777
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":778
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":782
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":783
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":784
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":785
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":789
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":790
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":799
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":800
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":801
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":803
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":804
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":805
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":807
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":808
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":810
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":811
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":812
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 
-/* "bw2speedups/_indexer.pyx":8
+/* "bw2speedups/_consolidate.pyx":10
+ * VTYPE = np.float64
+ * 
+ * ctypedef np.int64_t TTYPE_t             # <<<<<<<<<<<<<<
+ * ctypedef np.float64_t VTYPE_t
  * 
- * DTYPE = np.uint32
- * ctypedef np.uint32_t DTYPE_t             # <<<<<<<<<<<<<<
+ */
+typedef __pyx_t_5numpy_int64_t __pyx_t_11bw2speedups_12_consolidate_TTYPE_t;
+
+/* "bw2speedups/_consolidate.pyx":11
+ * 
+ * ctypedef np.int64_t TTYPE_t
+ * ctypedef np.float64_t VTYPE_t             # <<<<<<<<<<<<<<
  * 
  * try:
  */
-typedef __pyx_t_5numpy_uint32_t __pyx_t_11bw2speedups_8_indexer_DTYPE_t;
+typedef __pyx_t_5numpy_float64_t __pyx_t_11bw2speedups_12_consolidate_VTYPE_t;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
@@ -1237,42 +1252,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":814
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":815
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":816
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":818
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1414,26 +1429,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1489,14 +1504,21 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
+/* PyObjectCallNoArg.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+#else
+#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+#endif
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1511,14 +1533,17 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
@@ -1554,40 +1579,14 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1612,23 +1611,34 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -1779,27 +1789,21 @@
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_uint32(npy_uint32 value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
@@ -1842,145 +1846,151 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *, char *, char *, int *); /*proto*/
 
 /* Module declarations from 'cython' */
 
-/* Module declarations from 'bw2speedups._indexer' */
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_11bw2speedups_8_indexer_DTYPE_t = { "DTYPE_t", NULL, sizeof(__pyx_t_11bw2speedups_8_indexer_DTYPE_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_11bw2speedups_8_indexer_DTYPE_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_11bw2speedups_8_indexer_DTYPE_t), 0 };
-#define __Pyx_MODULE_NAME "bw2speedups._indexer"
-extern int __pyx_module_is_main_bw2speedups___indexer;
-int __pyx_module_is_main_bw2speedups___indexer = 0;
+/* Module declarations from 'bw2speedups._consolidate' */
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_TTYPE_t = { "TTYPE_t", NULL, sizeof(__pyx_t_11bw2speedups_12_consolidate_TTYPE_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_11bw2speedups_12_consolidate_TTYPE_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_11bw2speedups_12_consolidate_TTYPE_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_VTYPE_t = { "VTYPE_t", NULL, sizeof(__pyx_t_11bw2speedups_12_consolidate_VTYPE_t), { 0 }, 0, 'R', 0, 0 };
+#define __Pyx_MODULE_NAME "bw2speedups._consolidate"
+extern int __pyx_module_is_main_bw2speedups___consolidate;
+int __pyx_module_is_main_bw2speedups___consolidate = 0;
 
-/* Implementation of 'bw2speedups._indexer' */
+/* Implementation of 'bw2speedups._consolidate' */
 static PyObject *__pyx_builtin_xrange;
 static PyObject *__pyx_builtin_NameError;
 static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
-static const char __pyx_k_x[] = "x";
+static const char __pyx_k_c[] = "c";
+static const char __pyx_k_d[] = "d";
 static const char __pyx_k_np[] = "np";
-static const char __pyx_k_get[] = "get";
+static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_sort[] = "sort";
+static const char __pyx_k_take[] = "take";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_DTYPE[] = "DTYPE";
-static const char __pyx_k_b_max[] = "b_max";
+static const char __pyx_k_view[] = "view";
+static const char __pyx_k_TTYPE[] = "TTYPE";
+static const char __pyx_k_VTYPE[] = "VTYPE";
+static const char __pyx_k_dtype[] = "dtype";
+static const char __pyx_k_index[] = "index";
+static const char __pyx_k_int64[] = "int64";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
+static const char __pyx_k_shape[] = "shape";
+static const char __pyx_k_where[] = "where";
+static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_import[] = "__import__";
-static const char __pyx_k_uint32[] = "uint32";
+static const char __pyx_k_unique[] = "unique";
 static const char __pyx_k_xrange[] = "xrange";
-static const char __pyx_k_indexer[] = "indexer";
-static const char __pyx_k_mapping[] = "mapping";
+static const char __pyx_k_float64[] = "float64";
 static const char __pyx_k_range_2[] = "_range";
 static const char __pyx_k_NameError[] = "NameError";
-static const char __pyx_k_MAX_INT_32[] = "MAX_INT_32";
-static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_new_shape[] = "new_shape";
 static const char __pyx_k_ImportError[] = "ImportError";
-static const char __pyx_k_RuntimeError[] = "RuntimeError";
+static const char __pyx_k_consolidate[] = "consolidate";
+static const char __pyx_k_index_values[] = "index_values";
+static const char __pyx_k_timedelta64_D[] = "timedelta64[D]";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_bw2speedups__indexer[] = "bw2speedups._indexer";
-static const char __pyx_k_bw2speedups__indexer_pyx[] = "bw2speedups/_indexer.pyx";
-static const char __pyx_k_ndarray_is_not_C_contiguous[] = "ndarray is not C contiguous";
+static const char __pyx_k_bw2speedups__consolidate[] = "bw2speedups._consolidate";
+static const char __pyx_k_bw2speedups__consolidate_pyx[] = "bw2speedups/_consolidate.pyx";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
-static const char __pyx_k_unknown_dtype_code_in_numpy_pxd[] = "unknown dtype code in numpy.pxd (%d)";
-static const char __pyx_k_Format_string_allocated_too_shor[] = "Format string allocated too short, see comment in numpy.pxd";
-static const char __pyx_k_Non_native_byte_order_not_suppor[] = "Non-native byte order not supported";
-static const char __pyx_k_ndarray_is_not_Fortran_contiguou[] = "ndarray is not Fortran contiguous";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static const char __pyx_k_Format_string_allocated_too_shor_2[] = "Format string allocated too short.";
-static PyObject *__pyx_n_s_DTYPE;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor;
-static PyObject *__pyx_kp_u_Format_string_allocated_too_shor_2;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_MAX_INT_32;
 static PyObject *__pyx_n_s_NameError;
-static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
-static PyObject *__pyx_n_s_RuntimeError;
-static PyObject *__pyx_n_s_ValueError;
+static PyObject *__pyx_n_s_TTYPE;
+static PyObject *__pyx_n_s_VTYPE;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_b;
-static PyObject *__pyx_n_s_b_max;
-static PyObject *__pyx_n_s_bw2speedups__indexer;
-static PyObject *__pyx_kp_s_bw2speedups__indexer_pyx;
+static PyObject *__pyx_n_s_bw2speedups__consolidate;
+static PyObject *__pyx_kp_s_bw2speedups__consolidate_pyx;
+static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_get;
+static PyObject *__pyx_n_s_consolidate;
+static PyObject *__pyx_n_s_d;
+static PyObject *__pyx_n_s_dtype;
+static PyObject *__pyx_n_s_float64;
 static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_indexer;
+static PyObject *__pyx_n_s_index;
+static PyObject *__pyx_n_s_index_values;
+static PyObject *__pyx_n_s_int64;
 static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_mapping;
 static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_kp_u_ndarray_is_not_C_contiguous;
-static PyObject *__pyx_kp_u_ndarray_is_not_Fortran_contiguou;
+static PyObject *__pyx_n_s_new_shape;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_range_2;
+static PyObject *__pyx_n_s_shape;
+static PyObject *__pyx_n_s_sort;
+static PyObject *__pyx_n_s_sum;
+static PyObject *__pyx_n_s_take;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_uint32;
-static PyObject *__pyx_kp_u_unknown_dtype_code_in_numpy_pxd;
-static PyObject *__pyx_n_s_x;
+static PyObject *__pyx_kp_u_timedelta64_D;
+static PyObject *__pyx_n_s_unique;
+static PyObject *__pyx_n_s_view;
+static PyObject *__pyx_n_s_where;
 static PyObject *__pyx_n_s_xrange;
-static PyObject *__pyx_pf_11bw2speedups_8_indexer_indexer(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b, PyObject *__pyx_v_mapping); /* proto */
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
+static PyObject *__pyx_n_s_zeros;
+static PyObject *__pyx_pf_11bw2speedups_12_consolidate_consolidate(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__4;
 /* Late includes */
 
-/* "bw2speedups/_indexer.pyx":17
+/* "bw2speedups/_consolidate.pyx":19
  * 
  * @cython.boundscheck(False)
- * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
- *             mapping):
- *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
+ * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
+ *                 np.ndarray[VTYPE_t, ndim=1] b):
+ *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_11bw2speedups_8_indexer_1indexer(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_11bw2speedups_8_indexer_indexer[] = "Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.\n\n    Modifies numpy arrays in place.\n\n    Much faster than plain python because of direct access without conversion to Numpy array.";
-static PyMethodDef __pyx_mdef_11bw2speedups_8_indexer_1indexer = {"indexer", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11bw2speedups_8_indexer_1indexer, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11bw2speedups_8_indexer_indexer};
-static PyObject *__pyx_pw_11bw2speedups_8_indexer_1indexer(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_11bw2speedups_12_consolidate_1consolidate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_11bw2speedups_12_consolidate_consolidate[] = "Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.\n\n    For example:\n\n    .. code-block:: python\n\n        import numpy as np\n        a = np.array((0.5, 1, 2, 2, -1, -1)).astype('timedelta64[s]')\n        b = np.arange(6).astype(float)\n\n    Would return:\n\n    .. code-block:: python\n\n        np.array([-1, 0.5, 1, 2], dtype='timedelta64[s]'),\n        np.array((9, 0, 1, 5))\n\n    ``a``, the index array, must by one-dimensional NumPy arrays with dtype ``timedelta64[s]`` and ``b``, the value array, must by one-dimensional NumPy arrays with dtype ``float64``.\n\n    Returns:\n        Consolidated sorted index array and consolidated values array.\n\n    ";
+static PyMethodDef __pyx_mdef_11bw2speedups_12_consolidate_1consolidate = {"consolidate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11bw2speedups_12_consolidate_1consolidate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11bw2speedups_12_consolidate_consolidate};
+static PyObject *__pyx_pw_11bw2speedups_12_consolidate_1consolidate(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_a = 0;
   PyArrayObject *__pyx_v_b = 0;
-  PyObject *__pyx_v_mapping = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("indexer (wrapper)", 0);
+  __Pyx_RefNannySetupContext("consolidate (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_a,&__pyx_n_s_b,&__pyx_n_s_mapping,0};
-    PyObject* values[3] = {0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_a,&__pyx_n_s_b,0};
+    PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -1989,1170 +1999,529 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("indexer", 1, 3, 3, 1); __PYX_ERR(0, 17, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mapping)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("indexer", 1, 3, 3, 2); __PYX_ERR(0, 17, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("consolidate", 1, 2, 2, 1); __PYX_ERR(0, 19, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "indexer") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "consolidate") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_a = ((PyArrayObject *)values[0]);
     __pyx_v_b = ((PyArrayObject *)values[1]);
-    __pyx_v_mapping = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("indexer", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 17, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("consolidate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("bw2speedups._indexer.indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bw2speedups._consolidate.consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 17, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_5numpy_ndarray, 1, "b", 0))) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_r = __pyx_pf_11bw2speedups_8_indexer_indexer(__pyx_self, __pyx_v_a, __pyx_v_b, __pyx_v_mapping);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_5numpy_ndarray, 1, "b", 0))) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_r = __pyx_pf_11bw2speedups_12_consolidate_consolidate(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_11bw2speedups_8_indexer_indexer(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b, PyObject *__pyx_v_mapping) {
-  __pyx_t_11bw2speedups_8_indexer_DTYPE_t __pyx_v_MAX_INT_32;
-  int __pyx_v_b_max;
-  PyObject *__pyx_v_x = NULL;
+static PyObject *__pyx_pf_11bw2speedups_12_consolidate_consolidate(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_b) {
+  PyObject *__pyx_v_index_values = NULL;
+  int __pyx_v_new_shape;
+  PyArrayObject *__pyx_v_c = 0;
+  PyArrayObject *__pyx_v_d = 0;
+  PyObject *__pyx_v_index = NULL;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_a;
   __Pyx_Buffer __pyx_pybuffer_a;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_b;
   __Pyx_Buffer __pyx_pybuffer_b;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_c;
+  __Pyx_Buffer __pyx_pybuffer_c;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_d;
+  __Pyx_Buffer __pyx_pybuffer_d;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyArrayObject *__pyx_t_6 = NULL;
+  PyArrayObject *__pyx_t_7 = NULL;
+  Py_ssize_t __pyx_t_8;
+  PyObject *(*__pyx_t_9)(PyObject *);
   PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("indexer", 0);
+  __Pyx_RefNannySetupContext("consolidate", 0);
+  __pyx_pybuffer_c.pybuffer.buf = NULL;
+  __pyx_pybuffer_c.refcount = 0;
+  __pyx_pybuffernd_c.data = NULL;
+  __pyx_pybuffernd_c.rcbuffer = &__pyx_pybuffer_c;
+  __pyx_pybuffer_d.pybuffer.buf = NULL;
+  __pyx_pybuffer_d.refcount = 0;
+  __pyx_pybuffernd_d.data = NULL;
+  __pyx_pybuffernd_d.rcbuffer = &__pyx_pybuffer_d;
   __pyx_pybuffer_a.pybuffer.buf = NULL;
   __pyx_pybuffer_a.refcount = 0;
   __pyx_pybuffernd_a.data = NULL;
   __pyx_pybuffernd_a.rcbuffer = &__pyx_pybuffer_a;
   __pyx_pybuffer_b.pybuffer.buf = NULL;
   __pyx_pybuffer_b.refcount = 0;
   __pyx_pybuffernd_b.data = NULL;
   __pyx_pybuffernd_b.rcbuffer = &__pyx_pybuffer_b;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_8_indexer_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 17, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_TTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 19, __pyx_L1_error)
   }
   __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b.rcbuffer->pybuffer, (PyObject*)__pyx_v_b, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_8_indexer_DTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 17, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b.rcbuffer->pybuffer, (PyObject*)__pyx_v_b, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_VTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 19, __pyx_L1_error)
   }
   __pyx_pybuffernd_b.diminfo[0].strides = __pyx_pybuffernd_b.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_b.diminfo[0].shape = __pyx_pybuffernd_b.rcbuffer->pybuffer.shape[0];
 
-  /* "bw2speedups/_indexer.pyx":24
- * 
- *     Much faster than plain python because of direct access without conversion to Numpy array."""
- *     cdef DTYPE_t MAX_INT_32 = 4294967295             # <<<<<<<<<<<<<<
- *     cdef int b_max = b.shape[0]
- *     for x in _range(b_max):
- */
-  __pyx_v_MAX_INT_32 = 0xFFFFFFFF;
-
-  /* "bw2speedups/_indexer.pyx":25
- *     Much faster than plain python because of direct access without conversion to Numpy array."""
- *     cdef DTYPE_t MAX_INT_32 = 4294967295
- *     cdef int b_max = b.shape[0]             # <<<<<<<<<<<<<<
- *     for x in _range(b_max):
- *         b[x] = mapping.get(a[x], MAX_INT_32)
- */
-  __pyx_v_b_max = (__pyx_v_b->dimensions[0]);
-
-  /* "bw2speedups/_indexer.pyx":26
- *     cdef DTYPE_t MAX_INT_32 = 4294967295
- *     cdef int b_max = b.shape[0]
- *     for x in _range(b_max):             # <<<<<<<<<<<<<<
- *         b[x] = mapping.get(a[x], MAX_INT_32)
- *     return True
+  /* "bw2speedups/_consolidate.pyx":46
+ *     #integration of timedelta based on http://stackoverflow.com/questions/33522626/using-datetime-and-bool-in-cython
+ *     #it works with view so `times.view('int64')` has to be passed to consolidate instead of `times`
+ *     assert a.shape[0] == b.shape[0]             # <<<<<<<<<<<<<<
+ *     index_values = np.unique(a)
+ *     index_values.sort()
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(!(((__pyx_v_a->dimensions[0]) == (__pyx_v_b->dimensions[0])) != 0))) {
+      PyErr_SetNone(PyExc_AssertionError);
+      __PYX_ERR(0, 46, __pyx_L1_error)
+    }
+  }
+  #endif
+
+  /* "bw2speedups/_consolidate.pyx":47
+ *     #it works with view so `times.view('int64')` has to be passed to consolidate instead of `times`
+ *     assert a.shape[0] == b.shape[0]
+ *     index_values = np.unique(a)             # <<<<<<<<<<<<<<
+ *     index_values.sort()
+ *     cdef int new_shape = index_values.shape[0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_range_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_b_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_unique); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, ((PyObject *)__pyx_v_a)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_a));
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_index_values = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "bw2speedups/_consolidate.pyx":48
+ *     assert a.shape[0] == b.shape[0]
+ *     index_values = np.unique(a)
+ *     index_values.sort()             # <<<<<<<<<<<<<<
+ *     cdef int new_shape = index_values.shape[0]
+ *     cdef np.ndarray[TTYPE_t, ndim=1] c = \
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_values, __pyx_n_s_sort); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "bw2speedups/_consolidate.pyx":49
+ *     index_values = np.unique(a)
+ *     index_values.sort()
+ *     cdef int new_shape = index_values.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[TTYPE_t, ndim=1] c = \
+ *             np.zeros(new_shape, dtype=TTYPE)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_values, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_new_shape = __pyx_t_4;
+
+  /* "bw2speedups/_consolidate.pyx":51
+ *     cdef int new_shape = index_values.shape[0]
+ *     cdef np.ndarray[TTYPE_t, ndim=1] c = \
+ *             np.zeros(new_shape, dtype=TTYPE)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[VTYPE_t, ndim=1] d = \
+ *             np.zeros(new_shape, dtype=VTYPE)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_new_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_TTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_c.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_TTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_c = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_c.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 50, __pyx_L1_error)
+    } else {__pyx_pybuffernd_c.diminfo[0].strides = __pyx_pybuffernd_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_c.diminfo[0].shape = __pyx_pybuffernd_c.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_6 = 0;
+  __pyx_v_c = ((PyArrayObject *)__pyx_t_5);
+  __pyx_t_5 = 0;
+
+  /* "bw2speedups/_consolidate.pyx":53
+ *             np.zeros(new_shape, dtype=TTYPE)
+ *     cdef np.ndarray[VTYPE_t, ndim=1] d = \
+ *             np.zeros(new_shape, dtype=VTYPE)             # <<<<<<<<<<<<<<
+ * 
+ *     for index in _range(new_shape):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_new_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_VTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_d.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_11bw2speedups_12_consolidate_VTYPE_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_d = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_d.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 52, __pyx_L1_error)
+    } else {__pyx_pybuffernd_d.diminfo[0].strides = __pyx_pybuffernd_d.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_d.diminfo[0].shape = __pyx_pybuffernd_d.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_7 = 0;
+  __pyx_v_d = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "bw2speedups/_consolidate.pyx":55
+ *             np.zeros(new_shape, dtype=VTYPE)
+ * 
+ *     for index in _range(new_shape):             # <<<<<<<<<<<<<<
+ *         c[index] = index_values[index]
+ *         d[index] = b.take(np.where(a == index_values[index])).sum()
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_range_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_new_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
-    __pyx_t_6 = NULL;
+    __pyx_t_5 = __pyx_t_1; __Pyx_INCREF(__pyx_t_5); __pyx_t_8 = 0;
+    __pyx_t_9 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __pyx_t_8 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_9 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 55, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
-    if (likely(!__pyx_t_6)) {
-      if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
+    if (likely(!__pyx_t_9)) {
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 26, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
-        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 26, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_1); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
-      __pyx_t_1 = __pyx_t_6(__pyx_t_2);
+      __pyx_t_1 = __pyx_t_9(__pyx_t_5);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 26, __pyx_L1_error)
+          else __PYX_ERR(0, 55, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
-    __Pyx_XDECREF_SET(__pyx_v_x, __pyx_t_1);
+    __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "bw2speedups/_indexer.pyx":27
- *     cdef int b_max = b.shape[0]
- *     for x in _range(b_max):
- *         b[x] = mapping.get(a[x], MAX_INT_32)             # <<<<<<<<<<<<<<
- *     return True
+    /* "bw2speedups/_consolidate.pyx":56
+ * 
+ *     for index in _range(new_shape):
+ *         c[index] = index_values[index]             # <<<<<<<<<<<<<<
+ *         d[index] = b.take(np.where(a == index_values[index])).sum()
+ *     return c.view('timedelta64[D]'), d
+ */
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_index_values, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_c), __pyx_v_index, __pyx_t_1) < 0)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "bw2speedups/_consolidate.pyx":57
+ *     for index in _range(new_shape):
+ *         c[index] = index_values[index]
+ *         d[index] = b.take(np.where(a == index_values[index])).sum()             # <<<<<<<<<<<<<<
+ *     return c.view('timedelta64[D]'), d
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_mapping, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_take); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_a), __pyx_v_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyInt_From_npy_uint32(__pyx_v_MAX_INT_32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 27, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = NULL;
-    __pyx_t_9 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_where); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_v_index_values, __pyx_v_index); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_13 = PyObject_RichCompare(((PyObject *)__pyx_v_a), __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_12);
+      if (likely(__pyx_t_11)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+        __Pyx_INCREF(__pyx_t_11);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_12, function);
+      }
+    }
+    __pyx_t_10 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_11, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_13);
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_8)) {
+      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
-        __pyx_t_9 = 1;
       }
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_7};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_4, __pyx_t_7};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    } else
-    #endif
-    {
-      __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 27, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      if (__pyx_t_8) {
-        __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
+    __pyx_t_2 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_12, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_4);
-      __Pyx_GIVEREF(__pyx_t_7);
-      PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_7);
-      __pyx_t_4 = 0;
-      __pyx_t_7 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
+    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_b), __pyx_v_x, __pyx_t_1) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_d), __pyx_v_index, __pyx_t_1) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "bw2speedups/_indexer.pyx":26
- *     cdef DTYPE_t MAX_INT_32 = 4294967295
- *     cdef int b_max = b.shape[0]
- *     for x in _range(b_max):             # <<<<<<<<<<<<<<
- *         b[x] = mapping.get(a[x], MAX_INT_32)
- *     return True
+    /* "bw2speedups/_consolidate.pyx":55
+ *             np.zeros(new_shape, dtype=VTYPE)
+ * 
+ *     for index in _range(new_shape):             # <<<<<<<<<<<<<<
+ *         c[index] = index_values[index]
+ *         d[index] = b.take(np.where(a == index_values[index])).sum()
  */
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "bw2speedups/_indexer.pyx":28
- *     for x in _range(b_max):
- *         b[x] = mapping.get(a[x], MAX_INT_32)
- *     return True             # <<<<<<<<<<<<<<
+  /* "bw2speedups/_consolidate.pyx":58
+ *         c[index] = index_values[index]
+ *         d[index] = b.take(np.where(a == index_values[index])).sum()
+ *     return c.view('timedelta64[D]'), d             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(Py_True);
-  __pyx_r = Py_True;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_c), __pyx_n_s_view); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
+    }
+  }
+  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_u_timedelta64_D) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_timedelta64_D);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+  __Pyx_INCREF(((PyObject *)__pyx_v_d));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_d));
+  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_d));
+  __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "bw2speedups/_indexer.pyx":17
+  /* "bw2speedups/_consolidate.pyx":19
  * 
  * @cython.boundscheck(False)
- * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
- *             mapping):
- *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
+ * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
+ *                 np.ndarray[VTYPE_t, ndim=1] b):
+ *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_c.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_d.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("bw2speedups._indexer.indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bw2speedups._consolidate.consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_c.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_d.rcbuffer->pybuffer);
   __pyx_L2:;
-  __Pyx_XDECREF(__pyx_v_x);
+  __Pyx_XDECREF(__pyx_v_index_values);
+  __Pyx_XDECREF((PyObject *)__pyx_v_c);
+  __Pyx_XDECREF((PyObject *)__pyx_v_d);
+  __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
-static CYTHON_UNUSED int __pyx_pw_5numpy_7ndarray_1__getbuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5numpy_7ndarray___getbuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_5numpy_7ndarray___getbuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  int __pyx_v_i;
-  int __pyx_v_ndim;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  int __pyx_v_t;
-  char *__pyx_v_f;
-  PyArray_Descr *__pyx_v_descr = 0;
-  int __pyx_v_offset;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  PyArray_Descr *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  if (__pyx_v_info == NULL) {
-    PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
-    return -1;
-  }
-  __Pyx_RefNannySetupContext("__getbuffer__", 0);
-  __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(__pyx_v_info->obj);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":265
- * 
- *             cdef int i, ndim
- *             cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":266
- *             cdef int i, ndim
- *             cdef int endian_detector = 1
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- * 
- *             ndim = PyArray_NDIM(self)
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":268
- *             cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- * 
- *             ndim = PyArray_NDIM(self)             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- */
-  __pyx_v_ndim = PyArray_NDIM(__pyx_v_self);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_C_CONTIGUOUS) == PyBUF_C_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":271
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_C_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 272, __pyx_L1_error)
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":270
- *             ndim = PyArray_NDIM(self)
- * 
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")
- */
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  __pyx_t_2 = (((__pyx_v_flags & PyBUF_F_CONTIGUOUS) == PyBUF_F_CONTIGUOUS) != 0);
-  if (__pyx_t_2) {
-  } else {
-    __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L7_bool_binop_done;
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":275
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):             # <<<<<<<<<<<<<<
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- */
-  __pyx_t_2 = ((!(PyArray_CHKFLAGS(__pyx_v_self, NPY_ARRAY_F_CONTIGUOUS) != 0)) != 0);
-  __pyx_t_1 = __pyx_t_2;
-  __pyx_L7_bool_binop_done:;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  if (unlikely(__pyx_t_1)) {
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 276, __pyx_L1_error)
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":274
- *                 raise ValueError(u"ndarray is not C contiguous")
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)             # <<<<<<<<<<<<<<
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- */
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":278
- *                 raise ValueError(u"ndarray is not Fortran contiguous")
- * 
- *             info.buf = PyArray_DATA(self)             # <<<<<<<<<<<<<<
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_v_info->buf = PyArray_DATA(__pyx_v_self);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":279
- * 
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 # Allocate new buffer for strides and shape info.
- */
-  __pyx_v_info->ndim = __pyx_v_ndim;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":283
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)             # <<<<<<<<<<<<<<
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- */
-    __pyx_v_info->strides = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * 2) * ((size_t)__pyx_v_ndim))));
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":284
- *                 # This is allocated as one block, strides first.
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim             # <<<<<<<<<<<<<<
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- */
-    __pyx_v_info->shape = (__pyx_v_info->strides + __pyx_v_ndim);
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":285
- *                 info.strides = <Py_ssize_t*>PyObject_Malloc(sizeof(Py_ssize_t) * 2 * <size_t>ndim)
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):             # <<<<<<<<<<<<<<
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- */
-    __pyx_t_4 = __pyx_v_ndim;
-    __pyx_t_5 = __pyx_t_4;
-    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-      __pyx_v_i = __pyx_t_6;
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":286
- *                 info.shape = info.strides + ndim
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]             # <<<<<<<<<<<<<<
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- */
-      (__pyx_v_info->strides[__pyx_v_i]) = (PyArray_STRIDES(__pyx_v_self)[__pyx_v_i]);
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":287
- *                 for i in range(ndim):
- *                     info.strides[i] = PyArray_STRIDES(self)[i]
- *                     info.shape[i] = PyArray_DIMS(self)[i]             # <<<<<<<<<<<<<<
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- */
-      (__pyx_v_info->shape[__pyx_v_i]) = (PyArray_DIMS(__pyx_v_self)[__pyx_v_i]);
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":280
- *             info.buf = PyArray_DATA(self)
- *             info.ndim = ndim
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 # Allocate new buffer for strides and shape info.
- *                 # This is allocated as one block, strides first.
- */
-    goto __pyx_L9;
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":289
- *                     info.shape[i] = PyArray_DIMS(self)[i]
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- */
-  /*else*/ {
-    __pyx_v_info->strides = ((Py_ssize_t *)PyArray_STRIDES(__pyx_v_self));
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":290
- *             else:
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)             # <<<<<<<<<<<<<<
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- */
-    __pyx_v_info->shape = ((Py_ssize_t *)PyArray_DIMS(__pyx_v_self));
-  }
-  __pyx_L9:;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":291
- *                 info.strides = <Py_ssize_t*>PyArray_STRIDES(self)
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- */
-  __pyx_v_info->suboffsets = NULL;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":292
- *                 info.shape = <Py_ssize_t*>PyArray_DIMS(self)
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)             # <<<<<<<<<<<<<<
- *             info.readonly = not PyArray_ISWRITEABLE(self)
- * 
- */
-  __pyx_v_info->itemsize = PyArray_ITEMSIZE(__pyx_v_self);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":293
- *             info.suboffsets = NULL
- *             info.itemsize = PyArray_ITEMSIZE(self)
- *             info.readonly = not PyArray_ISWRITEABLE(self)             # <<<<<<<<<<<<<<
- * 
- *             cdef int t
- */
-  __pyx_v_info->readonly = (!(PyArray_ISWRITEABLE(__pyx_v_self) != 0));
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":296
- * 
- *             cdef int t
- *             cdef char* f = NULL             # <<<<<<<<<<<<<<
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)
- *             cdef int offset
- */
-  __pyx_v_f = NULL;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":297
- *             cdef int t
- *             cdef char* f = NULL
- *             cdef dtype descr = <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
- *             cdef int offset
- * 
- */
-  __pyx_t_7 = PyArray_DESCR(__pyx_v_self);
-  __pyx_t_3 = ((PyObject *)__pyx_t_7);
-  __Pyx_INCREF(__pyx_t_3);
-  __pyx_v_descr = ((PyArray_Descr *)__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":300
- *             cdef int offset
- * 
- *             info.obj = self             # <<<<<<<<<<<<<<
- * 
- *             if not PyDataType_HASFIELDS(descr):
- */
-  __Pyx_INCREF(((PyObject *)__pyx_v_self));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
-  __Pyx_GOTREF(__pyx_v_info->obj);
-  __Pyx_DECREF(__pyx_v_info->obj);
-  __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  __pyx_t_1 = ((!(PyDataType_HASFIELDS(__pyx_v_descr) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":303
- * 
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num             # <<<<<<<<<<<<<<
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- */
-    __pyx_t_4 = __pyx_v_descr->type_num;
-    __pyx_v_t = __pyx_t_4;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '>') != 0);
-    if (!__pyx_t_2) {
-      goto __pyx_L15_next_or;
-    } else {
-    }
-    __pyx_t_2 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_L15_next_or:;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":305
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- */
-    __pyx_t_2 = ((__pyx_v_descr->byteorder == '<') != 0);
-    if (__pyx_t_2) {
-    } else {
-      __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L14_bool_binop_done;
-    }
-    __pyx_t_2 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_1 = __pyx_t_2;
-    __pyx_L14_bool_binop_done:;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_1)) {
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 306, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 306, __pyx_L1_error)
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":304
- *             if not PyDataType_HASFIELDS(descr):
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":307
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- */
-    switch (__pyx_v_t) {
-      case NPY_BYTE:
-      __pyx_v_f = ((char *)"b");
-      break;
-      case NPY_UBYTE:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":308
- *                     raise ValueError(u"Non-native byte order not supported")
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- */
-      __pyx_v_f = ((char *)"B");
-      break;
-      case NPY_SHORT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":309
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- */
-      __pyx_v_f = ((char *)"h");
-      break;
-      case NPY_USHORT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":310
- *                 elif t == NPY_UBYTE:       f = "B"
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- */
-      __pyx_v_f = ((char *)"H");
-      break;
-      case NPY_INT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":311
- *                 elif t == NPY_SHORT:       f = "h"
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- */
-      __pyx_v_f = ((char *)"i");
-      break;
-      case NPY_UINT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":312
- *                 elif t == NPY_USHORT:      f = "H"
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- */
-      __pyx_v_f = ((char *)"I");
-      break;
-      case NPY_LONG:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":313
- *                 elif t == NPY_INT:         f = "i"
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- */
-      __pyx_v_f = ((char *)"l");
-      break;
-      case NPY_ULONG:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":314
- *                 elif t == NPY_UINT:        f = "I"
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- */
-      __pyx_v_f = ((char *)"L");
-      break;
-      case NPY_LONGLONG:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":315
- *                 elif t == NPY_LONG:        f = "l"
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- */
-      __pyx_v_f = ((char *)"q");
-      break;
-      case NPY_ULONGLONG:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":316
- *                 elif t == NPY_ULONG:       f = "L"
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- */
-      __pyx_v_f = ((char *)"Q");
-      break;
-      case NPY_FLOAT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":317
- *                 elif t == NPY_LONGLONG:    f = "q"
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- */
-      __pyx_v_f = ((char *)"f");
-      break;
-      case NPY_DOUBLE:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":318
- *                 elif t == NPY_ULONGLONG:   f = "Q"
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- */
-      __pyx_v_f = ((char *)"d");
-      break;
-      case NPY_LONGDOUBLE:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":319
- *                 elif t == NPY_FLOAT:       f = "f"
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- */
-      __pyx_v_f = ((char *)"g");
-      break;
-      case NPY_CFLOAT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":320
- *                 elif t == NPY_DOUBLE:      f = "d"
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- */
-      __pyx_v_f = ((char *)"Zf");
-      break;
-      case NPY_CDOUBLE:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":321
- *                 elif t == NPY_LONGDOUBLE:  f = "g"
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"
- */
-      __pyx_v_f = ((char *)"Zd");
-      break;
-      case NPY_CLONGDOUBLE:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":322
- *                 elif t == NPY_CFLOAT:      f = "Zf"
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"             # <<<<<<<<<<<<<<
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- */
-      __pyx_v_f = ((char *)"Zg");
-      break;
-      case NPY_OBJECT:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":323
- *                 elif t == NPY_CDOUBLE:     f = "Zd"
- *                 elif t == NPY_CLONGDOUBLE: f = "Zg"
- *                 elif t == NPY_OBJECT:      f = "O"             # <<<<<<<<<<<<<<
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_v_f = ((char *)"O");
-      break;
-      default:
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":325
- *                 elif t == NPY_OBJECT:      f = "O"
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *                 info.format = f
- *                 return
- */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = PyUnicode_Format(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 325, __pyx_L1_error)
-      break;
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":326
- *                 else:
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f             # <<<<<<<<<<<<<<
- *                 return
- *             else:
- */
-    __pyx_v_info->format = __pyx_v_f;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":327
- *                     raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *                 info.format = f
- *                 return             # <<<<<<<<<<<<<<
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":302
- *             info.obj = self
- * 
- *             if not PyDataType_HASFIELDS(descr):             # <<<<<<<<<<<<<<
- *                 t = descr.type_num
- *                 if ((descr.byteorder == c'>' and little_endian) or
- */
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":329
- *                 return
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)             # <<<<<<<<<<<<<<
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- */
-  /*else*/ {
-    __pyx_v_info->format = ((char *)PyObject_Malloc(0xFF));
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":330
- *             else:
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment             # <<<<<<<<<<<<<<
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,
- */
-    (__pyx_v_info->format[0]) = '^';
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":331
- *                 info.format = <char*>PyObject_Malloc(_buffer_format_string_len)
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0             # <<<<<<<<<<<<<<
- *                 f = _util_dtypestring(descr, info.format + 1,
- *                                       info.format + _buffer_format_string_len,
- */
-    __pyx_v_offset = 0;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":332
- *                 info.format[0] = c'^' # Native data types, manual alignment
- *                 offset = 0
- *                 f = _util_dtypestring(descr, info.format + 1,             # <<<<<<<<<<<<<<
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- */
-    __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_descr, (__pyx_v_info->format + 1), (__pyx_v_info->format + 0xFF), (&__pyx_v_offset)); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 332, __pyx_L1_error)
-    __pyx_v_f = __pyx_t_9;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":335
- *                                       info.format + _buffer_format_string_len,
- *                                       &offset)
- *                 f[0] = c'\0' # Terminate format string             # <<<<<<<<<<<<<<
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- */
-    (__pyx_v_f[0]) = '\x00';
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":258
- *         # experimental exception made for __getbuffer__ and __releasebuffer__
- *         # -- the details of this may change.
- *         def __getbuffer__(ndarray self, Py_buffer* info, int flags):             # <<<<<<<<<<<<<<
- *             # This implementation of getbuffer is geared towards Cython
- *             # requirements, and does not yet fulfill the PEP.
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.ndarray.__getbuffer__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  if (__pyx_v_info->obj != NULL) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  goto __pyx_L2;
-  __pyx_L0:;
-  if (__pyx_v_info->obj == Py_None) {
-    __Pyx_GOTREF(__pyx_v_info->obj);
-    __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
-  }
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_descr);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-/* Python wrapper */
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info); /*proto*/
-static CYTHON_UNUSED void __pyx_pw_5numpy_7ndarray_3__releasebuffer__(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__releasebuffer__ (wrapper)", 0);
-  __pyx_pf_5numpy_7ndarray_2__releasebuffer__(((PyArrayObject *)__pyx_v_self), ((Py_buffer *)__pyx_v_info));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-static void __pyx_pf_5numpy_7ndarray_2__releasebuffer__(PyArrayObject *__pyx_v_self, Py_buffer *__pyx_v_info) {
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__releasebuffer__", 0);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  __pyx_t_1 = (PyArray_HASFIELDS(__pyx_v_self) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":339
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)             # <<<<<<<<<<<<<<
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)
- */
-    PyObject_Free(__pyx_v_info->format);
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":338
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):
- *             if PyArray_HASFIELDS(self):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- */
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  __pyx_t_1 = (((sizeof(npy_intp)) != (sizeof(Py_ssize_t))) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":341
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):
- *                 PyObject_Free(info.strides)             # <<<<<<<<<<<<<<
- *                 # info.shape was stored after info.strides in the same block
- * 
- */
-    PyObject_Free(__pyx_v_info->strides);
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":340
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- *             if sizeof(npy_intp) != sizeof(Py_ssize_t):             # <<<<<<<<<<<<<<
- *                 PyObject_Free(info.strides)
- *                 # info.shape was stored after info.strides in the same block
- */
-  }
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":337
- *                 f[0] = c'\0' # Terminate format string
- * 
- *         def __releasebuffer__(ndarray self, Py_buffer* info):             # <<<<<<<<<<<<<<
- *             if PyArray_HASFIELDS(self):
- *                 PyObject_Free(info.format)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":820
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3161,29 +2530,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":821
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":820
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3194,15 +2563,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":823
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3211,29 +2580,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":824
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 824, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":823
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3244,15 +2613,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":826
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3261,29 +2630,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":827
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":826
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3294,15 +2663,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":829
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3311,29 +2680,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":830
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 830, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":829
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3344,15 +2713,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":832
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3361,29 +2730,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":833
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 833, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":832
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3394,966 +2763,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":835
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":836
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":837
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":836
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":839
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:
+ * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":835
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-static CYTHON_INLINE char *__pyx_f_5numpy__util_dtypestring(PyArray_Descr *__pyx_v_descr, char *__pyx_v_f, char *__pyx_v_end, int *__pyx_v_offset) {
-  PyArray_Descr *__pyx_v_child = 0;
-  int __pyx_v_endian_detector;
-  int __pyx_v_little_endian;
-  PyObject *__pyx_v_fields = 0;
-  PyObject *__pyx_v_childname = NULL;
-  PyObject *__pyx_v_new_offset = NULL;
-  PyObject *__pyx_v_t = NULL;
-  char *__pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  long __pyx_t_8;
-  char *__pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_util_dtypestring", 0);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":846
- * 
- *     cdef dtype child
- *     cdef int endian_detector = 1             # <<<<<<<<<<<<<<
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)
- *     cdef tuple fields
- */
-  __pyx_v_endian_detector = 1;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":847
- *     cdef dtype child
- *     cdef int endian_detector = 1
- *     cdef bint little_endian = ((<char*>&endian_detector)[0] != 0)             # <<<<<<<<<<<<<<
- *     cdef tuple fields
- * 
- */
-  __pyx_v_little_endian = ((((char *)(&__pyx_v_endian_detector))[0]) != 0);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  if (unlikely(__pyx_v_descr->names == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(1, 850, __pyx_L1_error)
-  }
-  __pyx_t_1 = __pyx_v_descr->names; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-  for (;;) {
-    if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 850, __pyx_L1_error)
-    #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 850, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_childname, __pyx_t_3);
-    __pyx_t_3 = 0;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":851
- * 
- *     for childname in descr.names:
- *         fields = descr.fields[childname]             # <<<<<<<<<<<<<<
- *         child, new_offset = fields
- * 
- */
-    if (unlikely(__pyx_v_descr->fields == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 851, __pyx_L1_error)
-    }
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_descr->fields, __pyx_v_childname); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(PyTuple_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(1, 851, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_fields, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":852
- *     for childname in descr.names:
- *         fields = descr.fields[childname]
- *         child, new_offset = fields             # <<<<<<<<<<<<<<
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- */
-    if (likely(__pyx_v_fields != Py_None)) {
-      PyObject* sequence = __pyx_v_fields;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 852, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 852, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-    } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 852, __pyx_L1_error)
-    }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_dtype))))) __PYX_ERR(1, 852, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((PyArray_Descr *)__pyx_t_3));
-    __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_new_offset, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_v_new_offset, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 854, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = ((((__pyx_v_end - __pyx_v_f) - ((int)__pyx_t_5)) < 15) != 0);
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 855, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 855, __pyx_L1_error)
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":854
- *         child, new_offset = fields
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:             # <<<<<<<<<<<<<<
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- */
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '>') != 0);
-    if (!__pyx_t_7) {
-      goto __pyx_L8_next_or;
-    } else {
-    }
-    __pyx_t_7 = (__pyx_v_little_endian != 0);
-    if (!__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_L8_next_or:;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":858
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):             # <<<<<<<<<<<<<<
- *             raise ValueError(u"Non-native byte order not supported")
- *             # One could encode it in the format string and have Cython
- */
-    __pyx_t_7 = ((__pyx_v_child->byteorder == '<') != 0);
-    if (__pyx_t_7) {
-    } else {
-      __pyx_t_6 = __pyx_t_7;
-      goto __pyx_L7_bool_binop_done;
-    }
-    __pyx_t_7 = ((!(__pyx_v_little_endian != 0)) != 0);
-    __pyx_t_6 = __pyx_t_7;
-    __pyx_L7_bool_binop_done:;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    if (unlikely(__pyx_t_6)) {
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":859
- *         if ((child.byteorder == c'>' and little_endian) or
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *             # One could encode it in the format string and have Cython
- *             # complain instead, BUT: < and > in format strings also imply
- */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 859, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 859, __pyx_L1_error)
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":857
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")
- * 
- *         if ((child.byteorder == c'>' and little_endian) or             # <<<<<<<<<<<<<<
- *             (child.byteorder == c'<' and not little_endian)):
- *             raise ValueError(u"Non-native byte order not supported")
- */
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":869
- * 
- *         # Output padding bytes
- *         while offset[0] < new_offset:             # <<<<<<<<<<<<<<
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- */
-    while (1) {
-      __pyx_t_3 = __Pyx_PyInt_From_int((__pyx_v_offset[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_new_offset, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 869, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (!__pyx_t_6) break;
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":870
- *         # Output padding bytes
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte             # <<<<<<<<<<<<<<
- *             f += 1
- *             offset[0] += 1
- */
-      (__pyx_v_f[0]) = 0x78;
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":871
- *         while offset[0] < new_offset:
- *             f[0] = 120 # "x"; pad byte
- *             f += 1             # <<<<<<<<<<<<<<
- *             offset[0] += 1
- * 
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":872
- *             f[0] = 120 # "x"; pad byte
- *             f += 1
- *             offset[0] += 1             # <<<<<<<<<<<<<<
- * 
- *         offset[0] += child.itemsize
- */
-      __pyx_t_8 = 0;
-      (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + 1);
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":874
- *             offset[0] += 1
- * 
- *         offset[0] += child.itemsize             # <<<<<<<<<<<<<<
- * 
- *         if not PyDataType_HASFIELDS(child):
- */
-    __pyx_t_8 = 0;
-    (__pyx_v_offset[__pyx_t_8]) = ((__pyx_v_offset[__pyx_t_8]) + __pyx_v_child->elsize);
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-    __pyx_t_6 = ((!(PyDataType_HASFIELDS(__pyx_v_child) != 0)) != 0);
-    if (__pyx_t_6) {
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":877
- * 
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num             # <<<<<<<<<<<<<<
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")
- */
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_child->type_num); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 877, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_XDECREF_SET(__pyx_v_t, __pyx_t_4);
-      __pyx_t_4 = 0;
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      __pyx_t_6 = (((__pyx_v_end - __pyx_v_f) < 5) != 0);
-      if (unlikely(__pyx_t_6)) {
-
-        /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 879, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 879, __pyx_L1_error)
-
-        /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":878
- *         if not PyDataType_HASFIELDS(child):
- *             t = child.type_num
- *             if end - f < 5:             # <<<<<<<<<<<<<<
- *                 raise RuntimeError(u"Format string allocated too short.")
- * 
- */
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":882
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_BYTE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 882, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 98;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":883
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"             # <<<<<<<<<<<<<<
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UBYTE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 883, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":884
- *             if   t == NPY_BYTE:        f[0] =  98 #"b"
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"             # <<<<<<<<<<<<<<
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_SHORT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 884, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x68;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":885
- *             elif t == NPY_UBYTE:       f[0] =  66 #"B"
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"             # <<<<<<<<<<<<<<
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_USHORT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 885, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 72;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":886
- *             elif t == NPY_SHORT:       f[0] = 104 #"h"
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"             # <<<<<<<<<<<<<<
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_INT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 886, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x69;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":887
- *             elif t == NPY_USHORT:      f[0] =  72 #"H"
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_UINT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 887, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 73;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":888
- *             elif t == NPY_INT:         f[0] = 105 #"i"
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 888, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x6C;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":889
- *             elif t == NPY_UINT:        f[0] =  73 #"I"
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 889, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 76;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":890
- *             elif t == NPY_LONG:        f[0] = 108 #"l"
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGLONG); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 890, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x71;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":891
- *             elif t == NPY_ULONG:       f[0] = 76  #"L"
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"             # <<<<<<<<<<<<<<
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_ULONGLONG); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 891, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 81;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":892
- *             elif t == NPY_LONGLONG:    f[0] = 113 #"q"
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"             # <<<<<<<<<<<<<<
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_FLOAT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 892, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x66;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":893
- *             elif t == NPY_ULONGLONG:   f[0] = 81  #"Q"
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"             # <<<<<<<<<<<<<<
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_DOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 893, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x64;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":894
- *             elif t == NPY_FLOAT:       f[0] = 102 #"f"
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"             # <<<<<<<<<<<<<<
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_LONGDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 894, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 0x67;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":895
- *             elif t == NPY_DOUBLE:      f[0] = 100 #"d"
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf             # <<<<<<<<<<<<<<
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CFLOAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 895, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x66;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":896
- *             elif t == NPY_LONGDOUBLE:  f[0] = 103 #"g"
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd             # <<<<<<<<<<<<<<
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CDOUBLE); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 896, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x64;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":897
- *             elif t == NPY_CFLOAT:      f[0] = 90; f[1] = 102; f += 1 # Zf
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg             # <<<<<<<<<<<<<<
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- */
-      __pyx_t_3 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_CLONGDOUBLE); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_t, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 897, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (__pyx_t_6) {
-        (__pyx_v_f[0]) = 90;
-        (__pyx_v_f[1]) = 0x67;
-        __pyx_v_f = (__pyx_v_f + 1);
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":898
- *             elif t == NPY_CDOUBLE:     f[0] = 90; f[1] = 100; f += 1 # Zd
- *             elif t == NPY_CLONGDOUBLE: f[0] = 90; f[1] = 103; f += 1 # Zg
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"             # <<<<<<<<<<<<<<
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- */
-      __pyx_t_4 = __Pyx_PyInt_From_enum__NPY_TYPES(NPY_OBJECT); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_t, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 898, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (likely(__pyx_t_6)) {
-        (__pyx_v_f[0]) = 79;
-        goto __pyx_L15;
-      }
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":900
- *             elif t == NPY_OBJECT:      f[0] = 79 #"O"
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)             # <<<<<<<<<<<<<<
- *             f += 1
- *         else:
- */
-      /*else*/ {
-        __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 900, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(1, 900, __pyx_L1_error)
-      }
-      __pyx_L15:;
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":901
- *             else:
- *                 raise ValueError(u"unknown dtype code in numpy.pxd (%d)" % t)
- *             f += 1             # <<<<<<<<<<<<<<
- *         else:
- *             # Cython ignores struct boundary information ("T{...}"),
- */
-      __pyx_v_f = (__pyx_v_f + 1);
-
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":876
- *         offset[0] += child.itemsize
- * 
- *         if not PyDataType_HASFIELDS(child):             # <<<<<<<<<<<<<<
- *             t = child.type_num
- *             if end - f < 5:
- */
-      goto __pyx_L13;
-    }
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":905
- *             # Cython ignores struct boundary information ("T{...}"),
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)             # <<<<<<<<<<<<<<
- *     return f
- * 
- */
-    /*else*/ {
-      __pyx_t_9 = __pyx_f_5numpy__util_dtypestring(__pyx_v_child, __pyx_v_f, __pyx_v_end, __pyx_v_offset); if (unlikely(__pyx_t_9 == ((char *)NULL))) __PYX_ERR(1, 905, __pyx_L1_error)
-      __pyx_v_f = __pyx_t_9;
-    }
-    __pyx_L13:;
-
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":850
- *     cdef tuple fields
- * 
- *     for childname in descr.names:             # <<<<<<<<<<<<<<
- *         fields = descr.fields[childname]
- *         child, new_offset = fields
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":906
- *             # so don't output it
- *             f = _util_dtypestring(child, f, end, offset)
- *     return f             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_f;
-  goto __pyx_L0;
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":841
- *         return ()
- * 
- * cdef inline char* _util_dtypestring(dtype descr, char* f, char* end, int* offset) except NULL:             # <<<<<<<<<<<<<<
- *     # Recursive utility function used in __getbuffer__ to get format
- *     # string. The new location in the format string is returned.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("numpy._util_dtypestring", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_fields);
-  __Pyx_XDECREF(__pyx_v_childname);
-  __Pyx_XDECREF(__pyx_v_new_offset);
-  __Pyx_XDECREF(__pyx_v_t);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1022
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1023
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1021
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1026
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1028
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1027
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1029
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1025
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -4364,105 +2984,105 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1035
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
- *         _import_array()             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1035, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1036
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1036, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":944
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1037, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1034
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
- *         _import_array()
+ *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1033
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
- *         _import_array()
+ *         __pyx_import_array()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -4472,15 +3092,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4496,15 +3116,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4512,84 +3132,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1041
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1041, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1042
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1042, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1043, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1040
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1039
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4604,15 +3224,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4628,15 +3248,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4644,81 +3264,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1047
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 1047, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1048
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
+ * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 1048, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1049
+      /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 1049, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1046
+    /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1045
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4733,32 +3356,206 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":966
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":978
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":966
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":981
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":993
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":981
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":996
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":996
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec__indexer(PyObject* module); /*proto*/
+static int __pyx_pymod_exec__consolidate(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec__indexer},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__consolidate},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "_indexer",
+    "_consolidate",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -4779,167 +3576,114 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_DTYPE, __pyx_k_DTYPE, sizeof(__pyx_k_DTYPE), 0, 0, 1, 1},
-  {&__pyx_kp_u_Format_string_allocated_too_shor, __pyx_k_Format_string_allocated_too_shor, sizeof(__pyx_k_Format_string_allocated_too_shor), 0, 1, 0, 0},
-  {&__pyx_kp_u_Format_string_allocated_too_shor_2, __pyx_k_Format_string_allocated_too_shor_2, sizeof(__pyx_k_Format_string_allocated_too_shor_2), 0, 1, 0, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_MAX_INT_32, __pyx_k_MAX_INT_32, sizeof(__pyx_k_MAX_INT_32), 0, 0, 1, 1},
   {&__pyx_n_s_NameError, __pyx_k_NameError, sizeof(__pyx_k_NameError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
-  {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+  {&__pyx_n_s_TTYPE, __pyx_k_TTYPE, sizeof(__pyx_k_TTYPE), 0, 0, 1, 1},
+  {&__pyx_n_s_VTYPE, __pyx_k_VTYPE, sizeof(__pyx_k_VTYPE), 0, 0, 1, 1},
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
-  {&__pyx_n_s_b_max, __pyx_k_b_max, sizeof(__pyx_k_b_max), 0, 0, 1, 1},
-  {&__pyx_n_s_bw2speedups__indexer, __pyx_k_bw2speedups__indexer, sizeof(__pyx_k_bw2speedups__indexer), 0, 0, 1, 1},
-  {&__pyx_kp_s_bw2speedups__indexer_pyx, __pyx_k_bw2speedups__indexer_pyx, sizeof(__pyx_k_bw2speedups__indexer_pyx), 0, 0, 1, 0},
+  {&__pyx_n_s_bw2speedups__consolidate, __pyx_k_bw2speedups__consolidate, sizeof(__pyx_k_bw2speedups__consolidate), 0, 0, 1, 1},
+  {&__pyx_kp_s_bw2speedups__consolidate_pyx, __pyx_k_bw2speedups__consolidate_pyx, sizeof(__pyx_k_bw2speedups__consolidate_pyx), 0, 0, 1, 0},
+  {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
+  {&__pyx_n_s_consolidate, __pyx_k_consolidate, sizeof(__pyx_k_consolidate), 0, 0, 1, 1},
+  {&__pyx_n_s_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 1, 1},
+  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+  {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_indexer, __pyx_k_indexer, sizeof(__pyx_k_indexer), 0, 0, 1, 1},
+  {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
+  {&__pyx_n_s_index_values, __pyx_k_index_values, sizeof(__pyx_k_index_values), 0, 0, 1, 1},
+  {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_mapping, __pyx_k_mapping, sizeof(__pyx_k_mapping), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_kp_u_ndarray_is_not_C_contiguous, __pyx_k_ndarray_is_not_C_contiguous, sizeof(__pyx_k_ndarray_is_not_C_contiguous), 0, 1, 0, 0},
-  {&__pyx_kp_u_ndarray_is_not_Fortran_contiguou, __pyx_k_ndarray_is_not_Fortran_contiguou, sizeof(__pyx_k_ndarray_is_not_Fortran_contiguou), 0, 1, 0, 0},
+  {&__pyx_n_s_new_shape, __pyx_k_new_shape, sizeof(__pyx_k_new_shape), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_range_2, __pyx_k_range_2, sizeof(__pyx_k_range_2), 0, 0, 1, 1},
+  {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
+  {&__pyx_n_s_sort, __pyx_k_sort, sizeof(__pyx_k_sort), 0, 0, 1, 1},
+  {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
+  {&__pyx_n_s_take, __pyx_k_take, sizeof(__pyx_k_take), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
-  {&__pyx_kp_u_unknown_dtype_code_in_numpy_pxd, __pyx_k_unknown_dtype_code_in_numpy_pxd, sizeof(__pyx_k_unknown_dtype_code_in_numpy_pxd), 0, 1, 0, 0},
-  {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
+  {&__pyx_kp_u_timedelta64_D, __pyx_k_timedelta64_D, sizeof(__pyx_k_timedelta64_D), 0, 1, 0, 0},
+  {&__pyx_n_s_unique, __pyx_k_unique, sizeof(__pyx_k_unique), 0, 0, 1, 1},
+  {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
+  {&__pyx_n_s_where, __pyx_k_where, sizeof(__pyx_k_where), 0, 0, 1, 1},
   {&__pyx_n_s_xrange, __pyx_k_xrange, sizeof(__pyx_k_xrange), 0, 0, 1, 1},
+  {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   #if PY_MAJOR_VERSION >= 3
-  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_xrange) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_xrange) __PYX_ERR(0, 14, __pyx_L1_error)
   #else
-  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 14, __pyx_L1_error)
   #endif
-  __pyx_builtin_NameError = __Pyx_GetBuiltinName(__pyx_n_s_NameError); if (!__pyx_builtin_NameError) __PYX_ERR(0, 12, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 13, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 272, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 855, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 1037, __pyx_L1_error)
+  __pyx_builtin_NameError = __Pyx_GetBuiltinName(__pyx_n_s_NameError); if (!__pyx_builtin_NameError) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":272
- *             if ((flags & pybuf.PyBUF_C_CONTIGUOUS == pybuf.PyBUF_C_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_C_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not C contiguous")             # <<<<<<<<<<<<<<
- * 
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_C_contiguous); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 272, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":276
- *             if ((flags & pybuf.PyBUF_F_CONTIGUOUS == pybuf.PyBUF_F_CONTIGUOUS)
- *                 and not PyArray_CHKFLAGS(self, NPY_ARRAY_F_CONTIGUOUS)):
- *                 raise ValueError(u"ndarray is not Fortran contiguous")             # <<<<<<<<<<<<<<
- * 
- *             info.buf = PyArray_DATA(self)
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_ndarray_is_not_Fortran_contiguou); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 276, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":306
- *                 if ((descr.byteorder == c'>' and little_endian) or
- *                     (descr.byteorder == c'<' and not little_endian)):
- *                     raise ValueError(u"Non-native byte order not supported")             # <<<<<<<<<<<<<<
- *                 if   t == NPY_BYTE:        f = "b"
- *                 elif t == NPY_UBYTE:       f = "B"
- */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Non_native_byte_order_not_suppor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":855
- * 
- *         if (end - f) - <int>(new_offset - offset[0]) < 15:
- *             raise RuntimeError(u"Format string allocated too short, see comment in numpy.pxd")             # <<<<<<<<<<<<<<
- * 
- *         if ((child.byteorder == c'>' and little_endian) or
- */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 855, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":879
- *             t = child.type_num
- *             if end - f < 5:
- *                 raise RuntimeError(u"Format string allocated too short.")             # <<<<<<<<<<<<<<
- * 
- *             # Until ticket #99 is fixed, use integers to avoid warnings
- */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Format_string_allocated_too_shor_2); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 879, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1037
- *         _import_array()
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":944
+ *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1037, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1043
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 1043, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "bw2speedups/_indexer.pyx":17
+  /* "bw2speedups/_consolidate.pyx":19
  * 
  * @cython.boundscheck(False)
- * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
- *             mapping):
- *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
- */
-  __pyx_tuple__8 = PyTuple_Pack(6, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_mapping, __pyx_n_s_MAX_INT_32, __pyx_n_s_b_max, __pyx_n_s_x); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bw2speedups__indexer_pyx, __pyx_n_s_indexer, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 17, __pyx_L1_error)
+ * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
+ *                 np.ndarray[VTYPE_t, ndim=1] b):
+ *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
+ */
+  __pyx_tuple__3 = PyTuple_Pack(7, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_index_values, __pyx_n_s_new_shape, __pyx_n_s_c, __pyx_n_s_d, __pyx_n_s_index); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bw2speedups__consolidate_pyx, __pyx_n_s_consolidate, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -4989,33 +3733,68 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 206, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 233, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 242, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 917, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5052,19 +3831,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC init_indexer(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC init_indexer(void)
+__Pyx_PyMODINIT_FUNC init_consolidate(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC init_consolidate(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit__indexer(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit__indexer(void)
+__Pyx_PyMODINIT_FUNC PyInit__consolidate(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit__consolidate(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -5123,15 +3902,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec__indexer(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec__consolidate(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -5141,30 +3920,30 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module '_indexer' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module '_consolidate' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__indexer(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__consolidate(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5193,40 +3972,40 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("_indexer", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("_consolidate", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_bw2speedups___indexer) {
+  if (__pyx_module_is_main_bw2speedups___consolidate) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "bw2speedups._indexer")) {
-      if (unlikely(PyDict_SetItemString(modules, "bw2speedups._indexer", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "bw2speedups._consolidate")) {
+      if (unlikely(PyDict_SetItemString(modules, "bw2speedups._consolidate", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5239,115 +4018,130 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bw2speedups/_indexer.pyx":3
+  /* "bw2speedups/_consolidate.pyx":3
  * #cython: language_level=3
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * cimport cython
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bw2speedups/_indexer.pyx":7
+  /* "bw2speedups/_consolidate.pyx":7
  * cimport cython
  * 
- * DTYPE = np.uint32             # <<<<<<<<<<<<<<
- * ctypedef np.uint32_t DTYPE_t
+ * TTYPE= np.int64             # <<<<<<<<<<<<<<
+ * VTYPE = np.float64
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DTYPE, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TTYPE, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "bw2speedups/_consolidate.pyx":8
+ * 
+ * TTYPE= np.int64
+ * VTYPE = np.float64             # <<<<<<<<<<<<<<
+ * 
+ * ctypedef np.int64_t TTYPE_t
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_VTYPE, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bw2speedups/_indexer.pyx":10
- * ctypedef np.uint32_t DTYPE_t
+  /* "bw2speedups/_consolidate.pyx":13
+ * ctypedef np.float64_t VTYPE_t
  * 
  * try:             # <<<<<<<<<<<<<<
  *     _range = xrange
  * except NameError:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "bw2speedups/_indexer.pyx":11
+      /* "bw2speedups/_consolidate.pyx":14
  * 
  * try:
  *     _range = xrange             # <<<<<<<<<<<<<<
  * except NameError:
  *     _range = range
  */
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_xrange) < 0) __PYX_ERR(0, 11, __pyx_L2_error)
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_xrange) < 0) __PYX_ERR(0, 14, __pyx_L2_error)
 
-      /* "bw2speedups/_indexer.pyx":10
- * ctypedef np.uint32_t DTYPE_t
+      /* "bw2speedups/_consolidate.pyx":13
+ * ctypedef np.float64_t VTYPE_t
  * 
  * try:             # <<<<<<<<<<<<<<
  *     _range = xrange
  * except NameError:
  */
     }
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L7_try_end;
     __pyx_L2_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bw2speedups/_indexer.pyx":12
+    /* "bw2speedups/_consolidate.pyx":15
  * try:
  *     _range = xrange
  * except NameError:             # <<<<<<<<<<<<<<
  *     _range = range
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_NameError);
     if (__pyx_t_6) {
-      __Pyx_AddTraceback("bw2speedups._indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_7) < 0) __PYX_ERR(0, 12, __pyx_L4_except_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_AddTraceback("bw2speedups._consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_7) < 0) __PYX_ERR(0, 15, __pyx_L4_except_error)
       __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "bw2speedups/_indexer.pyx":13
+      /* "bw2speedups/_consolidate.pyx":16
  *     _range = xrange
  * except NameError:
  *     _range = range             # <<<<<<<<<<<<<<
  * 
- * 
+ * @cython.boundscheck(False)
  */
-      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_range) < 0) __PYX_ERR(0, 13, __pyx_L4_except_error)
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (PyDict_SetItem(__pyx_d, __pyx_n_s_range_2, __pyx_builtin_range) < 0) __PYX_ERR(0, 16, __pyx_L4_except_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L3_exception_handled;
     }
     goto __pyx_L4_except_error;
     __pyx_L4_except_error:;
 
-    /* "bw2speedups/_indexer.pyx":10
- * ctypedef np.uint32_t DTYPE_t
+    /* "bw2speedups/_consolidate.pyx":13
+ * ctypedef np.float64_t VTYPE_t
  * 
  * try:             # <<<<<<<<<<<<<<
  *     _range = xrange
  * except NameError:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
@@ -5358,58 +4152,58 @@
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     __pyx_L7_try_end:;
   }
 
-  /* "bw2speedups/_indexer.pyx":17
+  /* "bw2speedups/_consolidate.pyx":19
  * 
  * @cython.boundscheck(False)
- * def indexer(np.ndarray[DTYPE_t, ndim=1] a, np.ndarray[DTYPE_t, ndim=1] b,             # <<<<<<<<<<<<<<
- *             mapping):
- *     """Replace each element of ``b`` with ``mapping.get(a, MAX_INT_32)``.
+ * def consolidate(np.ndarray[TTYPE_t, ndim=1] a,             # <<<<<<<<<<<<<<
+ *                 np.ndarray[VTYPE_t, ndim=1] b):
+ *     """Consolidate an index array and values array, summing elements in the values array for each unique element of the index array.
  */
-  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_11bw2speedups_8_indexer_1indexer, NULL, __pyx_n_s_bw2speedups__indexer); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_11bw2speedups_12_consolidate_1consolidate, NULL, __pyx_n_s_bw2speedups__consolidate); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_indexer, __pyx_t_7) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_consolidate, __pyx_t_7) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "bw2speedups/_indexer.pyx":1
+  /* "bw2speedups/_consolidate.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * import numpy as np
  */
   __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "../../../miniconda3/envs/cython/lib/python3.11/site-packages/Cython/Includes/numpy/__init__.pxd":1045
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../miniconda3/envs/bw25_graph_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init bw2speedups._indexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init bw2speedups._consolidate", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init bw2speedups._indexer");
+    PyErr_SetString(PyExc_ImportError, "init bw2speedups._consolidate");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -6495,14 +5289,36 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
+/* PyObjectCallNoArg */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    }
+#endif
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+#else
+    if (likely(PyCFunction_Check(func)))
+#endif
+    {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+            return __Pyx_PyObject_CallMethO(func, NULL);
+        }
+    }
+    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+}
+#endif
+
 /* GetItemInt */
   static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -6582,18 +5398,31 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* ExtTypeTest */
+  static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
 /* ObjectGetItem */
   #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -6635,228 +5464,14 @@
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
-/* RaiseException */
-  #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
-/* DictGetItem */
-  #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
-/* RaiseTooManyValuesToUnpack */
-  static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-  static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseNoneIterError */
-  static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
-/* ExtTypeTest */
-  static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -7004,48 +5619,225 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
+/* RaiseException */
+  #if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -7132,15 +5924,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -7362,34 +6154,54 @@
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-        if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) return __pyx_pw_5numpy_7ndarray_1__getbuffer__(obj, view, flags);
     PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
         return;
     }
     if ((0)) {}
-        else if (__Pyx_TypeCheck(obj, __pyx_ptype_5numpy_ndarray)) __pyx_pw_5numpy_7ndarray_3__releasebuffer__(obj, view);
     view->obj = NULL;
     Py_DECREF(obj);
 }
 #endif
 
 
-  /* Declarations */
+  /* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
+/* Declarations */
   #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
@@ -7510,15 +6322,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -7664,15 +6476,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -7689,108 +6501,48 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
-/* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_uint32(npy_uint32 value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const npy_uint32 neg_one = (npy_uint32) -1, const_zero = (npy_uint32) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(npy_uint32) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(npy_uint32) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(npy_uint32) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(npy_uint32) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(npy_uint32) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(npy_uint32),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
@@ -7984,85 +6736,47 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__NPY_TYPES(enum NPY_TYPES value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const enum NPY_TYPES neg_one = (enum NPY_TYPES) -1, const_zero = (enum NPY_TYPES) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(enum NPY_TYPES) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(enum NPY_TYPES) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(enum NPY_TYPES) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(enum NPY_TYPES),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
+        if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(long) <= sizeof(long)) {
+        if (sizeof(int) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
+        return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `bw2speedups-3.0/bw2speedups/_indexer.pyx` & `bw2speedups-3.1/bw2speedups/_indexer.pyx`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/bw2speedups/test/test_consolidate.py` & `bw2speedups-3.1/bw2speedups/test/test_consolidate.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,27 @@
     #     self.output_array = np.zeros((5,), dtype=np.uint32)
     #     self.mapping = dict([(x+1, x) for x in range(5)])
     #     self.reference = np.array((4294967295, 0, 1, 2, 3))
 
     def test_main(self):
         # a = np.array((-1, 0, 1)).astype(float)
         # b = np.array((-0.5, 0.5))
-        a = np.array((-2, 0, 2)).astype('timedelta64[s]')
-        b = np.array((-1, 1)).astype('timedelta64[s]')        
+        a = np.array((-2, 0, 2)).astype('timedelta64[D]')
+        b = np.array((-1, 1)).astype('timedelta64[D]')
         c = (a.reshape((-1, 1)) + b.reshape((1, -1))).ravel()
         d = np.arange(6).astype(float)
         # e, f = consolidate(c, d)
         # self.assertTrue(np.allclose(e, np.array((-1.5, -.5, .5, 1.5))))
         e, f = consolidate(c.view('int64'), d)
-        # self.assertTrue(np.allclose(e.astype('timedelta64[s]'), np.array((-3, -1, 1, 3), dtype='timedelta64[s]')))
-        self.assertTrue(np.array_equal(e.astype('timedelta64[s]'), np.array((-3, -1, 1, 3), dtype='timedelta64[s]')))
+        # self.assertTrue(np.allclose(e.astype('timedelta64[D]'), np.array((-3, -1, 1, 3), dtype='timedelta64[D]')))
+        self.assertTrue(np.array_equal(e.astype('timedelta64[D]'), np.array((-3, -1, 1, 3), dtype='timedelta64[D]')))
         self.assertTrue(np.allclose(f, np.array((0, 3, 7, 5))))
 
     def test_shapes(self):
-        #a = np.array((0.5, 1.5, 2.5))
-        #b = np.array((-0.5, 0.5))
-        a = np.array((0.5, 1.5, 2.5)).astype('timedelta64[s]') 
+        a = np.array((0.5, 1.5, 2.5)).astype('timedelta64[D]')
         b = np.array((-0.5, 0.5))
         with self.assertRaises(AssertionError):
             consolidate(a.view('int64'), b)
             #consolidate(a, b)
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `bw2speedups-3.0/bw2speedups/test/test_indexer.py` & `bw2speedups-3.1/bw2speedups/test/test_indexer.py`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/bw2speedups.egg-info/PKG-INFO` & `bw2speedups-3.1/bw2speedups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2speedups
-Version: 3.0
+Version: 3.1
 Summary: Cython functions to speed up Brightway2 LCA calculations
 Home-page: https://github.com/brightway-lca/brightway2-speedups
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bw2speedups-3.0/bw2speedups.egg-info/SOURCES.txt` & `bw2speedups-3.1/bw2speedups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2speedups-3.0/setup.py` & `bw2speedups-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         url="https://github.com/brightway-lca/brightway2-speedups",
         description="""Cython functions to speed up Brightway2 LCA calculations""",
         long_description=open('README.md').read(),
         ext_modules = [extension_1, extension_2, extension_3],
         install_requires=['numpy'],
         name = 'bw2speedups',
         packages=[SRC_DIR],
-        version="3.0",
+        version="3.1",
         zip_safe=False,
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: BSD License',
             'Operating System :: MacOS :: MacOS X',
             'Operating System :: Microsoft :: Windows',
```

