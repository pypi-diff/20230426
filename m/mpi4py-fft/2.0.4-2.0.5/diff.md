# Comparing `tmp/mpi4py-fft-2.0.4.tar.gz` & `tmp/mpi4py-fft-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpi4py-fft-2.0.4.tar", last modified: Thu Apr 29 14:25:20 2021, max compression
+gzip compressed data, was "mpi4py-fft-2.0.5.tar", last modified: Wed Apr 26 08:43:50 2023, max compression
```

## Comparing `mpi4py-fft-2.0.4.tar` & `mpi4py-fft-2.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2021-04-29 14:25:20.915041 mpi4py-fft-2.0.4/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1439 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/LICENSE.rst
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      160 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/MANIFEST.in
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4754 2021-04-29 14:25:20.914771 mpi4py-fft-2.0.4/PKG-INFO
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3245 2021-04-29 14:14:31.000000 mpi4py-fft-2.0.4/README.rst
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2021-04-29 14:25:20.908068 mpi4py-fft-2.0.4/mpi4py_fft/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      976 2021-04-29 14:12:35.000000 mpi4py-fft-2.0.4/mpi4py_fft/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    17868 2021-03-25 15:20:19.000000 mpi4py-fft-2.0.4/mpi4py_fft/distarray.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2021-04-29 14:25:20.912733 mpi4py-fft-2.0.4/mpi4py_fft/fftw/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      147 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5262 2020-02-27 07:33:08.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/factory.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2467 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_planxfftn.c
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      530 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_planxfftn.h
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1550 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_xfftn.pxd
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11115 2021-03-25 16:57:58.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_xfftn.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2458 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/utilities.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    27897 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/fftw/xfftn.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2021-04-29 14:25:20.914353 mpi4py-fft-2.0.4/mpi4py_fft/io/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      114 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/io/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4705 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/io/file_base.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11668 2020-03-08 10:51:50.000000 mpi4py-fft-2.0.4/mpi4py_fft/io/generate_xdmf.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5889 2020-06-25 09:14:17.000000 mpi4py-fft-2.0.4/mpi4py_fft/io/h5py_file.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7675 2021-03-25 15:19:51.000000 mpi4py-fft-2.0.4/mpi4py_fft/io/nc_file.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    15717 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/mpi4py_fft/libfft.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    15684 2021-03-25 15:20:05.000000 mpi4py-fft-2.0.4/mpi4py_fft/mpifft.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11808 2021-03-25 15:19:35.000000 mpi4py-fft-2.0.4/mpi4py_fft/pencil.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2021-04-29 14:25:20.909223 mpi4py-fft-2.0.4/mpi4py_fft.egg-info/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4754 2021-04-29 14:25:20.000000 mpi4py-fft-2.0.4/mpi4py_fft.egg-info/PKG-INFO
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1254 2021-04-29 14:25:20.000000 mpi4py-fft-2.0.4/mpi4py_fft.egg-info/SOURCES.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)        1 2021-04-29 14:25:20.000000 mpi4py-fft-2.0.4/mpi4py_fft.egg-info/dependency_links.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       13 2021-04-29 14:25:20.000000 mpi4py-fft-2.0.4/mpi4py_fft.egg-info/requires.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       11 2021-04-29 14:25:20.000000 mpi4py-fft-2.0.4/mpi4py_fft.egg-info/top_level.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       20 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/requirements.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       38 2021-04-29 14:25:20.915121 mpi4py-fft-2.0.4/setup.cfg
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7375 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.4/setup.py
+drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.846779 mpi4py-fft-2.0.5/
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1439 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/LICENSE.rst
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)      160 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/MANIFEST.in
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3810 2023-04-26 08:43:50.846459 mpi4py-fft-2.0.5/PKG-INFO
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2980 2023-04-26 08:39:58.000000 mpi4py-fft-2.0.5/README.rst
+drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.835841 mpi4py-fft-2.0.5/mpi4py_fft/
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1001 2023-04-26 08:42:41.000000 mpi4py-fft-2.0.5/mpi4py_fft/__init__.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    17899 2022-06-10 04:50:35.000000 mpi4py-fft-2.0.5/mpi4py_fft/distarray.py
+drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.842475 mpi4py-fft-2.0.5/mpi4py_fft/fftw/
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)      155 2022-11-02 13:12:48.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/__init__.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5262 2022-11-02 13:56:49.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/factory.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2467 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.c
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)      530 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.h
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1550 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pxd
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11115 2021-03-25 16:57:58.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pyx
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2458 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/utilities.pyx
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    27897 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/xfftn.py
+drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.845694 mpi4py-fft-2.0.5/mpi4py_fft/io/
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)      114 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/__init__.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4705 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/file_base.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11792 2023-04-26 07:18:14.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/generate_xdmf.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5889 2022-05-31 13:12:18.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/h5py_file.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7675 2021-03-25 15:19:51.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/nc_file.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    15717 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/libfft.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    15692 2023-04-14 11:12:30.000000 mpi4py-fft-2.0.5/mpi4py_fft/mpifft.py
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11808 2023-04-14 11:15:06.000000 mpi4py-fft-2.0.5/mpi4py_fft/pencil.py
+drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.837671 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3810 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/PKG-INFO
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1254 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/SOURCES.txt
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)        1 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/dependency_links.txt
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)       13 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/requires.txt
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)       11 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/top_level.txt
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)       20 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/requirements.txt
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)       38 2023-04-26 08:43:50.846875 mpi4py-fft-2.0.5/setup.cfg
+-rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7375 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/setup.py
```

### Comparing `mpi4py-fft-2.0.4/LICENSE.rst` & `mpi4py-fft-2.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/README.rst` & `mpi4py-fft-2.0.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 mpi4py-fft
 ----------
 
 
 .. image:: https://dev.azure.com/mpi4py/mpi4py-fft/_apis/build/status/mpi4py.mpi4py-fft?branchName=master
     :target: https://dev.azure.com/mpi4py/mpi4py-fft
 
-.. image:: https://api.codacy.com/project/badge/Grade/7e236bbdc44e4a68b8f6dfc3d3170cf0    
-    :target: https://www.codacy.com/app/mpi4py/mpi4py-fft?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mpi4py/mpi4py-fft&amp;utm_campaign=Badge_Grade
-
 .. image:: https://codecov.io/bb/mpi4py/mpi4py-fft/branch/master/graph/badge.svg
   :target: https://codecov.io/bb/mpi4py/mpi4py-fft
 
 .. image:: https://readthedocs.org/projects/mpi4py-fft/badge/?version=latest
    :target: https://mpi4py-fft.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
@@ -38,17 +35,17 @@
 Installation
 ------------
 
 The mpi4py-fft package can be installed using::
 
     pip install mpi4py-fft
 
-or, to get the latest version from bitbucket::
+or, to get the latest version from GitHub::
 
-    pip install git+https://bitbucket.org/mpi4py/mpi4py-fft@master
+    pip install git+https://github.com/mpi4py/mpi4py-fft@master
 
 Install with conda from the coda-forge channel::
 
     conda install -c conda-forge mpi4py-fft
 
 or build it with conda build from the main source directory::
```

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/__init__.py` & `mpi4py-fft-2.0.5/mpi4py_fft/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 is supported. Furthermore, **mpi4py-fft** can also be used simply to perform
 global redistributions (distribute and communicate) of large arrays with MPI,
 without any transforms at all.
 
 For more information, see `documentation <https://mpi4py-fft.readthedocs.io>`_.
 
 """
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 __author__ = 'Lisandro Dalcin and Mikael Mortensen'
 
 from .distarray import DistArray, newDistArray, Function
 from .mpifft import PFFT
 from . import fftw
+from .fftw import fftlib
 from .io import HDF5File, NCFile, generate_xdmf
```

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/distarray.py` & `mpi4py-fft-2.0.5/mpi4py_fft/distarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
     Also note that the ``alignment`` keyword does not take rank into
     consideration. Setting alignment=2 for the array above means that the last
     axis will be aligned, also when rank>0.
 
     """
     def __new__(cls, global_shape, subcomm=None, val=None, dtype=float,
-                buffer=None, alignment=None, rank=0):
+                buffer=None, strides=None, alignment=None, rank=0):
         if len(global_shape[rank:]) < 2: # 1D case
-            obj = np.ndarray.__new__(cls, global_shape, dtype=dtype, buffer=buffer)
+            obj = np.ndarray.__new__(cls, global_shape, dtype=dtype, buffer=buffer, strides=strides)
             if buffer is None and isinstance(val, Number):
                 obj.fill(val)
             obj._rank = rank
             obj._p0 = None
             return obj
 
         if isinstance(subcomm, Subcomm):
```

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/factory.py` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/factory.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_planxfftn.c` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.c`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_planxfftn.h` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.h`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_xfftn.pxd` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pxd`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/fftw_xfftn.pyx` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pyx`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/utilities.pyx` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/utilities.pyx`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/fftw/xfftn.py` & `mpi4py-fft-2.0.5/mpi4py_fft/fftw/xfftn.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/io/file_base.py` & `mpi4py-fft-2.0.5/mpi4py_fft/io/file_base.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/io/generate_xdmf.py` & `mpi4py-fft-2.0.5/mpi4py_fft/io/generate_xdmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,24 @@
             {0} {1}
           </DataItem>
           <DataItem Format="XML" NumberType="Float" Dimensions="2">
             {2} {3}
           </DataItem>
         </Geometry>"""
 
-        return """<Geometry Type="VXVY">
+        return """<Geometry Type="VXVYVZ">
           <DataItem Format="HDF" NumberType="Float" Precision="{0}" Dimensions="{1}">
             {3}:{6}/mesh/{4}
           </DataItem>
           <DataItem Format="HDF" NumberType="Float" Precision="{0}" Dimensions="{2}">
             {3}:{6}/mesh/{5}
           </DataItem>
+          <DataItem Format="XML" NumberType="Float" Precision="8" Dimensions="1">
+            0
+          </DataItem>
         </Geometry>"""
 
     if dim == 3:
         if kind == 0:
             return """<Geometry Type="ORIGIN_DXDYDZ">
           <DataItem Format="XML" NumberType="Float" Dimensions="3">
             {0} {1} {2}
@@ -70,24 +73,24 @@
           </DataItem>
         </Geometry>"""
 
 def get_topology(dims, kind=0):
     assert len(dims) in (2, 3)
     co = 'Co' if kind == 0 else ''
     if len(dims) == 2:
-        return """<Topology Dimensions="{0} {1}" Type="2D{2}RectMesh"/>""".format(dims[0], dims[1], co)
+        return """<Topology Dimensions="1 {0} {1}" Type="3D{2}RectMesh"/>""".format(dims[0], dims[1], co)
     if len(dims) == 3:
         return """<Topology Dimensions="{0} {1} {2}" Type="3D{3}RectMesh"/>""".format(dims[0], dims[1], dims[2], co)
 
 def get_attribute(attr, h5filename, dims, prec):
     name = attr.split("/")[0]
     assert len(dims) in (2, 3)
     if len(dims) == 2:
         return """<Attribute Name="{0}" Center="Node">
-          <DataItem Format="HDF" NumberType="Float" Precision="{5}" Dimensions="{1} {2}">
+          <DataItem Format="HDF" NumberType="Float" Precision="{5}" Dimensions="1 {1} {2}">
             {3}:/{4}
           </DataItem>
         </Attribute>
         """.format(name, dims[0], dims[1], h5filename, attr, prec)
 
     return """<Attribute Name="{0}" Center="Node">
           <DataItem Format="HDF" NumberType="Float" Precision="{6}" Dimensions="{1} {2} {3}">
```

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/io/h5py_file.py` & `mpi4py-fft-2.0.5/mpi4py_fft/io/h5py_file.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/io/nc_file.py` & `mpi4py-fft-2.0.5/mpi4py_fft/io/nc_file.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/libfft.py` & `mpi4py-fft-2.0.5/mpi4py_fft/libfft.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/mpifft.py` & `mpi4py-fft-2.0.5/mpi4py_fft/mpifft.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         # pylint: disable=too-many-statements
 
         if shape is None:
             assert darray is not None
             shape = darray.pencil.shape
 
         if axes is not None:
-            axes = list(axes) if np.ndim(axes) else [axes]
+            axes = list(axes) if not isinstance(axes, int) else [axes]
         else:
             axes = list(range(len(shape)))
             if darray is not None:
                 # Make sure aligned axis of darray is transformed first
                 axes = list(np.roll(axes, len(shape)-1-darray.alignment))
 
         for i, ax in enumerate(axes):
@@ -359,15 +359,15 @@
         ----------
         forward_output : bool, optional
             Return shape of output array (spectral space) if True, else return
             shape of input array (physical space)
         """
         if forward_output is not True:
             return self.forward.input_pencil.subshape
-        return self.backward.input_pencil.subshape
+        return self.forward.output_array.shape
 
     def local_slice(self, forward_output=True):
         """The local view into the global data
 
         Parameters
         ----------
         forward_output : bool, optional
```

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft/pencil.py` & `mpi4py-fft-2.0.5/mpi4py_fft/pencil.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/mpi4py_fft.egg-info/SOURCES.txt` & `mpi4py-fft-2.0.5/mpi4py_fft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.4/setup.py` & `mpi4py-fft-2.0.5/setup.py`

 * *Files identical despite different names*

