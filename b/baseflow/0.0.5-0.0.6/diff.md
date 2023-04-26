# Comparing `tmp/baseflow-0.0.5.tar.gz` & `tmp/baseflow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseflow-0.0.5.tar", last modified: Mon Mar 20 14:14:32 2023, max compression
+gzip compressed data, was "baseflow-0.0.6.tar", last modified: Wed Apr 26 08:34:16 2023, max compression
```

## Comparing `baseflow-0.0.5.tar` & `baseflow-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 14:14:32.520816 baseflow-0.0.5/
--rw-rw-rw-   0        0        0     2736 2023-03-20 14:14:32.520816 baseflow-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2076 2023-03-20 14:08:59.000000 baseflow-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 14:14:32.503822 baseflow-0.0.5/baseflow/
--rw-rw-rw-   0        0        0      251 2023-03-20 14:08:26.000000 baseflow-0.0.5/baseflow/__init__.py
--rw-rw-rw-   0        0        0     3502 2023-02-16 04:15:40.000000 baseflow-0.0.5/baseflow/comparision.py
--rw-rw-rw-   0        0        0   678801 2021-11-26 09:44:13.000000 baseflow-0.0.5/baseflow/example.csv
-drwxrwxrwx   0        0        0        0 2023-03-20 14:14:32.519816 baseflow-0.0.5/baseflow/methods/
--rw-rw-rw-   0        0        0      686 2023-02-09 18:09:45.000000 baseflow-0.0.5/baseflow/methods/Boughton.py
--rw-rw-rw-   0        0        0      611 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/CM.py
--rw-rw-rw-   0        0        0      630 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/Chapman.py
--rw-rw-rw-   0        0        0      633 2023-02-09 18:12:19.000000 baseflow-0.0.5/baseflow/methods/EWMA.py
--rw-rw-rw-   0        0        0      710 2023-02-09 18:09:15.000000 baseflow-0.0.5/baseflow/methods/Eckhardt.py
--rw-rw-rw-   0        0        0      669 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/Fixed.py
--rw-rw-rw-   0        0        0      684 2023-02-09 18:10:00.000000 baseflow-0.0.5/baseflow/methods/Furey.py
--rw-rw-rw-   0        0        0      949 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/LH.py
--rw-rw-rw-   0        0        0     1577 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/Local.py
--rw-rw-rw-   0        0        0      805 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/Slide.py
--rw-rw-rw-   0        0        0     1561 2023-02-09 17:52:56.000000 baseflow-0.0.5/baseflow/methods/UKIH.py
--rw-rw-rw-   0        0        0      810 2023-02-09 18:10:14.000000 baseflow-0.0.5/baseflow/methods/Willems.py
--rw-rw-rw-   0        0        0      458 2021-09-23 13:22:08.000000 baseflow-0.0.5/baseflow/methods/__init__.py
--rw-rw-rw-   0        0        0     2847 2023-02-16 04:13:46.000000 baseflow-0.0.5/baseflow/param_estimate.py
--rw-rw-rw-   0        0        0     2442 2023-02-24 21:05:37.000000 baseflow-0.0.5/baseflow/separation.py
--rw-rw-rw-   0        0        0     3842 2023-02-21 18:18:24.000000 baseflow-0.0.5/baseflow/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:14:32.508816 baseflow-0.0.5/baseflow.egg-info/
--rw-rw-rw-   0        0        0     2736 2023-03-20 14:14:32.000000 baseflow-0.0.5/baseflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-03-20 14:14:32.000000 baseflow-0.0.5/baseflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 14:14:32.000000 baseflow-0.0.5/baseflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-20 14:14:32.000000 baseflow-0.0.5/baseflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 14:14:32.000000 baseflow-0.0.5/baseflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 14:14:32.520816 baseflow-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3997 2022-02-11 00:54:27.000000 baseflow-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.311876 baseflow-0.0.6/
+-rw-rw-rw-   0        0        0     2696 2023-04-26 08:34:16.311876 baseflow-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2036 2023-03-20 14:16:11.000000 baseflow-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.295880 baseflow-0.0.6/baseflow/
+-rw-rw-rw-   0        0        0      251 2023-03-20 14:08:26.000000 baseflow-0.0.6/baseflow/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-02-16 04:15:40.000000 baseflow-0.0.6/baseflow/comparision.py
+-rw-rw-rw-   0        0        0   678801 2021-11-26 09:44:13.000000 baseflow-0.0.6/baseflow/example.csv
+drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.310877 baseflow-0.0.6/baseflow/methods/
+-rw-rw-rw-   0        0        0      686 2023-02-09 18:09:45.000000 baseflow-0.0.6/baseflow/methods/Boughton.py
+-rw-rw-rw-   0        0        0      611 2023-02-09 17:52:56.000000 baseflow-0.0.6/baseflow/methods/CM.py
+-rw-rw-rw-   0        0        0      630 2023-02-09 17:52:56.000000 baseflow-0.0.6/baseflow/methods/Chapman.py
+-rw-rw-rw-   0        0        0      633 2023-02-09 18:12:19.000000 baseflow-0.0.6/baseflow/methods/EWMA.py
+-rw-rw-rw-   0        0        0      710 2023-02-09 18:09:15.000000 baseflow-0.0.6/baseflow/methods/Eckhardt.py
+-rw-rw-rw-   0        0        0      660 2023-04-26 08:31:08.000000 baseflow-0.0.6/baseflow/methods/Fixed.py
+-rw-rw-rw-   0        0        0      684 2023-02-09 18:10:00.000000 baseflow-0.0.6/baseflow/methods/Furey.py
+-rw-rw-rw-   0        0        0      949 2023-02-09 17:52:56.000000 baseflow-0.0.6/baseflow/methods/LH.py
+-rw-rw-rw-   0        0        0     1568 2023-04-26 08:31:14.000000 baseflow-0.0.6/baseflow/methods/Local.py
+-rw-rw-rw-   0        0        0      796 2023-04-26 08:31:49.000000 baseflow-0.0.6/baseflow/methods/Slide.py
+-rw-rw-rw-   0        0        0     1552 2023-04-26 08:31:56.000000 baseflow-0.0.6/baseflow/methods/UKIH.py
+-rw-rw-rw-   0        0        0      810 2023-02-09 18:10:14.000000 baseflow-0.0.6/baseflow/methods/Willems.py
+-rw-rw-rw-   0        0        0      458 2021-09-23 13:22:08.000000 baseflow-0.0.6/baseflow/methods/__init__.py
+-rw-rw-rw-   0        0        0     2838 2023-04-26 08:30:39.000000 baseflow-0.0.6/baseflow/param_estimate.py
+-rw-rw-rw-   0        0        0     2464 2023-03-20 15:16:19.000000 baseflow-0.0.6/baseflow/separation.py
+-rw-rw-rw-   0        0        0     3842 2023-02-21 18:18:24.000000 baseflow-0.0.6/baseflow/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:34:16.299878 baseflow-0.0.6/baseflow.egg-info/
+-rw-rw-rw-   0        0        0     2696 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 08:34:16.000000 baseflow-0.0.6/baseflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 08:34:16.311876 baseflow-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3997 2023-04-26 08:32:45.000000 baseflow-0.0.6/setup.py
```

### Comparing `baseflow-0.0.5/PKG-INFO` & `baseflow-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for baseflow separation
 Home-page: https://github.com/xiejx5/baseflow
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -43,15 +43,14 @@
 <br>
 
 
 ### Example
 ```python
 import baseflow
 
-path = f'{baseflow._path}/example.csv'
 Q, date = baseflow.load_streamflow(baseflow.example)
 b, KGEs = baseflow.separation(Q, date, area=276)
 print(f'Best Method: {b.dtype.names[KGEs.argmax()]}')
 ```
 <br>
```

### Comparing `baseflow-0.0.5/README.md` & `baseflow-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 <br>
 
 
 ### Example
 ```python
 import baseflow
 
-path = f'{baseflow._path}/example.csv'
 Q, date = baseflow.load_streamflow(baseflow.example)
 b, KGEs = baseflow.separation(Q, date, area=276)
 print(f'Best Method: {b.dtype.names[KGEs.argmax()]}')
 ```
 <br>
```

### Comparing `baseflow-0.0.5/baseflow/comparision.py` & `baseflow-0.0.6/baseflow/comparision.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/example.csv` & `baseflow-0.0.6/baseflow/example.csv`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/Boughton.py` & `baseflow-0.0.6/baseflow/methods/Boughton.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/CM.py` & `baseflow-0.0.6/baseflow/methods/CM.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/Chapman.py` & `baseflow-0.0.6/baseflow/methods/Chapman.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/EWMA.py` & `baseflow-0.0.6/baseflow/methods/EWMA.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/Eckhardt.py` & `baseflow-0.0.6/baseflow/methods/Eckhardt.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/Fixed.py` & `baseflow-0.0.6/baseflow/methods/Fixed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import njit, prange
+from numba import njit
 from baseflow.methods.Local import hysep_interval
 
 
 def Fixed(Q, area=None):
     """Fixed interval graphical method from HYSEP program (Sloto & Crouse, 1996)
 
     Args:
@@ -14,12 +14,12 @@
     return Fixed_interpolation(Q, inN)
 
 
 @njit
 def Fixed_interpolation(Q, inN):
     b = np.zeros(Q.shape[0])
     n = Q.shape[0] // inN
-    for i in prange(n):
+    for i in range(n):
         b[inN * i:inN * (i + 1)] = np.min(Q[inN * i:inN * (i + 1)])
     if n * inN != Q.shape[0]:
         b[n * inN:] = np.min(Q[n * inN:])
     return b
```

### Comparing `baseflow-0.0.5/baseflow/methods/Furey.py` & `baseflow-0.0.6/baseflow/methods/Furey.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/LH.py` & `baseflow-0.0.6/baseflow/methods/LH.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/methods/Local.py` & `baseflow-0.0.6/baseflow/methods/Local.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import njit, prange
+from numba import njit
 from baseflow.methods.UKIH import linear_interpolation
 
 
 def Local(Q, b_LH, area=None, return_exceed=False):
     """Local minimum graphical method from HYSEP program (Sloto & Crouse, 1996)
 
     Args:
@@ -33,11 +33,11 @@
     inN = np.int64(min(max(inN, 3), 11))
     return inN
 
 
 @njit
 def Local_turn(Q, inN):
     idx_turn = np.zeros(Q.shape[0], dtype=np.int64)
-    for i in prange(np.int64((inN - 1) / 2), np.int64(Q.shape[0] - (inN - 1) / 2)):
+    for i in range(np.int64((inN - 1) / 2), np.int64(Q.shape[0] - (inN - 1) / 2)):
         if Q[i] == np.min(Q[np.int64(i - (inN - 1) / 2):np.int64(i + (inN + 1) / 2)]):
             idx_turn[i] = i
     return idx_turn[idx_turn != 0]
```

### Comparing `baseflow-0.0.5/baseflow/methods/Slide.py` & `baseflow-0.0.6/baseflow/methods/Slide.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import njit, prange
+from numba import njit
 from baseflow.methods.Local import hysep_interval
 
 
 def Slide(Q, area):
     """Slide interval graphical method from HYSEP program (Sloto & Crouse, 1996)
 
     Args:
@@ -13,12 +13,12 @@
     inN = hysep_interval(area)
     return Slide_interpolation(Q, inN)
 
 
 @njit
 def Slide_interpolation(Q, inN):
     b = np.zeros(Q.shape[0])
-    for i in prange(np.int64((inN - 1) / 2), np.int64(Q.shape[0] - (inN - 1) / 2)):
+    for i in range(np.int64((inN - 1) / 2), np.int64(Q.shape[0] - (inN - 1) / 2)):
         b[i] = np.min(Q[np.int64(i - (inN - 1) / 2):np.int64(i + (inN + 1) / 2)])
     b[:np.int64((inN - 1) / 2)] = np.min(Q[:np.int64((inN - 1) / 2)])
     b[np.int64(Q.shape[0] - (inN - 1) / 2):] = np.min(Q[np.int64(Q.shape[0] - (inN - 1) / 2):])
     return b
```

### Comparing `baseflow-0.0.5/baseflow/methods/UKIH.py` & `baseflow-0.0.6/baseflow/methods/UKIH.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import njit, prange
+from numba import njit
 
 
 def UKIH(Q, b_LH, return_exceed=False):
     """graphical method developed by UK Institute of Hydrology (UKIH, 1980)
 
     Args:
         Q (np.array): streamflow
@@ -18,15 +18,15 @@
     b[idx_turn[-1] + 1:] = b_LH[idx_turn[-1] + 1:]
     return b
 
 
 @njit
 def UKIH_turn(Q, idx_min):
     idx_turn = np.zeros(idx_min.shape[0], dtype=np.int64)
-    for i in prange(idx_min.shape[0] - 2):
+    for i in range(idx_min.shape[0] - 2):
         if ((0.9 * Q[idx_min[i + 1]] < Q[idx_min[i]]) &
                 (0.9 * Q[idx_min[i + 1]] < Q[idx_min[i + 2]])):
             idx_turn[i] = idx_min[i + 1]
     return idx_turn[idx_turn != 0]
 
 
 @njit
```

### Comparing `baseflow-0.0.5/baseflow/methods/Willems.py` & `baseflow-0.0.6/baseflow/methods/Willems.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow/param_estimate.py` & `baseflow-0.0.6/baseflow/param_estimate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import njit, prange
+from numba import njit
 from baseflow.utils import NSE, moving_average, multi_arange
 
 
 def recession_coefficient(Q, strict):
     cQ, dQ = Q[1:-1], (Q[2:] - Q[:-2]) / 2
     cQ, dQ = cQ[strict[1:-1]], dQ[strict[1:-1]]
 
@@ -19,15 +19,15 @@
     return param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth)
 
 
 @njit
 def param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth):
     logQ = np.log1p(Q)
     loss = np.zeros(param_range.shape)
-    for i in prange(param_range.shape[0]):
+    for i in range(param_range.shape[0]):
         p = param_range[i]
         b_exceed = method(Q, b_LH, a, p, return_exceed=True)
         f_exd, logb = b_exceed[-1] / Q.shape[0], np.log1p(b_exceed[:-1])
         NSE_rec = NSE(logQ[idx_rec], logb[idx_rec])
         NSE_oth = NSE(logQ[idx_oth], logb[idx_oth])
         loss[i] = 1 - (1 - (1 - NSE_rec) / (1 - NSE_oth)) * (1 - f_exd)
     return param_range[np.argmin(loss)]
```

### Comparing `baseflow-0.0.5/baseflow/separation.py` & `baseflow-0.0.6/baseflow/separation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if method == 'all':
         method = ['UKIH', 'Local', 'Fixed', 'Slide', 'LH', 'Chapman',
                   'CM', 'Boughton', 'Furey', 'Eckhardt', 'EWMA', 'Willems']
     elif isinstance(method, str):
         method = [method]
 
     # convert ice_period ([11, 1], [3, 31]) to bool array
-    if not isinstance(ice, np.ndarray):
+    if not isinstance(ice, np.ndarray) or ice.shape[0] == 12:
         ice = exist_ice(date, ice)
     strict = strict_baseflow(Q, ice)
     if any(m in ['Chapman', 'CM', 'Boughton', 'Furey', 'Eckhardt', 'Willems'] for m in method):
         a = recession_coefficient(Q, strict)
 
     b_LH = LH(Q)
     b = np.recarray(Q.shape[0], dtype=list(zip(method, [float] * len(method))))
```

### Comparing `baseflow-0.0.5/baseflow/utils.py` & `baseflow-0.0.6/baseflow/utils.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/baseflow.egg-info/PKG-INFO` & `baseflow-0.0.6/baseflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package for baseflow separation
 Home-page: https://github.com/xiejx5/baseflow
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -43,15 +43,14 @@
 <br>
 
 
 ### Example
 ```python
 import baseflow
 
-path = f'{baseflow._path}/example.csv'
 Q, date = baseflow.load_streamflow(baseflow.example)
 b, KGEs = baseflow.separation(Q, date, area=276)
 print(f'Best Method: {b.dtype.names[KGEs.argmax()]}')
 ```
 <br>
```

### Comparing `baseflow-0.0.5/baseflow.egg-info/SOURCES.txt` & `baseflow-0.0.6/baseflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.5/setup.py` & `baseflow-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'baseflow'
 DESCRIPTION = 'A python package for baseflow separation'
 URL = 'https://github.com/xiejx5/baseflow'
 EMAIL = 'xiejx5@gmail.com'
 AUTHOR = 'Cody James'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'numba',
 ]
 
 # What packages are optional?
```

