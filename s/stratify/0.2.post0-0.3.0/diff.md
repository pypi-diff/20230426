# Comparing `tmp/stratify-0.2.post0.tar.gz` & `tmp/stratify-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stratify-0.2.post0.tar", last modified: Thu May 20 01:05:29 2021, max compression
+gzip compressed data, was "stratify-0.3.0.tar", last modified: Tue Apr 25 15:22:55 2023, max compression
```

## Comparing `stratify-0.2.post0.tar` & `stratify-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,29 @@
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2021-05-20 01:05:29.203169 stratify-0.2.post0/
--rw-r--r--   0 bill      (1000) bill      (1000)     3231 2021-05-19 23:23:12.000000 stratify-0.2.post0/.cirrus.yml
--rw-r--r--   0 bill      (1000) bill      (1000)      741 2021-05-19 23:23:12.000000 stratify-0.2.post0/.flake8
--rw-r--r--   0 bill      (1000) bill      (1000)     1849 2021-05-19 23:23:12.000000 stratify-0.2.post0/.gitignore
--rw-r--r--   0 bill      (1000) bill      (1000)     1375 2021-05-19 23:23:12.000000 stratify-0.2.post0/.pre-commit-config.yaml
--rw-rw-r--   0 bill      (1000) bill      (1000)     4124 2019-06-06 20:28:17.000000 stratify-0.2.post0/CONTRIBUTING.md
--rw-rw-r--   0 bill      (1000) bill      (1000)      185 2019-06-06 20:30:21.000000 stratify-0.2.post0/Dockerfile
--rw-rw-r--   0 bill      (1000) bill      (1000)     1513 2019-06-06 20:30:21.000000 stratify-0.2.post0/LICENSE
--rw-r--r--   0 bill      (1000) bill      (1000)       57 2021-03-22 23:13:50.000000 stratify-0.2.post0/MANIFEST.in
--rw-r--r--   0 bill      (1000) bill      (1000)     3432 2021-05-20 01:05:29.203169 stratify-0.2.post0/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)     2026 2021-05-20 00:44:10.000000 stratify-0.2.post0/README.md
--rw-rw-r--   0 bill      (1000) bill      (1000)   175983 2019-06-06 20:30:21.000000 stratify-0.2.post0/index.ipynb
--rw-r--r--   0 bill      (1000) bill      (1000)      566 2021-05-19 23:23:12.000000 stratify-0.2.post0/pyproject.toml
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2021-05-20 01:05:29.199169 stratify-0.2.post0/requirements/
--rw-r--r--   0 bill      (1000) bill      (1000)      336 2021-05-19 23:36:38.000000 stratify-0.2.post0/requirements/py38.yml
--rw-r--r--   0 bill      (1000) bill      (1000)      336 2021-05-19 23:23:12.000000 stratify-0.2.post0/requirements/py39.yml
--rw-r--r--   0 bill      (1000) bill      (1000)      336 2021-05-19 23:23:12.000000 stratify-0.2.post0/requirements/stratify.yml
--rw-r--r--   0 bill      (1000) bill      (1000)     1388 2021-05-20 01:05:29.203169 stratify-0.2.post0/setup.cfg
--rw-r--r--   0 bill      (1000) bill      (1000)     1805 2021-05-19 23:23:12.000000 stratify-0.2.post0/setup.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2021-05-20 01:05:29.199169 stratify-0.2.post0/stratify/
--rw-r--r--   0 bill      (1000) bill      (1000)      172 2021-05-19 23:23:12.000000 stratify-0.2.post0/stratify/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)     5516 2021-05-19 23:23:12.000000 stratify-0.2.post0/stratify/_bounded_vinterp.py
--rw-rw-r--   0 bill      (1000) bill      (1000)     4943 2019-06-06 20:30:21.000000 stratify-0.2.post0/stratify/_conservative.pyx
--rw-r--r--   0 bill      (1000) bill      (1000)      152 2021-05-20 01:05:28.000000 stratify-0.2.post0/stratify/_version.py
--rw-r--r--   0 bill      (1000) bill      (1000)    29987 2021-05-19 23:23:12.000000 stratify-0.2.post0/stratify/_vinterp.pyx
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2021-05-20 01:05:29.203169 stratify-0.2.post0/stratify/tests/
--rw-rw-r--   0 bill      (1000) bill      (1000)        0 2019-06-06 20:28:17.000000 stratify-0.2.post0/stratify/tests/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)      672 2021-05-19 23:23:12.000000 stratify-0.2.post0/stratify/tests/performance.py
--rw-r--r--   0 bill      (1000) bill      (1000)     9396 2021-05-19 23:23:12.000000 stratify-0.2.post0/stratify/tests/test_bounded_vinterp.py
--rw-r--r--   0 bill      (1000) bill      (1000)    19158 2021-05-19 23:23:12.000000 stratify-0.2.post0/stratify/tests/test_vinterp.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2021-05-20 01:05:29.203169 stratify-0.2.post0/stratify.egg-info/
--rw-r--r--   0 bill      (1000) bill      (1000)     3432 2021-05-20 01:05:28.000000 stratify-0.2.post0/stratify.egg-info/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)      805 2021-05-20 01:05:29.000000 stratify-0.2.post0/stratify.egg-info/SOURCES.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        1 2021-05-20 01:05:28.000000 stratify-0.2.post0/stratify.egg-info/dependency_links.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        1 2021-05-20 01:05:28.000000 stratify-0.2.post0/stratify.egg-info/not-zip-safe
--rw-r--r--   0 bill      (1000) bill      (1000)      116 2021-05-20 01:05:28.000000 stratify-0.2.post0/stratify.egg-info/requires.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        9 2021-05-20 01:05:28.000000 stratify-0.2.post0/stratify.egg-info/top_level.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)    31350 2019-06-06 20:28:17.000000 stratify-0.2.post0/summary.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:55.580018 stratify-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-25 15:22:38.000000 stratify-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-25 15:22:38.000000 stratify-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-04-25 15:22:55.580018 stratify-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-25 15:22:38.000000 stratify-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 15:22:38.000000 stratify-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:55.576017 stratify-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 15:22:38.000000 stratify-0.3.0/requirements/pypi-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:22:55.580018 stratify-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 15:22:38.000000 stratify-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:55.572018 stratify-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:55.576017 stratify-0.3.0/src/stratify/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/_bounded_vinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/_conservative.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 15:22:55.000000 stratify-0.3.0/src/stratify/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/_vinterp.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:55.576017 stratify-0.3.0/src/stratify/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/tests/test_bounded_vinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-25 15:22:38.000000 stratify-0.3.0/src/stratify/tests/test_vinterp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:22:55.576017 stratify-0.3.0/src/stratify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-04-25 15:22:55.000000 stratify-0.3.0/src/stratify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-25 15:22:55.000000 stratify-0.3.0/src/stratify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:22:55.000000 stratify-0.3.0/src/stratify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:22:54.000000 stratify-0.3.0/src/stratify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 15:22:55.000000 stratify-0.3.0/src/stratify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 15:22:55.000000 stratify-0.3.0/src/stratify.egg-info/top_level.txt
```

### Comparing `stratify-0.2.post0/LICENSE` & `stratify-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stratify-0.2.post0/setup.py` & `stratify-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,80 @@
-import builtins
 import os
 import sys
+import warnings
 from pathlib import Path
 
-from setuptools import Extension, setup
-from setuptools.command.build_ext import build_ext
+# safe to import numpy here thanks to pep518
+import numpy as np
+from setuptools import Command, Extension, setup
 
 try:
     from Cython.Build import cythonize  # isort:skip
 except ImportError:
-    wmsg = "WARNING: Cython unavailable, unable to build stratify extensions"
-    print(wmsg)
+    wmsg = "Cython unavailable, unable to build stratify extensions!"
+    warnings.warn(wmsg)
     cythonize = None
 
 
+BASE_DIR = Path(__file__).resolve().parent
 PACKAGE_NAME = "stratify"
+SRC_DIR = BASE_DIR / "src"
+STRATIFY_DIR = SRC_DIR / PACKAGE_NAME
 CMDS_NOCYTHONIZE = ["clean", "sdist"]
+FLAG_COVERAGE = "--cython-coverage"  # custom flag enabling Cython line tracing
 
 
-class NumpyBuildExt(build_ext):
-    # Delay numpy import so that setup.py can be run
-    # without numpy already being installed.
+class CleanCython(Command):
+    description = "Purge artifacts built by Cython"
+    user_options = []
+
+    def initialize_options(self):
+        pass
+
     def finalize_options(self):
-        build_ext.finalize_options(self)
-        builtins.__NUMPY_SETUP__ = False
-        import numpy
+        pass
 
-        self.include_dirs.append(numpy.get_include())
+    def run(self):
+        for path in STRATIFY_DIR.rglob("*"):
+            if path.suffix in (".pyc", ".pyo", ".c", ".so"):
+                msg = f"clean: removing file {path}"
+                print(msg)
+                path.unlink()
 
 
-cython_coverage_enabled = os.environ.get("CYTHON_COVERAGE", None)
+cython_coverage_enabled = (
+    os.environ.get("CYTHON_COVERAGE", None) or FLAG_COVERAGE in sys.argv
+)
 cython_directives = {}
-# TODO: investigate "'PyArrayObject' has no member named 'dimensions'" cython error
-#       https://cython.readthedocs.io/en/latest/src/userguide/source_files_and_compilation.html#configuring-the-c-build
-# define_macros = [("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")]
 define_macros = []
 extensions = []
 
 if cythonize and cython_coverage_enabled:
-    define_macros.append(("CYTHON_TRACE_NOGIL", "1"))
+    define_macros.extend(
+        [
+            ("CYTHON_TRACE", "1"),
+            ("CYTHON_TRACE_NOGIL", "1"),
+        ]
+    )
     cython_directives.update({"linetrace": True})
-
-for fname in Path.cwd().glob(f"{PACKAGE_NAME}/*.pyx"):
-    extensions.append(
-        Extension(
-            f"{PACKAGE_NAME}.{fname.stem}",
-            sources=[str(fname)],
-            define_macros=define_macros,
-        )
+    if FLAG_COVERAGE in sys.argv:
+        sys.argv.remove(FLAG_COVERAGE)
+    print('enabled "linetrace" Cython compiler directive')
+
+for fname in SRC_DIR.glob(f"{PACKAGE_NAME}/*.pyx"):
+    # ref: https://setuptools.pypa.io/en/latest/userguide/ext_modules.html
+    extension = Extension(
+        f"{PACKAGE_NAME}.{fname.stem}",
+        sources=[str(fname.relative_to(BASE_DIR))],
+        include_dirs=[np.get_include()],
+        define_macros=define_macros,
     )
+    extensions.append(extension)
 
 if cythonize and not any([arg in CMDS_NOCYTHONIZE for arg in sys.argv]):
     extensions = cythonize(
         extensions, compiler_directives=cython_directives, language_level=3
     )
 
-kwargs = dict(
-    cmdclass={"build_ext": NumpyBuildExt},
-    ext_modules=extensions,
-)
-
+cmdclass = {"clean_cython": CleanCython}
+kwargs = {"cmdclass": cmdclass, "ext_modules": extensions}
 setup(**kwargs)
```

### Comparing `stratify-0.2.post0/stratify/_bounded_vinterp.py` & `stratify-0.3.0/src/stratify/_bounded_vinterp.py`

 * *Files identical despite different names*

### Comparing `stratify-0.2.post0/stratify/_conservative.pyx` & `stratify-0.3.0/src/stratify/_conservative.pyx`

 * *Files identical despite different names*

### Comparing `stratify-0.2.post0/stratify/_vinterp.pyx` & `stratify-0.3.0/src/stratify/_vinterp.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Terminology:
 # Z - the coordinate over which we are interpolating.
 # z_src - the values of Z where fz_src is defined
 # z_target - the desired values of Z to generate new data for.
 # fz_src - the data, defined at each z_src
+import functools
+
 import numpy as np
 
 cimport cython
 cimport numpy as np
 
 
 cdef extern from "numpy/npy_math.h" nogil:
@@ -498,14 +500,74 @@
         iterpolation modes. Linear interpolation is the default.
     extrapolation: :class:`.Extrapolator` instance or valid scheme name
         The core extrapolation operation to use. :attr:`.EXTRAPOLATE_NAN` and
         :attr:`.EXTRAPOLATE_NEAREST` are provided for convenient extrapolation
         modes. NaN extrapolation is the default.
 
     """
+    func = functools.partial(
+        _interpolate,
+        axis=axis,
+        rising=rising,
+        interpolation=interpolation,
+        extrapolation=extrapolation
+    )
+    if not hasattr(fz_src, 'compute'):
+        # Numpy array
+        return func(z_target, z_src, fz_src)
+
+    # Dask array
+    import dask.array as da
+
+    # Ensure z_target is an array.
+    if not isinstance(z_target, (np.ndarray, da.Array)):
+      z_target = np.array(z_target)
+
+    # Compute chunk sizes
+    if axis < 0:
+      axis += fz_src.ndim
+    in_chunks = list(fz_src.chunks)
+    in_chunks[axis] = fz_src.shape[axis]
+
+    out_chunks = list(in_chunks)
+    if z_target.ndim == 1:
+        out_chunks[axis] = z_target.shape[0]
+    else:
+        out_chunks[axis] = z_target.shape[axis]
+
+    # Ensure `fz_src` is not chunked along `axis`.
+    fz_src = fz_src.rechunk(in_chunks)
+
+    # Ensure z_src is a dask array with the correct chunks.
+    if isinstance(z_src, da.Array):
+        z_src = z_src.rechunk(in_chunks)
+    else:
+        z_src = da.asarray(z_src, chunks=in_chunks)
+
+    # Compute with 1-dimensional target array.
+    if z_target.ndim == 1:
+        func = functools.partial(func, z_target)
+        return da.map_blocks(func, z_src, fz_src,
+                             chunks=out_chunks, dtype=fz_src.dtype,
+                             meta=np.array((), dtype=fz_src.dtype))
+
+    # Ensure z_target is a dask array with the correct chunks
+    if isinstance(z_target, da.Array):
+       z_target = z_target.rechunk(out_chunks)
+    else:
+       z_target = da.asarray(z_target, chunks=out_chunks)
+
+    # Compute with multi-dimensional target array.
+    return da.map_blocks(func, z_target, z_src, fz_src,
+                         chunks=out_chunks, dtype=fz_src.dtype,
+                         meta=np.array((), dtype=fz_src.dtype))
+
+
+def _interpolate(z_target, z_src, fz_src, axis=-1, rising=None,
+                 interpolation='linear', extrapolation='nan'):
     if interpolation in interp_schemes:
         interpolation = interp_schemes[interpolation]()
     if extrapolation in extrap_schemes:
         extrapolation = extrap_schemes[extrapolation]()
 
     interp = _Interpolation(z_target, z_src, fz_src, rising=rising, axis=axis,
                             interpolation=interpolation,
```

### Comparing `stratify-0.2.post0/stratify/tests/test_bounded_vinterp.py` & `stratify-0.3.0/src/stratify/tests/test_bounded_vinterp.py`

 * *Files identical despite different names*

### Comparing `stratify-0.2.post0/stratify/tests/test_vinterp.py` & `stratify-0.3.0/src/stratify/tests/test_vinterp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 
+import dask.array as da
 import numpy as np
 from numpy.testing import assert_array_almost_equal, assert_array_equal
 
 import stratify
 import stratify._vinterp as vinterp
 
 
@@ -42,14 +43,25 @@
                 fx_src,
                 rising=not rising,
                 interpolation=index_interp,
                 extrapolation=extrap_direct,
             )
             assert_array_equal(r1, r2)
 
+        lazy_fx_src = da.asarray(fx_src, chunks=tuple(range(1, x_src.ndim + 1)))
+        r3 = stratify.interpolate(
+            x_target,
+            x_src,
+            lazy_fx_src,
+            rising=rising,
+            interpolation=index_interp,
+            extrapolation=extrap_direct,
+        )
+        assert_array_equal(r1, r3.compute())
+
         return r1
 
     def test_interp_only(self):
         r = self.interpolate([1, 2, 3], [1, 3])
         assert_array_equal(r, [0, 1, 1])
 
     def test_interp_multi_level_single_source(self):
@@ -529,10 +541,39 @@
     def test_target_z_3d_axis_0(self):
         z_target = z_source = f_source = np.arange(3) * np.ones([4, 2, 3])
         result = vinterp.interpolate(
             z_target, z_source, f_source, extrapolation="linear"
         )
         assert_array_equal(result, f_source)
 
+    def test_dask(self):
+        z_target = z_source = f_source = np.arange(3) * np.ones([4, 2, 3])
+        reference = vinterp.interpolate(
+            z_target, z_source, f_source, extrapolation="linear"
+        )
+        # Test with various combinations of lazy input
+        f_src = da.asarray(f_source, chunks=(2, 1, 2))
+        for z_tgt in (z_target, z_target.tolist(), da.asarray(z_target)):
+            for z_src in (z_source, da.asarray(z_source)):
+                result = vinterp.interpolate(
+                    z_tgt, z_src, f_src, extrapolation="linear"
+                )
+                assert_array_equal(reference, result.compute())
+
+    def test_dask_1d_target(self):
+        z_target = np.array([0.5])
+        z_source = f_source = np.arange(3) * np.ones([4, 2, 3])
+        reference = vinterp.interpolate(
+            z_target, z_source, f_source, axis=1, extrapolation="linear"
+        )
+        # Test with various combinations of lazy input
+        f_src = da.asarray(f_source, chunks=(2, 1, 2))
+        for z_tgt in (z_target, z_target.tolist(), da.asarray(z_target)):
+            for z_src in (z_source, da.asarray(z_source)):
+                result = vinterp.interpolate(
+                    z_tgt, z_src, f_src, axis=1, extrapolation="linear"
+                )
+                assert_array_equal(reference, result.compute())
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `stratify-0.2.post0/stratify.egg-info/SOURCES.txt` & `stratify-0.3.0/src/stratify.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-.cirrus.yml
-.flake8
-.gitignore
-.pre-commit-config.yaml
-CONTRIBUTING.md
-Dockerfile
 LICENSE
 MANIFEST.in
 README.md
-index.ipynb
 pyproject.toml
-setup.cfg
 setup.py
-summary.png
-/home/bill/projects/git/python-stratify/stratify/_conservative.pyx
-/home/bill/projects/git/python-stratify/stratify/_vinterp.pyx
-requirements/py38.yml
-requirements/py39.yml
-requirements/stratify.yml
-stratify/__init__.py
-stratify/_bounded_vinterp.py
-stratify/_conservative.pyx
-stratify/_version.py
-stratify/_vinterp.pyx
-stratify.egg-info/PKG-INFO
-stratify.egg-info/SOURCES.txt
-stratify.egg-info/dependency_links.txt
-stratify.egg-info/not-zip-safe
-stratify.egg-info/requires.txt
-stratify.egg-info/top_level.txt
-stratify/tests/__init__.py
-stratify/tests/performance.py
-stratify/tests/test_bounded_vinterp.py
-stratify/tests/test_vinterp.py
+requirements/pypi-core.txt
+src/stratify/__init__.py
+src/stratify/_bounded_vinterp.py
+src/stratify/_conservative.pyx
+src/stratify/_version.py
+src/stratify/_vinterp.pyx
+src/stratify.egg-info/PKG-INFO
+src/stratify.egg-info/SOURCES.txt
+src/stratify.egg-info/dependency_links.txt
+src/stratify.egg-info/not-zip-safe
+src/stratify.egg-info/requires.txt
+src/stratify.egg-info/top_level.txt
+src/stratify/tests/__init__.py
+src/stratify/tests/performance.py
+src/stratify/tests/test_bounded_vinterp.py
+src/stratify/tests/test_vinterp.py
```

