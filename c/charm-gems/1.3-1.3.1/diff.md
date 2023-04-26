# Comparing `tmp/charm_gems-1.3-cp39-cp39-win_amd64.whl.zip` & `tmp/charm_gems-1.3.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2821080 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       29 b- defN 22-Mar-15 08:20 charm_gems/__init__.py
--rw-rw-rw-  2.0 fat  7817216 b- defN 22-Mar-15 08:57 charm_gems/gemsbindings.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    35823 b- defN 22-Mar-15 08:57 charm_gems-1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2671 b- defN 22-Mar-15 08:57 charm_gems-1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Mar-15 08:57 charm_gems-1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Mar-15 08:57 charm_gems-1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      572 b- defN 22-Mar-15 08:57 charm_gems-1.3.dist-info/RECORD
-7 files, 7856422 bytes uncompressed, 2820070 bytes compressed:  64.1%
+Zip file size: 2821580 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       29 b- defN 23-Apr-25 17:27 charm_gems/__init__.py
+-rw-rw-rw-  2.0 fat  7818752 b- defN 23-Apr-25 18:16 charm_gems/gemsbindings.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-25 18:16 charm_gems-1.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2746 b- defN 23-Apr-25 18:16 charm_gems-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-25 18:16 charm_gems-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-25 18:16 charm_gems-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      582 b- defN 23-Apr-25 18:16 charm_gems-1.3.1.dist-info/RECORD
+7 files, 7858043 bytes uncompressed, 2820550 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: charm_gems/__init__.py
 Comment: 
 
 Filename: charm_gems/gemsbindings.cp39-win_amd64.pyd
 Comment: 
 
-Filename: charm_gems-1.3.dist-info/LICENSE
+Filename: charm_gems-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: charm_gems-1.3.dist-info/METADATA
+Filename: charm_gems-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: charm_gems-1.3.dist-info/WHEEL
+Filename: charm_gems-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: charm_gems-1.3.dist-info/top_level.txt
+Filename: charm_gems-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: charm_gems-1.3.dist-info/RECORD
+Filename: charm_gems-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `charm_gems-1.3.dist-info/LICENSE` & `charm_gems-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `charm_gems-1.3.dist-info/METADATA` & `charm_gems-1.3.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,92 @@
-Metadata-Version: 2.1
-Name: charm-gems
-Version: 1.3
-Summary: Python bindings of the gems segmentation package.
-Home-page: https://github.com/simnibs/charm-gems
-Author: Koen Van Leemput, Oula Puonti and Juan Eugenio Iglesias
-Author-email: oulap@drcmr.dk
-License: GPL3
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
-# charm-gems
-
-[![PyPI version](https://badge.fury.io/py/charm-gems.svg)](https://badge.fury.io/py/charm-gems) ![Linux Build](https://github.com/simnibs/charm-gems/workflows/Linux%20Build/badge.svg)  ![MacOS Build](https://github.com/simnibs/charm-gems/workflows/MacOS%20Build/badge.svg) ![Windows Build](https://github.com/simnibs/charm-gems/workflows/Windows%20Build/badge.svg)
-
-This repository contains the gems C++ code and python bindings used in Freesurfer's Sequence-Adaptive Multimodal SEGmentation ([SAMSEG](https://github.com/freesurfer/freesurfer/tree/dev/python/freesurfer/samseg)) ([Puonti et al., NeuroImage, 2016](https://www.sciencedirect.com/science/article/pii/S1053811916304724)) and in SimNIBS 4.0 Complete Head Anatomy Reconstruction Method (CHARM) ([Puonti et al., NeuroImage, 2020](https://www.sciencedirect.com/science/article/pii/S1053811920305309)) to create individualized head models for electric field simulations.
-## Installation
-
-The compiled charm-gems library is available via pip â‰¥ 19.3, for python 3.6, 3.7 and 3.8
-
-```bash
-pip install --upgrade pip
-pip install charm-gems
-```
-Afterwards the package can be imported by calling
-
-```python
-import charm_gems as gems
-```
-
-## Manual Installation
-
-
-### Requirements
-* A C++ compiler compatible with C++ 11
-* Python â‰¥ 3.6
-* CMake
-* Make (Linux/MacOS)
-* Visual Studio (Windows)
-* zlib (for windows, see https://github.com/horta/zlib.install)
-
-### Preparation
-This repository uses submodules. To start it, use
-
-```bash
-git submodule init
-git submodule update
-```
-
-### Linux/MacOS
-1. Build ITK
-```
-mkdir ITK-build
-cd ITK-build
-cmake \
-    -DBUILD_SHARED_LIBS=OFF \
-    -DBUILD_TESTING=OFF \
-    -DBUILD_EXAMPLES=OFF \
-    -DCMAKE_BUILD_TYPE=Release \
-    -DCMAKE_INSTALL_PREFIX=../ITK-install \
-    ../ITK
-make install
-cd ..
-```
-
-2. Install charm-gems
-```
-ITK_DIR=ITK-install python setup.py install
-```
-### Windows (Tested on Visual Studio 2019)
-1. Build ITK
-```
-md ITK-build
-cd ITK-build
-cmake.exe ^
-    -DBUILD_SHARED_LIBS=OFF ^
-    -DBUILD_TESTING=OFF ^
-    -DBUILD_EXAMPLES=OFF ^
-    -DCMAKE_BUILD_TYPE=Release ^
-    -DCMAKE_INSTALL_PREFIX=..\ITK-install ^
-    ..\ITK
-cmake --build . --config Release --target Install
-cd ..
-```
-
-2. Install charm-gems
-```
-set ITK_DIR=ITK-install
-python setup.py install
-``` 
-
-
+Metadata-Version: 2.1
+Name: charm-gems
+Version: 1.3.1
+Summary: Python bindings of the gems segmentation package.
+Home-page: https://github.com/simnibs/charm-gems
+Author: Koen Van Leemput, Oula Puonti and Juan Eugenio Iglesias
+Author-email: oulap@drcmr.dk
+License: GPL3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+
+# charm-gems
+
+[![PyPI version](https://badge.fury.io/py/charm-gems.svg)](https://badge.fury.io/py/charm-gems) ![Linux Build](https://github.com/simnibs/charm-gems/workflows/Linux%20Build/badge.svg)  ![MacOS Build](https://github.com/simnibs/charm-gems/workflows/MacOS%20Build/badge.svg) ![Windows Build](https://github.com/simnibs/charm-gems/workflows/Windows%20Build/badge.svg)
+
+This repository contains the gems C++ code and python bindings used in Freesurfer's Sequence-Adaptive Multimodal SEGmentation ([SAMSEG](https://github.com/freesurfer/freesurfer/tree/dev/python/freesurfer/samseg)) ([Puonti et al., NeuroImage, 2016](https://www.sciencedirect.com/science/article/pii/S1053811916304724)) and in SimNIBS 4.0 Complete Head Anatomy Reconstruction Method (CHARM) ([Puonti et al., NeuroImage, 2020](https://www.sciencedirect.com/science/article/pii/S1053811920305309)) to create individualized head models for electric field simulations.
+## Installation
+
+The compiled charm-gems library is available via pip â‰¥ 19.3, for python 3.6, 3.7 and 3.8
+
+
+```bash
+pip install --upgrade pip
+pip install charm-gems
+```
+Afterwards the package can be imported by calling
+
+```python
+import charm_gems as gems
+```
+
+## Manual Installation
+
+
+### Requirements
+* A C++ compiler compatible with C++ 11
+* Python â‰¥ 3.6
+* CMake
+* Make (Linux/MacOS)
+* Visual Studio (Windows)
+* zlib (for windows, see https://github.com/horta/zlib.install)
+
+### Preparation
+This repository uses submodules. To start it, use
+
+```bash
+git submodule init
+git submodule update
+```
+
+### Linux/MacOS
+1. Build ITK
+```
+mkdir ITK-build
+cd ITK-build
+cmake \
+    -DBUILD_SHARED_LIBS=OFF \
+    -DBUILD_TESTING=OFF \
+    -DBUILD_EXAMPLES=OFF \
+    -DCMAKE_BUILD_TYPE=Release \
+    -DCMAKE_INSTALL_PREFIX=../ITK-install \
+    ../ITK
+make install
+cd ..
+```
+
+2. Install charm-gems
+```
+ITK_DIR=ITK-install python setup.py install
+```
+### Windows (Tested on Visual Studio 2019)
+1. Build ITK
+```
+md ITK-build
+cd ITK-build
+cmake.exe ^
+    -DBUILD_SHARED_LIBS=OFF ^
+    -DBUILD_TESTING=OFF ^
+    -DBUILD_EXAMPLES=OFF ^
+    -DCMAKE_BUILD_TYPE=Release ^
+    -DCMAKE_INSTALL_PREFIX=..\ITK-install ^
+    ..\ITK
+cmake --build . --config Release --target Install
+cd ..
+```
+
+2. Install charm-gems
+```
+set ITK_DIR=ITK-install
+python setup.py install
+```
```

