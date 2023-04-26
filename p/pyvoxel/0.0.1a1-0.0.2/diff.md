# Comparing `tmp/pyvoxel-0.0.1a1.tar.gz` & `tmp/pyvoxel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoxel-0.0.1a1.tar", last modified: Tue Oct  4 09:04:43 2022, max compression
+gzip compressed data, was "pyvoxel-0.0.2.tar", last modified: Tue Apr 25 22:28:27 2023, max compression
```

## Comparing `pyvoxel-0.0.1a1.tar` & `pyvoxel-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-10-04 09:04:42.511043 pyvoxel-0.0.1a1/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4288 2022-10-04 09:04:42.511043 pyvoxel-0.0.1a1/PKG-INFO
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3728 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/README.md
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       73 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/pyproject.toml
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-10-04 09:04:42.454043 pyvoxel-0.0.1a1/pyvoxel.egg-info/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4288 2022-10-04 09:04:42.000000 pyvoxel-0.0.1a1/pyvoxel.egg-info/PKG-INFO
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      483 2022-10-04 09:04:42.000000 pyvoxel-0.0.1a1/pyvoxel.egg-info/SOURCES.txt
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)        1 2022-10-04 09:04:42.000000 pyvoxel-0.0.1a1/pyvoxel.egg-info/dependency_links.txt
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      330 2022-10-04 09:04:42.000000 pyvoxel-0.0.1a1/pyvoxel.egg-info/requires.txt
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)        6 2022-10-04 09:04:42.000000 pyvoxel-0.0.1a1/pyvoxel.egg-info/top_level.txt
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      503 2022-10-04 09:04:42.513043 pyvoxel-0.0.1a1/setup.cfg
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4076 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/setup.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-10-04 09:04:42.463043 pyvoxel-0.0.1a1/voxel/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1041 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      998 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/config.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7282 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/device.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-10-04 09:04:42.505043 pyvoxel-0.0.1a1/voxel/io/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8109 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/io/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    30028 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/io/dicom.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5644 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/io/format_io.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2820 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/io/nifti.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    54219 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/med_volume.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    23412 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/numpy_routines.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    11748 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/orientation.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-10-04 09:04:42.509043 pyvoxel-0.0.1a1/voxel/utils/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)        0 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/utils/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1087 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/utils/collect_env.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3989 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/utils/env.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5467 2022-10-04 09:03:30.000000 pyvoxel-0.0.1a1/voxel/utils/logger.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.631818 pyvoxel-0.0.2/
+-rw-r--r--   0 arjundd    (501) staff       (20)    11357 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/LICENSE
+-rw-r--r--   0 arjundd    (501) staff       (20)     5192 2023-04-25 22:28:27.631872 pyvoxel-0.0.2/PKG-INFO
+-rw-r--r--   0 arjundd    (501) staff       (20)     4637 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/README.md
+-rw-r--r--   0 arjundd    (501) staff       (20)       74 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/pyproject.toml
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.628978 pyvoxel-0.0.2/pyvoxel.egg-info/
+-rw-r--r--   0 arjundd    (501) staff       (20)     5192 2023-04-25 22:28:27.000000 pyvoxel-0.0.2/pyvoxel.egg-info/PKG-INFO
+-rw-r--r--   0 arjundd    (501) staff       (20)      693 2023-04-25 22:28:27.000000 pyvoxel-0.0.2/pyvoxel.egg-info/SOURCES.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)        1 2023-04-25 22:28:27.000000 pyvoxel-0.0.2/pyvoxel.egg-info/dependency_links.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)      367 2023-04-25 22:28:27.000000 pyvoxel-0.0.2/pyvoxel.egg-info/requires.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)        6 2023-04-25 22:28:27.000000 pyvoxel-0.0.2/pyvoxel.egg-info/top_level.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)      503 2023-04-25 22:28:27.632111 pyvoxel-0.0.2/setup.cfg
+-rw-r--r--   0 arjundd    (501) staff       (20)     4685 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/setup.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.629479 pyvoxel-0.0.2/tests/
+-rw-r--r--   0 arjundd    (501) staff       (20)     2210 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/tests/test_device.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    30894 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/tests/test_med_volume.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    14641 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/tests/test_numpy_routines.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7319 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/tests/test_orientation.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.630261 pyvoxel-0.0.2/voxel/
+-rw-r--r--   0 arjundd    (501) staff       (20)     1108 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)      998 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/config.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7356 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/device.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.630518 pyvoxel-0.0.2/voxel/experimental/
+-rw-r--r--   0 arjundd    (501) staff       (20)      151 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/experimental/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4029 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/experimental/plot.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.631114 pyvoxel-0.0.2/voxel/io/
+-rw-r--r--   0 arjundd    (501) staff       (20)     8323 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/io/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    32270 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/io/dicom.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5695 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/io/format_io.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7817 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/io/http.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4525 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/io/nifti.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    71329 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/med_volume.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    24300 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/numpy_routines.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    18569 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/orientation.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-25 22:28:27.631687 pyvoxel-0.0.2/voxel/utils/
+-rw-r--r--   0 arjundd    (501) staff       (20)        0 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/utils/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1087 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/utils/collect_env.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3989 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/utils/env.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5462 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/utils/logger.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6822 2023-04-25 20:41:20.000000 pyvoxel-0.0.2/voxel/utils/pixel_data.py
```

### Comparing `pyvoxel-0.0.1a1/PKG-INFO` & `pyvoxel-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,120 @@
-Metadata-Version: 2.1
-Name: pyvoxel
-Version: 0.0.1a1
-Summary: An AI-powered open-source medical image analysis toolbox
-Home-page: https://github.com/voxelimaging/pyvoxel
-Author: Arjun Desai
-License: GNU
-Project-URL: Documentation, https://pyvoxel.readthedocs.io/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-
 # Voxel
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/voxelimaging/pyvoxel/CI)
-[![codecov](https://codecov.io/gh/voxelimaging/pyvoxel/branch/master/graph/badge.svg?token=X2FRQJHV2M)](https://codecov.io/gh/voxelimaging/pyvoxel)
-<!-- [![Documentation Status](https://readthedocs.org/projects/dosma/badge/?version=latest)](https://dosma.readthedocs.io/en/latest/?badge=latest) -->
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/pyvoxel/pyvoxel/ci.yml?branch=main)
+[![codecov](https://codecov.io/gh/pyvoxel/pyvoxel/branch/master/graph/badge.svg?token=X2FRQJHV2M)](https://codecov.io/gh/pyvoxel/pyvoxel)
+[![Documentation Status](https://readthedocs.org/projects/pyvoxel/badge/?version=latest)](https://pyvoxel.readthedocs.io/en/latest/?badge=latest)
 
-[Documentation](http://dosma.readthedocs.io/) | [DOSMA Basics Tutorial](https://colab.research.google.com/drive/1zY5-3ZyTBrn7hoGE5lH0IoQqBzumzP1i?usp=sharing)
+[Documentation](http://pyvoxel.readthedocs.io/) | [Installation](https://pyvoxel.readthedocs.io/en/latest/introduction.html) | [Basic Usage](https://pyvoxel.readthedocs.io/en/latest/user_guide.html)
 
 Voxel provides fast Pythonic data structures and tools for wrangling with medical images.
 
 ## Installation
-Voxel requires Python 3.7+. The core module depends on numpy, nibabel, pydicom, PyYAML, and tqdm.
+Voxel requires Python 3.7+. The core module depends on numpy, nibabel, pydicom, requests, and tqdm.
 
 To install Voxel, run:
 
 ```bash
 pip install pyvoxel
 ```
 
-If you would like to contribute to Voxel, we recommend you clone the repository and
-install Voxel with `pip` in editable mode.
-
-```bash
-git clone git@github.com:voxelimaging/pyvoxel.git
-cd pyvoxel
-pip install -e '.[dev,docs]'
-make dev
-```
-
-To run tests, build documentation and contribute, run
-```bash
-make autoformat test build-docs
-```
-
 ## Features
 ### Simplified, Efficient I/O
 Voxel provides efficient readers for DICOM and NIfTI formats built on nibabel and pydicom.
 Multi-slice DICOM data can be loaded in parallel with multiple workers and structured into
 the appropriate 3D volume(s). For example, multi-echo and dynamic contrast-enhanced
 (DCE) MRI scans have multiple volumes acquired at different echo times and trigger times,
 respectively. These can be loaded into multiple volumes with ease:
 
 ```python
 import voxel as vx
 
-multi_echo_scan = dm.load("/path/to/multi-echo/scan", group_by="EchoNumbers", num_workers=8, verbose=True)
-dce_scan = dm.load("/path/to/dce/scan", group_by="TriggerTime")
+xray = vx.load("path/to/xray.dcm")
+ct_scan = vx.load("path/to/ct/folder/")
+
+multi_echo_scan = vx.load("/path/to/multi-echo/scan", group_by="EchoNumbers")
+dce_scan = vx.load("/path/to/dce/scan", group_by="TriggerTime")
 ```
 
 ### Data-Embedded Medical Images
-Voxel's [MedicalVolume](https://dosma.readthedocs.io/en/latest/generated/dosma.MedicalVolume.html#dosma.MedicalVolume)
-data structure supports array-like operations (arithmetic, slicing, etc.) on medical images while preserving spatial
-attributes and accompanying metadata. This structure supports NumPy interoperability, intelligent reformatting,
-fast low-level computations, and native GPU support. For example, given MedicalVolumes `mvA` and `mvB` we can do the following:
+Voxel's `MedicalVolume` data structure supports array-like operations (arithmetic, slicing, etc.) on medical images while preserving spatial
+attributes and accompanying metadata. This structure supports NumPy interoperability intelligent reformatting, fast low-level computations, and native GPU support. For example, given MedicalVolumes `mv_a` and `mv_b` we can do the following:
 
 ```python
 # Reformat image into Superior->Inferior, Anterior->Posterior, Left->Right directions.
-mvA = mvA.reformat(("SI", "AP", "LR"))
+mv_a = mv_a.reformat(("SI", "AP", "LR"))
 
 # Get and set metadata
-study_description = mvA.get_metadata("StudyDescription")
-mvA.set_metadata("StudyDescription", "A sample study")
+study_description = mv_a.get_metadata("StudyDescription")
+mv_a.set_metadata("StudyDescription", "A sample study")
 
 # Perform NumPy operations like you would on image data.
-rss = np.sqrt(mvA**2 + mvB**2)
+rss = np.sqrt(mv_a**2 + mv_b**2)
 
 # Move to GPU 0 for CuPy operations
-mv_gpu = mvA.to(dosma.Device(0))
+mv_gpu = mv_a.to(vx.Device(0))
 
 # Take slices. Metadata will be sliced appropriately.
-mv_subvolume = mvA[10:20, 10:20, 4:6]
+mv_subvolume = mv_a[10:20, 10:20, 4:6]
+```
+
+### Easily Prepare Data for AI Pipelines
+Voxel enables you to preprocess DICOM images for deep learning in a few lines of code:
+
+```python
+# Load a scan, and prepare it for AI/visualization
+mv = (
+  vx.load("/dicoms")
+  .apply_rescale()
+  .apply_window()
+  .to_grayscale()
+)
+
+# Zero-copy to PyTorch
+arr = mv.to_torch()
+```
+
+### Connect with PACS
+Voxel provides easy access to data stored in a PACS environment through DICOMweb.
+This makes loading data from a remote server just as easy as using the local filesystem.
+
+```python
+# Download an MRI from a local Orthanc instance
+mv = vx.load("http://localhost:8042/dicom-web/studies/x/series/y", params={"Modality": "MR"})
+
+# Re-use the session for multiple requests
+with vx.HttpReader(verbose=True) as hr:
+  mv_a = hr.load("http://localhost:8042/dicom-web/studies/v/series/w")
+  mv_b = hr.load("http://localhost:8042/dicom-web/studies/x/series/y")
+```
+
+## Contribute
+If you would like to contribute to Voxel, we recommend you clone the repository and
+install Voxel with `pip` in editable mode.
+
+```bash
+git clone git@github.com:pyvoxel/pyvoxel.git
+cd pyvoxel
+pip install -e '.[dev,docs]'
+make dev
+```
+
+To run tests, build documentation and contribute, run
+```bash
+make autoformat test build-docs
 ```
 
 ## Citation
-Voxel is a refactored version of the [dosma](https://github.com/ad12/dosma) package that focuses on medical image data structures and I/O.
+Voxel is a refactored version of the [DOSMA](https://github.com/ad12/dosma) package that focuses on medical image data structures and I/O.
 If you use Voxel in your research, please cite the following work:
 
 ```
 @inproceedings{desai2019dosma,
   title={DOSMA: A deep-learning, open-source framework for musculoskeletal MRI analysis},
   author={Desai, Arjun D and Barbieri, Marco and Mazzoli, Valentina and Rubin, Elka and Black, Marianne S and Watkins, Lauren E and Gold, Garry E and Hargreaves, Brian A and Chaudhari, Akshay S},
   booktitle={Proc 27th Annual Meeting ISMRM, Montreal},
   pages={1135},
   year={2019}
 }
 ```
 
-In addition to DOSMA, please also consider citing the work that introduced the method used for analysis.
-
-
+In addition to Voxel, please also consider citing the work that introduced the method used for analysis.
```

### Comparing `pyvoxel-0.0.1a1/pyvoxel.egg-info/PKG-INFO` & `pyvoxel-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,137 @@
 Metadata-Version: 2.1
 Name: pyvoxel
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: An AI-powered open-source medical image analysis toolbox
-Home-page: https://github.com/voxelimaging/pyvoxel
+Home-page: https://github.com/pyvoxel/pyvoxel
 Author: Arjun Desai
 License: GNU
 Project-URL: Documentation, https://pyvoxel.readthedocs.io/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
 
 # Voxel
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/voxelimaging/pyvoxel/CI)
-[![codecov](https://codecov.io/gh/voxelimaging/pyvoxel/branch/master/graph/badge.svg?token=X2FRQJHV2M)](https://codecov.io/gh/voxelimaging/pyvoxel)
-<!-- [![Documentation Status](https://readthedocs.org/projects/dosma/badge/?version=latest)](https://dosma.readthedocs.io/en/latest/?badge=latest) -->
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/pyvoxel/pyvoxel/ci.yml?branch=main)
+[![codecov](https://codecov.io/gh/pyvoxel/pyvoxel/branch/master/graph/badge.svg?token=X2FRQJHV2M)](https://codecov.io/gh/pyvoxel/pyvoxel)
+[![Documentation Status](https://readthedocs.org/projects/pyvoxel/badge/?version=latest)](https://pyvoxel.readthedocs.io/en/latest/?badge=latest)
 
-[Documentation](http://dosma.readthedocs.io/) | [DOSMA Basics Tutorial](https://colab.research.google.com/drive/1zY5-3ZyTBrn7hoGE5lH0IoQqBzumzP1i?usp=sharing)
+[Documentation](http://pyvoxel.readthedocs.io/) | [Installation](https://pyvoxel.readthedocs.io/en/latest/introduction.html) | [Basic Usage](https://pyvoxel.readthedocs.io/en/latest/user_guide.html)
 
 Voxel provides fast Pythonic data structures and tools for wrangling with medical images.
 
 ## Installation
-Voxel requires Python 3.7+. The core module depends on numpy, nibabel, pydicom, PyYAML, and tqdm.
+Voxel requires Python 3.7+. The core module depends on numpy, nibabel, pydicom, requests, and tqdm.
 
 To install Voxel, run:
 
 ```bash
 pip install pyvoxel
 ```
 
-If you would like to contribute to Voxel, we recommend you clone the repository and
-install Voxel with `pip` in editable mode.
-
-```bash
-git clone git@github.com:voxelimaging/pyvoxel.git
-cd pyvoxel
-pip install -e '.[dev,docs]'
-make dev
-```
-
-To run tests, build documentation and contribute, run
-```bash
-make autoformat test build-docs
-```
-
 ## Features
 ### Simplified, Efficient I/O
 Voxel provides efficient readers for DICOM and NIfTI formats built on nibabel and pydicom.
 Multi-slice DICOM data can be loaded in parallel with multiple workers and structured into
 the appropriate 3D volume(s). For example, multi-echo and dynamic contrast-enhanced
 (DCE) MRI scans have multiple volumes acquired at different echo times and trigger times,
 respectively. These can be loaded into multiple volumes with ease:
 
 ```python
 import voxel as vx
 
-multi_echo_scan = dm.load("/path/to/multi-echo/scan", group_by="EchoNumbers", num_workers=8, verbose=True)
-dce_scan = dm.load("/path/to/dce/scan", group_by="TriggerTime")
+xray = vx.load("path/to/xray.dcm")
+ct_scan = vx.load("path/to/ct/folder/")
+
+multi_echo_scan = vx.load("/path/to/multi-echo/scan", group_by="EchoNumbers")
+dce_scan = vx.load("/path/to/dce/scan", group_by="TriggerTime")
 ```
 
 ### Data-Embedded Medical Images
-Voxel's [MedicalVolume](https://dosma.readthedocs.io/en/latest/generated/dosma.MedicalVolume.html#dosma.MedicalVolume)
-data structure supports array-like operations (arithmetic, slicing, etc.) on medical images while preserving spatial
-attributes and accompanying metadata. This structure supports NumPy interoperability, intelligent reformatting,
-fast low-level computations, and native GPU support. For example, given MedicalVolumes `mvA` and `mvB` we can do the following:
+Voxel's `MedicalVolume` data structure supports array-like operations (arithmetic, slicing, etc.) on medical images while preserving spatial
+attributes and accompanying metadata. This structure supports NumPy interoperability intelligent reformatting, fast low-level computations, and native GPU support. For example, given MedicalVolumes `mv_a` and `mv_b` we can do the following:
 
 ```python
 # Reformat image into Superior->Inferior, Anterior->Posterior, Left->Right directions.
-mvA = mvA.reformat(("SI", "AP", "LR"))
+mv_a = mv_a.reformat(("SI", "AP", "LR"))
 
 # Get and set metadata
-study_description = mvA.get_metadata("StudyDescription")
-mvA.set_metadata("StudyDescription", "A sample study")
+study_description = mv_a.get_metadata("StudyDescription")
+mv_a.set_metadata("StudyDescription", "A sample study")
 
 # Perform NumPy operations like you would on image data.
-rss = np.sqrt(mvA**2 + mvB**2)
+rss = np.sqrt(mv_a**2 + mv_b**2)
 
 # Move to GPU 0 for CuPy operations
-mv_gpu = mvA.to(dosma.Device(0))
+mv_gpu = mv_a.to(vx.Device(0))
 
 # Take slices. Metadata will be sliced appropriately.
-mv_subvolume = mvA[10:20, 10:20, 4:6]
+mv_subvolume = mv_a[10:20, 10:20, 4:6]
+```
+
+### Easily Prepare Data for AI Pipelines
+Voxel enables you to preprocess DICOM images for deep learning in a few lines of code:
+
+```python
+# Load a scan, and prepare it for AI/visualization
+mv = (
+  vx.load("/dicoms")
+  .apply_rescale()
+  .apply_window()
+  .to_grayscale()
+)
+
+# Zero-copy to PyTorch
+arr = mv.to_torch()
+```
+
+### Connect with PACS
+Voxel provides easy access to data stored in a PACS environment through DICOMweb.
+This makes loading data from a remote server just as easy as using the local filesystem.
+
+```python
+# Download an MRI from a local Orthanc instance
+mv = vx.load("http://localhost:8042/dicom-web/studies/x/series/y", params={"Modality": "MR"})
+
+# Re-use the session for multiple requests
+with vx.HttpReader(verbose=True) as hr:
+  mv_a = hr.load("http://localhost:8042/dicom-web/studies/v/series/w")
+  mv_b = hr.load("http://localhost:8042/dicom-web/studies/x/series/y")
+```
+
+## Contribute
+If you would like to contribute to Voxel, we recommend you clone the repository and
+install Voxel with `pip` in editable mode.
+
+```bash
+git clone git@github.com:pyvoxel/pyvoxel.git
+cd pyvoxel
+pip install -e '.[dev,docs]'
+make dev
+```
+
+To run tests, build documentation and contribute, run
+```bash
+make autoformat test build-docs
 ```
 
 ## Citation
-Voxel is a refactored version of the [dosma](https://github.com/ad12/dosma) package that focuses on medical image data structures and I/O.
+Voxel is a refactored version of the [DOSMA](https://github.com/ad12/dosma) package that focuses on medical image data structures and I/O.
 If you use Voxel in your research, please cite the following work:
 
 ```
 @inproceedings{desai2019dosma,
   title={DOSMA: A deep-learning, open-source framework for musculoskeletal MRI analysis},
   author={Desai, Arjun D and Barbieri, Marco and Mazzoli, Valentina and Rubin, Elka and Black, Marianne S and Watkins, Lauren E and Gold, Garry E and Hargreaves, Brian A and Chaudhari, Akshay S},
   booktitle={Proc 27th Annual Meeting ISMRM, Montreal},
   pages={1135},
   year={2019}
 }
 ```
 
-In addition to DOSMA, please also consider citing the work that introduced the method used for analysis.
-
-
+In addition to Voxel, please also consider citing the work that introduced the method used for analysis.
```

### Comparing `pyvoxel-0.0.1a1/setup.py` & `pyvoxel-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
 import os
+import subprocess
 import sys
 from shutil import rmtree
 
 from setuptools import Command, find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
@@ -31,14 +32,16 @@
             f.write("".join(new_init_py))
     return version
 
 
 class UploadCommand(Command):
     """Support setup.py upload.
 
+    Only run upload from the main branch.
+
     Adapted from https://github.com/robustness-gym/meerkat.
     """
 
     description = "Build and publish the package."
     user_options = []
 
     @staticmethod
@@ -49,14 +52,24 @@
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
+        # Only upload from the main branch
+        branches = subprocess.getoutput("git branch").split("\n")
+        branches = [x.strip() for x in branches]
+        curr_branch = [x for x in branches if x.startswith("*")]
+        if len(curr_branch) != 1:
+            raise RuntimeError("Could not determine current branch.")
+        curr_branch = curr_branch[0].split(" ")[-1]
+        if curr_branch != "main":
+            raise RuntimeError("Uploads only allowed from main branch.")
+
         try:
             self.status("Removing previous builds…")
             rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
         self.status("Building Source and Wheel (universal) distribution…")
@@ -81,14 +94,15 @@
     "dataclasses>=0.6",
     "numpy",
     "natsort",
     "nibabel",
     "packaging",
     "pydicom>=1.6.0",
     "PyYAML>=5.4.1",
+    "requests",
     "tabulate",
     "termcolor",
     "tqdm>=4.42.0",
 ]
 
 # Optional packages.
 # TODO Issue #106: Fix to only import tensorflow version with fixed version
@@ -106,29 +120,31 @@
         "flake8-comprehensions",
         "isort",
         "black==22.8.0",
         "click==8.0.2",
         # testing.
         "pytest-cov>=2.10.1",
         "pre-commit>=2.9.3",
+        "requests-mock",
+        "parameterized",
         # upload.
         "twine",
     ],
     "docs": ["mistune>=0.8.1,<2.0.0", "sphinx", "sphinxcontrib.bibtex", "m2r2"],
 }
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pyvoxel",
     version=get_version(),
     author="Arjun Desai",
-    url="https://github.com/voxelimaging/pyvoxel",
+    url="https://github.com/pyvoxel/pyvoxel",
     project_urls={"Documentation": "https://pyvoxel.readthedocs.io/"},
     description="An AI-powered open-source medical image analysis toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("configs", "tests", "tests.*")),
     python_requires=">=3.6",
     install_requires=REQUIRED,
```

### Comparing `pyvoxel-0.0.1a1/voxel/__init__.py` & `pyvoxel-0.0.2/voxel/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Voxel."""
 from voxel.device import Device, cpu_device, get_array_module, get_device, to_device  # noqa: F401
 from voxel.io import load, read, save, write  # noqa: F401
 from voxel.io.dicom import DicomReader, DicomWriter  # noqa: F401
 from voxel.io.format_io import ImageDataFormat  # noqa: F401
+from voxel.io.http import HttpReader  # noqa: F401
 from voxel.io.nifti import NiftiReader, NiftiWriter  # noqa: F401
 from voxel.med_volume import MedicalVolume  # noqa: F401
 from voxel.orientation import to_affine  # noqa: F401
 from voxel.utils.collect_env import collect_env_info  # noqa
 
 from .config import config  # noqa: F401
 
 __all__ = [
     "MedicalVolume",
     "DicomReader",
     "DicomWriter",
+    "HttpReader",
     "NiftiReader",
     "NiftiWriter",
     "read",
     "save",
     "load",
     "write",
     "ImageDataFormat",
@@ -28,8 +30,8 @@
     "get_array_module",
     "to_affine",
     "collect_env_info",
 ]
 
 # This line will be programatically read/write by setup.py.
 # Leave them at the bottom of this file and don't touch them.
-__version__ = "0.0.1a1"
+__version__ = "0.0.2"
```

### Comparing `pyvoxel-0.0.1a1/voxel/config.py` & `pyvoxel-0.0.2/voxel/config.py`

 * *Files identical despite different names*

### Comparing `pyvoxel-0.0.1a1/voxel/device.py` & `pyvoxel-0.0.2/voxel/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""Functions and classes for getting and setting computing devices.
-
-"""
+"""Functions and classes for getting and setting computing devices."""
 import numpy as np
 
 from voxel.utils import env
 
 if env.cupy_available():
     import cupy as cp
 if env.sigpy_available():
@@ -41,23 +39,24 @@
     Attributes:
         type (str): Device type. Either ``'cpu'`` or ``'cuda'``.
         index (int): index = -1 represents CPU, and others represents the id_th ordinances.
 
     Note:
         This class is heavily based on
         `sigpy.Device <https://sigpy.readthedocs.io/en/latest/generated/sigpy.Device.html>`_.
-
     """
 
     def __init__(self, id_or_device):
         _type, id = None, None
         if isinstance(id_or_device, int):
             id = id_or_device
         elif id_or_device == "cpu":
             _type, id = id_or_device, -1
+        elif id_or_device == "cuda":
+            _type, id = id_or_device, 0
         elif isinstance(id_or_device, Device):
             _type, id = id_or_device.type, id_or_device.id
         elif env.cupy_available() and isinstance(id_or_device, cp.cuda.Device):
             _type, id = "cuda", id_or_device.id
         elif env.sigpy_available() and isinstance(id_or_device, sp.Device):
             id = id_or_device.id
         elif env.torch_available() and isinstance(id_or_device, torch.device):
```

### Comparing `pyvoxel-0.0.1a1/voxel/io/__init__.py` & `pyvoxel-0.0.2/voxel/io/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Utilities for medical image I/O."""
 import os
 from pathlib import Path
 from typing import List, Union
 
-from voxel.io import dicom, nifti  # noqa: F401
+from voxel.device import Device
+from voxel.io import dicom, http, nifti  # noqa: F401
 from voxel.io.dicom import *  # noqa
 from voxel.io.dicom import DicomReader, DicomWriter
 from voxel.io.format_io import ImageDataFormat  # noqa
 from voxel.io.format_io import DataReader, DataWriter
+from voxel.io.http import *  # noqa
+from voxel.io.http import HttpReader
 from voxel.io.nifti import *  # noqa
 from voxel.io.nifti import NiftiReader, NiftiWriter
 from voxel.med_volume import MedicalVolume
 
 __all__ = [
     "read",
     "write",
@@ -20,14 +23,15 @@
     "get_reader",
     "get_writer",
     "get_filepath_variations",
     "convert_image_data_format",
     "generic_load",
 ]
 __all__.extend(dicom.__all__)
+__all__.extend(http.__all__)
 __all__.extend(["ImageDataFormat"])
 __all__.extend(nifti.__all__)
 
 
 _READERS = {ImageDataFormat.dicom: DicomReader, ImageDataFormat.nifti: NiftiReader}
 _WRITERS = {ImageDataFormat.dicom: DicomWriter, ImageDataFormat.nifti: NiftiWriter}
 
@@ -166,45 +170,50 @@
 
     return vols
 
 
 def read(
     path: Union[str, Path, os.PathLike],
     data_format: ImageDataFormat = None,
-    unpack: bool = False,
+    device: Union[Device, str, int] = "cpu",
     **kwargs
 ) -> Union[MedicalVolume, List[MedicalVolume]]:
     """Read MedicalVolume(s) from file.
 
     Args:
         path (str): File/directory path.
         data_format (ImageDataFormat, optional): Data format
             (e.g. ``'dicom'``, ``'nifti'``, etc.). Use this is disambiguate between different
             data formats. If this function is not working, try using this argument.
             If not provided, voxel will try to infer data format from file extension.
-        unpack (bool, optional): If ``True`` and only 1 volume is loaded, return a single
-            volume instead of a list of volumes. This only applied to dicom loading.
         **kwargs: Additional keyword arguments passed to the data format reader.
 
     Returns:
         MedicalVolume | List[MedicalVolume]: Volume(s) loaded.
 
     Examples:
-        >>> vx.read("/path/to/multi-echo/dicom/folder", group_by="EchoNumbers")
-        >>> vx.read("/path/to/ct/dicom/folder")
-        >>> vx.read("/path/to/ct/nifti/file.nii.gz", mmap=True)
-    """
+        >>> vx.load("/path/to/multi-echo/dicom/folder", group_by="EchoNumbers")
+        >>> vx.load("/path/to/ct/dicom/folder")
+        >>> vx.load("/path/to/ct/nifti/file.nii.gz", mmap=True)
+    """
+    if path.startswith("http://") or path.startswith("https://"):
+        with HttpReader() as hr:
+            out = hr.load(path, data_format=data_format, **kwargs)
+            return out
+
     if data_format is None:
         data_format = ImageDataFormat.get_image_data_format(path)
     elif isinstance(data_format, str):
         data_format = ImageDataFormat[data_format]
 
     out = get_reader(data_format).load(path, **kwargs)
-    if unpack and isinstance(out, (tuple, list)) and len(out) == 1:
-        out = out[0]
+    if isinstance(out, (list, tuple)):
+        out = type(out)(v.to(device) for v in out)
+    else:
+        out = out.to(device)
     return out
 
 
 def write(
     vol: MedicalVolume,
     path: Union[str, Path, os.PathLike],
     data_format: ImageDataFormat = None,
```

### Comparing `pyvoxel-0.0.1a1/voxel/io/dicom.py` & `pyvoxel-0.0.2/voxel/io/dicom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-"""
-DICOM I/O.
+"""DICOM I/O.
 
 This module contains DICOM input/output helpers.
 
 Note:
 
     1. Dicom utilizes LPS convention:
         - LPS: right --> left, anterior --> posterior, inferior --> superior
         - we will call it LPS+, such that letters correspond to increasing end of axis
-
-Attributes:
-    TOTAL_NUM_ECHOS_KEY (tuple[int]): Hexadecimal encoding of DICOM tag corresponding
-        to number of echos.
 """
 
 import copy
 import functools
 import itertools
 import multiprocessing as mp
 import os
 import re
 from math import ceil, log10
-from typing import Collection, List, Sequence, Tuple, Union
+from typing import Any, Collection, Dict, List, Sequence, Tuple, Union
 
 import nibabel as nib
 import numpy as np
 import pydicom
 from natsort import index_natsorted, natsorted
 from tqdm.auto import tqdm
 from tqdm.contrib.concurrent import process_map
 
-import voxel as vx
 from voxel import orientation as stdo
 from voxel.io.format_io import DataReader, DataWriter, ImageDataFormat
 from voxel.med_volume import MedicalVolume
 
 __all__ = ["DicomReader", "DicomWriter"]
 
-TOTAL_NUM_ECHOS_KEY = (0x19, 0x107E)
 PATH_LIKE = (str, os.PathLike)
 
 
 class DicomReader(DataReader):
     """A class for reading DICOM files.
 
     Attributes:
@@ -76,15 +69,15 @@
 
     data_format_code = ImageDataFormat.dicom
 
     def __init__(
         self,
         num_workers: int = 0,
         verbose: bool = False,
-        group_by: Union[str, int, Sequence[Union[str, int]]] = "EchoNumbers",
+        group_by: Union[str, int, Sequence[Union[str, int]]] = None,
         sort_by: Union[str, int, Sequence[Union[str, int]]] = None,
         ignore_ext: bool = False,
         default_ornt: Tuple[str, str] = None,
     ):
         """
         Args:
             num_workers (int, optional): Number of workers to use for loading.
@@ -146,29 +139,29 @@
         exclude = _wrap_as_tuple(exclude, default=())
         assert isinstance(include, tuple)
         assert isinstance(exclude, tuple)
         if ignore_hidden:
             exclude += ("^\.",)  # noqa: W605
 
         possible_files = os.listdir(path)
-        lstFilesDCM = []
+        lst_files_dicom = []
         for f in possible_files:
             # If ignore extension, don't look for '.dcm' extension.
             is_file = os.path.isfile(os.path.join(path, f))
             match_ext = ignore_ext or self.data_format_code.is_filetype(f)
             if (
                 is_file
                 and match_ext
                 and (not include or any(re.match(x, f) for x in include))
                 and (not exclude or all(not re.match(x, f) for x in exclude))
             ):
-                lstFilesDCM.append(os.path.join(path, f))
+                lst_files_dicom.append(os.path.join(path, f))
 
-        lstFilesDCM = natsorted(lstFilesDCM)
-        return lstFilesDCM
+        lst_files_dicom = natsorted(lst_files_dicom)
+        return lst_files_dicom
 
     def _handle_files(self, path, ignore_ext):
         """Gets and organize pydicom data from file(s) or directory.
 
         Args:
             path (str | path-like): The file path(s) or directory path to
                 load from.
@@ -176,32 +169,32 @@
                 when loading dicoms from directory.
 
         Returns:
             Sequence[path-like]: The filepaths for different slices.
         """
         if isinstance(path, str) or not isinstance(path, Sequence):
             if os.path.isdir(path):
-                lstFilesDCM = self.get_files(path, ignore_hidden=True, ignore_ext=ignore_ext)
+                lst_files_dicom = self.get_files(path, ignore_hidden=True, ignore_ext=ignore_ext)
             elif os.path.isfile(path):
-                lstFilesDCM = [path]
+                lst_files_dicom = [path]
             else:
                 raise IOError(f"No directory or file found - {path}")
         else:
             not_files = [x for x in path if not os.path.isfile(x)]
             if len(not_files) > 0:
                 raise IOError(
                     "Files not found:\n{}".format("".join("\t{}\n".format(x) for x in not_files))
                 )
-            lstFilesDCM = path
+            lst_files_dicom = path
 
-        lstFilesDCM = natsorted(lstFilesDCM)
-        if len(lstFilesDCM) == 0:
+        lst_files_dicom = natsorted(lst_files_dicom)
+        if len(lst_files_dicom) == 0:
             raise FileNotFoundError("No valid dicom files found in {}".format(path))
 
-        return lstFilesDCM
+        return lst_files_dicom
 
     def load(
         self,
         path_or_bytes: Union[str, os.PathLike, bytes, Sequence[Union[str, os.PathLike, bytes]]],
         group_by: Union[str, int, Sequence[Union[str, int]]] = np._NoValue,
         sort_by: Union[str, int, Sequence[Union[str, int]]] = np._NoValue,
         ignore_ext: bool = np._NoValue,
@@ -226,15 +219,16 @@
                 when loading dicoms from directory. Defaults to ``self.ignore_ext``.
             default_ornt (Tuple[str, str], optional): Default in-plane orientation to use if
                 orientation cannot be determined from DICOM header. If not specified
                 and orientation cannot be determined, error will be raised.
                 Defaults to ``self.default_ornt``.
 
         Returns:
-            list[MedicalVolume]: Different volumes grouped by the `group_by` DICOM tag.
+            Union[List[MedicalVolume], MedicalVolume]: Different volumes grouped by the
+                `group_by` DICOM tag or a single volume if ``group_by`` is ``None``.
 
         Raises:
             ValueError: If `group_by` not specified or if single dicom file specified.
             IOError: If directory or dicom file(s) specified by `path` do not exist.
             FileNotFoundError: If no valid dicom files found.
 
         Note:
@@ -249,40 +243,40 @@
 
         group_by = _wrap_as_tuple(group_by, default=())
         sort_by = _wrap_as_tuple(sort_by, default=())
 
         if isinstance(path_or_bytes, PATH_LIKE) or (
             isinstance(path_or_bytes, Sequence) and isinstance(path_or_bytes[0], PATH_LIKE)
         ):
-            lstFilesDCM = self._handle_files(path_or_bytes, ignore_ext)
+            lst_files_dicom = self._handle_files(path_or_bytes, ignore_ext)
         else:
             # We explicitly specify list/tuple because other objects can be sequences
             # (e.g. bytes) that we cannot thoroughly account for.
-            lstFilesDCM = (
+            lst_files_dicom = (
                 [path_or_bytes] if not isinstance(path_or_bytes, (list, tuple)) else path_or_bytes
             )
 
         if self.num_workers:
             fn = functools.partial(pydicom.read_file, force=True)
             if self.verbose:
-                dicom_slices = process_map(fn, lstFilesDCM, max_workers=self.num_workers)
+                dicom_slices = process_map(fn, lst_files_dicom, max_workers=self.num_workers)
             else:
                 with mp.Pool(self.num_workers) as p:
-                    dicom_slices = p.map(fn, lstFilesDCM)
+                    dicom_slices = p.map(fn, lst_files_dicom)
         else:
             dicom_slices = [
                 pydicom.read_file(fp, force=True)
-                for fp in tqdm(lstFilesDCM, disable=not self.verbose)
+                for fp in tqdm(lst_files_dicom, disable=not self.verbose)
             ]
 
         # Check if dicom file has the group_by element specified
         temp_dicom = dicom_slices[0]
         for _group in group_by:
             if _group not in temp_dicom:
-                raise KeyError("Tag {} does not exist in dicom".format(_group))
+                raise KeyError(f"Tag {_group} does not exist in dicom")
 
         if sort_by:
             try:
                 dicom_slices = natsorted(
                     dicom_slices,
                     key=lambda x: tuple(
                         _unpack_dicom_attr(x, attr, required=True) for attr in sort_by
@@ -290,34 +284,35 @@
                 )
             except KeyError as e:
                 raise KeyError(f"Tag not found in dicom - {e}")
 
         dicom_data = {}
         for ds in dicom_slices:
             val_groupby = tuple(_unpack_dicom_attr(ds, attr, required=True) for attr in group_by)
+
             if val_groupby not in dicom_data.keys():
                 dicom_data[val_groupby] = {"headers": [], "arr": []}
 
             dicom_data[val_groupby]["headers"].append(ds)
             dicom_data[val_groupby]["arr"].append(ds.pixel_array)
 
         vols = []
         for k in sorted(dicom_data.keys()):
             dd = dicom_data[k]
             headers = dd["headers"]
             if len(headers) == 0:
                 continue
             arr = np.stack(dd["arr"], axis=-1)
 
-            affine = to_RAS_affine(headers, default_ornt=default_ornt)
+            affine = stdo.to_RAS_affine(headers, default_ornt=default_ornt)
 
             vol = MedicalVolume(arr, affine, headers=headers)
             vols.append(vol)
 
-        return vols
+        return vols if len(group_by) > 0 else vols[0]
 
     def __serializable_variables__(self) -> Collection[str]:
         return self.__dict__.keys()
 
     read = load  # pragma: no cover
 
 
@@ -488,154 +483,41 @@
 
     def __serializable_variables__(self) -> Collection[str]:
         return self.__dict__.keys()
 
     write = save  # pragma: no cover
 
 
-def to_RAS_affine(headers: List[pydicom.FileDataset], default_ornt: Tuple[str, str] = None):
-    """Convert from LPS+ orientation (default for DICOM) to RAS+ standardized orientation.
-
-    Args:
-        headers (list[pydicom.FileDataset]): Headers for DICOM files to reorient.
-            Files should correspond to single volume.
-
-    Returns:
-        np.ndarray: Affine matrix.
-    """
-    try:
-        im_dir = headers[0].ImageOrientationPatient
-    except AttributeError:
-        im_dir = _decode_inplane_direction(headers, default_ornt=default_ornt)
-        if im_dir is None:
-            raise RuntimeError("Could not determine in-plane directions from headers.")
-    try:
-        in_plane_pixel_spacing = headers[0].PixelSpacing
-    except AttributeError:
-        try:
-            in_plane_pixel_spacing = headers[0].ImagerPixelSpacing
-        except AttributeError:
-            raise RuntimeError(
-                "Could not determine in-plane pixel spacing from headers. "
-                "Neither attribute 'PixelSpacing' nor 'ImagerPixelSpacing' found."
-            )
-
-    orientation = np.zeros([3, 3])
-
-    # Determine vector for in-plane pixel directions (i, j).
-    i_vec, j_vec = (
-        np.asarray(im_dir[:3]).astype(np.float64),
-        np.asarray(im_dir[3:]).astype(np.float64),
-    )  # unique to pydicom, please revise if using different library to load dicoms
-    i_vec, j_vec = (
-        np.round(i_vec, vx.config.affine_precision),
-        np.round(j_vec, vx.config.affine_precision),
-    )
-    i_vec = i_vec * in_plane_pixel_spacing[0]
-    j_vec = j_vec * in_plane_pixel_spacing[1]
-
-    # Determine vector for through-plane pixel direction (k).
-    # Compute difference in patient position between consecutive headers.
-    # This is the preferred method to determine the k vector.
-    # If single header, take cross product between i/j vectors.
-    # These actions are done to avoid rounding errors that might result from float subtraction.
-    if len(headers) > 1:
-        k_vec = np.asarray(headers[1].ImagePositionPatient).astype(np.float64) - np.asarray(
-            headers[0].ImagePositionPatient
-        ).astype(np.float64)
-    else:
-        slice_thickness = headers[0].get("SliceThickness", 1.0)
-        i_norm = 1 / np.linalg.norm(i_vec) * i_vec
-        j_norm = 1 / np.linalg.norm(j_vec) * j_vec
-        k_norm = np.cross(i_norm, j_norm)
-        k_vec = k_norm / np.linalg.norm(k_norm) * slice_thickness
-        if hasattr(headers[0], "SpacingBetweenSlices") and headers[0].SpacingBetweenSlices < 0:
-            k_vec *= -1
-    k_vec = np.round(k_vec, vx.config.affine_precision)
-
-    orientation[:3, :3] = np.stack([j_vec, i_vec, k_vec], axis=1)
-    scanner_origin = headers[0].get("ImagePositionPatient", np.zeros((3,)))
-    scanner_origin = np.asarray(scanner_origin).astype(np.float64)
-    scanner_origin = np.round(scanner_origin, vx.config.affine_precision)
-
-    affine = np.zeros([4, 4])
-    affine[:3, :3] = orientation
-    affine[:3, 3] = scanner_origin
-    affine[:2, :] = -1 * affine[:2, :]
-    affine[3, 3] = 1
-
-    affine[affine == 0] = 0
-
-    return affine
-
-
-def _decode_inplane_direction(headers: Sequence[pydicom.FileDataset], default_ornt=None):
-    """Helper function to decode in-plane direction from header(s).
-
-    Recall the direction in dicoms are in cartesian order ``(x,y)``,
-    but numpy/voxel are in matrix order ``(y,x)``. When adding new
-    methods, make sure to account for this.
-
-    Returns:
-        np.ndarray: 6-element LPS direction array where first 3 elements define
-            direction for x-direction (columns) and second 3 elements define
-            direction for y-direction (rows)
-    """
-    _patient_ornt_to_nib = {"H": "S", "F": "I"}
-
-    if (
-        len(headers) == 1
-        and hasattr(headers[0], "PatientOrientation")
-        and headers[0].PatientOrientation
-    ):
-        # Decoder: patient orientation.
-        # Patient orientation is only decoded along principal direction (e.g. "FR" -> "F").
-        ornt = [
-            _patient_ornt_to_nib.get(k[:1], k[:1]) for k in headers[0].PatientOrientation
-        ]  # (x,y)
-        ornt = stdo.orientation_nib_to_standard(ornt)
-        affine = stdo.to_affine(ornt)
-        affine[:2, :] = -1 * affine[:2, :]
-        return np.concatenate([affine[:3, 0], affine[:3, 1]], axis=0)
-
-    if default_ornt:
-        affine = stdo.to_affine(default_ornt)
-        affine[:2, :] = -1 * affine[:2, :]
-        return np.concatenate([affine[:3, 0], affine[:3, 1]], axis=0)
-
-    return None
-
-
-def _format_volume_to_header(volume: MedicalVolume) -> MedicalVolume:
+def _format_volume_to_header(mv: MedicalVolume) -> MedicalVolume:
     """Reformats the volume according to its header.
 
     Args:
         volume (MedicalVolume): The volume to reformat.
             Must be 3D and have headers of shape (1, 1, volume.shape[2]).
 
     Returns:
         MedicalVolume: The reformatted volume.
     """
-    headers = volume.headers()
-    assert headers.shape == (1, 1, volume.shape[2])
+    headers = mv.headers()
+    assert headers.shape == (1, 1, mv.shape[2])
 
-    affine = to_RAS_affine(headers.flatten())
+    affine = stdo.to_RAS_affine(headers.flatten())
     orientation = stdo.orientation_nib_to_standard(nib.aff2axcodes(affine))
 
     # Currently do not support mismatch in scanner_origin.
-    if tuple(affine[:3, 3]) != volume.scanner_origin:
+    if tuple(affine[:3, 3]) != mv.scanner_origin:
         raise ValueError(
             "Scanner origin mismatch. "
             "Currently we do not handle mismatch in scanner origin "
             "(i.e. cannot flip across axis)"
         )
 
-    volume = volume.reformat(orientation)
-    assert volume.headers().shape == (1, 1, volume.shape[2])
-    return volume
+    mv = mv.reformat(orientation)
+    assert mv.headers().shape == (1, 1, mv.shape[2])
+    return mv
 
 
 def _write_dicom_file(np_slice: np.ndarray, header: pydicom.FileDataset, file_path: str):
     """Replace data in header with 2D numpy array and write to `file_path`.
 
     Args:
         np_slice (np.ndarray): 2D slice to encode in dicom file.
@@ -740,7 +622,189 @@
         return default
 
     if isinstance(x, str) or not isinstance(x, Sequence):
         x = (x,)
     elif isinstance(x, Sequence) and not isinstance(x, tuple):
         x = tuple(x)
     return x
+
+
+def add_dicom_headers(
+    mv: MedicalVolume,
+    *,
+    modality: str,
+    **metadata,
+) -> MedicalVolume:
+    """Add metadata and required DICOM tags to the MedicalVolume.
+
+    TODO:
+        - Add support for non-int16 dtypes
+        - Add support for multi-dimensional headers.
+
+    Args:
+        mv: The medical volume to add DICOM headers to.
+        modality: The modality of the DICOM file (e.g. "MR").
+        high_bit: The high bit of the recon.
+        series_uid: The series unique id.
+        study_uid: The study unique id.
+        series_number: The series number.
+        metadata: Additional metadata to add to the DICOM headers.
+
+    Returns:
+        MedicalVolume: The medical volume with DICOM headers added.
+    """
+    # Convert inputs xval_yval to XvalYval following pydicom syntax.
+    def _split_and_capitalize(x):
+        return "".join([s.capitalize() for s in x.split("_")])
+
+    metadata = {_split_and_capitalize(k) if "_" in k else k: v for k, v in metadata.items()}
+
+    min_val = np.min(mv.A)
+    max_val = np.max(mv.A)
+    window_center = (min_val + max_val) / 2
+    window_width = max_val - min_val
+
+    dtype = mv.dtype
+    dtype = getattr(np, dtype.name)
+    nbits = dtype(0).nbytes * 8
+    high_bit = metadata.get("HighBit", None)
+    if high_bit is not None and high_bit > nbits:
+        raise ValueError(f"high_bit cannot be greater than {nbits}")
+    if high_bit is None:
+        # TODO: Change this to be based on the dynamic range of the data.
+        # This should also handle data with negative values.
+        metadata["HighBit"] = nbits
+
+    metadata = dict(metadata)
+    default_metadata = {
+        # Series Information.
+        "SeriesInstanceUID": str(pydicom.uid.generate_uid()),
+        "StudyInstanceUID": str(pydicom.uid.generate_uid()),
+        "SeriesNumber": 1,
+        "ImageType": ["DERIVED", "PRIMARY", "OTHER"],
+        "StudyDate": "00010101",
+        "SeriesDate": "00010101",
+        "AcquisitionDate": "00010101",
+        "ContentDate": "00010101",
+        "StudyTime": "000000",
+        "SeriesTime": "000000",
+        "AcquisitionTime": "000000",
+        "ContentTime": "000000",
+        "AccessionNumber": "",
+        "Modality": modality,
+        "InstitutionName": "Anonymized",
+        "ReferringPhysicianName": "",
+        "StationName": "Anonymized",
+        # Patient Information.
+        "PatientName": "Anonymized",
+        "PatientID": "Anonymized",
+        "PatientBirthDate": "00010101",
+        "PatientSex": "",
+        # Image Information.
+        "Rows": mv.shape[0],
+        "Columns": mv.shape[1],
+        "PixelRepresentation": 1,
+        "SamplesPerPixel": 1,
+        "PhotometricInterpretation": "MONOCHROME2",
+        "BitsAllocated": nbits,
+        "BitsStored": nbits,
+        "SmallestImagePixelValue": int(min_val.round()),
+        "LargestImagePixelValue": int(max_val.round()),
+        "WindowCenter": float(window_center.round()),
+        "WindowWidth": float(window_width.round()),
+    }
+    default_metadata.update(metadata)
+
+    # Update headers for each slice.
+    shared_uid = pydicom.uid.generate_uid()
+
+    def _generate_file_meta(sl: int):
+        """Generates a little endian formatted file meta info."""
+        file_meta = pydicom.dataset.FileMetaDataset()
+        file_meta.MediaStorageSOPClassUID = pydicom.uid.UID("1.2.840.10008.5.1.4.1.1.4")
+        file_meta.MediaStorageSOPInstanceUID = pydicom.uid.UID(f"{shared_uid}.{sl+1}")
+        file_meta.ImplementationClassUID = pydicom.uid.UID("1.2.840.113619.6.374")
+        file_meta.TransferSyntaxUID = pydicom.uid.ExplicitVRLittleEndian
+        # file_meta.SOPInstanceUID = pydicom.uid.generate_uid()
+        # file_meta.MediaStorageSOPInstanceUID = pydicom.uid.generate_uid()
+        return file_meta
+
+    VR_registry = {float: "DS", int: "IS", str: "CS"}
+    sl_header_metadata = _get_per_slice_metadata(mv.affine, mv.shape[2])
+    headers = [
+        pydicom.FileDataset("./file", {}, file_meta=_generate_file_meta(sl), preamble=b"\0" * 128)
+        for sl in range(mv.shape[2])
+    ]
+    for i, header in enumerate(headers):
+        metadata = {**default_metadata, **sl_header_metadata[i]}
+        for k, v in metadata.items():
+            try:
+                dtype = type(v[0]) if isinstance(v, (list, tuple)) else type(v)
+                header.add_new(k, VR_registry[dtype], v)
+            except Exception as e:
+                print(f"Failed to set {k} to {v}: {e}")
+                raise e
+
+        header.is_little_endian = True
+        header.is_implicit_VR = False
+
+    mv = mv._partial_clone(volume=mv.A, headers=headers)
+
+    return mv
+
+
+def _get_per_slice_metadata(affine, num_slices: int) -> List[Dict[str, Any]]:
+    """Convert affine matrix into dicom metadata for each slice.
+
+    Args:
+        affine (ndarray): The 4x4 RAS+ affine matrix.
+            This is the default affine matrix in DOSMA
+            (i.e. MedicalVolume.affine).
+        num_slices (int): The number of slices in the volume.
+            This should be equal to the number of slices in the last dimension
+            of the volume.
+
+    Returns:
+        List[Dict[str, Any]]: The metadata for each slice.
+    """
+    dim = 2
+
+    # DICOM is in the LPS orientation.
+    # Convert RAS+ affine matrix -> LPS affine matrix.
+    lps_affine = affine.copy()
+    lps_affine[:2, :] = -1 * lps_affine[:2, :]
+
+    image_orientation_patient = np.concatenate([lps_affine[:3, 1], lps_affine[:3, 0]])
+    slice_thickness = float(np.linalg.norm(lps_affine[:3, dim]).round(4))
+    metadata = {
+        "SliceThickness": slice_thickness,
+        "SpacingBetweenSlices": slice_thickness,  # spacing is the same as the slice thickness
+        "PixelSpacing": (
+            np.linalg.norm(lps_affine[:3, 1]),
+            np.linalg.norm(lps_affine[:3, 1]),
+        ),
+        "ImageOrientationPatient": image_orientation_patient.round(4),
+    }
+    metadatas = []
+    for sl in range(num_slices):
+        relative_image_position = lps_affine[:3, :3] @ np.asarray([0, 0, sl]).T
+        image_position_patient = relative_image_position + lps_affine[:3, 3]
+        metadatas.append(
+            {
+                **metadata,
+                "PatientPosition": "FFS",
+                "ImagePositionPatient": image_position_patient.round(4),
+                "SliceLocation": slice_thickness * sl,
+                # "InStackPositionNumber": sl + 1,
+                "InstanceNumber": sl + 1,
+            }
+        )
+
+        md = metadatas[-1]
+        for k, v in md.items():
+            if isinstance(v, np.ndarray):
+                v = v.flatten()
+            if isinstance(v, (np.ndarray, list, tuple)):
+                dtype = int if v[0].dtype in (np.int, np.int16, np.int32, np.int64) else float
+                md[k] = [dtype(x) for x in v]
+
+    return metadatas
```

### Comparing `pyvoxel-0.0.1a1/voxel/io/format_io.py` & `pyvoxel-0.0.2/voxel/io/format_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __all__ = ["ImageDataFormat", "DataReader", "DataWriter"]
 
 
 class ImageDataFormat(enum.Enum):
     """Enum describing supported data formats for medical volume I/O."""
 
     nifti = 1, ("nii", "nii.gz")
-    dicom = 2, ("dcm", "ima")
+    dicom = 2, ("dcm", "ima", "dicom", "dic")
 
     def __new__(cls, key_code, extensions):
         """
         Args:
             key_code (int): Enum value.
             extensions (tuple[str]): Extensions supported by format.
         """
@@ -66,15 +66,15 @@
 
         # if no extension found, assume the name corresponds to a directory
         # and assume that format is dicom.
         # We cannot check if the path is a directory path because it may not
         # have been created yet.
         file_or_dir_path = str(file_or_dir_path)
         filename_base, ext = os.path.splitext(file_or_dir_path)
-        if filename_base == file_or_dir_path:
+        if filename_base == file_or_dir_path or os.path.isdir(file_or_dir_path):
             return ImageDataFormat.dicom
 
         raise ValueError(f"Unknown data format for {file_or_dir_path}")
 
 
 class _StateMixin(ABC):
     """Temporary mixin that supports fetching and loading from state dictionaries.
```

### Comparing `pyvoxel-0.0.1a1/voxel/med_volume.py` & `pyvoxel-0.0.2/voxel/med_volume.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 
 import nibabel as nib
 import numpy as np
 import pydicom
 from nibabel.spatialimages import SpatialFirstSlicer as _SpatialFirstSlicerNib
 from numpy.lib.mixins import NDArrayOperatorsMixin
 from packaging import version
+from pydicom import Dataset
 
 import voxel as vx
 import voxel.orientation as stdo
 from voxel.device import Device, cpu_device, get_array_module, get_device, to_device
 from voxel.utils import env
+from voxel.utils.pixel_data import apply_rescale, apply_window, invert, invert_window
 
 if env.sitk_available():
     import SimpleITK as sitk
 if env.cupy_available():
     import cupy as cp
 if env.package_available("h5py"):
     import h5py
 
 if TYPE_CHECKING:
     from voxel.io.format_io import ImageDataFormat
 
+
 __all__ = ["MedicalVolume"]
 
 
 # PyTorch version introducing complex tensor support.
 _TORCH_COMPLEX_SUPPORT_VERSION = version.Version("1.5.0")
 
 
@@ -116,26 +119,26 @@
     >>> log_arr = np.log(mv)
     >>> type(log_arr)
     <class 'voxel.MedicalVolume'>
     >>> exp_arr_gpu = cp.exp(mv_gpu)
     >>> type(exp_arr_gpu)
     <class 'voxel.MedicalVolume'>
 
-    **ALPHA**: MedicalVolumes are also interoperable with popular image data structures
+    MedicalVolumes are also interoperable with popular image data structures
     with zero-copy, meaning array data will not be copied. Formats currently include the
     SimpleITK Image, Nibabel Nifti1Image, and PyTorch tensors:
 
     >>> sitk_img = mv.to_sitk()  # Convert to SimpleITK Image
     >>> mv_from_sitk = MedicalVolume.from_sitk(sitk_img)  # Convert back to MedicalVolume
     >>> nib_img = mv.to_nib()  # Convert to nibabel Nifti1Image
     >>> mv_from_nib = MedicalVolume.from_nib(nib_img)
     >>> torch_tensor = mv.to_torch()  # Convert to torch tensor
     >>> mv_from_tensor = MedicalVolume.from_torch(torch_tensor, affine)
 
-    **ALPHA**: MedicalVolumes can also be used with memmapped arrays.
+    MedicalVolumes can also be used with memmapped arrays.
     This makes loading much faster and allows interaction with larger-than-memory
     arrays. Only when the volume is modified will the volume be loaded
     into memory and modified. If you take a slice of the memmaped array, the underlying
     array will also remain memmapped:
 
     >>> arr = np.load("/path/to/volume.npy", mmap_mode="r")
     >>> mv = MedicalVolume(arr, np.eye(4))
@@ -176,15 +179,15 @@
             raise RuntimeError(f"MedicalVolume must be on cpu, got {self.device}")
         if data_format is None:
             data_format = vx.config.save_format
 
         writer = vio.get_writer(data_format)
         writer.save(self, file_path)
 
-    def reformat(self, new_orientation: Sequence, inplace: bool = False) -> "MedicalVolume":
+    def reformat(self, new_orientation: Sequence, *args, inplace: bool = False) -> "MedicalVolume":
         """Reorients volume to a specified orientation.
 
         Flipping and transposing the volume array (``self.volume``) returns a view if possible.
 
         Reorientation method:
         ---------------------
         - Axis transpose and flipping are linear operations and therefore can be treated
@@ -210,14 +213,22 @@
         Returns:
             MedicalVolume: The reformatted volume. If ``inplace=True``, returns ``self``.
         """
         xp = self.device.xp
         device = self.device
         headers = self._headers
 
+        if len(args):
+            if any(isinstance(x, bool) for x in args):
+                raise ValueError(
+                    "`inplace` is a keyword only argument. Use `inplace=` to specify "
+                    "if the operation should be in-place."
+                )
+            new_orientation = (new_orientation, *args)
+
         new_orientation = tuple(new_orientation)
         if new_orientation == self.orientation:
             if inplace:
                 return self
             return self._partial_clone(volume=self._volume)
 
         temp_orientation = self.orientation
@@ -277,16 +288,16 @@
 
         assert (
             mv.orientation == new_orientation
         ), f"Orientation mismatch: Expected: {self.orientation}. Got {new_orientation}"
         return mv
 
     def reformat_as(self, other, inplace: bool = False) -> "MedicalVolume":
-        """Reformat this to the same orientation as ``other``.
-        Equivalent to ``self.reformat(other.orientation, inplace)``.
+        """Reformat this to the same orientation as ``other``. Equivalent to
+        ``self.reformat(other.orientation, inplace)``.
 
         Args:
             other (MedicalVolume): The result volume has the same orientation as ``other``.
             inplace (bool, optional): If `True`, do operation in-place and return ``self``.
 
         Returns:
             MedicalVolume: The reformatted volume. If ``inplace=True``, returns ``self``.
@@ -639,14 +650,72 @@
             tensor = from_dlpack(array.toDlpack())
 
         tensor.requires_grad = requires_grad
         if contiguous:
             tensor = tensor.contiguous()
         return tensor
 
+    def to_zarr(
+        self,
+        affine_attr: str = None,
+        headers_attr: str = None,
+        read_only: bool = True,
+        **kwargs,
+    ):
+        """Converts a `MedicalVolume` to a Zarr array/store.
+
+        Zarr stores can be used to store and access data on disk or in memory. The `store` argument
+        can be set to persist the data to disk. See `zarr.open_array` for more information. The
+        `affine` and `headers` attributes of `MedicalVolume` are stored as Zarr attributes. To do
+        so, the DICOM headers are serialized to DICOM+JSON format.
+
+        The default `mode` is set to `w-` to prevent overwriting existing data. If you want to
+        overwrite existing data, set `mode` to `w`.
+
+        Args:
+            affine_attr (str, optional): Attribute key of the Zarr Array where the affine matrix
+                will be stored in. If `None`, the affine matrix will not be saved.
+            headers_attr (str, optional): Attribute key of the Zarr Array where the headers of the
+                `MedicalVolume` will be stored in. If `None`, headers will not be saved.
+            read_only (bool, optional): If `True`, the returned Zarr store will be read-only.
+            **kwargs: Additional parameters passed to `zarr.creation.open_array`.
+        Returns:
+            zarr.Array
+        Examples:
+            >>> mv = vx.load("path/to/dicoms")
+            >>> store = zarr.DirectoryStore("/path/to/store")
+            >>> mv.to_zarr(store=store)
+
+            >>> # Save headers to zarr attributes
+            >>> mv.to_zarr(store=store, headers_attr="headers")
+
+            >>> # Load with headers
+            >>> MedicalVolume.from_zarr(store, headers_attr="headers")
+        """
+
+        if not env.package_available("zarr"):
+            raise ImportError(  # pragma: no cover
+                "zarr is not installed. Install it with `pip install zarr`. "
+            )
+
+        import zarr
+
+        arr = zarr.open_array(**{"mode": "w-", **kwargs, "shape": self.shape, "dtype": self.dtype})
+        arr[:] = self._volume
+
+        if affine_attr is not None:
+            arr.attrs[affine_attr] = self.affine.tolist()
+
+        if headers_attr is not None:
+            json_headers = [h.to_json_dict() for h in self._headers.flatten().tolist()]
+            arr.attrs[headers_attr] = json_headers
+
+        arr.read_only = read_only
+        return arr
+
     def headers(self, flatten=False):
         """Returns headers.
 
         If headers exist, they are currently stored as an array of
         pydicom dataset headers, though this is subject to change.
 
         Args:
@@ -656,15 +725,15 @@
         Returns:
             Optional[ndarray[pydicom.dataset.FileDataset]]: Array of headers (if they exist).
         """
         if flatten and self._headers is not None:
             return self._headers.flatten()
         return self._headers
 
-    def get_metadata(self, key, dtype=None, default=np._NoValue):
+    def get_metadata(self, key, index: int = None, dtype=None, default=np._NoValue):
         """Get metadata value from first header.
 
         The first header is defined as the first header in ``np.flatten(self._headers)``.
         To extract header information for other headers, use ``self.headers()``.
 
         Args:
             key (``str`` or pydicom.BaseTag``): Metadata field to access.
@@ -695,17 +764,22 @@
             raise RuntimeError("No headers found. MedicalVolume must be initialized with `headers`")
         headers = self.headers(flatten=True)
 
         if key not in headers[0] and default != np._NoValue:
             return default
         else:
             element = headers[0][key]
+
         val = element.value
+        if isinstance(val, list) and index is not None:
+            val = val[index]
+
         if dtype is not None:
             val = dtype(val)
+
         return val
 
     def set_metadata(self, key, value, force: bool = False):
         """Sets metadata for all headers.
 
         Args:
             key (str or pydicom.BaseTag): Metadata field to access.
@@ -733,16 +807,207 @@
                 try:
                     setattr(h, key, value)
                 except TypeError:
                     h.add_new(key, VR_registry[type(value)], value)
             else:
                 h[key].value = value
 
+    def apply_rescale(
+        self,
+        slope: float = None,
+        intercept: float = None,
+        dtype: np.dtype = None,
+        inplace: bool = False,
+        sync: bool = True,
+    ) -> "MedicalVolume":
+        """Rescales the volume by applying the intercept and slope.
+
+        Args:
+            intercept (float, optional): Rescale intercept. If ``None``, will
+                use the value in the header.
+            slope (float, optional): Rescale slope. If ``None``, will
+                use the value in the header.
+            dtype (np.dtype, optional): Data type to cast volume to before
+                rescale is applied.
+            inplace (bool, optional): If ``True``, rescales the volume in place.
+            sync (bool, optional): If ``True``, updates the headers.
+
+        Returns:
+            MedicalVolume: Volume with rescale applied.
+        """
+        if self._headers is None and (intercept is None or slope is None):
+            return self
+
+        mv = self if inplace else self.clone()
+        mv = mv.astype(np.dtype(dtype), copy=False)
+
+        h: pydicom.Dataset = self._headers.flat[0]
+        rs = float(h.get("RescaleSlope", 1)) if slope is None else slope
+        ri = float(h.get("RescaleIntercept", 0)) if intercept is None else intercept
+        apply_rescale(mv._volume, rs, ri, inplace=True)
+
+        if sync:
+            mv._delete_metadata("RescaleSlope")
+            mv._delete_metadata("RescaleIntercept")
+
+        return mv
+
+    def apply_modality_lut(self, inplace: bool = False, sync: bool = True) -> "MedicalVolume":
+        """Applies modality LUT to volume.
+
+        Args:
+            inplace (bool, optional): If ``True``, applies modality LUT in place.
+            sync (bool, optional): If ``True``, updates the headers.
+
+        Returns:
+            MedicalVolume: Volume with modality LUT applied.
+        """
+        if self._headers is None:
+            return self
+
+        return self._apply_lut("ModalityLUTSequence", index=0, inplace=inplace, sync=sync)
+
+    def apply_window(
+        self,
+        index: int = 0,
+        center: float = None,
+        width: float = None,
+        output_range: Tuple[float, float] = None,
+        mode: str = None,
+        dtype: np.dtype = None,
+        inplace: bool = False,
+        sync: bool = True,
+    ) -> "MedicalVolume":
+        """Windows the volume using the window center and width.
+        User supplied values will override the values in the header.
+
+        Args:
+            index (int, optional): Index of window to apply.
+            center (float, optional): Window center. If ``None``, will
+                use the value in the header.
+            width (float, optional): Window width. If ``None``, will
+                use the value in the header.
+            output_range (Tuple[float, float], optional): Output range to
+                apply window to. If ``None``, will use the value in the header.
+            mode (str, optional): VOI LUT function. If ``None``, will
+                use the value in the header.
+            dtype (np.dtype, optional): Data type to cast volume to before
+                window is applied.
+            inplace (bool, optional): If ``True``, applies window in place.
+            sync (bool, optional): If ``True``, updates the headers.
+
+        Returns:
+            ``MedicalVolume`` with window applied.
+        """
+        if self._headers is None and (center is None or width is None):
+            return self
+
+        # Define the window center, window width, and VOI LUT function
+        wc, ww, vlf = center, width, mode
+        if self._headers is not None:
+            h: pydicom.Dataset = self._headers.flat[0]
+            if center is None:
+                if "WindowCenter" not in h:
+                    return self
+
+                wc = h["WindowCenter"]
+                wc = float(wc.value[index]) if wc.VM > 1 else float(wc.value)
+
+            if width is None:
+                if "WindowWidth" not in h:
+                    return self
+
+                ww = h["WindowWidth"]
+                ww = float(ww.value[index]) if ww.VM > 1 else float(ww.value)
+
+            if mode is None:
+                vlf = h.get("VOILUTFunction", None)
+
+        # Apply the window transformation
+        mv = self if inplace else self.clone()
+        mv = self.astype(dtype, copy=False)
+        apply_window(mv._volume, wc, ww, output_range, vlf, inplace=True)
+
+        if sync:
+            for key in ["WindowCenter", "WindowWidth", "VOILUTFunction"]:
+                mv._delete_metadata(key)
+
+        return mv
+
+    def apply_voi_lut(
+        self, index: int = 0, inplace: bool = False, sync: bool = True
+    ) -> "MedicalVolume":
+        """Applies VOI LUT to volume.
+
+        Args:
+            index (int, optional): Index of VOI LUT to apply.
+            inplace (bool, optional): If ``True``, applies VOI LUT in place.
+            sync (bool, optional): If ``True``, updates the headers by removing
+                the VOI LUT Sequence and setting the window to the dynamic range.
+
+        Returns:
+            ``MedicalVolume`` with VOI LUT applied.
+        """
+        if self._headers is None:
+            return self
+
+        return self._apply_lut("VOILUTSequence", index=index, inplace=inplace, sync=sync)
+
+    def to_grayscale(
+        self,
+        mode: str = "MONOCHROME2",
+        output_range: Tuple[float, float] = None,
+        inplace: bool = False,
+        sync: bool = True,
+    ) -> "MedicalVolume":
+        """Converts volume to a grayscale mode."""
+        if self._headers is None:
+            return self
+
+        options = ["MONOCHROME1", "MONOCHROME2"]
+        if mode not in options:
+            raise ValueError(f"Photometric Interpretation {mode} is not a grayscale mode.")
+
+        h: pydicom.Dataset = self._headers.flat[0]
+        if "PhotometricInterpretation" not in h or h.PhotometricInterpretation == mode:
+            return self
+
+        mv = self if inplace else self.clone()
+        if sync:
+            # Toggle the photometric interpretation
+            mv.set_metadata("PhotometricInterpretation", mode)
+
+            # Update the window center and width
+            center = np.array(h.get("WindowCenter", [])).flatten()
+            width = np.array(h.get("WindowWidth", [])).flatten()
+
+            if len(center) > 0 and len(width) > 0:
+                wcs, wws = [], []
+                for wc, ww in zip(center, width):
+                    new_wc, new_ww = invert_window(mv._volume, wc, ww, output_range)
+                    wcs.append(new_wc)
+                    wws.append(new_ww)
+
+                if len(wcs) == 1:
+                    wcs, wws = wcs[0], wws[0]
+
+                mv.set_metadata("WindowCenter", wcs)
+                mv.set_metadata("WindowWidth", wws)
+                mv.set_metadata("VOILUTFunction", "LINEAR_EXACT", force=True)
+
+        # Invert the volume
+        invert(mv._volume, output_range, inplace=True)
+        return mv
+
     def materialize(self):
         if not self.is_mmap:
+            return self[:]
+        else:
+            xp = self.device.xp
+            self._volume = xp.asarray(self._volume)
             return self
 
     def round(self, decimals=0, affine=False) -> "MedicalVolume":
         """Round array (and optionally affine matrix).
 
         Args:
             decimals (int, optional): Number of decimals to round to.
@@ -811,14 +1076,59 @@
         from voxel.numpy_routines import mean_np
 
         # `out` is required for cupy arrays because of how cupy calls array.
         if out is not None:
             raise ValueError("`out` must be None")
         return mean_np(self, axis=axis, dtype=dtype, keepdims=keepdims, where=where)
 
+    def std(self, axis=None, dtype=None, out=None, keepdims=False, where=np._NoValue):
+        """Compute the standard deviation along the specified axis. Identical to :meth:`std`.
+
+        See :meth:`std` for more information.
+
+        Args:
+            axis: Same as :meth:`std`.
+            dtype: Same as :meth:`std`.
+            out: Same as :meth:`std`.
+            keepdims: Same as :meth:`std`.
+            initial: Same as :meth:`std`.
+            where: Same as :meth:`std`.
+        """
+        from voxel.numpy_routines import std
+
+        # `out` is required for cupy arrays because of how cupy calls array.
+        if out is not None:
+            raise ValueError("`out` must be None")
+        return std(self, axis=axis, dtype=dtype, keepdims=keepdims, where=where)
+
+    def contiguous(self) -> "MedicalVolume":
+        """Returns a MedicalVolume with pixel data contiguous in memory.
+
+        If the pixel data is already contiguous, returns the ``self``
+        medical volume.
+
+        Returns:
+            MedicalVolume: MedicalVolume with contiguous pixel data.
+        """
+        from voxel.numpy_routines import ascontiguousarray
+
+        if self.is_contiguous():
+            return self
+        return ascontiguousarray(self)
+
+    def is_contiguous(self) -> bool:
+        """Returns whether the pixel data is contiguous in memory.
+
+        Returns:
+            bool: Whether the pixel data is contiguous in memory.
+        """
+        from voxel.numpy_routines import is_contiguous
+
+        return is_contiguous(self)
+
     @property
     def A(self):
         """The pixel array. Same as ``self.volume``.
 
         Examples:
             >>> mv = MedicalVolume([[[1,2],[3,4]]], np.eye(4))
             >>> mv.A
@@ -830,18 +1140,16 @@
     @property
     def volume(self):
         """ndarray: ndarray representing volume values."""
         return self._volume
 
     @volume.setter
     def volume(self, value):
-        """
-        If the volume is of a different shape, the headers are no longer valid,
-        so delete all reorientations are done as part of MedicalVolume,
-        so reorientations are permitted.
+        """If the volume is of a different shape, the headers are no longer valid, so delete all
+        reorientations are done as part of MedicalVolume, so reorientations are permitted.
 
         However, external setting of the volume to a different shape array is not allowed.
         """
         if value.ndim != self._volume.ndim:
             raise ValueError("New volume must be same as current volume")
 
         if self._volume.shape != value.shape:
@@ -891,15 +1199,18 @@
     @property
     def device(self) -> Device:
         """The device the object is on."""
         return get_device(self._volume)
 
     @property
     def dtype(self):
-        """The ``dtype`` of the ndarray. Same as ``self.volume.dtype``."""
+        """The ``dtype`` of the ndarray.
+
+        Same as ``self.volume.dtype``.
+        """
         return self._volume.dtype
 
     @property
     def is_mmap(self) -> bool:
         """bool: Whether the volume is a memory-mapped array."""
         # important to check if .base is a python mmap object, since a view of a mmap
         # is also a memmap object, but should not be symlinked or copied
@@ -1131,14 +1442,84 @@
                 kwargs[k] = getattr(self, f"_{k}").copy()
         if "headers" not in kwargs:
             kwargs["headers"] = self._headers
         elif isinstance(kwargs["headers"], bool) and kwargs["headers"]:
             kwargs["headers"] = deepcopy(self._headers)
         return self.__class__(**kwargs)
 
+    @classmethod
+    def from_zarr(
+        cls,
+        store,
+        affine_attr: str = None,
+        headers_attr: str = None,
+        default_ornt: Tuple[str, str] = np._NoValue,
+        **kwargs,
+    ) -> "MedicalVolume":
+        """Construct a MedicalVolume from a Zarr store.
+
+        This method safely opens a Zarr store and lazily loads the associated volume. The affine
+        matrix and headers can be opened through the ``affine_attr`` and ``headers_attr``, if
+        applicable.
+
+        Args:
+            store (Union[MutableMapping, str]): A zarr store.
+            affine_attr (str, optional): Attribute key from the Zarr array where the affine matrix
+                is stored in. If `None`, then the affine matrix is assumed to be the identity.
+            headers_attr (str, optional): Attribute key to retrieve the headers of the
+                `MedicalVolume` from. If `None`, headers will not be retrieved.
+            default_ornt (Tuple[str, str], optional): See `MedicalVolume` class parameters.
+            **kwargs: Additional parameters are passed along to `zarr.creation.open_array`.
+
+        Returns:
+            MedicalVolume: The medical image.
+
+        Examples:
+            >>> # load a zarr array from disk
+            >>> store = zarr.ZipStore("/path/to/store")
+            >>> zarr.save_array(store, np.zeros((10, 10)))
+            >>> MedicalVolume.from_zarr(store)
+
+            >>> # load zarr array, affine matrix, and headers
+            >>> mv = vx.load("path/to/dicoms")
+            >>> mv.to_zarr(store=store, affine_attr="affine", headers_attr="headers")
+            >>> MedicalVolume.from_zarr(store=store, affine_attr="affine", headers_attr="headers")
+        """
+
+        if not env.package_available("zarr"):
+            raise ImportError(  # pragma: no cover
+                "zarr is not installed. Install it with `pip install zarr`. "
+            )
+
+        import zarr
+
+        arr = zarr.open_array(store, **{"mode": "r", **kwargs})
+
+        # Determine if DICOM+JSON headers are stored in the zarr array. If so, retrieve them and
+        # convert them back to a list of pydicom.Dataset instances.
+        headers, affine = None, np.eye(4)
+        if headers_attr is not None:
+            zarr_header = arr.attrs.get(headers_attr, None)
+            if zarr_header is None:
+                raise KeyError(f"Attribute `{headers_attr}` does not exist on the zarr.Array.")
+            headers = [Dataset.from_json(h) for h in zarr_header]
+
+        # Determine if the affine matrix is stored in the zarr array. If so, retrieve it, else
+        # try to infer it from the headers. If no headers are available, use the identity matrix.
+        if affine_attr is not None:
+            if affine_attr not in arr.attrs:
+                raise KeyError(f"Attribute `{affine_attr}` does not exist on the zarr.Array.")
+            affine = np.array(arr.attrs.get(affine_attr)).reshape(4, 4)
+            return cls(arr, affine, headers)
+
+        if headers is not None:
+            affine = stdo.to_RAS_affine(headers, default_ornt)
+
+        return cls(arr, affine, headers)
+
     def _validate_and_format_headers(self, headers):
         """Validate headers are of appropriate shape and format into standardized shape.
 
         Headers are stored an ndarray of dictionary-like objects with explicit dimensions
         that match the dimensions of ``self._volume``. If header objects are not
 
         Assumes ``self._volume`` and ``self._affine`` have been set.
@@ -1157,14 +1538,81 @@
                 )
 
         ndim = self._volume.ndim
         shape = (1,) * (ndim - len(headers.shape)) + headers.shape
         headers = np.reshape(headers, shape)
         return headers
 
+    def _delete_metadata(self, key: Union[str, pydicom.BaseTag]):
+        """Deletes metadata for all headers.
+
+        Args:
+            key (str or pydicom.BaseTag): Metadata field to access.
+        """
+        if self._headers is not None:
+            for h in self._headers.flat:
+                if key in h:
+                    del h[key]
+
+    def _apply_lut(
+        self,
+        key: Union[str, pydicom.BaseTag],
+        index: int = 0,
+        inplace: bool = False,
+        sync: bool = True,
+    ) -> "MedicalVolume":
+        """Applies a LUT to the volume.
+
+        Args:
+            lut (pydicom.Dataset): LUT dataset.
+            inplace (bool, optional): If ``True``, applies LUT inplace.
+
+        Returns:
+            ``MedicalVolume`` with a LUT applied.
+        """
+        h: pydicom.Dataset = self._headers.flat[0]
+        xp = self.device.xp
+
+        if key not in h or index > len(h.get(key)) - 1:
+            return self
+
+        lut = h.get(key)[index]
+        mv = self if inplace else self.clone()
+        entries = lut.LUTDescriptor[0] if lut.LUTDescriptor[0] > 0 else 2**16
+        first_mapped = lut.LUTDescriptor[1]
+
+        bits_stored = int(lut.LUTDescriptor[2])
+        bits_allocated = 16 if bits_stored in range(9, 16) else bits_stored
+        if bits_allocated not in [8, 16]:
+            raise ValueError(f"Unsupported LUT bit depth: {bits_allocated}.")
+
+        sign = "u" if h.PixelRepresentation == 0 else "i"
+        lut_dtype = f"<{sign}{bits_allocated // 8}"
+
+        if lut["LUTData"].VR == "OW":
+            lut_dtype = "<" if h.is_little_endian else ">" + lut_dtype[1:]
+            lut_data = xp.frombuffer(bytearray(lut["LUTData"].value), dtype=lut_dtype)
+        else:
+            lut_data = xp.array(lut["LUTData"].value, dtype=lut_dtype)
+
+        # Convert all pixel values into LUT indices
+        lut_idxs = xp.zeros_like(self._volume, dtype=f"{sign}{bits_allocated // 8}")
+        mapped_pixels = self._volume >= first_mapped
+        lut_idxs[mapped_pixels] = self._volume[mapped_pixels] - first_mapped
+        xp.clip(lut_idxs, 0, entries - 1, out=lut_idxs)
+        mv._volume = lut_data[lut_idxs]
+
+        if sync:
+            mv._delete_metadata(key)
+            mv.set_metadata("BitsStored", bits_stored, force=True)
+            mv.set_metadata("BitsAllocated", bits_allocated, force=True)
+            mv.set_metadata("HighBit", bits_stored - 1, force=True)
+
+        return mv
+
     def _extract_input_array_ufunc(self, input, device=None):
         if device is None:
             device = self.device
         device_err = "Expected device {} but got device ".format(device) + "{}"
         if isinstance(input, Number):
             return input
         elif isinstance(input, np.ndarray):
@@ -1194,17 +1642,15 @@
         if any(x < 3 for x in axis):
             raise ValueError("Cannot reduce MedicalVolume along spatial dimensions")
         if not is_sequence:
             axis = axis[0]
         return axis
 
     def _reduce_array(self, func, *inputs, **kwargs) -> "MedicalVolume":
-        """
-        Assumes inputs have been verified.
-        """
+        """Assumes inputs have been verified."""
         device = self.device
         xp = device.xp
 
         keepdims = kwargs.get("keepdims", False)
         reduce_axis = self._check_reduce_axis(kwargs["axis"])
         kwargs["axis"] = reduce_axis
         if not isinstance(reduce_axis, Sequence):
```

### Comparing `pyvoxel-0.0.1a1/voxel/numpy_routines.py` & `pyvoxel-0.0.2/voxel/numpy_routines.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""List of numpy functions supported for MedicalVolumes.
-"""
+"""List of numpy functions supported for MedicalVolumes."""
 import warnings
 from typing import Sequence, Union
 
 import numpy as np
 
+from voxel.device import cpu_device
 from voxel.med_volume import MedicalVolume
 
 __all__ = [
     "amin",
     "amax",
     "argmin",
     "argmax",
@@ -363,15 +363,15 @@
     volume = np.concatenate([x.volume for x in xs], axis=axis)
     headers = [x.headers() for x in xs]
     if any(x is None for x in headers):
         headers = None
     else:
         headers = np.concatenate(headers, axis=axis)
         if headers.ndim != volume.ndim or any(
-            [hs != 1 and hs != vs for hs, vs in zip(headers.shape, volume.shape)]
+            hs != 1 and hs != vs for hs, vs in zip(headers.shape, volume.shape)
         ):
             warnings.warn(
                 "Got invalid headers shape ({}) given concatenated output shape ({}). "
                 "Expected header dimensions to be 1 or same as volume dimension for all axes. "
                 "Dropping all headers in concatenated output.".format(volume.shape, headers.shape)
             )
             headers = None
@@ -616,14 +616,44 @@
     vol = np.may_share_memory(a.A, b.A, max_work=max_work)
     headers = True
     if a.headers() is not None or b.headers() is not None:
         headers = np.may_share_memory(a.headers(), b.headers(), max_work=max_work)
     return vol and headers
 
 
+@implements(np.ascontiguousarray)
+def ascontiguousarray(a, dtype=None, *, like=None):
+    if isinstance(like, MedicalVolume):
+        like = like.A
+    if like is not None:
+        raise ValueError("Does not support `like` argument.")
+    return a._partial_clone(volume=np.ascontiguousarray(a.A, dtype=dtype))
+
+
+def is_contiguous(x: MedicalVolume) -> bool:
+    """Check if the pixel array is contiguous.
+
+    If the underlying array (``mv.A``) is a CuPy array,
+    returns ``True`` iff the array is C contiguous.
+
+    Args:
+        a (MedicalVolume): Input volume.
+
+    Returns:
+        bool: ``True`` if the pixel array is contiguous.
+    """
+    if x.device == cpu_device:
+        # numpy
+        return x.A.data.contiguous
+    else:
+        # cupy
+        # TODO: check if it is sufficient to check c_contiguous
+        return x.A.flags.c_contiguous
+
+
 def _to_positive_axis(
     axis: Union[int, Sequence[int]],
     ndim: int,
     grow: bool = False,
     invalid_axis: Union[int, Sequence[int]] = None,
 ):
     """
```

### Comparing `pyvoxel-0.0.1a1/voxel/utils/collect_env.py` & `pyvoxel-0.0.2/voxel/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pyvoxel-0.0.1a1/voxel/utils/env.py` & `pyvoxel-0.0.2/voxel/utils/env.py`

 * *Files identical despite different names*

### Comparing `pyvoxel-0.0.1a1/voxel/utils/logger.py` & `pyvoxel-0.0.2/voxel/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Logging utility.
-"""
+"""Logging utility."""
 
 import atexit
 import functools
 import logging
 import os
 import sys
 from time import localtime, strftime
@@ -13,16 +12,16 @@
 
 from voxel.utils import env
 
 __all__ = ["setup_logger"]
 
 
 class _ColorfulFormatter(logging.Formatter):
-    """
-    This class is adapted from Facebook's detectron2:
+    """This class is adapted from Facebook's detectron2:
+
     https://github.com/facebookresearch/detectron2/blob/master/detectron2/utils/logger.py
     """
 
     def __init__(self, *args, **kwargs):
         self._root_name = kwargs.pop("root_name") + "."
         self._abbrev_name = kwargs.pop("abbrev_name", "")
         if len(self._abbrev_name):
```

