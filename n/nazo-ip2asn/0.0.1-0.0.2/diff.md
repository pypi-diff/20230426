# Comparing `tmp/nazo_ip2asn-0.0.1.tar.gz` & `tmp/nazo_ip2asn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_ip2asn-0.0.1.tar", last modified: Tue Apr 25 16:22:54 2023, max compression
+gzip compressed data, was "nazo_ip2asn-0.0.2.tar", last modified: Wed Apr 26 15:09:16 2023, max compression
```

## Comparing `nazo_ip2asn-0.0.1.tar` & `nazo_ip2asn-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:54.083828 nazo_ip2asn-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-25 16:22:54.083828 nazo_ip2asn-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:54.083828 nazo_ip2asn-0.0.1/nazo_ip2asn/
--rw-r--r--   0 runner    (1001) docker     (123)   213592 2023-04-25 16:22:41.000000 nazo_ip2asn-0.0.1/nazo_ip2asn/ip2asn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/nazo_ip2asn/ip2asn.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/nazo_ip2asn/ip2asn.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:22:54.083828 nazo_ip2asn-0.0.1/nazo_ip2asn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-25 16:22:54.000000 nazo_ip2asn-0.0.1/nazo_ip2asn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 16:22:54.000000 nazo_ip2asn-0.0.1/nazo_ip2asn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:22:54.000000 nazo_ip2asn-0.0.1/nazo_ip2asn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 16:22:54.000000 nazo_ip2asn-0.0.1/nazo_ip2asn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:22:54.083828 nazo_ip2asn-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-25 16:22:10.000000 nazo_ip2asn-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:16.178455 nazo_ip2asn-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 15:09:16.178455 nazo_ip2asn-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:16.174455 nazo_ip2asn-0.0.2/nazo_ip2asn/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/nazo_ip2asn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215399 2023-04-26 15:08:46.000000 nazo_ip2asn-0.0.2/nazo_ip2asn/ip2asn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/nazo_ip2asn/ip2asn.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/nazo_ip2asn/ip2asn.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:16.174455 nazo_ip2asn-0.0.2/nazo_ip2asn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 15:09:16.000000 nazo_ip2asn-0.0.2/nazo_ip2asn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 15:09:16.000000 nazo_ip2asn-0.0.2/nazo_ip2asn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:09:16.000000 nazo_ip2asn-0.0.2/nazo_ip2asn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 15:09:16.000000 nazo_ip2asn-0.0.2/nazo_ip2asn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:09:16.178455 nazo_ip2asn-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-26 15:07:23.000000 nazo_ip2asn-0.0.2/setup.py
```

### Comparing `nazo_ip2asn-0.0.1/LICENSE` & `nazo_ip2asn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nazo_ip2asn-0.0.1/nazo_ip2asn/ip2asn.cpp` & `nazo_ip2asn-0.0.2/nazo_ip2asn/ip2asn.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
         "extra_link_args": [
             "-Wl,-O3"
         ],
         "include_dirs": [
             "nazo_ip2asn"
         ],
         "language": "c++",
-        "name": "ip2asn",
+        "name": "nazo_ip2asn.ip2asn",
         "sources": [
             "nazo_ip2asn/ip2asn.pyx"
         ]
     },
-    "module_name": "ip2asn"
+    "module_name": "nazo_ip2asn.ip2asn"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -774,24 +774,24 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__ip2asn
-#define __PYX_HAVE_API__ip2asn
+#define __PYX_HAVE__nazo_ip2asn__ip2asn
+#define __PYX_HAVE_API__nazo_ip2asn__ip2asn
 /* Early includes */
+#include <string.h>
+#include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
-#include <string.h>
-#include <string>
 #include <utility>
 
     #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
     // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
     #include <type_traits>
 
     namespace cython_std {
@@ -1012,34 +1012,34 @@
 
 static const char *__pyx_f[] = {
   "nazo_ip2asn/ip2asn.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_6ip2asn_Ip2Asn;
+struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn;
 
-/* "ip2asn.pyx":11
+/* "nazo_ip2asn/ip2asn.pyx":11
  *     DataPair lookup(const string &ip)
  * 
  * cdef class Ip2Asn:             # <<<<<<<<<<<<<<
  *     def __cinit__(self,str ipv4file,str ipv6file):
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  */
-struct __pyx_obj_6ip2asn_Ip2Asn {
+struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn {
   PyObject_HEAD
-  struct __pyx_vtabstruct_6ip2asn_Ip2Asn *__pyx_vtab;
+  struct __pyx_vtabstruct_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_vtab;
 };
 
 
 
-struct __pyx_vtabstruct_6ip2asn_Ip2Asn {
-  PyObject *(*lookup)(struct __pyx_obj_6ip2asn_Ip2Asn *, std::string, int __pyx_skip_dispatch);
+struct __pyx_vtabstruct_11nazo_ip2asn_6ip2asn_Ip2Asn {
+  PyObject *(*lookup)(struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *, std::string, int __pyx_skip_dispatch);
 };
-static struct __pyx_vtabstruct_6ip2asn_Ip2Asn *__pyx_vtabptr_6ip2asn_Ip2Asn;
+static struct __pyx_vtabstruct_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_vtabptr_11nazo_ip2asn_6ip2asn_Ip2Asn;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1399,49 +1399,48 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static PyObject *__pyx_f_6ip2asn_6Ip2Asn_lookup(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip, int __pyx_skip_dispatch); /* proto*/
-
-/* Module declarations from 'libcpp.vector' */
+static PyObject *__pyx_f_11nazo_ip2asn_6ip2asn_6Ip2Asn_lookup(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from 'libc.string' */
 
 /* Module declarations from 'libcpp.string' */
 
+/* Module declarations from 'libcpp.vector' */
+
 /* Module declarations from 'libcpp.utility' */
 
 /* Module declarations from 'libcpp.pair' */
 
-/* Module declarations from 'ip2asn' */
-static PyTypeObject *__pyx_ptype_6ip2asn_Ip2Asn = 0;
+/* Module declarations from 'nazo_ip2asn.ip2asn' */
+static PyTypeObject *__pyx_ptype_11nazo_ip2asn_6ip2asn_Ip2Asn = 0;
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
-#define __Pyx_MODULE_NAME "ip2asn"
-extern int __pyx_module_is_main_ip2asn;
-int __pyx_module_is_main_ip2asn = 0;
+#define __Pyx_MODULE_NAME "nazo_ip2asn.ip2asn"
+extern int __pyx_module_is_main_nazo_ip2asn__ip2asn;
+int __pyx_module_is_main_nazo_ip2asn__ip2asn = 0;
 
-/* Implementation of 'ip2asn' */
+/* Implementation of 'nazo_ip2asn.ip2asn' */
 static PyObject *__pyx_builtin_IndexError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_TypeError;
 static const char __pyx_k_ip[] = "ip";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_Ip2Asn[] = "Ip2Asn";
-static const char __pyx_k_ip2asn[] = "ip2asn";
 static const char __pyx_k_lookup[] = "lookup";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_ipv4file[] = "ipv4file";
 static const char __pyx_k_ipv6file[] = "ipv6file";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
@@ -1451,72 +1450,73 @@
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_Ip2Asn_lookup[] = "Ip2Asn.lookup";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_nazo_ip2asn_ip2asn[] = "nazo_ip2asn.ip2asn";
 static const char __pyx_k_Ip2Asn___reduce_cython[] = "Ip2Asn.__reduce_cython__";
 static const char __pyx_k_nazo_ip2asn_ip2asn_pyx[] = "nazo_ip2asn/ip2asn.pyx";
 static const char __pyx_k_Ip2Asn___setstate_cython[] = "Ip2Asn.__setstate_cython__";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_n_s_Ip2Asn;
 static PyObject *__pyx_n_s_Ip2Asn___reduce_cython;
 static PyObject *__pyx_n_s_Ip2Asn___setstate_cython;
 static PyObject *__pyx_n_s_Ip2Asn_lookup;
 static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_ip;
-static PyObject *__pyx_n_s_ip2asn;
 static PyObject *__pyx_n_s_ipv4file;
 static PyObject *__pyx_n_s_ipv6file;
 static PyObject *__pyx_n_s_lookup;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
+static PyObject *__pyx_n_s_nazo_ip2asn_ip2asn;
 static PyObject *__pyx_kp_s_nazo_ip2asn_ip2asn_pyx;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
-static int __pyx_pf_6ip2asn_6Ip2Asn___cinit__(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, PyObject *__pyx_v_ipv4file, PyObject *__pyx_v_ipv6file); /* proto */
-static PyObject *__pyx_pf_6ip2asn_6Ip2Asn_2lookup(struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip); /* proto */
-static PyObject *__pyx_pf_6ip2asn_6Ip2Asn_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6ip2asn_6Ip2Asn_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_6ip2asn_Ip2Asn(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static int __pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn___cinit__(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, PyObject *__pyx_v_ipv4file, PyObject *__pyx_v_ipv6file); /* proto */
+static PyObject *__pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_2lookup(struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip); /* proto */
+static PyObject *__pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_11nazo_ip2asn_6ip2asn_Ip2Asn(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__8;
 /* Late includes */
 
-/* "ip2asn.pyx":12
+/* "nazo_ip2asn/ip2asn.pyx":12
  * 
  * cdef class Ip2Asn:
  *     def __cinit__(self,str ipv4file,str ipv6file):             # <<<<<<<<<<<<<<
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_6ip2asn_6Ip2Asn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_6ip2asn_6Ip2Asn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_ipv4file = 0;
   PyObject *__pyx_v_ipv6file = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -1559,43 +1559,43 @@
     __pyx_v_ipv4file = ((PyObject*)values[0]);
     __pyx_v_ipv6file = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 12, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ipv4file), (&PyUnicode_Type), 1, "ipv4file", 1))) __PYX_ERR(0, 12, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ipv6file), (&PyUnicode_Type), 1, "ipv6file", 1))) __PYX_ERR(0, 12, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6ip2asn_6Ip2Asn___cinit__(((struct __pyx_obj_6ip2asn_Ip2Asn *)__pyx_v_self), __pyx_v_ipv4file, __pyx_v_ipv6file);
+  __pyx_r = __pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn___cinit__(((struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *)__pyx_v_self), __pyx_v_ipv4file, __pyx_v_ipv6file);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_6ip2asn_6Ip2Asn___cinit__(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, PyObject *__pyx_v_ipv4file, PyObject *__pyx_v_ipv6file) {
+static int __pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn___cinit__(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, PyObject *__pyx_v_ipv4file, PyObject *__pyx_v_ipv6file) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::string __pyx_t_2;
   std::string __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "ip2asn.pyx":13
+  /* "nazo_ip2asn/ip2asn.pyx":13
  * cdef class Ip2Asn:
  *     def __cinit__(self,str ipv4file,str ipv6file):
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))             # <<<<<<<<<<<<<<
  * 
  *     cpdef tuple lookup(self,string ip):
  */
   if (unlikely(__pyx_v_ipv4file == Py_None)) {
@@ -1612,44 +1612,44 @@
   }
   __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_ipv6file); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   Address::init(__pyx_t_2, __pyx_t_3);
 
-  /* "ip2asn.pyx":12
+  /* "nazo_ip2asn/ip2asn.pyx":12
  * 
  * cdef class Ip2Asn:
  *     def __cinit__(self,str ipv4file,str ipv6file):             # <<<<<<<<<<<<<<
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ip2asn.pyx":15
+/* "nazo_ip2asn/ip2asn.pyx":15
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  * 
  *     cpdef tuple lookup(self,string ip):             # <<<<<<<<<<<<<<
  *         cdef DataPair result
  *         try:
  */
 
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_3lookup(PyObject *__pyx_v_self, PyObject *__pyx_arg_ip); /*proto*/
-static PyObject *__pyx_f_6ip2asn_6Ip2Asn_lookup(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip, int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup(PyObject *__pyx_v_self, PyObject *__pyx_arg_ip); /*proto*/
+static PyObject *__pyx_f_11nazo_ip2asn_6ip2asn_6Ip2Asn_lookup(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip, int __pyx_skip_dispatch) {
   Address::DataPair __pyx_v_result;
   PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -1669,15 +1669,15 @@
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_lookup); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_6ip2asn_6Ip2Asn_3lookup)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup)) {
         __Pyx_XDECREF(__pyx_r);
         __pyx_t_3 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_ip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
@@ -1709,45 +1709,45 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "ip2asn.pyx":17
+  /* "nazo_ip2asn/ip2asn.pyx":17
  *     cpdef tuple lookup(self,string ip):
  *         cdef DataPair result
  *         try:             # <<<<<<<<<<<<<<
  *             result = lookup(ip)
  *         except IndexError:
  */
   {
     (void)__pyx_t_6; (void)__pyx_t_7; (void)__pyx_t_8; /* mark used */
     /*try:*/ {
 
-      /* "ip2asn.pyx":18
+      /* "nazo_ip2asn/ip2asn.pyx":18
  *         cdef DataPair result
  *         try:
  *             result = lookup(ip)             # <<<<<<<<<<<<<<
  *         except IndexError:
  *             return (None,"")
  */
       __pyx_v_result = Address::lookup(__pyx_v_ip);
 
-      /* "ip2asn.pyx":17
+      /* "nazo_ip2asn/ip2asn.pyx":17
  *     cpdef tuple lookup(self,string ip):
  *         cdef DataPair result
  *         try:             # <<<<<<<<<<<<<<
  *             result = lookup(ip)
  *         except IndexError:
  */
     }
   }
 
-  /* "ip2asn.pyx":24
+  /* "nazo_ip2asn/ip2asn.pyx":24
  *             return (None,f": {e}" )
  * 
  *         return (result.first, result.second)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_result.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -1761,112 +1761,112 @@
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_r = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "ip2asn.pyx":15
+  /* "nazo_ip2asn/ip2asn.pyx":15
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  * 
  *     cpdef tuple lookup(self,string ip):             # <<<<<<<<<<<<<<
  *         cdef DataPair result
  *         try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.lookup", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.lookup", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_3lookup(PyObject *__pyx_v_self, PyObject *__pyx_arg_ip); /*proto*/
-static PyMethodDef __pyx_mdef_6ip2asn_6Ip2Asn_3lookup = {"lookup", (PyCFunction)__pyx_pw_6ip2asn_6Ip2Asn_3lookup, METH_O, 0};
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_3lookup(PyObject *__pyx_v_self, PyObject *__pyx_arg_ip) {
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup(PyObject *__pyx_v_self, PyObject *__pyx_arg_ip); /*proto*/
+static PyMethodDef __pyx_mdef_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup = {"lookup", (PyCFunction)__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup, METH_O, 0};
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup(PyObject *__pyx_v_self, PyObject *__pyx_arg_ip) {
   std::string __pyx_v_ip;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lookup (wrapper)", 0);
   assert(__pyx_arg_ip); {
     __pyx_v_ip = __pyx_convert_string_from_py_std__in_string(__pyx_arg_ip); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.lookup", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.lookup", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6ip2asn_6Ip2Asn_2lookup(((struct __pyx_obj_6ip2asn_Ip2Asn *)__pyx_v_self), ((std::string)__pyx_v_ip));
+  __pyx_r = __pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_2lookup(((struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *)__pyx_v_self), ((std::string)__pyx_v_ip));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6ip2asn_6Ip2Asn_2lookup(struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip) {
+static PyObject *__pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_2lookup(struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, std::string __pyx_v_ip) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lookup", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6ip2asn_6Ip2Asn_lookup(__pyx_v_self, __pyx_v_ip, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_11nazo_ip2asn_6ip2asn_6Ip2Asn_lookup(__pyx_v_self, __pyx_v_ip, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.lookup", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.lookup", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_6ip2asn_6Ip2Asn_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)__pyx_pw_6ip2asn_6Ip2Asn_5__reduce_cython__, METH_NOARGS, 0};
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_11nazo_ip2asn_6ip2asn_6Ip2Asn_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_5__reduce_cython__, METH_NOARGS, 0};
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6ip2asn_6Ip2Asn_4__reduce_cython__(((struct __pyx_obj_6ip2asn_Ip2Asn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_4__reduce_cython__(((struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6ip2asn_6Ip2Asn_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self) {
+static PyObject *__pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -1888,43 +1888,43 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyMethodDef __pyx_mdef_6ip2asn_6Ip2Asn_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)__pyx_pw_6ip2asn_6Ip2Asn_7__setstate_cython__, METH_O, 0};
-static PyObject *__pyx_pw_6ip2asn_6Ip2Asn_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyMethodDef __pyx_mdef_11nazo_ip2asn_6ip2asn_6Ip2Asn_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_7__setstate_cython__, METH_O, 0};
+static PyObject *__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6ip2asn_6Ip2Asn_6__setstate_cython__(((struct __pyx_obj_6ip2asn_Ip2Asn *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_6__setstate_cython__(((struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6ip2asn_6Ip2Asn_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6ip2asn_Ip2Asn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_11nazo_ip2asn_6ip2asn_6Ip2Asn_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -1946,15 +1946,15 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ip2asn.Ip2Asn.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_ip2asn.ip2asn.Ip2Asn.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.from_py":13
@@ -2266,55 +2266,55 @@
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_6ip2asn_Ip2Asn __pyx_vtable_6ip2asn_Ip2Asn;
+static struct __pyx_vtabstruct_11nazo_ip2asn_6ip2asn_Ip2Asn __pyx_vtable_11nazo_ip2asn_6ip2asn_Ip2Asn;
 
-static PyObject *__pyx_tp_new_6ip2asn_Ip2Asn(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_6ip2asn_Ip2Asn *p;
+static PyObject *__pyx_tp_new_11nazo_ip2asn_6ip2asn_Ip2Asn(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_6ip2asn_Ip2Asn *)o);
-  p->__pyx_vtab = __pyx_vtabptr_6ip2asn_Ip2Asn;
-  if (unlikely(__pyx_pw_6ip2asn_6Ip2Asn_1__cinit__(o, a, k) < 0)) goto bad;
+  p = ((struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *)o);
+  p->__pyx_vtab = __pyx_vtabptr_11nazo_ip2asn_6ip2asn_Ip2Asn;
+  if (unlikely(__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_6ip2asn_Ip2Asn(PyObject *o) {
+static void __pyx_tp_dealloc_11nazo_ip2asn_6ip2asn_Ip2Asn(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyMethodDef __pyx_methods_6ip2asn_Ip2Asn[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_6ip2asn_6Ip2Asn_5__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_6ip2asn_6Ip2Asn_7__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_11nazo_ip2asn_6ip2asn_Ip2Asn[] = {
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_5__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_11nazo_ip2asn_6ip2asn_6Ip2Asn_7__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_6ip2asn_Ip2Asn = {
+static PyTypeObject __pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn = {
   PyVarObject_HEAD_INIT(0, 0)
-  "ip2asn.Ip2Asn", /*tp_name*/
-  sizeof(struct __pyx_obj_6ip2asn_Ip2Asn), /*tp_basicsize*/
+  "nazo_ip2asn.ip2asn.Ip2Asn", /*tp_name*/
+  sizeof(struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6ip2asn_Ip2Asn, /*tp_dealloc*/
+  __pyx_tp_dealloc_11nazo_ip2asn_6ip2asn_Ip2Asn, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -2339,25 +2339,25 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_6ip2asn_Ip2Asn, /*tp_methods*/
+  __pyx_methods_11nazo_ip2asn_6ip2asn_Ip2Asn, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6ip2asn_Ip2Asn, /*tp_new*/
+  __pyx_tp_new_11nazo_ip2asn_6ip2asn_Ip2Asn, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -2429,20 +2429,20 @@
   {&__pyx_n_s_Ip2Asn___setstate_cython, __pyx_k_Ip2Asn___setstate_cython, sizeof(__pyx_k_Ip2Asn___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Ip2Asn_lookup, __pyx_k_Ip2Asn_lookup, sizeof(__pyx_k_Ip2Asn_lookup), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_ip, __pyx_k_ip, sizeof(__pyx_k_ip), 0, 0, 1, 1},
-  {&__pyx_n_s_ip2asn, __pyx_k_ip2asn, sizeof(__pyx_k_ip2asn), 0, 0, 1, 1},
   {&__pyx_n_s_ipv4file, __pyx_k_ipv4file, sizeof(__pyx_k_ipv4file), 0, 0, 1, 1},
   {&__pyx_n_s_ipv6file, __pyx_k_ipv6file, sizeof(__pyx_k_ipv6file), 0, 0, 1, 1},
   {&__pyx_n_s_lookup, __pyx_k_lookup, sizeof(__pyx_k_lookup), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+  {&__pyx_n_s_nazo_ip2asn_ip2asn, __pyx_k_nazo_ip2asn_ip2asn, sizeof(__pyx_k_nazo_ip2asn_ip2asn), 0, 0, 1, 1},
   {&__pyx_kp_s_nazo_ip2asn_ip2asn_pyx, __pyx_k_nazo_ip2asn_ip2asn_pyx, sizeof(__pyx_k_nazo_ip2asn_ip2asn_pyx), 0, 0, 1, 0},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
@@ -2481,15 +2481,15 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "ip2asn.pyx":15
+  /* "nazo_ip2asn/ip2asn.pyx":15
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  * 
  *     cpdef tuple lookup(self,string ip):             # <<<<<<<<<<<<<<
  *         cdef DataPair result
  *         try:
  */
   __pyx_tuple__3 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_ip, __pyx_n_s_ip); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 15, __pyx_L1_error)
@@ -2566,27 +2566,27 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_6ip2asn_Ip2Asn = &__pyx_vtable_6ip2asn_Ip2Asn;
-  __pyx_vtable_6ip2asn_Ip2Asn.lookup = (PyObject *(*)(struct __pyx_obj_6ip2asn_Ip2Asn *, std::string, int __pyx_skip_dispatch))__pyx_f_6ip2asn_6Ip2Asn_lookup;
-  if (PyType_Ready(&__pyx_type_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_vtabptr_11nazo_ip2asn_6ip2asn_Ip2Asn = &__pyx_vtable_11nazo_ip2asn_6ip2asn_Ip2Asn;
+  __pyx_vtable_11nazo_ip2asn_6ip2asn_Ip2Asn.lookup = (PyObject *(*)(struct __pyx_obj_11nazo_ip2asn_6ip2asn_Ip2Asn *, std::string, int __pyx_skip_dispatch))__pyx_f_11nazo_ip2asn_6ip2asn_6Ip2Asn_lookup;
+  if (PyType_Ready(&__pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6ip2asn_Ip2Asn.tp_print = 0;
+  __pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6ip2asn_Ip2Asn.tp_dictoffset && __pyx_type_6ip2asn_Ip2Asn.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6ip2asn_Ip2Asn.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn.tp_dictoffset && __pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6ip2asn_Ip2Asn.tp_dict, __pyx_vtabptr_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Ip2Asn, (PyObject *)&__pyx_type_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  __pyx_ptype_6ip2asn_Ip2Asn = &__pyx_type_6ip2asn_Ip2Asn;
+  if (__Pyx_SetVtable(__pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn.tp_dict, __pyx_vtabptr_11nazo_ip2asn_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Ip2Asn, (PyObject *)&__pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_ptype_11nazo_ip2asn_6ip2asn_Ip2Asn = &__pyx_type_11nazo_ip2asn_6ip2asn_Ip2Asn;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2782,22 +2782,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_ip2asn) {
+  if (__pyx_module_is_main_nazo_ip2asn__ip2asn) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "ip2asn")) {
-      if (unlikely(PyDict_SetItemString(modules, "ip2asn", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "nazo_ip2asn.ip2asn")) {
+      if (unlikely(PyDict_SetItemString(modules, "nazo_ip2asn.ip2asn", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2810,52 +2810,52 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "ip2asn.pyx":15
+  /* "nazo_ip2asn/ip2asn.pyx":15
  *         init(ipv4file.encode('UTF-8'),ipv6file.encode('UTF-8'))
  * 
  *     cpdef tuple lookup(self,string ip):             # <<<<<<<<<<<<<<
  *         cdef DataPair result
  *         try:
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6ip2asn_6Ip2Asn_3lookup, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Ip2Asn_lookup, NULL, __pyx_n_s_ip2asn, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11nazo_ip2asn_6ip2asn_6Ip2Asn_3lookup, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Ip2Asn_lookup, NULL, __pyx_n_s_nazo_ip2asn_ip2asn, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6ip2asn_Ip2Asn->tp_dict, __pyx_n_s_lookup, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_11nazo_ip2asn_6ip2asn_Ip2Asn->tp_dict, __pyx_n_s_lookup, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  PyType_Modified(__pyx_ptype_6ip2asn_Ip2Asn);
+  PyType_Modified(__pyx_ptype_11nazo_ip2asn_6ip2asn_Ip2Asn);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6ip2asn_6Ip2Asn_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Ip2Asn___reduce_cython, NULL, __pyx_n_s_ip2asn, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11nazo_ip2asn_6ip2asn_6Ip2Asn_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Ip2Asn___reduce_cython, NULL, __pyx_n_s_nazo_ip2asn_ip2asn, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6ip2asn_6Ip2Asn_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Ip2Asn___setstate_cython, NULL, __pyx_n_s_ip2asn, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11nazo_ip2asn_6ip2asn_6Ip2Asn_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Ip2Asn___setstate_cython, NULL, __pyx_n_s_nazo_ip2asn_ip2asn, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_1) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ip2asn.pyx":1
+  /* "nazo_ip2asn/ip2asn.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
- * from libcpp.vector cimport vector
+ * from libcpp.string cimport string
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "string.to_py":55
@@ -2869,19 +2869,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init ip2asn", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init nazo_ip2asn.ip2asn", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init ip2asn");
+    PyErr_SetString(PyExc_ImportError, "init nazo_ip2asn.ip2asn");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `nazo_ip2asn-0.0.1/nazo_ip2asn/ip2asn.pyx` & `nazo_ip2asn-0.0.2/nazo_ip2asn/ip2asn.pyx`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # cython: language_level=3
 # distutils: language = c++
-from libcpp.vector cimport vector
 from libcpp.string cimport string
+from libcpp.vector cimport vector
 from libcpp.pair cimport pair
 cdef extern from "ipasn.hpp" namespace "Address":
     ctypedef pair[string, string] DataPair
     void init(const string &ipv4file, const string &ipv6file)
     DataPair lookup(const string &ip)
 
 cdef class Ip2Asn:
```

### Comparing `nazo_ip2asn-0.0.1/setup.py` & `nazo_ip2asn-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, Extension
 from Cython.Build import cythonize
 from sys import platform
 import os
 
+
 def readme():
     with open("README.md") as f:
         return f.read()
 
+
 boost_include_dir = None
 include_dirs = []
 extra_compile_args = []
 extra_link_args = []
 
 if platform == "win32":
     extra_compile_args = ["/std:c++17", "/O2"]
@@ -41,15 +43,15 @@
             "binding": True,
             "cdivision": True,
         },
     ),
     include_dirs=include_dirs,
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.0.1",
+    version="0.0.2",
     description="A ip2asn tools for python.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     package_data={
         "": [
             "nazo_ip2asn/ip2asn.pyi",
@@ -63,12 +65,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Cython",
         "Programming Language :: C++",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.8",
     packages=["nazo_ip2asn"],
 )
```

