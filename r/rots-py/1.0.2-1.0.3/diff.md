# Comparing `tmp/rots-py-1.0.2.tar.gz` & `tmp/rots-py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rots-py-1.0.2.tar", last modified: Thu Apr 20 14:13:00 2023, max compression
+gzip compressed data, was "rots-py-1.0.3.tar", last modified: Wed Apr 26 17:17:29 2023, max compression
```

## Comparing `rots-py-1.0.2.tar` & `rots-py-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 14:13:00.338101 rots-py-1.0.2/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2070 2023-04-20 14:13:00.338101 rots-py-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-18 14:24:25.000000 rots-py-1.0.2/README.md
--rw-rw-rw-   0        0        0      724 2023-04-20 14:10:58.000000 rots-py-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 14:13:00.338101 rots-py-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 14:13:00.291235 rots-py-1.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.0.2/src/__init__.py
--rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.0.2/src/__main__.py
--rw-rw-rw-   0        0        0     3017 2023-04-19 21:46:21.000000 rots-py-1.0.2/src/calculateOverlaps1.py
--rw-rw-rw-   0        0        0     2732 2023-04-19 22:23:51.000000 rots-py-1.0.2/src/calculateOverlaps2.py
--rw-rw-rw-   0        0        0     8324 2023-04-19 22:04:50.000000 rots-py-1.0.2/src/helpers.py
--rw-rw-rw-   0        0        0    11266 2023-04-19 22:18:42.000000 rots-py-1.0.2/src/rots.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:13:00.338101 rots-py-1.0.2/src/rots_py.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2023-04-20 14:13:00.000000 rots-py-1.0.2/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 17:17:29.739342 rots-py-1.0.3/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2070 2023-04-26 17:17:29.738347 rots-py-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-18 14:24:25.000000 rots-py-1.0.3/README.md
+-rw-rw-rw-   0        0        0      724 2023-04-26 17:16:08.000000 rots-py-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 17:17:29.740340 rots-py-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 17:17:29.658219 rots-py-1.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.0.3/src/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.0.3/src/__main__.py
+-rw-rw-rw-   0        0        0     3101 2023-04-26 17:07:58.000000 rots-py-1.0.3/src/calculateOverlaps1.py
+-rw-rw-rw-   0        0        0     2816 2023-04-26 17:08:25.000000 rots-py-1.0.3/src/calculateOverlaps2.py
+-rw-rw-rw-   0        0        0     8416 2023-04-26 17:11:26.000000 rots-py-1.0.3/src/helpers.py
+-rw-rw-rw-   0        0        0    11266 2023-04-19 22:18:42.000000 rots-py-1.0.3/src/rots.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:17:29.735353 rots-py-1.0.3/src/rots_py.egg-info/
+-rw-rw-rw-   0        0        0     2070 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/top_level.txt
```

### Comparing `rots-py-1.0.2/LICENSE` & `rots-py-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.2/PKG-INFO` & `rots-py-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rots-py-1.0.2/pyproject.toml` & `rots-py-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "rots-py"
-version = "1.0.2"
+version = "1.0.3"
 description = "ROTS gene ranking implementation in Python"
 readme = "README.md"
 authors = [{ name = "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq", email = "fmamadbe@abo.fi" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rots-py-1.0.2/src/calculateOverlaps1.py` & `rots-py-1.0.3/src/calculateOverlaps1.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     res1, res2, pres1, pres2 = fast_make_res(res1, res2, pres1, pres2, D_ovlp, S_ovlp, pD_ovlp, pS_ovlp, D_len, ssq_i, b, B)
             
     overlaps_ovlp = calculateOverlap_1(res1, res2, D_len, N, N_len, b, B, overlaps_ovlp)        
     overlaps_P_ovlp = calculateOverlap_1(pres1, pres2, D_len, N, N_len, b, B, overlaps_P_ovlp)    
 
   return {'overlaps': overlaps_ovlp.reshape(overlaps.shape), 'overlaps_P': overlaps_P_ovlp.reshape(overlaps_P.shape)} 
 
-@jit(nopython=True)
+@jit(nopython=True, error_model='numpy')
 def fast_make_res(res1, res2, pres1, pres2, D_ovlp, S_ovlp, pD_ovlp, pS_ovlp, D_len, ssq_i, b, B):
   for i in range(D_len):
     res1[i] = np.abs( D_ovlp[(b-1) * D_len + i] / ( S_ovlp[(b-1) * D_len + i] + ssq_i) )
     res2[i] = np.abs( D_ovlp[(b + B - 1) * D_len + i] / ( S_ovlp[(b + B - 1) * D_len + i] + ssq_i) )
     pres1[i] = np.abs( pD_ovlp[(b-1) * D_len + i] / (pS_ovlp[(b-1) * D_len + i] + ssq_i))
     pres2[i] = np.abs( pD_ovlp[(b + B - 1) * D_len + i] / (pS_ovlp[(b + B -1) * D_len + i] + ssq_i))
   return res1, res2, pres1, pres2  
@@ -44,15 +44,15 @@
   typed_r3 = List()
   [typed_r3.append(x) for x in r3]
   #Calculate the overlap
   overlaps = fast_ovlp(r2, typed_r3, N_len, N, B, b, overlaps)
 
   return overlaps
 
-@jit(nopython=True)
+@jit(nopython=True, error_model='numpy')
 def fast_ovlp(r2, r3, N_len, N, B, b, overlaps):
   #Calculate the overlap
   for i in range(N_len):
     sum = 0
     for j in range(N[i]):
       sum += (r2[j] <= r3[N[i] - 1])
     overlaps[ (b-1) + i*B ] = sum / N[i]
@@ -66,22 +66,22 @@
   # in the case of a tie, the second values are used.
   pairs = pairs[np.lexsort((pairs[:, 0], pairs[:, 1]))]
 
   # Split the pairs back into the original vectors (dec).
   a, b = split_pairs(pairs, n)
   return (a, b)
 
-@jit(nopython=True, parallel=True)
+@jit(nopython=True, parallel=True, error_model='numpy')
 def make_pairs(a, b, n):
   pairs = np.empty((n, 2))
   for i in prange(n):
     pairs[i] = [a[i], b[i]]
   return pairs
 
-@jit(nopython=True, parallel=True)
+@jit(nopython=True, parallel=True, error_model='numpy')
 def split_pairs(pairs, n):
   # Split the pairs back into the original vectors (dec).
   a = np.empty(n)
   b = np.empty(n)
   for i in prange(n):
     a[n-1-i] = pairs[i][0]
     b[n-1-i] = pairs[i][1]
```

### Comparing `rots-py-1.0.2/src/calculateOverlaps2.py` & `rots-py-1.0.3/src/calculateOverlaps2.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     res1, res2, pres1, pres2 = fast_make_res(res1, res2, pres1, pres2, D_ovlp, pD_ovlp, D_len, b, B)
 
     overlaps_ovlp = calculateOverlap_2(res1, res2, D_len, N, N_len, b, B, overlaps_ovlp)      
     overlaps_P_ovlp = calculateOverlap_2(pres1, pres2, D_len, N, N_len, b, B, overlaps_P_ovlp)    
 
   return {'overlaps': overlaps_ovlp.reshape(overlaps.shape), 'overlaps_P': overlaps_P_ovlp.reshape(overlaps_P.shape)}
 
-@jit(nopython=True)
+@jit(nopython=True, error_model='numpy')
 def fast_make_res(res1, res2, pres1, pres2, D_ovlp, pD_ovlp, D_len, b, B):
   for i in range(D_len):      
     res1[i] = np.abs( D_ovlp[(b-1) * D_len + i] )
     res2[i] = np.abs( D_ovlp[(b + B - 1) * D_len + i] )
     pres1[i] = np.abs( pD_ovlp[(b-1) * D_len + i] )
     pres2[i] = np.abs( pD_ovlp[(b + B - 1) * D_len + i] )
 
@@ -44,15 +44,15 @@
   typed_r3 = List()
   [typed_r3.append(x) for x in r3]
   #Calculate the overlap
   overlaps = fast_ovlp(r2, typed_r3, N_len, N, B, b, overlaps)
 
   return overlaps
 
-@jit(nopython=True)
+@jit(nopython=True, error_model='numpy')
 def fast_ovlp(r2, r3, N_len, N, B, b, overlaps):
   #Calculate the overlap
   for i in range(N_len):
     sum = 0
     for j in range(N[i]):
       sum += (r2[j] >= r3[N[i] - 1])
     overlaps[ (b-1) + i*B ] = sum / N[i]
@@ -67,22 +67,22 @@
   pairs = pairs[np.lexsort((pairs[:, 0], pairs[:, 1]))]
 
   # Split the pairs back into the original vectors (dec).
   a, b = split_pairs(pairs, n)
 
   return (a, b)
 
-@jit(nopython=True, parallel=True)
+@jit(nopython=True, parallel=True, error_model='numpy')
 def make_pairs(a, b, n):
   pairs = np.empty((n, 2))
   for i in prange(n):
     pairs[i] = [a[i], b[i]]
   return pairs
 
-@jit(nopython=True, parallel=True)
+@jit(nopython=True, parallel=True, error_model='numpy')
 def split_pairs(pairs, n):
   # Split the pairs back into the original vectors (dec).
   a = np.empty(n)
   b = np.empty(n)
   for i in prange(n):
     a[n-1-i] = pairs[i][0]
     b[n-1-i] = pairs[i][1]
```

### Comparing `rots-py-1.0.2/src/helpers.py` & `rots-py-1.0.3/src/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from numba import njit, jit
 import pandas as pd
 from tqdm import tqdm
 
-@jit(nopython=True)
+@jit(nopython=True, error_model='numpy')
 def bootstrapSamples(B, labels, paired):
   samples = np.zeros((B, len(labels)))#matrix(nrow=B, ncol=length(labels))
   
   for i in range(B):
     for label in np.unique(labels):
       pos = np.where(labels == label)[0]
       #samples[i, pos] = np.random.choice(pos, size=len(pos), replace=True)            
@@ -22,15 +22,15 @@
         #samples[i, pos] = samples[i, np.where(labels == 1)[0]] + pos[0]-1
         _samp = samples[i]
         _samp[pos] = _samp[np.where(labels == 1)[0]] + pos[0]-1
         samples[i] = _samp
   
   return samples
 
-@njit
+@jit(nopython=True, error_model='numpy')
 def permutatedSamples(B, cl):
   samples = np.zeros((B, len(cl)))
   for i in range(B):
     samples[i, :] = np.random.permutation(len(cl))
 
   return samples
 
@@ -48,37 +48,37 @@
      
      #ipdb.set_trace(context=6)   ## BREAKPOINT
 
      ## Row means
      mX = np.nanmean(X, axis=1, keepdims=True) #rowMeans(X, na.rm=TRUE)
      mY = np.nanmean(Y, axis=1, keepdims=True) #rowMeans(Y, na.rm=TRUE)
      
-     mX[np.isnan(mX)] = 0
-     mY[np.isnan(mY)] = 0
+     #mX[np.isnan(mX)] = 0
+     #mY[np.isnan(mY)] = 0
 
      ## Pooled standard deviations for each row
      sX = np.nansum((X - mX)**2, axis=1) #rowSums((X - mX)^2, na.rm=TRUE)
      sY = np.nansum((Y - mY)**2, axis=1) #rowSums((Y - mY)^2, na.rm=TRUE)
 
-     sX[np.isnan(sX)] = 0
-     sY[np.isnan(sY)] = 0
+     #sX[np.isnan(sX)] = 0
+     #sY[np.isnan(sY)] = 0
      
      if not paired:
        ## Number of not NA values in each row
        nX = np.sum(~np.isnan(X), axis=1)
        nY = np.sum(~np.isnan(Y), axis=1)             
 
        ## d == difference between the group means for each row (==gene)
        ## s == pooled standard deviation for each row (==gene)        
        d = mY - mX
        s = np.sqrt(((sX + sY) / (nX + nY - 2)) * (1 / nX + 1 / nY))
        
        ## Cases with less than two non-missing values.
        ## Set d = 0, s = 1
-       ind = np.where( (nY < 2) | (nX < 2) )[0]
+       ind = np.where( (nY < 2) | (nX < 2) )
        d[ind] = 0
        s[ind] = 1
      
      
      if paired:
        ## Add for paired
        sXY = np.nansum((X - mX)*(Y - mY), axis=1)
@@ -193,15 +193,15 @@
   # d = matches
   #ipdb.set_trace(context=10)   ## BREAKPOINT
   d = np.array([np.where(z == v)[0][0] if v in z else None for v in x])
   res = d - a + b
 
   return res
 
-@njit
+@jit(nopython=True, error_model='numpy')
 def pvalue(a, b):
   observed = a.ravel()
   permuted = b.ravel()
   pvalues = np.zeros(len(observed))
 
   j = 0
   for i in range(len(observed)):
```

### Comparing `rots-py-1.0.2/src/rots.py` & `rots-py-1.0.3/src/rots.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.2/src/rots_py.egg-info/PKG-INFO` & `rots-py-1.0.3/src/rots_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

