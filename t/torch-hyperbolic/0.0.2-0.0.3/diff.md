# Comparing `tmp/torch_hyperbolic-0.0.2.tar.gz` & `tmp/torch_hyperbolic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_hyperbolic-0.0.2.tar", last modified: Tue Apr 25 10:27:19 2023, max compression
+gzip compressed data, was "torch_hyperbolic-0.0.3.tar", last modified: Tue Apr 25 14:44:00 2023, max compression
```

## Comparing `torch_hyperbolic-0.0.2.tar` & `torch_hyperbolic-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.254868 torch_hyperbolic-0.0.2/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1073 2023-04-24 11:21:18.000000 torch_hyperbolic-0.0.2/LICENSE.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-25 10:27:19.253980 torch_hyperbolic-0.0.2/PKG-INFO
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     3429 2023-04-25 10:19:14.000000 torch_hyperbolic-0.0.2/README.md
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       38 2023-04-25 10:27:19.255067 torch_hyperbolic-0.0.2/setup.cfg
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      318 2023-04-25 10:26:27.000000 torch_hyperbolic-0.0.2/setup.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.232031 torch_hyperbolic-0.0.2/torch_hyperbolic/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 11:39:11.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/__init__.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594    14001 2023-04-25 09:46:50.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/manifolds.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.239075 torch_hyperbolic-0.0.2/torch_hyperbolic/models/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       19 2023-04-25 08:18:26.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/models/__init__.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     2560 2023-04-25 09:35:38.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/models/hgnn.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 16:01:54.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/models/hmlp.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.252761 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      130 2023-04-24 16:20:44.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/__init__.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      999 2023-04-25 08:25:34.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hact.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1036 2023-04-24 15:34:16.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hdecoder.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1053 2023-04-24 15:39:13.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hencoder.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     9837 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgat.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     4397 2023-04-24 12:49:54.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgcn.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1784 2023-04-25 08:26:39.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hlinear.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     7252 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/optim.py
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1542 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.2/torch_hyperbolic/utils.py
-drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 10:27:19.236581 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/PKG-INFO
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594      651 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/SOURCES.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594        1 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/dependency_links.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       31 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/requires.txt
--rw-r--r--   0 florin.ratajczak (471454700) 2125895594       17 2023-04-25 10:27:19.000000 torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/top_level.txt
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 14:44:00.704282 torch_hyperbolic-0.0.3/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1073 2023-04-24 11:21:18.000000 torch_hyperbolic-0.0.3/LICENSE.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-25 14:44:00.703465 torch_hyperbolic-0.0.3/PKG-INFO
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     3336 2023-04-25 10:31:43.000000 torch_hyperbolic-0.0.3/README.md
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       38 2023-04-25 14:44:00.704360 torch_hyperbolic-0.0.3/setup.cfg
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      325 2023-04-25 14:43:10.000000 torch_hyperbolic-0.0.3/setup.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 14:44:00.692345 torch_hyperbolic-0.0.3/torch_hyperbolic/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594        0 2023-04-24 11:39:11.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/__init__.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594    14200 2023-04-25 14:09:35.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/manifolds.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 14:44:00.696585 torch_hyperbolic-0.0.3/torch_hyperbolic/models/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       44 2023-04-25 14:42:16.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/models/__init__.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     2559 2023-04-25 13:15:06.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/models/hgnn.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     2970 2023-04-25 14:34:24.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/models/hgnn_film.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 14:44:00.702904 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      151 2023-04-25 12:49:04.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/__init__.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      836 2023-04-25 14:17:06.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hact.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1036 2023-04-24 15:34:16.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hdecoder.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1058 2023-04-25 13:37:19.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hencoder.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     6248 2023-04-25 14:12:52.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hfilm.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     9817 2023-04-25 12:38:46.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hgat.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     4397 2023-04-24 12:49:54.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hgcn.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1784 2023-04-25 08:26:39.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hlinear.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     7252 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/optim.py
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594     1542 2023-04-24 10:36:01.000000 torch_hyperbolic-0.0.3/torch_hyperbolic/utils.py
+drwxr-xr-x   0 florin.ratajczak (471454700) 2125895594        0 2023-04-25 14:44:00.694652 torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      153 2023-04-25 14:44:00.000000 torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/PKG-INFO
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594      685 2023-04-25 14:44:00.000000 torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/SOURCES.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594        1 2023-04-25 14:44:00.000000 torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/dependency_links.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       31 2023-04-25 14:44:00.000000 torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/requires.txt
+-rw-r--r--   0 florin.ratajczak (471454700) 2125895594       17 2023-04-25 14:44:00.000000 torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/top_level.txt
```

### Comparing `torch_hyperbolic-0.0.2/LICENSE.txt` & `torch_hyperbolic-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.2/README.md` & `torch_hyperbolic-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ![build](https://github.com/fratajcz/pytorch_hyperbolic/actions/workflows/build.yml/badge.svg)
-![pypi](https://github.com/fratajcz/pytorch_hyperbolic/actions/workflows/pypi.yml/badge.svg)
 
 # pytorch_hyperbolic
 Implementation of hyperbolic NNs and GNNs 
 
 # Installation
 
 ```
```

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/manifolds.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/manifolds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import torch
 
 """Base manifold."""
 
 from torch.nn import Parameter
-from .utils import artanh, tanh, arcosh, cosh, sinh
-
+from .utils import tanh, arcosh, cosh, sinh, artanh
 
 class Manifold(object):
     """
     Abstract class to define operations on a manifold.
     """
 
     def __init__(self):
@@ -146,26 +145,30 @@
         sub = self.mobius_add(-p1, p2, c)
         sub_norm = sub.norm(dim=-1, p=2, keepdim=True).clamp_min(self.min_norm)
         lam = self._lambda_x(p1, c)
         sqrt_c = c ** 0.5
         return 2 / sqrt_c / lam * artanh(sqrt_c * sub_norm) * sub / sub_norm
 
     def expmap0(self, u, c):
-        sqrt_c = c ** 0.5
-        u_norm = torch.clamp_min(u.norm(dim=-1, p=2, keepdim=True), self.min_norm)
-        gamma_1 = tanh(sqrt_c * u_norm) * u / (sqrt_c * u_norm)
-        return gamma_1
+        #sqrt_c = c ** 0.5
+        #u_norm = torch.clamp_min(u.norm(dim=-1, p=2, keepdim=True), self.min_norm)
+        #gamma_1 = tan_k(u_norm, k) * (u / u_norm)
+        #left_side = torch.tanh(sqrt_c * u_norm)
+        #right_side = (u / (sqrt_c * u_norm))
+        #gamma_1 = left_side * right_side
+        zeros = torch.zeros_like(u)
+        #return gamma_1
+        return self.expmap(u, zeros, c)
 
     def expmap(self, u, p, c):
         sqrt_c = c ** 0.5
         u_norm = u.norm(dim=-1, p=2, keepdim=True).clamp_min(self.min_norm)
         second_term = (
-                tanh(sqrt_c / 2 * self._lambda_x(p, c) * u_norm)
-                * u
-                / (sqrt_c * u_norm)
+                torch.tanh(sqrt_c * ((self._lambda_x(p, c) * u_norm) / 2 ))
+                * (u / (sqrt_c * u_norm))
         )
         gamma_1 = self.mobius_add(p, second_term, c)
         return gamma_1
 
     def mobius_add(self, x, y, c, dim=-1):
         x2 = x.pow(2).sum(dim=dim, keepdim=True)
         y2 = y.pow(2).sum(dim=dim, keepdim=True)
```

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/models/hgnn.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/models/hgnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.act0 = hypnn.HypAct(act, manifold=manifold, c_in=self.curvatures[0], c_out=self.curvatures[1])
         self.dropout0 = nn.Dropout(p=dropout)
 
         self.gnn1 = hypnn.HGCNConv(in_channels=hidden_dim, out_channels=hidden_dim, manifold=manifold, c=self.curvatures[1], dropout=dropout, **gcn_kwargs)
         self.act1 = hypnn.HypAct(act, manifold=manifold, c_in=self.curvatures[1], c_out=self.curvatures[2])
         self.dropout1 = nn.Dropout(p=dropout)
 
-        self.gnn2 = hypnn.HGCNConv(in_channels=hidden_dim, out_channels=hidden_dim, manifold=manifold, c=self.curvatures[2], dropout=dropout, **gcn_kwargs)
+        self.gnn2 = hypnn.HGCNConv(in_channels=hidden_dim, out_channels=hidden_dim, manifold=manifold, c=self.curvatures[2], dropout=dropout, *gcn_kwargs)
         self.act2 = hypnn.HypAct(act, manifold=manifold, c_in=self.curvatures[2], c_out=self.curvatures[3])
         self.dropout2 = nn.Dropout(p=dropout)
 
         self.output_lin = hypnn.HypLinear(manifold=manifold, in_channels=hidden_dim, out_channels=out_channels, c=self.curvatures[3])
         self.decoder = hypnn.HyperbolicDecoder(manifold=manifold, curvature=self.curvatures[3])
 
     def forward(self, x, adj):
```

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hdecoder.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hdecoder.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hencoder.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hencoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
         self.curvature = nn.Parameter(torch.Tensor([1.])) if curvature is None else curvature
         self.manifold = getattr(manifolds, manifold)()
 
     def forward(self, x):
         """ Projects x into hyperbolic space """
         if isinstance(self.manifold, manifolds.Hyperboloid):
             x = torch.cat((torch.zeros_like(x)[:, 0:1], x), dim=-1)
+
         x_tan = self.manifold.proj_tan0(x, self.curvature)
+
         x_hyp = self.manifold.expmap0(x_tan, c=self.curvature)
+ 
         x_hyp = self.manifold.proj(x_hyp, c=self.curvature)
+
         return x_hyp
 
     def extra_repr(self):
         return 'c={}'.format(self.curvature)
```

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgat.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hgat.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from torch_geometric.nn import MessagePassing
 from torch_geometric.utils import degree
 from .hlinear import HypLinear
 import torch_hyperbolic.manifolds as manifolds
 from torch_geometric.typing import PairTensor
 from torch import Tensor
 from torch.nn import Parameter
-import torch_sparse
 
 from torch_geometric.typing import (
     Adj,
     OptPairTensor,
     OptTensor,
     Size,
     SparseTensor,
```

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hgcn.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hgcn.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/nn/hlinear.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/nn/hlinear.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/optim.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/optim.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic/utils.py` & `torch_hyperbolic-0.0.3/torch_hyperbolic/utils.py`

 * *Files identical despite different names*

### Comparing `torch_hyperbolic-0.0.2/torch_hyperbolic.egg-info/SOURCES.txt` & `torch_hyperbolic-0.0.3/torch_hyperbolic.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 torch_hyperbolic.egg-info/PKG-INFO
 torch_hyperbolic.egg-info/SOURCES.txt
 torch_hyperbolic.egg-info/dependency_links.txt
 torch_hyperbolic.egg-info/requires.txt
 torch_hyperbolic.egg-info/top_level.txt
 torch_hyperbolic/models/__init__.py
 torch_hyperbolic/models/hgnn.py
-torch_hyperbolic/models/hmlp.py
+torch_hyperbolic/models/hgnn_film.py
 torch_hyperbolic/nn/__init__.py
 torch_hyperbolic/nn/hact.py
 torch_hyperbolic/nn/hdecoder.py
 torch_hyperbolic/nn/hencoder.py
+torch_hyperbolic/nn/hfilm.py
 torch_hyperbolic/nn/hgat.py
 torch_hyperbolic/nn/hgcn.py
 torch_hyperbolic/nn/hlinear.py
```

