# Comparing `tmp/mzt-1.1.4a0.tar.gz` & `tmp/mzt-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzt-1.1.4a0.tar", last modified: Tue Nov 15 07:33:28 2022, max compression
+gzip compressed data, was "mzt-1.1.5.tar", last modified: Tue Apr 25 17:43:56 2023, max compression
```

## Comparing `mzt-1.1.4a0.tar` & `mzt-1.1.5.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    34523 2022-08-18 14:03:37.000000 mzt-1.1.4a0/LICENSE
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    41199 2022-11-15 07:33:28.158582 mzt-1.1.4a0/PKG-INFO
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      715 2022-11-15 07:23:34.000000 mzt-1.1.4a0/README.md
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.154582 mzt-1.1.4a0/modelZoo/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      853 2022-08-18 14:03:37.000000 mzt-1.1.4a0/modelZoo/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4341 2022-08-18 14:03:37.000000 mzt-1.1.4a0/modelZoo/mbnetv2.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2016 2022-08-18 14:03:37.000000 mzt-1.1.4a0/modelZoo/shufflenet.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.154582 mzt-1.1.4a0/moduleZoo/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      777 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/__init__.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.154582 mzt-1.1.4a0/moduleZoo/attention/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      680 2022-08-18 14:48:00.000000 mzt-1.1.4a0/moduleZoo/attention/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    10289 2022-09-07 14:47:25.000000 mzt-1.1.4a0/moduleZoo/attention/conv_multi_head_attention.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      708 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/attention/conv_self_attention.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4730 2022-09-07 11:36:52.000000 mzt-1.1.4a0/moduleZoo/attention/linear_multi_head_attention.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      379 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/attention/utils.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/moduleZoo/convolution/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      958 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/convolution/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     8907 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/convolution/convblocks.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     6880 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/convolution/invertedconvblocks.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/moduleZoo/dense/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       88 2022-08-18 14:49:30.000000 mzt-1.1.4a0/moduleZoo/dense/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1454 2022-08-18 14:48:27.000000 mzt-1.1.4a0/moduleZoo/dense/denseblocks.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/moduleZoo/graphs/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       63 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/graphs/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2519 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/graphs/grah_conv.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      947 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/graphs/utils.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/moduleZoo/resblocks/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1175 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/resblocks/__init__.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7821 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/resblocks/bottleneckresidual.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     5383 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/resblocks/invertedresidual.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     6098 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/resblocks/residual.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      487 2022-08-18 14:03:37.000000 mzt-1.1.4a0/moduleZoo/utils.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/mzExtras/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4018 2022-08-18 14:03:37.000000 mzt-1.1.4a0/mzExtras/LARC.py
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       44 2022-08-18 14:03:37.000000 mzt-1.1.4a0/mzExtras/__init__.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/mzLosses/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1963 2022-08-18 14:03:37.000000 mzt-1.1.4a0/mzLosses/contrastive.py
-drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2022-11-15 07:33:28.158582 mzt-1.1.4a0/mzt.egg-info/
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    41199 2022-11-15 07:33:28.000000 mzt-1.1.4a0/mzt.egg-info/PKG-INFO
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      924 2022-11-15 07:33:28.000000 mzt-1.1.4a0/mzt.egg-info/SOURCES.txt
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)        1 2022-11-15 07:33:28.000000 mzt-1.1.4a0/mzt.egg-info/dependency_links.txt
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       37 2022-11-15 07:33:28.000000 mzt-1.1.4a0/mzt.egg-info/top_level.txt
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      668 2022-11-15 07:33:08.000000 mzt-1.1.4a0/pyproject.toml
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       38 2022-11-15 07:33:28.158582 mzt-1.1.4a0/setup.cfg
--rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1290 2022-11-15 07:33:02.000000 mzt-1.1.4a0/setup.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    34523 2022-08-18 14:03:37.000000 mzt-1.1.5/LICENSE
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1246 2023-04-25 17:43:56.749558 mzt-1.1.5/PKG-INFO
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      715 2022-11-15 07:23:34.000000 mzt-1.1.5/README.md
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.745558 mzt-1.1.5/modelZoo/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      812 2023-04-25 17:36:17.000000 mzt-1.1.5/modelZoo/__init__.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.745558 mzt-1.1.5/modelZoo/graphs/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       47 2023-04-25 17:36:17.000000 mzt-1.1.5/modelZoo/graphs/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1585 2022-08-18 14:03:37.000000 mzt-1.1.5/modelZoo/graphs/dgcnn.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4341 2022-08-18 14:03:37.000000 mzt-1.1.5/modelZoo/mbnetv2.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2016 2022-08-18 14:03:37.000000 mzt-1.1.5/modelZoo/shufflenet.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.745558 mzt-1.1.5/moduleZoo/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      777 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/__init__.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/attention/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      680 2022-08-18 14:48:00.000000 mzt-1.1.5/moduleZoo/attention/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)    10289 2022-09-07 14:47:25.000000 mzt-1.1.5/moduleZoo/attention/conv_multi_head_attention.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      708 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/attention/conv_self_attention.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4730 2022-09-07 11:36:52.000000 mzt-1.1.5/moduleZoo/attention/linear_multi_head_attention.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      379 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/attention/utils.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/convolution/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      958 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/convolution/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     8907 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/convolution/convblocks.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7226 2023-04-25 17:36:17.000000 mzt-1.1.5/moduleZoo/convolution/invertedconvblocks.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/dense/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       88 2022-08-18 14:49:30.000000 mzt-1.1.5/moduleZoo/dense/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1454 2022-08-18 14:48:27.000000 mzt-1.1.5/moduleZoo/dense/denseblocks.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/graphs/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       63 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/graphs/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     2519 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/graphs/grah_conv.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      947 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/graphs/utils.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/moduleZoo/resblocks/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1175 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/resblocks/__init__.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     7821 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/resblocks/bottleneckresidual.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     5485 2023-04-25 17:36:17.000000 mzt-1.1.5/moduleZoo/resblocks/invertedresidual.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     6098 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/resblocks/residual.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      487 2022-08-18 14:03:37.000000 mzt-1.1.5/moduleZoo/utils.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/mzExtras/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     4018 2022-08-18 14:03:37.000000 mzt-1.1.5/mzExtras/LARC.py
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       44 2022-08-18 14:03:37.000000 mzt-1.1.5/mzExtras/__init__.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/mzLosses/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1963 2022-08-18 14:03:37.000000 mzt-1.1.5/mzLosses/contrastive.py
+drwxrwxr-x   0 shivampr21  (1000) shivampr21  (1000)        0 2023-04-25 17:43:56.749558 mzt-1.1.5/mzt.egg-info/
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1246 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/PKG-INFO
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)      962 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/SOURCES.txt
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)        1 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/dependency_links.txt
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       37 2023-04-25 17:43:56.000000 mzt-1.1.5/mzt.egg-info/top_level.txt
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)       38 2023-04-25 17:43:56.749558 mzt-1.1.5/setup.cfg
+-rw-rw-r--   0 shivampr21  (1000) shivampr21  (1000)     1317 2023-04-25 17:41:01.000000 mzt-1.1.5/setup.py
```

### Comparing `mzt-1.1.4a0/LICENSE` & `mzt-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/README.md` & `mzt-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/modelZoo/__init__.py` & `mzt-1.1.5/moduleZoo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,11 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
-from .graphs import DGCNN
-
-# from .mbnetv2 import MobileNetV2
-# from .shufflenet import ShuffleInvertedResidual
-
-__all__ = ('MobileNetV2', 'ShuffleInvertedResidual', 'DGCNN')
+from .attention import *
+from .convolution import *
+from .graphs import *
+from .resblocks import *
```

### Comparing `mzt-1.1.4a0/modelZoo/mbnetv2.py` & `mzt-1.1.5/modelZoo/mbnetv2.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/modelZoo/shufflenet.py` & `mzt-1.1.5/modelZoo/shufflenet.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/__init__.py` & `mzt-1.1.5/modelZoo/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,11 +11,13 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
-from .attention import *
-from .convolution import *
-from .graphs import *
-from .resblocks import *
+from .graphs import DGCNN
+
+# from .mbnetv2 import MobileNetV2
+# from .shufflenet import ShuffleInvertedResidual
+
+__all__ = ('DGCNN',)
```

### Comparing `mzt-1.1.4a0/moduleZoo/attention/__init__.py` & `mzt-1.1.5/moduleZoo/attention/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/attention/conv_multi_head_attention.py` & `mzt-1.1.5/moduleZoo/attention/conv_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/attention/conv_self_attention.py` & `mzt-1.1.5/moduleZoo/attention/conv_self_attention.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/attention/linear_multi_head_attention.py` & `mzt-1.1.5/moduleZoo/attention/linear_multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/convolution/__init__.py` & `mzt-1.1.5/moduleZoo/convolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/convolution/convblocks.py` & `mzt-1.1.5/moduleZoo/convolution/convblocks.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/convolution/invertedconvblocks.py` & `mzt-1.1.5/moduleZoo/convolution/invertedconvblocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,48 +24,50 @@
 
 
 class ConvInvertedBlock2d(nn.Module):
 
     def __init__(self,
                  in_channels: int,
                  expansion_ratio: float,
+                 out_channels: Optional[float] = None,
                  kernel_size: Union[int, Tuple[int, int]] = 3,
                  stride: Union[int, Tuple[int, int]] = 1,
                  norm_layer: Optional[Callable[..., nn.Module]] = None,
                  activation_layer: Optional[Callable[..., nn.Module]] = nn.ReLU6,
                  channel_shuffle: bool = False,
                  grouping: int = 1) -> None:
         super().__init__()
 
-        hidden_channels = round(in_channels * expansion_ratio)
+        self.hidden_channels = round(in_channels * expansion_ratio)
+        self.out_channels = in_channels if out_channels is None else out_channels
 
         self.activation = activation_layer() if activation_layer is not None else None
 
         self.conv1 = ConvNormActivation2d(in_channels,
-                                          hidden_channels,
+                                          self.hidden_channels,
                                           1,
                                           stride,
                                           padding='stride_effective',
                                           bias=norm_layer is None,
                                           norm_layer=norm_layer,
                                           activation_layer=activation_layer)
 
         self.channel_shuffle = nn.ChannelShuffle(grouping) if channel_shuffle else None
 
-        self.conv2 = ConvNormActivation2d(hidden_channels,
-                                          hidden_channels,
+        self.conv2 = ConvNormActivation2d(self.hidden_channels,
+                                          self.hidden_channels,
                                           kernel_size,
                                           padding='stride_effective',
-                                          groups=hidden_channels, # Depth wise convolution
+                                          groups=self.hidden_channels, # Depth wise convolution
                                           bias=norm_layer is None,
                                           norm_layer=norm_layer,
                                           activation_layer=activation_layer) # TODO@ShivamPR21: #8 Padding `same` applied though proxy (`stride_effective, stride=1`) for onnx support
 
-        self.conv3 = ConvNormActivation2d(hidden_channels,
-                                          in_channels,
+        self.conv3 = ConvNormActivation2d(self.hidden_channels,
+                                          self.out_channels,
                                           1,
                                           stride=1,
                                           padding='stride_effective',
                                           bias=norm_layer is None,
                                           norm_layer=norm_layer,
                                           activation_layer=None) # TODO@ShivamPR21: #8 Padding `same` applied though proxy (`stride_effective, stride=1`) for onnx support
 
@@ -90,48 +92,50 @@
 
 
 class ConvInvertedBlock1d(nn.Module):
 
     def __init__(self,
                  in_channels: int,
                  expansion_ratio: float,
+                 out_channels: Optional[float] = None,
                  kernel_size: Union[int, Tuple[int, int]] = 3,
                  stride: Union[int, Tuple[int, int]] = 1,
                  norm_layer: Optional[Callable[..., nn.Module]] = None,
                  activation_layer: Optional[Callable[..., nn.Module]] = nn.ReLU6,
                  channel_shuffle: bool = False,
                  grouping: int = 1) -> None:
         super().__init__()
 
-        hidden_channels = round(in_channels * expansion_ratio)
+        self.hidden_channels = round(in_channels * expansion_ratio)
+        self.out_channels = in_channels if out_channels is None else out_channels
 
         self.activation = activation_layer() if activation_layer is not None else None
 
         self.conv1 = ConvNormActivation1d(in_channels,
-                                          hidden_channels,
+                                          self.hidden_channels,
                                           1,
                                           stride,
                                           padding='stride_effective',
                                           bias=norm_layer is None,
                                           norm_layer=norm_layer,
                                           activation_layer=activation_layer)
 
         self.channel_shuffle = nn.ChannelShuffle(grouping) if channel_shuffle else None
 
-        self.conv2 = ConvNormActivation1d(hidden_channels,
-                                          hidden_channels,
+        self.conv2 = ConvNormActivation1d(self.hidden_channels,
+                                          self.hidden_channels,
                                           kernel_size,
                                           padding='stride_effective',
-                                          groups=hidden_channels, # Depth wise convolution
+                                          groups=self.hidden_channels, # Depth wise convolution
                                           bias=norm_layer is None,
                                           norm_layer=norm_layer,
                                           activation_layer=activation_layer) # TODO@ShivamPR21: #8 Padding `same` applied though proxy (`stride_effective, stride=1`) for onnx support
 
-        self.conv3 = ConvNormActivation1d(hidden_channels,
-                                          in_channels,
+        self.conv3 = ConvNormActivation1d(self.hidden_channels,
+                                          self.out_channels,
                                           1,
                                           stride=1,
                                           padding='stride_effective',
                                           bias=norm_layer is None,
                                           norm_layer=norm_layer,
                                           activation_layer=None) # TODO@ShivamPR21: #8 Padding `same` applied though proxy (`stride_effective, stride=1`) for onnx support
```

### Comparing `mzt-1.1.4a0/moduleZoo/dense/denseblocks.py` & `mzt-1.1.5/moduleZoo/dense/denseblocks.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/graphs/grah_conv.py` & `mzt-1.1.5/moduleZoo/graphs/grah_conv.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/graphs/utils.py` & `mzt-1.1.5/moduleZoo/graphs/utils.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/resblocks/__init__.py` & `mzt-1.1.5/moduleZoo/resblocks/__init__.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/resblocks/bottleneckresidual.py` & `mzt-1.1.5/moduleZoo/resblocks/bottleneckresidual.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/moduleZoo/resblocks/invertedresidual.py` & `mzt-1.1.5/moduleZoo/resblocks/invertedresidual.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 '''
 
 from typing import Callable, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
-from ..convolution import (
-    ConvInvertedBlock1d,
-    ConvInvertedBlock2d,
-    ConvNormActivation1d,
-    ConvNormActivation2d,
-)
+from ..convolution import (ConvInvertedBlock1d, ConvInvertedBlock2d,
+                           ConvNormActivation1d, ConvNormActivation2d)
 
 
 class ConvInvertedResidualBlock2d(ConvInvertedBlock2d):
 
     def __init__(self,
                  in_channels: int,
                  expansion_ratio: float,
+                 out_channels: Optional[float] = None,
                  kernel_size: Union[int, Tuple[int, int]] = 3,
                  stride: Union[int, Tuple[int, int]] = 1,
                  norm_layer: Optional[Callable[..., nn.Module]] = None,
                  activation_layer: Optional[Callable[..., nn.Module]] = nn.ReLU6,
                  channel_shuffle: bool = False,
                  grouping: int = 1) -> None:
         super().__init__(in_channels,
                          expansion_ratio,
+                         out_channels,
                          kernel_size,
                          stride,
                          norm_layer,
                          activation_layer,
                          channel_shuffle,
                          grouping)
```

### Comparing `mzt-1.1.4a0/moduleZoo/resblocks/residual.py` & `mzt-1.1.5/moduleZoo/resblocks/residual.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/mzExtras/LARC.py` & `mzt-1.1.5/mzExtras/LARC.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/mzLosses/contrastive.py` & `mzt-1.1.5/mzLosses/contrastive.py`

 * *Files identical despite different names*

### Comparing `mzt-1.1.4a0/setup.py` & `mzt-1.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "mzt",
-    version = "1.1.4-alpha",
+    version = "1.1.5",
     author = "Shivam Pandey",
     author_email = "pandeyshivam2017robotics@gmail.com",
     description = ("Package to host DeepLearning modules for pytorch ecosystem,"
                    " to ease out model implementations."),
     license = "AGPLv3+",
     keywords = "DeepLearning Pytorch Modules",
     url = "https://github.com/ShivamPR21/ModuleZooTorch.git",
     packages=['moduleZoo',
               'moduleZoo.convolution',
               'moduleZoo.resblocks',
               'moduleZoo.attention',
               'moduleZoo.dense',
               'moduleZoo.graphs',
               'modelZoo',
+              'modelZoo.graphs',
               'mzLosses',
               'mzExtras'],
     long_description=read('README.md'),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
```

