# Comparing `tmp/roma-1.3.1.tar.gz` & `tmp/roma-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roma-1.3.1.tar", last modified: Mon Sep 19 13:29:54 2022, max compression
+gzip compressed data, was "roma-1.3.2.tar", last modified: Wed Apr 26 16:22:56 2023, max compression
```

## Comparing `roma-1.3.1.tar` & `roma-1.3.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 rbregier (1809414175) domain users (1809400513)        0 2022-09-19 13:29:54.563865 roma-1.3.1/
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)    21068 2021-06-29 07:12:47.000000 roma-1.3.1/LICENSE
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     2276 2021-06-29 07:12:47.000000 roma-1.3.1/NOTICE
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     3987 2022-09-19 13:29:54.559865 roma-1.3.1/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     3509 2022-08-21 20:37:54.000000 roma-1.3.1/README.md
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)      103 2021-06-29 15:21:23.000000 roma-1.3.1/pyproject.toml
-drwxr-xr-x   0 rbregier (1809414175) domain users (1809400513)        0 2022-09-19 13:29:54.559865 roma-1.3.1/roma/
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)      145 2021-05-26 08:11:04.000000 roma-1.3.1/roma/__init__.py
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     2433 2022-09-19 09:34:33.000000 roma-1.3.1/roma/internal.py
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)    17830 2022-09-19 12:08:53.000000 roma-1.3.1/roma/mappings.py
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)    17322 2022-09-19 13:23:22.000000 roma-1.3.1/roma/utils.py
-drwxr-xr-x   0 rbregier (1809414175) domain users (1809400513)        0 2022-09-19 13:29:54.559865 roma-1.3.1/roma.egg-info/
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     3987 2022-09-19 13:29:54.000000 roma-1.3.1/roma.egg-info/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)      327 2022-09-19 13:29:54.000000 roma-1.3.1/roma.egg-info/SOURCES.txt
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)        1 2022-09-19 13:29:54.000000 roma-1.3.1/roma.egg-info/dependency_links.txt
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)        5 2022-09-19 13:29:54.000000 roma-1.3.1/roma.egg-info/top_level.txt
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)       38 2022-09-19 13:29:54.563865 roma-1.3.1/setup.cfg
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)      672 2022-09-19 13:09:17.000000 roma-1.3.1/setup.py
-drwxr-xr-x   0 rbregier (1809414175) domain users (1809400513)        0 2022-09-19 13:29:54.559865 roma-1.3.1/test/
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     1018 2021-05-26 08:11:04.000000 roma-1.3.1/test/test_derivatives.py
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     8457 2022-09-19 13:29:30.000000 roma-1.3.1/test/test_mappings.py
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)     3430 2022-09-19 08:17:03.000000 roma-1.3.1/test/test_procrustes_derivatives.py
--rw-r--r--   0 rbregier (1809414175) domain users (1809400513)    12395 2022-09-19 13:09:10.000000 roma-1.3.1/test/test_utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-04-26 16:22:56.371088 roma-1.3.2/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21068 2023-02-08 15:17:32.000000 roma-1.3.2/LICENSE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2023-02-08 15:17:32.000000 roma-1.3.2/NOTICE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3987 2023-04-26 16:22:56.371088 roma-1.3.2/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3509 2023-02-08 15:17:32.000000 roma-1.3.2/README.md
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.3.2/pyproject.toml
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-04-26 16:22:56.371088 roma-1.3.2/roma/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      145 2023-02-08 15:17:32.000000 roma-1.3.2/roma/__init__.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2433 2023-02-08 15:17:32.000000 roma-1.3.2/roma/internal.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    18038 2023-04-26 08:34:41.000000 roma-1.3.2/roma/mappings copy.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    17616 2023-04-26 08:34:54.000000 roma-1.3.2/roma/mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    18146 2023-04-26 15:40:11.000000 roma-1.3.2/roma/utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-04-26 16:22:56.371088 roma-1.3.2/roma.egg-info/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3987 2023-04-26 16:22:56.000000 roma-1.3.2/roma.egg-info/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      349 2023-04-26 16:22:56.000000 roma-1.3.2/roma.egg-info/SOURCES.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2023-04-26 16:22:56.000000 roma-1.3.2/roma.egg-info/dependency_links.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2023-04-26 16:22:56.000000 roma-1.3.2/roma.egg-info/top_level.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2023-04-26 16:22:56.371088 roma-1.3.2/setup.cfg
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2023-04-26 10:34:33.000000 roma-1.3.2/setup.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2023-04-26 16:22:56.371088 roma-1.3.2/test/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1018 2023-02-08 15:17:32.000000 roma-1.3.2/test/test_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8457 2023-02-08 15:17:32.000000 roma-1.3.2/test/test_mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3430 2023-02-08 15:17:32.000000 roma-1.3.2/test/test_procrustes_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    12634 2023-04-26 10:18:23.000000 roma-1.3.2/test/test_utils.py
```

### Comparing `roma-1.3.1/LICENSE` & `roma-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/NOTICE` & `roma-1.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/PKG-INFO` & `roma-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.3.1
+Version: 1.3.2
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `roma-1.3.1/README.md` & `roma-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/roma/internal.py` & `roma-1.3.2/roma/internal.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/roma/mappings.py` & `roma-1.3.2/roma/mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,57 +10,52 @@
 import torch
 import roma.internal
 
 class _ProcrustesManualDerivatives(torch.autograd.Function):
     @staticmethod
     def forward(ctx, M, force_rotation, regularization, gradient_eps):
         assert (M.dim() == 3 and M.shape[1] == M.shape[2]), "Input should be a BxDxD batch of matrices."
+        # Singular values of D are sorted in descending order
         U, D, V = roma.internal.svd(M)
-        # D is sorted in descending order
-        SVt = V.transpose(-1,-2)
         if force_rotation:
             # We flip the smallest singular value to ensure getting a rotation matrix
             with torch.no_grad():
-                flip = (torch.det(U) * torch.det(V) < 0)
-            SVt[flip,-1,:] *= -1
+                flip = (torch.det(U) * torch.det(V) < 0)            
+            # in-place modifications of variables not used afterwards.
+            DS = D
+            DS[flip, -1] *= -1
+            del D
+            US = U
+            US[flip,:,-1] *= -1
+            del U
         else:
             flip = None
-        R = U @ SVt
-        # Store data for backprop
-        ctx.save_for_backward(U, D, V, flip, M, R)
+            DS = D
+            US = U
+        R = US @ V.transpose(-1, -2)
+        # Store data for backprop:
+        ctx.save_for_backward(US, DS, V, M, R)
         ctx.gradient_eps = gradient_eps
         ctx.regularization = regularization
         return R
 
     @staticmethod
     def backward(ctx, grad_R):
-        U, D, V, flip, M, R = ctx.saved_tensors
+        US, DS, V, M, R = ctx.saved_tensors
         gradient_eps = ctx.gradient_eps
 
-        Uik_Vjl = torch.einsum('bik,bjl -> bklij', U, V)
-        Uil_Vjk = Uik_Vjl.transpose(1,2)
-
-        Dl = D[:,None,:,None,None]
-        Dk = D[:,:,None,None,None]
-
-        # Default Omega
-        Omega_klij = (Uik_Vjl - Uil_Vjk) * roma.internal._pseudo_inverse(Dk + Dl, gradient_eps)
-        # Diagonal should already be 0 thanks to clamping even in case of rank deficient input
-        # Deal with flips (det(U) det(V) < 0)
-        if flip is not None:
-            # k!=d, l=d
-            Omega_klij[flip,:-1,-1,:,:] = (Uik_Vjl[flip,:-1,-1] - Uil_Vjk[flip,:-1,-1]) * roma.internal._pseudo_inverse(Dk[flip,:-1,-1] - Dl[flip,:,-1], gradient_eps)
-            
-            # k=d, l!=d
-            Omega_klij[flip,-1,:-1,:,:] = -Omega_klij[flip,:-1,-1,:,:]
+        USik_Vjl = torch.einsum('bik,bjl -> bklij', US, V)
+        USil_Vjk = USik_Vjl.transpose(1,2)
+        DSl = DS[:,None,:,None,None]
+        DSk = DS[:,:,None,None,None]
+        Omega_klij = (USik_Vjl - USil_Vjk) * roma.internal._pseudo_inverse(DSk + DSl, gradient_eps)
+        # Note: this intermediary matrix may require lots of memory for large dimensional cases.
+        # Diagonal k==l should always be 0 thanks to the clamping of the pseudo-inverse.
         
-        UOmega = torch.einsum('bkm, bmlij -> bklij', U, Omega_klij)
-        Janalytical = torch.einsum('bkmij, bml -> bklij', UOmega, V.transpose(-1,-2))
-        grad_M = torch.einsum('bkl, bklij -> bij', grad_R, Janalytical)
-
+        grad_M = torch.einsum('bnm, bnk, bklij, bml -> bij', grad_R, US, Omega_klij, V)
         if ctx.regularization != 0.0:
             # Add a regularization term in the direction of the orthonormalized output.
             grad_M += ctx.regularization * (M - R)
         return grad_M, None, None, None
 
 def procrustes(M, force_rotation=False, regularization=0.0, gradient_eps=1e-5):
     """
```

### Comparing `roma-1.3.1/roma/utils.py` & `roma-1.3.2/roma/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         K. Shoemake, “Uniform Random Rotations”, in Graphics Gems III (IBM Version), Elsevier, 1992, pp. 124–132. doi: 10.1016/B978-0-08-050755-2.50036-1.
 
     """
     if type(size) == int:
         size = (size,)
 
     x0 = torch.rand(size, dtype=dtype, device=device)
-    theta1 = (2.0 * np.pi) * torch.rand(size)
-    theta2 = (2.0 * np.pi) * torch.rand(size)
+    theta1 = (2.0 * np.pi) * torch.rand(size, dtype=dtype, device=device)
+    theta2 = (2.0 * np.pi) * torch.rand(size, dtype=dtype, device=device)
     r1 = torch.sqrt(1.0 - x0)
     r2 = torch.sqrt(x0)
     return torch.stack((r1 * torch.sin(theta1), r1 * torch.cos(theta1), r2 * torch.sin(theta2), r2 * torch.cos(theta2)), dim=-1)
 
 def random_rotmat(size  = tuple(), dtype=torch.float, device=None):
     """
     Generates a batch of random 3x3 rotation matrices, uniformly sampled according to the usual rotation metric.
@@ -380,52 +380,61 @@
         batch of interpolated rotation matrices (BxAx3x3 tensor).
     """    
     q0 = roma.mappings.rotmat_to_unitquat(R0)
     q1 = roma.mappings.rotmat_to_unitquat(R1)
     interpolated_q = unitquat_slerp(q0, q1, steps, shortest_arc=True)
     return roma.mappings.unitquat_to_rotmat(interpolated_q)
 
-def rigid_vectors_registration(x, y):
+def rigid_vectors_registration(x, y, weights=None):
     """
-    Returns the rotation matrix :math:`R` that best aligns an input list of vectors :math:`(x_i)_{i=1...n}` to a target list of vectors :math:`(y_i)_{i=1...n}`,
-    by minimizing the sum of square distance :math:`\sum_i \|R x_i - y_i\|^2`.
-
+    Returns the rotation matrix :math:`R` that best aligns an input list of vectors :math:`(x_i)_{i=1...n}` to a target list of vectors :math:`(y_i)_{i=1...n}`
+    by minimizing the sum of square distance :math:`\sum_i w_i \|R x_i - y_i\|^2`, where :math:`(w_i)_{i=1...n}` denotes optional positive weights.
     See :func:`~roma.utils.rigid_points_registration` for details.
 
     Args:
         x (...xNxD tensor): list of N vectors of dimension D.
         y (...xNxD tensor): list of corresponding target vectors.
+        weights (None or ...xN tensor): optional list of weights associated to each vector.
     Returns:
         The rotation matrix :math:`R` (...xDxD tensor).
-    """    
-    M = torch.einsum("...ki, ...kj -> ...ij", y, x)
+    """
+    if weights is None:
+        M = torch.einsum("...ki, ...kj -> ...ij", y, x)
+    else:
+        M = torch.einsum("...k, ...ki, ...kj -> ...ij", weights, y, x)
     R = roma.special_procrustes(M)
     return R
 
-def rigid_points_registration(x, y):
+def rigid_points_registration(x, y, weights=None):
     """
     Returns the rigid transformation :math:`(R,t)` that best aligns an input list of points :math:`(x_i)_{i=1...n}` to a target list of points :math:`(y_i)_{i=1...n}`,
-    by minimizing the sum of square distance :math:`\sum_i \|R x_i + t - y_i\|^2`.
+    by minimizing the sum of square distance :math:`\sum_i w_i \|R x_i + t - y_i\|^2`, where :math:`(w_i)_{i=1...n}` denotes optional positive weights.
     This is sometimes referred to as the Kabsch/Umeyama algorithm.
 
     Args:
         x (...xNxD tensor): list of N points of dimension D.
         y (...xNxD tensor): list of corresponding target points.
+        weights (None or ...xN tensor): optional list of weights associated to each point.
     Returns:
         a tuple :math:`(R, t)` consisting of a rotation matrix :math:`R` (...xDxD tensor) and a translation vector :math:`t` (...xD tensor).
 
     References:
         S. Umeyama, “Least-squares estimation of transformation parameters between two point patterns,” IEEE Transactions on pattern analysis and machine intelligence, vol. 13, no. 4, Art. no. 4, 1991.        
 
         W. Kabsch, "A solution for the best rotation to relate two sets of vectors". Acta Crystallographica, A32, 1976.
     """
     # Center data
-    xmean = torch.mean(x, dim=-2, keepdim=True)
-    ymean = torch.mean(y, dim=-2, keepdim=True)
+    if weights is None:
+        xmean = torch.mean(x, dim=-2, keepdim=True)
+        ymean = torch.mean(y, dim=-2, keepdim=True)
+    else:
+        normalized_weights = weights / torch.sum(weights, dim=-1, keepdim=True)
+        xmean = torch.sum(normalized_weights[...,None] * x, dim=-2, keepdim=True)
+        ymean = torch.sum(normalized_weights[...,None] * y, dim=-2, keepdim=True)
     xhat = x - xmean
     yhat = y - ymean
     
-    # Solve the problem
-    R = rigid_vectors_registration(xhat, yhat)
+    # Solve the vectors registration problem
+    R = rigid_vectors_registration(xhat, yhat, weights)
     t = (ymean - torch.einsum('...ik, ...jk -> ...ji', R, xmean)).squeeze(-2)
     return R, t
```

### Comparing `roma-1.3.1/roma.egg-info/PKG-INFO` & `roma-1.3.2/roma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.3.1
+Version: 1.3.2
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `roma-1.3.1/setup.py` & `roma-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="roma",
-    version="1.3.1",
+    version="1.3.2",
     author="Romain Brégier",
     author_email="romain.bregier@naverlabs.com",
     description="A lightweight library to deal with 3D rotations in PyTorch.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/naver/roma",
     packages=["roma"],
```

### Comparing `roma-1.3.1/test/test_derivatives.py` & `roma-1.3.2/test/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/test/test_mappings.py` & `roma-1.3.2/test/test_mappings.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/test/test_procrustes_derivatives.py` & `roma-1.3.2/test/test_procrustes_derivatives.py`

 * *Files identical despite different names*

### Comparing `roma-1.3.1/test/test_utils.py` & `roma-1.3.2/test/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -218,31 +218,32 @@
             self.assertTrue(is_close(roma.quat_composition((q_list[0], roma.quat_inverse(q_list[0]))), torch.as_tensor([0.0, 0.0, 0.0, 1])))
             self.assertTrue(is_close(roma.rotvec_composition((rotvec_list[0], roma.rotvec_inverse(rotvec_list[0]))), torch.zeros(3)))
 
     def test_rigid_vectors_registration(self):
         batch_shape = (34, 16)
         n = 100
         for dtype in (torch.float32, torch.float64):
-            R_true = roma.random_rotmat(batch_shape, dtype=dtype)
-            X = torch.randn(batch_shape + (n, 3,), dtype=dtype)
-            Y = torch.einsum('...ik, ...jk -> ...ji', R_true, X)
-            R = roma.rigid_vectors_registration(X, Y)
-
-        self.assertTrue(is_close(R, R_true))
+            for weights in [None, torch.rand(size=batch_shape + (n,), dtype=dtype)]:
+                R_true = roma.random_rotmat(batch_shape, dtype=dtype)
+                X = torch.randn(batch_shape + (n, 3,), dtype=dtype)
+                Y = torch.einsum('...ik, ...jk -> ...ji', R_true, X)
+                R = roma.rigid_vectors_registration(X, Y, weights)
+                self.assertTrue(is_close(R, R_true))
 
     def test_rigid_point_registration(self):
         batch_shape = (34, 16)
         n = 100
         for dtype in (torch.float32, torch.float64):
-            R_true = roma.random_rotmat(batch_shape, dtype=dtype)
-            t_true = torch.randn(batch_shape + (3,), dtype=dtype)
-            X = torch.randn(batch_shape + (n, 3,), dtype=dtype)
-            Y = torch.einsum('...ik, ...jk -> ...ji', R_true, X) + t_true.unsqueeze(-2)
-            R, t = roma.rigid_points_registration(X, Y)
+            for weights in [None, torch.rand(size=batch_shape + (n,), dtype=dtype)]:
+                R_true = roma.random_rotmat(batch_shape, dtype=dtype)
+                t_true = torch.randn(batch_shape + (3,), dtype=dtype)
+                X = torch.randn(batch_shape + (n, 3,), dtype=dtype)
+                Y = torch.einsum('...ik, ...jk -> ...ji', R_true, X) + t_true.unsqueeze(-2)
+                R, t = roma.rigid_points_registration(X, Y, weights)
 
-            self.assertTrue(is_close(R, R_true))
-            self.assertTrue(is_close(t, t_true))
+                self.assertTrue(is_close(R, R_true))
+                self.assertTrue(is_close(t, t_true))
   
         
 if __name__ == "__main__":
     unittest.main()
```

