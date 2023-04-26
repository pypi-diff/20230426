# Comparing `tmp/psf-2022.9.26.tar.gz` & `tmp/psf-2023.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psf-2022.9.26.tar", last modified: Mon Sep 26 22:37:49 2022, max compression
+gzip compressed data, was "psf-2023.4.26.tar", last modified: Wed Apr 26 18:29:39 2023, max compression
```

## Comparing `psf-2022.9.26.tar` & `psf-2023.4.26.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-09-26 22:37:49.951248 psf-2022.9.26/
--rw-rw-rw-   0        0        0     1576 2022-09-26 22:37:47.000000 psf-2022.9.26/LICENSE
--rw-rw-rw-   0        0        0      130 2018-08-29 19:01:21.000000 psf-2022.9.26/MANIFEST.in
--rw-rw-rw-   0        0        0     4542 2022-09-26 22:37:49.950247 psf-2022.9.26/PKG-INFO
--rw-rw-rw-   0        0        0     3571 2022-09-26 22:37:47.000000 psf-2022.9.26/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-26 22:37:49.941224 psf-2022.9.26/psf/
--rw-rw-rw-   0        0        0       89 2020-01-01 02:37:31.000000 psf-2022.9.26/psf/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-26 22:37:49.949224 psf-2022.9.26/psf/examples/
--rw-rw-rw-   0        0        0     4372 2022-03-17 14:08:04.000000 psf-2022.9.26/psf/examples/psf_example.py
--rw-rw-rw-   0        0        0    38432 2022-09-12 17:56:31.000000 psf-2022.9.26/psf/psf.c
--rw-rw-rw-   0        0        0    29817 2022-09-26 22:36:18.000000 psf-2022.9.26/psf/psf.py
-drwxrwxrwx   0        0        0        0 2022-09-26 22:37:49.948248 psf-2022.9.26/psf.egg-info/
--rw-rw-rw-   0        0        0     4542 2022-09-26 22:37:48.000000 psf-2022.9.26/psf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2022-09-26 22:37:49.000000 psf-2022.9.26/psf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-26 22:37:48.000000 psf-2022.9.26/psf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-26 22:37:48.000000 psf-2022.9.26/psf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2022-09-26 22:37:48.000000 psf-2022.9.26/psf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-09-26 22:37:48.000000 psf-2022.9.26/psf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-26 22:37:49.951248 psf-2022.9.26/setup.cfg
--rw-rw-rw-   0        0        0     2955 2022-09-26 22:23:18.000000 psf-2022.9.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:29:39.926288 psf-2023.4.26/
+drwxrwxrwx   0        0        0        0 2023-04-26 18:29:39.905986 psf-2023.4.26/.github/
+drwxrwxrwx   0        0        0        0 2023-04-26 18:29:39.914067 psf-2023.4.26/.github/workflows/
+-rw-rw-rw-   0        0        0      829 2023-04-26 17:53:29.000000 psf-2023.4.26/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     1576 2023-04-26 18:29:34.000000 psf-2023.4.26/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-04-25 18:31:48.000000 psf-2023.4.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     4913 2023-04-26 18:29:39.926288 psf-2023.4.26/PKG-INFO
+-rw-rw-rw-   0        0        0     3972 2023-04-26 18:29:34.000000 psf-2023.4.26/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 18:29:39.914067 psf-2023.4.26/psf/
+-rw-rw-rw-   0        0        0       89 2020-01-01 02:37:31.000000 psf-2023.4.26/psf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:29:39.926288 psf-2023.4.26/psf/examples/
+-rw-rw-rw-   0        0        0     4486 2023-04-26 17:56:58.000000 psf-2023.4.26/psf/examples/psf_example.py
+-rw-rw-rw-   0        0        0    38415 2023-04-26 17:40:40.000000 psf-2023.4.26/psf/psf.c
+-rw-rw-rw-   0        0        0    33374 2023-04-26 18:27:23.000000 psf-2023.4.26/psf/psf.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:29:39.926288 psf-2023.4.26/psf.egg-info/
+-rw-rw-rw-   0        0        0     4913 2023-04-26 18:29:38.000000 psf-2023.4.26/psf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-26 18:29:39.000000 psf-2023.4.26/psf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:29:38.000000 psf-2023.4.26/psf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 18:29:38.000000 psf-2023.4.26/psf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-04-26 18:29:38.000000 psf-2023.4.26/psf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-26 18:29:38.000000 psf-2023.4.26/psf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:29:39.926288 psf-2023.4.26/setup.cfg
+-rw-rw-rw-   0        0        0     2925 2023-04-25 18:37:51.000000 psf-2023.4.26/setup.py
```

### Comparing `psf-2022.9.26/LICENSE` & `psf-2023.4.26/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2007-2022, Christoph Gohlke and Oliver Holub
+Copyright (c) 2007-2023, Christoph Gohlke and Oliver Holub
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `psf-2022.9.26/PKG-INFO` & `psf-2023.4.26/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psf
-Version: 2022.9.26
+Version: 2023.4.26
 Summary: Point Spread Function calculations for fluorescence microscopy
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psf/issues
 Project-URL: Source Code, https://github.com/cgohlke/psf
@@ -12,48 +12,68 @@
 Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: all
 License-File: LICENSE
 
 Point Spread Function calculations for fluorescence microscopy
 ==============================================================
 
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
-This library is no longer actively developed.
-Consider using the `pyotf <https://pypi.org/project/pyotf/>`_ package instead.
+The psf library is no longer actively developed.
 
-:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_ and Oliver Holub
+:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.26
+:Version: 2023.4.26
+
+Quickstart
+----------
+
+Install the psf package and all dependencies from the
+`Python Package Index <https://pypi.org/project/psf/>`_::
+
+    python -m pip install -U psf[all]
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/psf>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.7.1
   (optional for plotting)
 
 Revisions
 ---------
 
+2023.4.26
+
+- Use enums.
+- Derive Dimensions from UserDict.
+- Add type hints.
+- Convert to Google style docstrings.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.26
 
 - Fix setup.py.
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
```

### Comparing `psf-2022.9.26/README.rst` & `psf-2023.4.26/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,54 @@
 Point Spread Function calculations for fluorescence microscopy
 ==============================================================
 
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
-This library is no longer actively developed.
-Consider using the `pyotf <https://pypi.org/project/pyotf/>`_ package instead.
+The psf library is no longer actively developed.
 
-:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_ and Oliver Holub
+:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.26
+:Version: 2023.4.26
+
+Quickstart
+----------
+
+Install the psf package and all dependencies from the
+`Python Package Index <https://pypi.org/project/psf/>`_::
+
+    python -m pip install -U psf[all]
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/psf>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.7.1
   (optional for plotting)
 
 Revisions
 ---------
 
+2023.4.26
+
+- Use enums.
+- Derive Dimensions from UserDict.
+- Add type hints.
+- Convert to Google style docstrings.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.26
 
 - Fix setup.py.
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
```

### Comparing `psf-2022.9.26/psf/examples/psf_example.py` & `psf-2023.4.26/psf/examples/psf_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,24 @@
         'refr_index': 1.333,
         'magnification': 1.0,
         'pinhole_radius': 0.05,  # in micrometers
         'pinhole_shape': 'square',
     }
     args.update(kwargs)
 
-    obsvol = psf.PSF(psf.ISOTROPIC | psf.CONFOCAL, **args)
+    obsvol = psf.PSF(psf.ISOTROPIC | psf.CONFOCAL, **args)  # type: ignore
     expsf = obsvol.expsf
     empsf = obsvol.empsf
-    gauss = gauss2 = psf.PSF(psf.GAUSSIAN | psf.EXCITATION, **args)
+
+    gauss = gauss2 = psf.PSF(
+        psf.GAUSSIAN | psf.EXCITATION, **args  # type: ignore
+    )
+
+    assert expsf is not None
+    assert empsf is not None
 
     print(expsf)
     print(empsf)
     print(obsvol)
     print(gauss)
     print(gauss2)
 
@@ -83,19 +89,19 @@
         bottom=0.02, top=0.92, left=0.02, right=0.98, hspace=0.01, wspace=0.01
     )
 
     ax = expsf.imshow(241, cmap=cmap)[0]
     empsf.imshow(242, sharex=ax, sharey=ax, cmap=cmap)
     obsvol.imshow(243, sharex=ax, sharey=ax, cmap=cmap)
     gauss.imshow(244, sharex=ax, sharey=ax, cmap=cmap)
-    z = 0
-    psf.imshow(245, data=expsf.slice(z), sharex=ax, cmap=cmap)
-    psf.imshow(246, data=empsf.slice(z), sharex=ax, cmap=cmap)
-    psf.imshow(247, data=obsvol.slice(z), sharex=ax, cmap=cmap)
-    psf.imshow(248, data=gauss.slice(z), sharex=ax, cmap=cmap)
+    i = 0
+    psf.imshow(245, data=expsf.slice(i), sharex=ax, cmap=cmap)
+    psf.imshow(246, data=empsf.slice(i), sharex=ax, cmap=cmap)
+    psf.imshow(247, data=obsvol.slice(i), sharex=ax, cmap=cmap)
+    psf.imshow(248, data=gauss.slice(i), sharex=ax, cmap=cmap)
 
     # plot cross sections
     z = numpy.arange(0, gauss.dims.ou[0], gauss.dims.ou[0] / gauss.dims.px[0])
     r = numpy.arange(0, gauss.dims.ou[1], gauss.dims.ou[1] / gauss.dims.px[1])
     zr_max = 20.0
     pyplot.figure()
     pyplot.subplot(211)
@@ -116,15 +122,15 @@
     pyplot.title('Residuals of gaussian approximation')
     pyplot.plot(r, expsf[0] - gauss2[0], 'r-', label=expsf.name + ' (r)')
     pyplot.plot(r, obsvol[0] - gauss[0], 'b-', label=obsvol.name + ' (r)')
     pyplot.plot(z, expsf[:, 0] - gauss2[:, 0], 'm-', label=expsf.name + ' (z)')
     pyplot.plot(
         z, obsvol[:, 0] - gauss[:, 0], 'c-', label=obsvol.name + ' (z)'
     )
-    pyplot.axis([0, zr_max, -0.1, 0.1])
+    pyplot.axis([0, zr_max, -0.25, 0.25])
     pyplot.tight_layout()
 
     pyplot.show()
 
 
 if __name__ == '__main__':
     psf_example()
```

### Comparing `psf-2022.9.26/psf/psf.c` & `psf-2023.4.26/psf/psf.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /* psf.c */
 
 /*
-Copyright (c) 2007-2022, Christoph Gohlke
+Copyright (c) 2007-2023, Christoph Gohlke
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -34,20 +34,20 @@
 "Point Spread Function calculations for fluorescence microscopy.\n\
 \n\
 Psf.c is a Python C extension module that provides low level implementations\n\
 for the psf package.\n\
 \n\
 Refer to the psf.py module for a high level API, documentation, and tests.\n\
 \n\
-:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_ and Oliver Holub\n\
+:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_\n\
 :License: BSD 3-Clause\n\
-:Version: 2022.9.12\n\
+:Version: 2023.4.26\n\
 "
 
-#define _VERSION_ "2022.9.12"
+#define _VERSION_ "2023.4.26"
 
 #define WIN32_LEAN_AND_MEAN
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 #include "Python.h"
 #include "math.h"
 #include "float.h"
```

### Comparing `psf-2022.9.26/psf/psf.py` & `psf-2023.4.26/psf/psf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # psf.py
 
-# Copyright (c) 2007-2022, Christoph Gohlke and Oliver Holub
+# Copyright (c) 2007-2023, Christoph Gohlke and Oliver Holub
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -30,35 +30,55 @@
 # POSSIBILITY OF SUCH DAMAGE.
 
 """Point Spread Function calculations for fluorescence microscopy.
 
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
-This library is no longer actively developed.
-Consider using the `pyotf <https://pypi.org/project/pyotf/>`_ package instead.
+The psf library is no longer actively developed.
 
-:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_ and Oliver Holub
+:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.26
+:Version: 2023.4.26
+
+Quickstart
+----------
+
+Install the psf package and all dependencies from the
+`Python Package Index <https://pypi.org/project/psf/>`_::
+
+    python -m pip install -U psf[all]
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/psf>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.7.1
   (optional for plotting)
 
 Revisions
 ---------
 
+2023.4.26
+
+- Use enums.
+- Derive Dimensions from UserDict.
+- Add type hints.
+- Convert to Google style docstrings.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.26
 
 - Fix setup.py.
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
@@ -144,19 +164,23 @@
 >>> # save a full 3D PSF volume to file
 >>> obsvol.volume().tofile('_test_volume.bin')
 
 Refer to `psf_example.py` in the source distribution for more examples.
 
 """
 
-__version__ = '2022.9.26'
+from __future__ import annotations
+
+__version__ = '2023.4.26'
 
 __all__ = [
     'PSF',
+    'PsfType',
     'Pinhole',
+    'PinholeShape',
     'Dimensions',
     'uv2zr',
     'zr2uv',
     'mirror_symmetry',
     'imshow',
     'ANISOTROPIC',
     'ISOTROPIC',
@@ -169,91 +193,114 @@
     'TWOPHOTON',
     'PARAXIAL',
 ]
 
 import math
 import time
 import threading
+import enum
+from collections import UserDict
 
 import numpy
 
 try:
     from . import _psf
 except ImportError:
     import _psf  # type: ignore
 
-ANISOTROPIC = 1
-ISOTROPIC = 2
-GAUSSIAN = 4
-GAUSSLORENTZ = 8
-EXCITATION = 16
-EMISSION = 32
-WIDEFIELD = 64
-CONFOCAL = 128
-TWOPHOTON = 256
-PARAXIAL = 512
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Any, TypeVar
+    from collections.abc import Iterable, Mapping
+    from numpy.typing import ArrayLike, NDArray
+
+    DimensionT = TypeVar('DimensionT')
+else:
+    DimensionT = None
+
+
+class PsfType(enum.IntFlag):
+    """Type of PSF defined by combining one model and one type."""
+
+    ANISOTROPIC = 1
+    """Anisotropic model (not implemented)."""
+    ISOTROPIC = 2
+    """Isotropic model."""
+    GAUSSIAN = 4
+    """Gaussian model."""
+    GAUSSLORENTZ = 8
+    """Gaussian Lorenzian model."""
+
+    EXCITATION = 16
+    """Excitation type."""
+    EMISSION = 32
+    """Emission type."""
+    WIDEFIELD = 64
+    """Widefield type."""
+    CONFOCAL = 128
+    """Confocal type."""
+    TWOPHOTON = 256
+    """Two-photon type."""
+
+    PARAXIAL = 512
+    """Border case for Gaussian approximations."""
+
+
+class PinholeShape(enum.IntEnum):
+    """Pinhole shapes."""
+
+    ROUND = 0
+    """Round pinhole."""
+    SQUARE = 4
+    """Square pinhole."""
+
+
+ANISOTROPIC = PsfType.ANISOTROPIC
+ISOTROPIC = PsfType.ISOTROPIC
+GAUSSIAN = PsfType.GAUSSIAN
+GAUSSLORENTZ = PsfType.GAUSSLORENTZ
+EXCITATION = PsfType.EXCITATION
+EMISSION = PsfType.EMISSION
+WIDEFIELD = PsfType.WIDEFIELD
+CONFOCAL = PsfType.CONFOCAL
+TWOPHOTON = PsfType.TWOPHOTON
+PARAXIAL = PsfType.PARAXIAL
 
 
 class PSF:
     """Calculate point spread function of various types.
 
-    Attributes
-    ----------
-    psftype : int
-        A combination of the following properties. Valid combinations are
-        listed in PSF.psftype.
-
-        ANISOTROPIC or ISOTROPIC or GAUSSIAN or GAUSSLORENTZ
-            Specify calculation model.
-        EXCITATION or EMISSION or WIDEFIELD or CONFOCAL or TWOPHOTON
-            Specify type of PSF.
-        PARAXIAL
-            Border case for Gaussian approximations.
-    name : str
-        A human readable label.
-    data : 2D array of floats (C doubles)
-        PSF values in z,r space normalized to the value at the origin.
-    shape : sequence of int
-        Size of the data array in pixel. Default (256, 256)
-    dims : Dimension instance
-        Dimensions of the data array in px (pixel), um (micrometers),
-        ou (optical units), and au (airy units).
-    ex_wavelen and em_wavelen : float or None
-        Excitation or emission wavelengths in micrometers if applicable.
-    num_aperture : float
-        Numerical aperture (NA) of the objective. Default 1.2.
-    refr_index : float
-        Index of refraction of the sample medium. Default 1.333 (water).
-    magnification : float
-        Total magnification of the optical system. Default 1.0.
-    underfilling : float
-        Underfilling factor, i.e. the ratio of the radius of the objective
-        back aperture to the exp(-2) radius of the excitation laser.
-        Default 1.0.
-    sigma : Dimension instance or None
-        Gaussian sigma parameters in px (pixel), um (micrometers),
-        ou (optical units), and au (airy units) if applicable.
-    pinhole : Pinhole instance or None
-        Pinhole applies to confocal types only.
-    expsf, empsf : PSF instance or None
-        Excitation or Emission PSF objects if applicable (i.e. when calculated
-        intermediately for confocal)
-
-    Notes
-    -----
-    Calculations of the isotropic PSFs are based on the complex integration
-    representation for the diffraction near the image plane proposed by
-    Richards and Wolf [1-4].
+    Parameters:
+        psftype, shape, num_aperture, refr_index, magnification, underfilling,\
+        expsf, empsf, name:
+            See class attributes.
+        dims:
+            Dimensions of data array in *micrometers*.
+        ex_wavelen, em_wavelen:
+            Excitation or emission wavelengths in *nanometers* if applicable.
+        pinhole_radius:
+            Outer radius of pinhole in *micrometers* in object space.
+            This is the back-projected radius, i.e., the real physical radius
+            of the pinhole divided by the magnification of the system.
+        pinhole_shape:
+            Pinhole shape, round or square.
+
+    Notes:
+        Calculations of the isotropic PSFs are based on the complex integration
+        representation for the diffraction near the image plane proposed by
+        Richards and Wolf [1-4].
 
-    Gaussian approximations are calculated according to [5].
+        Gaussian approximations are calculated according to [5].
 
-    Widefield calculations are used if the pinhole radius is larger than ~8 au.
+        Widefield calculations are used if the pinhole radius is larger than
+        ~8 au.
 
-    Models for polarized excitation or emission light (ANISOTROPIC) and the
-    Gaussian-Lorentzian approximation (GAUSSLORENTZ) are not implemented.
+        Models for polarized excitation or emission light (ANISOTROPIC) and the
+        Gaussian-Lorentzian approximation (GAUSSLORENTZ) are not implemented.
 
     """
 
     TYPES = {
         ISOTROPIC | EXCITATION: 'Excitation, Isotropic',
         ISOTROPIC | EMISSION: 'Emission, Isotropic',
         ISOTROPIC | WIDEFIELD: 'Widefield, Isotropic',
@@ -267,77 +314,115 @@
         GAUSSIAN | EXCITATION | PARAXIAL: 'Excitation, Gaussian, Paraxial',
         GAUSSIAN | EMISSION | PARAXIAL: 'Emission, Gaussian, Paraxial',
         GAUSSIAN | WIDEFIELD | PARAXIAL: 'Widefield, Gaussian, Paraxial',
         GAUSSIAN | CONFOCAL | PARAXIAL: 'Confocal, Gaussian, Paraxial',
         GAUSSIAN | TWOPHOTON | PARAXIAL: 'Two-Photon, Gaussian, Paraxial',
     }
 
+    psftype: PsfType
+    """Type of PSF."""
+
+    name: str
+    """Human readable label."""
+
+    data: NDArray[numpy.float64]
+    """PSF values in z,r space normalized to value at origin."""
+
+    shape: tuple[int, int]
+    """Size of data array in pixel."""
+
+    dims: Dimensions[tuple[float, float]]
+    """
+    Dimensions of data array in px (pixel), um (micrometers),
+    ou (optical units), and au (airy units).
+    """
+    ex_wavelen: float
+    """Excitation wavelength in micrometers if applicable."""
+
+    em_wavelen: float
+    """Emission wavelength in micrometers if applicable."""
+
+    num_aperture: float
+    """Numerical aperture (NA) of objective."""
+
+    refr_index: float
+    """Index of refraction of sample medium."""
+
+    magnification: float
+    """Total magnification of optical system."""
+
+    underfilling: float
+    """
+    Ratio of radius of objective back aperture to exp(-2) radius of
+    excitation laser.
+    """
+
+    sigma: Dimensions[tuple[float, float]] | None
+    """
+    Gaussian sigmas in px (pixel), um (micrometers), ou (optical units),
+    and au (airy units) if applicable.
+    """
+
+    pinhole: Pinhole | None
+    """Pinhole for confocal types."""
+
+    expsf: PSF | None
+    """Excitation PSF object for confocal types."""
+
+    empsf: PSF | None
+    """Emission PSF object for confocal types."""
+
     def __init__(
         self,
-        psftype,
-        shape=(256, 256),
-        dims=(4.0, 4.0),
-        ex_wavelen=None,
-        em_wavelen=None,
-        num_aperture=1.2,
-        refr_index=1.333,
-        magnification=1.0,
-        underfilling=1.0,
-        pinhole_radius=None,
-        pinhole_shape='round',
-        expsf=None,
-        empsf=None,
-        name=None,
+        psftype: PsfType,
+        /,
+        shape: tuple[int, int] = (256, 256),
+        dims: tuple[float, float] = (4.0, 4.0),
+        *,
+        ex_wavelen: float = math.nan,
+        em_wavelen: float = math.nan,
+        num_aperture: float = 1.2,
+        refr_index: float = 1.333,
+        magnification: float = 1.0,
+        underfilling: float = 1.0,
+        pinhole_radius: float | None = None,
+        pinhole_shape: PinholeShape | str = PinholeShape.ROUND,
+        expsf: PSF | None = None,
+        empsf: PSF | None = None,
+        name: str | None = None,
     ):
-        """Initialize the PSF object.
-
-        Arguments
-        ---------
-        psftype, shape, num_aperture, refr_index, magnification, underfilling,
-            expsf, and empsf:
-            See PSF attributes.
-        dims : sequence of float
-            Dimensions of the data array in *micrometers*. Default (4., 4.)
-        ex_wavelen and em_wavelen : float or None
-            Excitation or emission wavelengths in *nanometers* if applicable.
-        pinhole_radius : float or None
-            Outer radius of the pinhole in *micrometers* in the object space.
-            This is the back-projected radius, i.e. the real physical radius
-            of the pinhole divided by the magnification of the system.
-        pinhole_shape : str
-            Either 'round' (default) or 'square'.
-
-        """
         try:
             self.name = PSF.TYPES[psftype]
             self.psftype = psftype
         except Exception as exc:
-            raise ValueError('PSF type is invalid or not supported') from exc
+            raise ValueError(
+                f'PSF type {psftype!r} is invalid or not supported'
+            ) from exc
 
         if name:
             self.name = str(name)
 
         self.shape = int(shape[0]), int(shape[1])
         self.dims = Dimensions(px=shape, um=(float(dims[0]), float(dims[1])))
 
-        self.ex_wavelen = ex_wavelen / 1e3 if ex_wavelen else None
-        self.em_wavelen = em_wavelen / 1e3 if em_wavelen else None
+        self.ex_wavelen = ex_wavelen / 1e3
+        self.em_wavelen = em_wavelen / 1e3
         self.num_aperture = num_aperture
         self.refr_index = refr_index
         self.magnification = magnification
         self.underfilling = underfilling
         self.sigma = None
         self.pinhole = None
         self.expsf = expsf
         self.empsf = empsf
 
-        if not (psftype & EXCITATION) and em_wavelen is None:
+        if not (psftype & EXCITATION) and em_wavelen is math.nan:
             raise ValueError('emission wavelength not specified')
 
-        if not (psftype & EMISSION) and ex_wavelen is None:
+        if not (psftype & EMISSION) and ex_wavelen is math.nan:
             raise ValueError('excitation wavelength not specified')
 
         if psftype & CONFOCAL and pinhole_radius is None:
             raise ValueError('pinhole radius not specified')
 
         self.sinalpha = self.num_aperture / self.refr_index
         if self.sinalpha >= 1.0:
@@ -365,54 +450,52 @@
                 self.refr_index,
                 1.0,
             )
         self.dims.update(
             ou=ou, au=(self.dims.um[0] / au, self.dims.um[1] / au)
         )
 
-        if pinhole_radius:
+        if pinhole_radius is not None:
             self.pinhole = Pinhole(pinhole_radius, self.dims, pinhole_shape)
 
-        try:
-            clock = time.perf_counter
-        except AttributeError:
-            clock = time.clock
-
+        clock = time.perf_counter
         start = clock()
+
         if psftype & GAUSSIAN:
             self.sigma = Dimensions(**self.dims)
             if self.underfilling != 1.0:
                 raise NotImplementedError(
                     'underfilling not supported in Gaussian approximation'
                 )
 
             if psftype & EXCITATION or psftype & TWOPHOTON:
                 widefield = True
-                self.em_wavelen = None
-                self.magnification = None
+                self.em_wavelen = math.nan
+                self.magnification = math.nan
                 self.pinh_radius = None
                 lex = lem = self.ex_wavelen
                 radius = 0.0
             elif psftype & EMISSION or psftype & WIDEFIELD:
                 widefield = True
-                self.ex_wavelen = None
-                self.magnification = None
+                self.ex_wavelen = math.nan
+                self.magnification = math.nan
                 lex = lem = self.em_wavelen
                 radius = 0.0
             elif psftype & CONFOCAL:
+                assert self.pinhole is not None
                 radius = self.pinhole.radius.um
                 if radius > 9.76 * self.ex_wavelen / self.num_aperture:
                     # use widefield approximation for pinholes > 8 AU
                     widefield = True
                     lex = lem = self.ex_wavelen
                 else:
                     widefield = False
                     lex = self.ex_wavelen
                     lem = self.em_wavelen
-                if self.pinhole.shape != 'round':
+                if self.pinhole.shape != PinholeShape.ROUND:
                     raise NotImplementedError(
                         'Gaussian approximation only valid for round pinhole'
                     )
 
             paraxial = bool(psftype & PARAXIAL)
             self.sigma.um = _psf.gaussian_sigma(
                 lex,
@@ -423,29 +506,29 @@
                 widefield,
                 paraxial,
             )
             self.data = _psf.gaussian2d(self.dims.px, self.sigma.px)
 
         elif psftype & ISOTROPIC:
             if psftype & EXCITATION or psftype & TWOPHOTON:
-                self.em_wavelen = None
-                self.magnification = None
+                self.em_wavelen = math.nan
+                self.magnification = math.nan
                 self.data = _psf.psf(
                     0,
                     self.shape,
                     self.dims.ou,
                     1.0,
                     self.sinalpha,
                     self.underfilling,
                     1.0,
                     80,
                 )
             elif psftype & EMISSION:
-                self.ex_wavelen = None
-                self.underfilling = None
+                self.ex_wavelen = math.nan
+                self.underfilling = math.nan
                 self.data = _psf.psf(
                     1,
                     self.shape,
                     self.dims.ou,
                     self.magnification,
                     self.sinalpha,
                     1.0,
@@ -454,363 +537,405 @@
                 )
             elif psftype & CONFOCAL or psftype & WIDEFIELD:
                 if em_wavelen < ex_wavelen:
                     raise ValueError('Excitation > Emission wavelength')
                 # start threads to calculate excitation and emission PSF
                 threads = []
                 if not (
-                    self.expsf and self.expsf.psftype == ISOTROPIC | EXCITATION
+                    self.expsf is not None
+                    and self.expsf.psftype == ISOTROPIC | EXCITATION
                 ):
                     threads.append(
                         (
                             'expsf',
                             PSFthread(
                                 ISOTROPIC | EXCITATION,
                                 shape,
                                 dims,
-                                ex_wavelen,
-                                None,
-                                num_aperture,
-                                refr_index,
-                                1.0,
-                                underfilling,
+                                ex_wavelen=ex_wavelen,
+                                em_wavelen=math.nan,
+                                num_aperture=num_aperture,
+                                refr_index=refr_index,
+                                magnification=1.0,
+                                underfilling=underfilling,
                             ),
                         )
                     )
                 if not (
-                    self.empsf and self.empsf.psftype == ISOTROPIC | EMISSION
+                    self.empsf is not None
+                    and self.empsf.psftype == ISOTROPIC | EMISSION
                 ):
                     threads.append(
                         (
                             'empsf',
                             PSFthread(
                                 ISOTROPIC | EMISSION,
                                 shape,
                                 dims,
-                                None,
-                                em_wavelen,
-                                num_aperture,
-                                refr_index,
-                                magnification,
-                                1.0,
+                                ex_wavelen=math.nan,
+                                em_wavelen=em_wavelen,
+                                num_aperture=num_aperture,
+                                refr_index=refr_index,
+                                magnification=magnification,
+                                underfilling=1.0,
                             ),
                         )
                     )
                 for a, t in threads:
                     t.start()
                 for a, t in threads:
                     t.join()
                     setattr(self, a, t.psf)
+                if self.expsf is None:
+                    raise ValueError('Excitation PSF is None')
+                if self.empsf is None:
+                    raise ValueError('Emission PSF is None')
                 if not self.expsf.iscompatible(self.empsf):
                     raise ValueError(
-                        'Excitation and Emission PSF not compatible'
+                        'Excitation and emission PSF not compatible'
                     )
                 if psftype & WIDEFIELD or (
-                    self.pinhole.radius.um
+                    self.pinhole is not None
+                    and self.pinhole.radius.um
                     > 9.76 * self.ex_wavelen / self.num_aperture
                 ):
                     # use widefield approximation for pinholes > 8 AU
                     self.data = _psf.obsvol(self.expsf.data, self.empsf.data)
                 else:
+                    assert self.pinhole is not None
                     self.data = _psf.obsvol(
                         self.expsf.data, self.empsf.data, self.pinhole.kernel()
                     )
 
         if psftype & TWOPHOTON:
             self.data *= self.data
         self.time = float(clock() - start) * 1e3
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: Any, /) -> NDArray[numpy.float64]:
         """Return value of data array at position."""
         return self.data[key]
 
-    def __str__(self):
-        """Return properties of PSF object as string."""
+    def __str__(self) -> str:
         s = [self.__class__.__name__, self.name]
         s.append(f'shape: ({self.dims.px[0]}, {self.dims.px[1]}) pixel')
         dims = self.dims.format(['um', 'ou', 'au'], ['%.2f', '%.2f', '%.2f'])
         s.append(f'dimensions: {dims}')
-        if self.ex_wavelen:
+        if self.ex_wavelen is not math.nan:
             s.append(f'excitation wavelength: {self.ex_wavelen * 1e3:.1f} nm')
-        if self.em_wavelen:
+        if self.em_wavelen is not math.nan:
             s.append(f'emission wavelength: {self.em_wavelen * 1e3:.1f} nm')
         s.append(f'numeric aperture: {self.num_aperture:.2f}')
         s.append(f'refractive index: {self.refr_index:.2f}')
         angle = math.degrees(math.asin(self.sinalpha))
         s.append(f'half cone angle: {angle:.2f} deg')
-        if self.magnification:
+        if self.magnification is not math.nan:
             s.append(f'magnification: {self.magnification:.2f}')
-        if self.underfilling:
+        if self.underfilling is not math.nan:
             s.append(f'underfilling: {self.underfilling:.2f}')
         if self.pinhole:
             pinhole = self.pinhole.radius.format(
                 ['um', 'ou', 'au', 'px'], ['%.3f', '%.3f', '%.4f', '%.2f']
             )
             s.append(f'pinhole radius: {pinhole}')
-        if self.sigma:
+        if self.sigma is not None:
             sigma = self.sigma.format(
                 ['um', 'ou', 'au', 'px'], ['%.3f', '%.3f', '%.3f', '%.2f']
             )
             s.append(f'gauss sigma: {sigma}')
         s.append(f'computing time: {self.time:.2f} ms\n')
         return '\n '.join(s)
 
-    def iscompatible(self, other):
-        """Return True if objects match dimensions and optical properties."""
+    def iscompatible(self, other: PSF, /) -> bool:
+        """Return True if PSFs match dimensions and optical properties."""
         return (
             (self.dims.px[0] == other.dims.px[0])
             and (self.dims.px[1] == other.dims.px[1])
             and (self.dims.um[0] == other.dims.um[0])
             and (self.dims.um[1] == other.dims.um[1])
             and (self.num_aperture == other.num_aperture)
             and (self.refr_index == other.refr_index)
         )
 
-    def slice(self, key=slice(None)):
-        """Return a z slice of the PSF with rotational symmetries applied."""
+    def slice(
+        self, key: int | slice = slice(None), /
+    ) -> NDArray[numpy.float64]:
+        """Return z-slice of PSF with rotational symmetries applied."""
         return _psf.zr2zxy(self.data[key])
 
-    def volume(self):
-        """Return a 3D volume of the PSF with all symmetries applied.
+    def volume(self) -> NDArray[numpy.float64]:
+        """Return 3D volume of PSF with all symmetries applied.
 
         The shape of the returned array is
-            (2*self.shape[0]-1, 2*self.shape[1]-1, 2*self.shape[1]-1)
+        `(2*self.shape[0]-1, 2*self.shape[1]-1, 2*self.shape[1]-1)`
 
         """
         return mirror_symmetry(_psf.zr2zxy(self.data))
 
-    def imshow(self, subplot=111, **kwargs):
+    def imshow(self, subplot: Any = 111, **kwargs: Any):
         """Log-plot PSF image using matplotlib.pyplot. Return plot axis."""
         title = kwargs.get('title', self.name)
         aspect = (
             self.shape[1] / self.shape[0] * self.dims.um[0] / self.dims.um[1]
         )
         kwargs.update(
             dict(data=self.data, title=title, subplot=subplot, aspect=aspect)
         )
         return imshow(**kwargs)
 
 
 class PSFthread(threading.Thread):
-    """Calculate point spread function in a thread."""
+    """Calculate point spread function in thread."""
+
+    psf: PSF | None
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         threading.Thread.__init__(self)
         self.args = args
         self.kwargs = kwargs
         self.psf = None
 
-    def run(self):
+    def run(self) -> None:
         self.psf = PSF(*self.args, **self.kwargs)
 
 
 class Pinhole:
     """Pinhole object for confocal microscopy.
 
-    Attributes
-    ----------
-    radius : Dimension instance
-        Dimensions of the outer pinhole radius in px (pixel), um (micrometers),
-        ou (optical units), and au (airy units).
-    shape : str
-        Shape of the pinhole. Either 'round' or 'square'.
-
-    Examples
-    --------
-    >>> ph = Pinhole(0.1, dict(px=16, um=1.0), 'round')
-    >>> print(f'{ph.radius.px:.5f}')
-    1.60000
-    >>> ph.kernel()
-    array([[1.     , 1.6    , 0.6    ],
-           [0.8    , 1.18579, 0.36393],
-           [0.3    , 0.36393, 0.     ]])
+    Parameters:
+        radius:
+            Outer pinhole radius in micrometers in object space.
+        dimensions:
+            Dimensions of object space in 'px' (pixel), 'um' (micrometers),
+            'ou' (optical units), and 'au' (airy units).
+        shape:
+            Shape of pinhole, round or square.
+
+    Examples:
+        >>> ph = Pinhole(0.1, dict(px=16, um=1.0), 'round')
+        >>> ph.shape
+        <PinholeShape.ROUND: 0>
+        >>> ph.radius.px
+        1.6
+        >>> ph.kernel()
+        array([[1.     , 1.6    , 0.6    ],
+               [0.8    , 1.18579, 0.36393],
+               [0.3    , 0.36393, 0.     ]])
 
     """
 
-    SHAPES = {'round': 0, 'square': 4}
-
-    def __init__(self, radius, dimensions, shape='round'):
-        """Initialize the pinhole object.
-
-        Arguments
-        ---------
-        radius : float
-            Outer pinhole radius in micrometers in object space.
-        dimensions : dict
-            Dimensions of the object space in 'px' (pixel), 'um' (micrometers),
-            'ou' (optical units), and 'au' (airy units).
-        shape : str
-            Shape of the pinhole. Either 'round' (default) or 'square'.
+    shape: PinholeShape
+    """Shape of pinhole, round or square."""
 
-        """
-        self._corners = Pinhole.SHAPES[shape]
-        self.shape = shape
+    radius: Dimensions[float]
+    """
+    Outer pinhole radius in px (pixel), um (micrometers), ou (optical units),
+    and au (airy units).
+    """
+
+    _kernel: NDArray[numpy.float64] | None
+
+    def __init__(
+        self,
+        radius: float,
+        dimensions: Mapping[str, float | tuple[float, float]],
+        shape: PinholeShape | str,
+    ) -> None:
+        self.shape = enumarg(PinholeShape, shape)  # type: ignore
         try:
-            dimensions = {k: v[1] for k, v in dimensions.items()}
-        except TypeError:
+            dimensions = {
+                k: v[1] for k, v in dimensions.items()  # type: ignore
+            }
+        except (TypeError, IndexError):
             pass
         self.radius = Dimensions(**dimensions)
         self.radius.um = float(radius)
         self._kernel = None
 
-    def __str__(self):
+    def kernel(self) -> NDArray[numpy.float64]:
+        """Return convolution kernel for integration over the pinhole."""
+        if self._kernel is None:
+            self._kernel = _psf.pinhole_kernel(self.radius.px, self.shape)
+        return self._kernel
+
+    def __str__(self) -> str:
         """Return string with information about Pinhole instance."""
         return '\n '.join(
             (
                 self.__class__.__name__,
                 f'shape: {self.shape}',
                 f'radius: {self.radius}',
             )
         )
 
-    def kernel(self):
-        """Return convolution kernel for integration over the pinhole."""
-        if self._kernel is None:
-            self._kernel = _psf.pinhole_kernel(self.radius.px, self._corners)
-        return self._kernel
-
 
-class Dimensions(dict):
+class Dimensions(UserDict[str, DimensionT]):
     """Store dimensions in various units and perform linear conversions.
 
-    Examples
-    --------
-    >>> dim = Dimensions(px=100, um=2)
-    >>> dim(50, 'px', 'um')
-    1.0
-    >>> dim.px, dim.um
-    (100, 2)
-    >>> dim.px = 50
-    >>> dim.um
-    1.0
-    >>> dim.format(('um', 'px'), ('%.2f', '%.1f'))
-    '1.00 um, 50.0 px'
-    >>> dim = Dimensions(px=(100, 200), um=(2, 8))
-    >>> dim((50, 50), 'px', 'um')
-    (1.0, 2.0)
-    >>> dim.ou = (1, 2)
-    >>> dim.px
-    (100, 200)
-    >>> dim['px'] = (50, 100)
-    >>> dim.ou
-    (0.5, 1.0)
+    Examples:
+        >>> dim = Dimensions(px=100, um=2)
+        >>> dim(50, 'px', 'um')
+        1.0
+        >>> dim.px, dim.um
+        (100, 2)
+        >>> dim.px = 50
+        >>> dim.um
+        1.0
+        >>> dim.format(('um', 'px'), ('%.2f', '%.1f'))
+        '1.00 um, 50.0 px'
+        >>> dim = Dimensions(px=(100, 200), um=(2, 8))
+        >>> dim((50, 50), 'px', 'um')
+        (1.0, 2.0)
+        >>> dim.ou = (1, 2)
+        >>> dim.px
+        (100, 200)
+        >>> dim['px'] = (50, 100)
+        >>> dim.ou
+        (0.5, 1.0)
 
     """
 
-    __slots__ = ()
+    # can not use slots when deriving from UserDict
+    # __slots__ = ('data',)
 
-    def __call__(self, value, unit, newunit):
+    def __init__(self, dict=None, /, **kwargs):
+        data = {}
+        if dict is not None:
+            data.update(dict)
+        if kwargs:
+            data.update(kwargs)
+        self.__dict__['data'] = data  # avoid __setattr__
+
+    def __call__(
+        self, value: DimensionT, unit: str, newunit: str, /
+    ) -> DimensionT:
         """Return value given in unit in another unit."""
-        dim = self[unit]
-        new = self[newunit]
+        dim = self.data[unit]
+        new = self.data[newunit]
         try:
-            return value * (new / dim)
+            return value * (new / dim)  # type: ignore
         except TypeError:
-            return tuple(v * (o / u) for v, u, o in zip(value, dim, new))
+            return tuple(
+                v * (o / u) for v, u, o in zip(value, dim, new)  # type: ignore
+            )
 
-    def __setitem__(self, unit, value):
-        """Add a dimension or rescale all dimensions to new value."""
+    def __getattr__(self, unit: str, /) -> DimensionT:
+        if unit == 'data':
+            raise AttributeError()
+        return self.data[unit]
+
+    def __setattr__(self, unit: str, value: DimensionT, /) -> None:
+        """Add dimension or rescale all dimensions to new value."""
+        if unit != 'data':
+            self.__setitem__(unit, value)
+
+    def __setitem__(self, unit: str, value: DimensionT, /) -> None:
+        """Add dimension or rescale all dimensions to new value."""
+        data = self.data
         try:
-            dim = self[unit]
+            dim = data[unit]
         except KeyError:
-            dict.__setitem__(self, unit, value)
-        else:
-            try:
-                scale = value / dim
-                for k, v in self.items():
-                    dict.__setitem__(self, k, v * scale)
-            except TypeError:
-                scale = tuple(v / d for v, d in zip(value, dim))
-                for k, v in self.items():
-                    dict.__setitem__(
-                        self, k, tuple(v * s for v, s in zip(self[k], scale))
-                    )
-
-    def __getattr__(self, unit):
-        """Return value of unit."""
-        return self[unit]
-
-    def __setattr__(self, unit, value):
-        """Add a dimension or rescale all dimensions to new value."""
-        self.__setitem__(unit, value)
+            data[unit] = value
+            return
+        try:
+            scale = value / dim  # type: ignore
+            for k, v in data.items():
+                data[k] = v * scale
+        except TypeError:
+            scale = tuple(v / d for v, d in zip(value, dim))  # type: ignore
+            for k, v in data.items():
+                data[k] = tuple(  # type: ignore
+                    v * s for v, s in zip(data[k], scale)  # type: ignore
+                )
 
-    def format(self, keys, formatstr):
+    def format(self, keys: Iterable[str], formatstr: Iterable[str], /) -> str:
         """Return formatted string."""
         s = []
         try:
             for k, f in zip(keys, formatstr):
                 f = f % self[k]
                 s.append(f'{f} {k}')
         except TypeError:
             for k, f in zip(keys, formatstr):
                 v = self[k]
                 t = []
-                for i in v:
+                for i in v:  # type: ignore
                     t.append(f % i)
                 s.append('({}) {}'.format(', '.join(t), k))
         return ', '.join(s)
 
 
-def uv2zr(uv, wavelength, sinalpha, refr_index, magnification=1.0):
-    """Return z,r in units of the wavelength from u,v given in optical units.
+def uv2zr(
+    uv: tuple[float, float],
+    /,
+    wavelength: float,
+    sinalpha: float,
+    refr_index: float,
+    magnification: float = 1.0,
+) -> tuple[float, float]:
+    """Return z,r in units of wavelength from u,v given in optical units.
 
     For excitation, magnification should be 1.
 
-    Examples
-    --------
-    >>> numpy.allclose(
-    ...     uv2zr((1, 1), 488, 0.9, 1.33),
-    ...     (72.094692498695736, 64.885223248826165)
-    ... )
-    True
+    Examples:
+        >>> numpy.allclose(
+        ...     uv2zr((1, 1), 488, 0.9, 1.33),
+        ...     (72.094692498695736, 64.885223248826165)
+        ... )
+        True
 
     """
     a = wavelength / (2.0 * math.pi * sinalpha * refr_index * magnification)
     b = a / (sinalpha * magnification)
     return uv[0] * b, uv[1] * a
 
 
-def zr2uv(zr, wavelength, sinalpha, refr_index, magnification=1.0):
-    """Return u,v in optical units from z,r given in units of the wavelength.
+def zr2uv(
+    zr: tuple[float, float],
+    /,
+    wavelength: float,
+    sinalpha: float,
+    refr_index: float,
+    magnification: float = 1.0,
+) -> tuple[float, float]:
+    """Return u,v in optical units from z,r given in units of wavelength.
 
     For excitation, magnification should be 1.
 
-    Examples
-    --------
-    >>> numpy.allclose(
-    ...     zr2uv((1e3, 1e3), 488, 0.9, 1.33),
-    ...     (13.870646580788051, 15.411829534208946)
-    ... )
-    True
+    Examples:
+        >>> numpy.allclose(
+        ...     zr2uv((1e3, 1e3), 488, 0.9, 1.33),
+        ...     (13.870646580788051, 15.411829534208946)
+        ... )
+        True
 
     """
     a = (2.0 * math.pi * refr_index * sinalpha * magnification) / wavelength
     b = a * sinalpha * magnification
     return zr[0] * b, zr[1] * a
 
 
-def mirror_symmetry(data):
+def mirror_symmetry(data: ArrayLike, /) -> NDArray[numpy.float64]:
     """Apply mirror symmetry along one face in each dimension.
 
-    The input array can be 1, 2 or 3-dimensional.
+    The input array can be 1, 2, or 3-dimensional.
+    The shape of the returned array is `2*data.shape-1` in each dimension.
 
-    The shape of the returned array is 2*data.shape-1 in each dimension.
-
-    Examples
-    --------
-    >>> mirror_symmetry([0, 1])
-    array([1., 0., 1.])
-    >>> mirror_symmetry([[0, 1],[0, 1]])
-    array([[1., 0., 1.],
-           [1., 0., 1.],
-           [1., 0., 1.]])
-    >>> mirror_symmetry([[[0, 1],[0, 1]], [[0, 1],[0, 1]], [[0, 1],[0, 1]]])[0]
-    array([[1., 0., 1.],
-           [1., 0., 1.],
-           [1., 0., 1.]])
+    Examples:
+        >>> mirror_symmetry([0, 1])
+        array([1., 0., 1.])
+        >>> mirror_symmetry([[0, 1],[0, 1]])
+        array([[1., 0., 1.],
+               [1., 0., 1.],
+               [1., 0., 1.]])
+        >>> mirror_symmetry(
+        ...     [[[0, 1],[0, 1]], [[0, 1],[0, 1]], [[0, 1],[0, 1]]]
+        ... )[0]
+        array([[1., 0., 1.],
+               [1., 0., 1.],
+               [1., 0., 1.]])
 
     """
     data = numpy.array(data)
     result = numpy.empty([2 * i - 1 for i in data.shape], numpy.float64)
     if data.ndim == 1:
         x = data.shape[0] - 1
         result[x:] = data
@@ -829,14 +954,25 @@
     else:
         raise NotImplementedError(
             f'{data.ndim}-dimensional arrays not supported'
         )
     return result
 
 
+def enumarg(enum: type[enum.IntEnum], arg: Any, /) -> enum.IntEnum:
+    """Return enum member from its name or value."""
+    try:
+        return enum(arg)
+    except Exception:
+        try:
+            return enum[arg.upper()]
+        except Exception:
+            raise ValueError(f'invalid argument {arg!r}')
+
+
 def imshow(
     subplot,
     data,
     title=None,
     sharex=None,
     sharey=None,
     vmin=-2.5,
```

### Comparing `psf-2022.9.26/psf.egg-info/PKG-INFO` & `psf-2023.4.26/psf.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psf
-Version: 2022.9.26
+Version: 2023.4.26
 Summary: Point Spread Function calculations for fluorescence microscopy
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psf/issues
 Project-URL: Source Code, https://github.com/cgohlke/psf
@@ -12,48 +12,68 @@
 Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: all
 License-File: LICENSE
 
 Point Spread Function calculations for fluorescence microscopy
 ==============================================================
 
 Psf is a Python library to calculate Point Spread Functions (PSF) for
 fluorescence microscopy.
 
-This library is no longer actively developed.
-Consider using the `pyotf <https://pypi.org/project/pyotf/>`_ package instead.
+The psf library is no longer actively developed.
 
-:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_ and Oliver Holub
+:Authors: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2022.9.26
+:Version: 2023.4.26
+
+Quickstart
+----------
+
+Install the psf package and all dependencies from the
+`Python Package Index <https://pypi.org/project/psf/>`_::
+
+    python -m pip install -U psf[all]
+
+See `Examples`_ for using the programming interface.
+
+Source code and support are available on
+`GitHub <https://github.com/cgohlke/psf>`_.
 
 Requirements
 ------------
 
-This release has been tested with the following requirements and dependencies
+This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython 3.8.10, 3.9.13, 3.10.7, 3.11.0rc2 <https://www.python.org>`_
-- `NumPy 1.22.4 <https://pypi.org/project/numpy/>`_
-- `Matplotlib 3.5.3 <https://pypi.org/project/matplotlib/>`_
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_  3.7.1
   (optional for plotting)
 
 Revisions
 ---------
 
+2023.4.26
+
+- Use enums.
+- Derive Dimensions from UserDict.
+- Add type hints.
+- Convert to Google style docstrings.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2022.9.26
 
 - Fix setup.py.
 
 2022.9.12
 
 - Remove support for Python 3.7 (NEP 29).
```

### Comparing `psf-2022.9.26/setup.py` & `psf-2023.4.26/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code)
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
-    r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}[__version__|from]',
+    r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
 )
 
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
@@ -75,29 +75,29 @@
     url='https://www.cgohlke.com',
     project_urls={
         'Bug Tracker': 'https://github.com/cgohlke/psf/issues',
         'Source Code': 'https://github.com/cgohlke/psf',
         # 'Documentation': 'https://',
     },
     python_requires='>=3.8',
-    install_requires=['numpy>=1.19.2'],
-    setup_requires=['setuptools>=18.0', 'numpy>=1.19.2'],
+    install_requires=['numpy'],
+    setup_requires=['setuptools', 'numpy'],
+    extras_require={'all': ['matplotlib']},
     cmdclass={'build_ext': build_ext},
     packages=['psf'],
     ext_modules=[Extension('psf._psf', ['psf/psf.c'])],
     package_data={'psf': ['examples/*.py']},
     zip_safe=False,
     platforms=['any'],
     classifiers=[
         'Development Status :: 7 - Inactive',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: C',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

