# Comparing `tmp/ctapipe_io_magic-0.4.7.tar.gz` & `tmp/ctapipe_io_magic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Documenti/Dottorato/MAGIC/GSPOT/Repo/gitlab/ctapipe_io_magic/dist/tmp46371oud/ctapipe_io_magic-0.4.7.tar", last modified: Fri Oct  7 07:53:50 2022, max compression
+gzip compressed data, was "ctapipe_io_magic-0.5.0.tar", last modified: Wed Apr 26 09:00:49 2023, max compression
```

## Comparing `ctapipe_io_magic-0.4.7.tar` & `ctapipe_io_magic-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0 shari90   (1000) shari90   (1000)        0 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     1069 2022-07-24 12:19:01.000000 ctapipe_io_magic-0.4.7/LICENSE
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      151 2022-07-24 12:19:01.000000 ctapipe_io_magic-0.4.7/MANIFEST.in
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     7087 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/PKG-INFO
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     6702 2022-10-07 07:47:10.000000 ctapipe_io_magic-0.4.7/README.md
-drwxrwxrwx   0 shari90   (1000) shari90   (1000)        0 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)    67320 2022-10-07 07:47:21.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/__init__.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      176 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/_version.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      420 2022-10-07 07:37:59.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/constants.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     1069 2022-09-05 11:52:04.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/mars_datalevels.py
-drwxrwxrwx   0 shari90   (1000) shari90   (1000)        0 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/resources/
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     7287 2022-01-17 13:17:28.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
-drwxrwxrwx   0 shari90   (1000) shari90   (1000)        0 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)    12711 2022-10-07 07:37:59.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/test_magic_event_source.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      187 2022-07-24 12:19:51.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/test_mars_datalevels.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     2557 2022-09-05 11:52:04.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/test_stage1.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      106 2022-09-05 11:52:04.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/test_version.py
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      822 2022-07-24 12:19:51.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic/version.py
-drwxrwxrwx   0 shari90   (1000) shari90   (1000)        0 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     7087 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/PKG-INFO
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      705 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/SOURCES.txt
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)        1 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/dependency_links.txt
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      258 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/requires.txt
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)       17 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/top_level.txt
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     2225 2022-09-05 11:52:04.000000 ctapipe_io_magic-0.4.7/download_test_data.sh
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      353 2022-07-24 12:19:51.000000 ctapipe_io_magic-0.4.7/environment.yml
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)     1170 2022-01-18 13:06:22.000000 ctapipe_io_magic-0.4.7/example_stage1_config.json
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      128 2022-07-24 12:19:51.000000 ctapipe_io_magic-0.4.7/pyproject.toml
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      357 2022-10-07 07:53:50.000000 ctapipe_io_magic-0.4.7/setup.cfg
--rwxrwxrwx   0 shari90   (1000) shari90   (1000)      733 2022-07-24 12:19:51.000000 ctapipe_io_magic-0.4.7/setup.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1090 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/LICENSE
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      159 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/MANIFEST.in
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     6861 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/PKG-INFO
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     6590 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/README.md
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)    69468 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/__init__.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      160 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/_version.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      420 2023-04-19 10:27:57.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/constants.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1069 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/mars_datalevels.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic/resources/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     7189 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)    12801 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_magic_event_source.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      193 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_mars_datalevels.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     2557 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_stage1.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      106 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_version.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      844 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/version.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     6861 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/PKG-INFO
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      731 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)        1 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      251 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/requires.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)       17 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/top_level.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     2232 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/download_test_data.sh
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      331 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/environment.yml
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      157 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/eventsource_subclasses.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1153 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/example_stage1_config.json
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      130 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/pyproject.toml
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      357 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/setup.cfg
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      749 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ctapipe_io_magic-0.4.7/LICENSE` & `ctapipe_io_magic-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ctapipe_io_magic-0.4.7/PKG-INFO` & `ctapipe_io_magic-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_magic
-Version: 0.4.7
+Version: 0.5.0
 Summary: ctapipe plugin for reading calibrated MAGIC files
 Home-page: https://github.com/cta-observatory/ctapipe_io_magic
 Author: Ievgen Vovk et al.
 Author-email: Ievgen.Vovk@mpp.mpg.de
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 ## *ctapipe* MAGIC event source
 
-EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.12.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=4.1) packages to run.
+EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.17.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
 
-Provided that *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
+If *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
 
 ```bash
 pip install ctapipe_io_magic
 ```
 
 Alternatively, you can always clone the repository and install like in the following:
 
 ```bash
 git clone https://github.com/cta-observatory/ctapipe_io_magic.git
-pip install ./ctapipe_io_magic/
-```
-
-This installation via *pip* (provided, *pip* is installed) has the advantage to be nicely controlled for belonging to a given conda environment (and to be uninstalled). Alternatively, do
-
-```bash
-git clone https://github.com/cta-observatory/ctapipe_io_magic.git
 cd ctapipe_io_magic
-python setup.py install --user
+conda env create -n ctapipe-io_magic -f environment.yml
+conda activate ctapipe-io_magic
+pip install .
 ```
 
-In all cases, using *pip* will check if the version of *ctapipe* and *uproot* is compatible with the requested version of *ctapipe_io_magic*.
-
 #### Usage
 
 ```python
 import ctapipe
 from ctapipe_io_magic import MAGICEventSource
 
 with MAGICEventSource(input_url=file_name) as event_source:
@@ -128,7 +121,8 @@
 -   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
 -   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
 -   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
+-   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the correct value used in MAGIC simulations (i.e. 16.97 meters)
```

### Comparing `ctapipe_io_magic-0.4.7/README.md` & `ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,43 @@
+Metadata-Version: 2.1
+Name: ctapipe-io-magic
+Version: 0.5.0
+Summary: ctapipe plugin for reading calibrated MAGIC files
+Home-page: https://github.com/cta-observatory/ctapipe_io_magic
+Author: Ievgen Vovk et al.
+Author-email: Ievgen.Vovk@mpp.mpg.de
+License: MIT
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
 ## *ctapipe* MAGIC event source
 
-EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.12.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=4.1) packages to run.
+EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.17.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
 
-Provided that *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
+If *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
 
 ```bash
 pip install ctapipe_io_magic
 ```
 
 Alternatively, you can always clone the repository and install like in the following:
 
 ```bash
 git clone https://github.com/cta-observatory/ctapipe_io_magic.git
-pip install ./ctapipe_io_magic/
-```
-
-This installation via *pip* (provided, *pip* is installed) has the advantage to be nicely controlled for belonging to a given conda environment (and to be uninstalled). Alternatively, do
-
-```bash
-git clone https://github.com/cta-observatory/ctapipe_io_magic.git
 cd ctapipe_io_magic
-python setup.py install --user
+conda env create -n ctapipe-io_magic -f environment.yml
+conda activate ctapipe-io_magic
+pip install .
 ```
 
-In all cases, using *pip* will check if the version of *ctapipe* and *uproot* is compatible with the requested version of *ctapipe_io_magic*.
-
 #### Usage
 
 ```python
 import ctapipe
 from ctapipe_io_magic import MAGICEventSource
 
 with MAGICEventSource(input_url=file_name) as event_source:
@@ -114,7 +121,8 @@
 -   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
 -   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
 -   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
+-   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the correct value used in MAGIC simulations (i.e. 16.97 meters)
```

### Comparing `ctapipe_io_magic-0.4.7/ctapipe_io_magic/__init__.py` & `ctapipe_io_magic-0.5.0/ctapipe_io_magic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,31 +14,37 @@
 from decimal import Decimal
 from astropy import units as u
 from astropy.time import Time
 from pkg_resources import resource_filename
 
 from ctapipe.io import EventSource, DataLevel
 from ctapipe.core import Provenance
-from ctapipe.core.traits import Bool, CaselessStrEnum
+from ctapipe.core.traits import Bool, UseEnum
 from ctapipe.coordinates import CameraFrame
 
 from ctapipe.containers import (
     EventType,
     ArrayEventContainer,
     SimulationConfigContainer,
     SimulatedEventContainer,
+    SchedulingBlockContainer,
+    ObservationBlockContainer,
+    PointingMode,
 )
 
 from ctapipe.instrument import (
     TelescopeDescription,
     SubarrayDescription,
     OpticsDescription,
     CameraDescription,
     CameraGeometry,
     CameraReadout,
+    SizeType,
+    ReflectorShape,
+    FocalLengthKind,
 )
 
 from .mars_datalevels import MARSDataLevel
 from .version import __version__
 
 from .constants import (
     DATA_MONO_TRIGGER_PATTERN,
@@ -108,15 +114,15 @@
         A ROOT file opened with uproot
     is_mc : bool
         Flag indicating real or simulated data
     mars_datalevel : int
         Data level according to MARS convention
     metadata : dict
         Dictionary containing metadata
-    run_numbers : int
+    run_id : int
         Run number of the file
     simulation_config : SimulationConfigContainer
         Container filled with the information about the simulation
     telescope : int
         The number of the telescope
     use_pedestals : bool
         Flag indicating if pedestal events should be returned by the generator
@@ -133,17 +139,17 @@
     ).tag(config=True)
 
     use_mc_mono_events = Bool(
         default_value=False,
         help='Use mono events in MC stereo data (needed for mono analysis).'
     ).tag(config=True)
 
-    focal_length_choice = CaselessStrEnum(
-        ['nominal', 'effective'],
-        default_value='effective',
+    focal_length_choice = UseEnum(
+        FocalLengthKind,
+        default_value=FocalLengthKind.EFFECTIVE,
         help='Which focal length to use when constructing the SubarrayDescription.',
     ).tag(config=True)
 
     def __init__(self, input_url=None, config=None, parent=None, **kwargs):
         """
         Constructor
 
@@ -195,26 +201,26 @@
         else:
             self.file_list = [self.input_url]
 
         # Retrieving the list of run numbers corresponding to the data files
         self.files_ = [uproot.open(rootf) for rootf in self.file_list]
         run_info = self.parse_run_info()
 
-        self.run_numbers = run_info[0]
+        self.run_id = run_info[0][0]
         self.is_mc = run_info[1][0]
         self.telescope = run_info[2][0]
         self.mars_datalevel = run_info[3][0]
 
         self.metadata = self.parse_metadata_info()
 
         # Retrieving the data level (so far HARDCODED Sorcerer)
         self.datalevel = DataLevel.DL0
 
         if self.is_simulation:
-            self.simulation_config = self.parse_simulation_header()
+            self._simulation_config = self.parse_simulation_header()
 
         self.is_stereo, self.is_sumt = self.parse_data_info()
 
         if self.is_simulation and self.use_mc_mono_events and not self.is_stereo:
             logger.warning("Processing mono simulation data with" \
                 " use_mc_mono_events=True. use_mc_mono_events will be ignored.")
 
@@ -230,14 +236,32 @@
 
         if not self.is_simulation:
             self.drive_information = self.prepare_drive_information()
 
             # Get the arrival time differences
             self.event_time_diffs = self.get_event_time_difference()
 
+        pointing_mode = PointingMode.TRACK
+
+        self._scheduling_blocks = {
+            self.run_id: SchedulingBlockContainer(
+                sb_id=np.uint64(self.run_id),
+                producer_id=f"MAGIC-{self.telescope}",
+                pointing_mode=pointing_mode,
+            )
+        }
+
+        self._observation_blocks = {
+            self.run_id: ObservationBlockContainer(
+                obs_id=np.uint64(self.run_id),
+                sb_id=np.uint64(self.run_id),
+                producer_id=f"MAGIC-{self.telescope}",
+            )
+        }
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         Releases resources (e.g. open files).
 
         Parameters
         ----------
         exc_type : Exception
@@ -616,51 +640,82 @@
         # MAGIC telescope positions in m wrt. to the center of MAGIC simulations, from
         # CORSIKA and reflector input card and recomputed (rotated) to be w.r.t. geographical North
         MAGIC_TEL_POSITIONS = {
             1: [34.99, -24.02, 0.00] * u.m,
             2: [-34.99, 24.02, 0.00] * u.m
         }
 
-        if self.focal_length_choice == 'effective':
-            # Use the effective focal length that the coma aberration is corrected
-            focal_length = u.Quantity(17*1.0713, u.m)
-        else:
-            focal_length = u.Quantity(17, u.m)
+        equivalent_focal_length = u.Quantity(16.97, u.m)
+        effective_focal_length = u.Quantity(17*1.0713, u.m)
 
         OPTICS = OpticsDescription(
-            'MAGIC',
-            num_mirrors=1,
-            equivalent_focal_length=focal_length,
+            name='MAGIC',
+            size_type=SizeType.LST,
+            n_mirrors=1,
+            n_mirror_tiles=964,
+            reflector_shape=ReflectorShape.PARABOLIC,
+            equivalent_focal_length=equivalent_focal_length,
+            effective_focal_length=effective_focal_length,
             mirror_area=u.Quantity(239.0, u.m**2),
-            num_mirror_tiles=964,
         )
 
+        if self.focal_length_choice is FocalLengthKind.EFFECTIVE:
+            focal_length = effective_focal_length
+        elif self.focal_length_choice is FocalLengthKind.EQUIVALENT:
+            focal_length = equivalent_focal_length
+        else:
+            raise ValueError(
+                f"Invalid focal length choice: {self.focal_length_choice}"
+            )
+
         # camera info from MAGICCam.camgeom.fits.gz file
         camera_geom = load_camera_geometry()
 
+        n_pixels = camera_geom.n_pixels
+
+        n_samples_array_list = ["MRawRunHeader.fNumSamplesHiGain"]
+        n_samples_list = []
+
+        for rootf in self.files_:
+            nsample_info = rootf['RunHeaders'].arrays(n_samples_array_list, library="np")
+            n_samples_file = int(nsample_info['MRawRunHeader.fNumSamplesHiGain'][0])
+            n_samples_list.append(n_samples_file)
+
+        n_samples_list = np.unique(n_samples_list).tolist()
+
+        if len(n_samples_list) > 1:
+            raise ValueError(
+                "Loaded files contain different number of readout samples. \
+                 Please load files with the same readout configuration.")
+
+        n_samples = n_samples_list[0]
+
         pulse_shape_lo_gain = np.array([0., 1., 2., 1., 0.])
         pulse_shape_hi_gain = np.array([1., 2., 3., 2., 1.])
         pulse_shape = np.vstack((pulse_shape_lo_gain, pulse_shape_hi_gain))
         sampling_speed = u.Quantity(
             self.files_[0]['RunHeaders']['MRawRunHeader.fSamplingFrequency'].array(library='np')[0]/1000,
             u.GHz
         )
         camera_readout = CameraReadout(
-            camera_name='MAGICCam',
+            name='MAGICCam',
             sampling_rate=sampling_speed,
             reference_pulse_shape=pulse_shape,
-            reference_pulse_sample_width=u.Quantity(0.5, u.ns)
+            reference_pulse_sample_width=u.Quantity(0.5, u.ns),
+            n_channels=1,
+            n_pixels=n_pixels,
+            n_samples=n_samples,
         )
 
         camera = CameraDescription('MAGICCam', camera_geom, camera_readout)
 
-        camera.geometry.frame = CameraFrame(focal_length=OPTICS.equivalent_focal_length)
+        camera.geometry.frame = CameraFrame(focal_length=focal_length)
 
         MAGIC_TEL_DESCRIPTION = TelescopeDescription(
-            name='MAGIC', tel_type='MAGIC', optics=OPTICS, camera=camera
+            name='MAGIC', optics=OPTICS, camera=camera
         )
 
         MAGIC_TEL_DESCRIPTIONS = {1: MAGIC_TEL_DESCRIPTION, 2: MAGIC_TEL_DESCRIPTION}
 
         subarray = SubarrayDescription(
             name='MAGIC',
             tel_positions=MAGIC_TEL_POSITIONS,
@@ -727,15 +782,15 @@
         metadatainfo_array_list_runtails = [
             'MMarsVersion_sorcerer.fMARSVersionCode',
             'MMarsVersion_sorcerer.fROOTVersionCode',
         ]
 
         metadata = dict()
         metadata["file_list"] = self.file_list
-        metadata['run_numbers'] = self.run_numbers
+        metadata['run_numbers'] = self.run_id
         metadata['is_simulation'] = self.is_simulation
         metadata['telescope'] = self.telescope
         metadata['subrun_number'] = []
         metadata['source_ra'] = []
         metadata['source_dec'] = []
         metadata['source_name'] = []
         metadata['observation_mode'] = []
@@ -814,15 +869,15 @@
         MAGIC_Bz = u.Quantity(23.0, u.uT)
         MAGIC_Btot = np.sqrt(MAGIC_Bx**2+MAGIC_Bz**2)
         MAGIC_Bdec = u.Quantity(-7.0, u.deg).to(u.rad)
         MAGIC_Binc = u.Quantity(np.arctan2(-MAGIC_Bz.value, MAGIC_Bx.value), u.rad)
 
         simulation_config = dict()
 
-        for run_number, rootf in zip(self.run_numbers, self.files_):
+        for rootf in self.files_:
 
             run_header_tree = rootf['RunHeaders']
             spectral_index = run_header_tree['MMcCorsikaRunHeader.fSlopeSpec'].array(library="np")[0]
             e_low = run_header_tree['MMcCorsikaRunHeader.fELowLim'].array(library="np")[0]
             e_high = run_header_tree['MMcCorsikaRunHeader.fEUppLim'].array(library="np")[0]
             corsika_version = run_header_tree['MMcCorsikaRunHeader.fCorsikaVersion'].array(library="np")[0]
             site_height = run_header_tree['MMcCorsikaRunHeader.fHeightLev[10]'].array(library="np")[0][0]
@@ -844,21 +899,21 @@
                 max_zd = run_header_tree['MMcRunHeader_1.fShowerThetaMax'].array(library="np")[0]
                 min_zd = run_header_tree['MMcRunHeader_1.fShowerThetaMin'].array(library="np")[0]
                 max_az = run_header_tree['MMcRunHeader_1.fShowerPhiMax'].array(library="np")[0]
                 min_az = run_header_tree['MMcRunHeader_1.fShowerPhiMin'].array(library="np")[0]
                 max_wavelength = run_header_tree['MMcRunHeader_1.fCWaveUpper'].array(library="np")[0]
                 min_wavelength = run_header_tree['MMcRunHeader_1.fCWaveLower'].array(library="np")[0]
 
-            simulation_config[run_number] = SimulationConfigContainer(
+            simulation_config[self.run_id] = SimulationConfigContainer(
                 corsika_version=corsika_version,
                 energy_range_min=u.Quantity(e_low, u.GeV).to(u.TeV),
                 energy_range_max=u.Quantity(e_high, u.GeV).to(u.TeV),
                 prod_site_alt=u.Quantity(site_height, u.cm).to(u.m),
                 spectral_index=spectral_index,
-                num_showers=n_showers,
+                n_showers=n_showers,
                 shower_reuse=1,
                 # shower_reuse not written in the magic root file, but since the
                 # sim_events already include shower reuse we artificially set it
                 # to 1 (actually every shower reused 5 times for std MAGIC MC)
                 shower_prog_id=1,
                 prod_site_B_total=MAGIC_Btot,
                 prod_site_B_declination=MAGIC_Bdec,
@@ -965,21 +1020,33 @@
         return self._subarray_info
 
     @property
     def is_simulation(self):
         return self.is_mc
 
     @property
+    def observation_blocks(self):
+        return self._observation_blocks
+
+    @property
+    def scheduling_blocks(self):
+        return self._scheduling_blocks
+
+    @property
+    def simulation_config(self):
+        return self._simulation_config
+
+    @property
     def datalevels(self):
         return (self.datalevel, )
 
     @property
     def obs_ids(self):
         # ToCheck: will this be compatible in the future, e.g. with merged MC files
-        return self.run_numbers
+        return list(self.observation_blocks)
 
     def _get_badrmspixel_mask(self, event):
         """
         Fetch bad RMS pixel mask for a given event.
 
         Parameters
         ----------
@@ -1406,17 +1473,17 @@
             else:
                 events_cut['cosmic_events'] = f'(MTriggerPattern.fPrescaled == {mc_trigger_pattern})' \
                                                           ' & (MRawEvtHeader.fStereoEvtNumber != 0)'
         else:
             data_trigger_pattern = DATA_STEREO_TRIGGER_PATTERN
             if not self.is_stereo:
                 if self.use_sumt_events:
-                    mc_trigger_pattern = DATA_MONO_SUMT_TRIGGER_PATTERN
+                    data_trigger_pattern = DATA_MONO_SUMT_TRIGGER_PATTERN
                 else:
-                    mc_trigger_pattern = DATA_MONO_TRIGGER_PATTERN
+                    data_trigger_pattern = DATA_MONO_TRIGGER_PATTERN
             events_cut['cosmic_events'] = f'(MTriggerPattern.fPrescaled == {data_trigger_pattern})'
             # Only for cosmic events because MC data do not have pedestal events:
             events_cut['pedestal_events'] = f'(MTriggerPattern.fPrescaled == {PEDESTAL_TRIGGER_PATTERN})'
 
         logger.info(f"Cosmic events selection: {events_cut['cosmic_events']}")
 
         # read common information from RunHeaders
```

### Comparing `ctapipe_io_magic-0.4.7/ctapipe_io_magic/mars_datalevels.py` & `ctapipe_io_magic-0.5.0/ctapipe_io_magic/mars_datalevels.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/test_magic_event_source.py` & `ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_magic_event_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
     with MAGICEventSource(input_url=dataset, process_run=False) as source:
         run_info = [MAGICEventSource.get_run_info_from_name(item.name) for item in source.file_list]
         run_numbers = [i[0] for i in run_info]
         is_mc = [i[1] for i in run_info][0]
         telescope = [i[2] for i in run_info][0]
         datalevel = [i[3] for i in run_info][0]
-        assert run_numbers == source.run_numbers
+        assert run_numbers == [source.run_id]
         assert is_mc == source.is_simulation
         assert telescope == source.telescope
         assert datalevel == source.mars_datalevel
         assert source.is_stereo == True
         assert source.is_sumt == False
 
 
@@ -235,24 +235,25 @@
         assert source.subarray.tels[2].camera.geometry.pix_x.size == 1039
 
 
 @pytest.mark.parametrize('dataset', test_calibrated_all)
 def test_focal_length_choice(dataset):
     from astropy import units as u
     from ctapipe_io_magic import MAGICEventSource
+    from ctapipe.instrument import FocalLengthKind
 
-    with MAGICEventSource(input_url=dataset, process_run=False, focal_length_choice='nominal') as source:
-        assert source.subarray.tel[1].optics.equivalent_focal_length == u.Quantity(17, u.m)
-        assert source.subarray.tel[2].optics.equivalent_focal_length == u.Quantity(17, u.m)
-        assert source.subarray.tel[1].camera.geometry.frame.focal_length == u.Quantity(17, u.m)
-        assert source.subarray.tel[2].camera.geometry.frame.focal_length == u.Quantity(17, u.m)
-
-    with MAGICEventSource(input_url=dataset, process_run=False, focal_length_choice='effective') as source:
-        assert source.subarray.tel[1].optics.equivalent_focal_length == u.Quantity(17*1.0713, u.m)
-        assert source.subarray.tel[2].optics.equivalent_focal_length == u.Quantity(17*1.0713, u.m)
+    with MAGICEventSource(input_url=dataset, process_run=False, focal_length_choice=FocalLengthKind.EQUIVALENT) as source:
+        assert source.subarray.tel[1].optics.equivalent_focal_length == u.Quantity(16.97, u.m)
+        assert source.subarray.tel[2].optics.equivalent_focal_length == u.Quantity(16.97, u.m)
+        assert source.subarray.tel[1].camera.geometry.frame.focal_length == u.Quantity(16.97, u.m)
+        assert source.subarray.tel[2].camera.geometry.frame.focal_length == u.Quantity(16.97, u.m)
+
+    with MAGICEventSource(input_url=dataset, process_run=False, focal_length_choice=FocalLengthKind.EFFECTIVE) as source:
+        assert source.subarray.tel[1].optics.effective_focal_length == u.Quantity(17*1.0713, u.m)
+        assert source.subarray.tel[2].optics.effective_focal_length == u.Quantity(17*1.0713, u.m)
         assert source.subarray.tel[1].camera.geometry.frame.focal_length == u.Quantity(17*1.0713, u.m)
         assert source.subarray.tel[2].camera.geometry.frame.focal_length == u.Quantity(17*1.0713, u.m)
 
 # def test_eventseeker():
 #    dataset = get_dataset_path("20131004_M1_05029747.003_Y_MagicCrab-W0.40+035.root")
 #
 #    with MAGICEventSource(input_url=dataset) as source:
```

### Comparing `ctapipe_io_magic-0.4.7/ctapipe_io_magic/tests/test_stage1.py` & `ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_stage1.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/PKG-INFO` & `ctapipe_io_magic-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,114 @@
-Metadata-Version: 2.1
-Name: ctapipe-io-magic
-Version: 0.4.7
-Summary: ctapipe plugin for reading calibrated MAGIC files
-Home-page: https://github.com/cta-observatory/ctapipe_io_magic
-Author: Ievgen Vovk et al.
-Author-email: Ievgen.Vovk@mpp.mpg.de
-License: MIT
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
-## *ctapipe* MAGIC event source
-
-EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.12.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=4.1) packages to run.
-
-#### Installation
-
-Provided that *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
-
-```bash
-pip install ctapipe_io_magic
-```
-
-Alternatively, you can always clone the repository and install like in the following:
-
-```bash
-git clone https://github.com/cta-observatory/ctapipe_io_magic.git
-pip install ./ctapipe_io_magic/
-```
-
-This installation via *pip* (provided, *pip* is installed) has the advantage to be nicely controlled for belonging to a given conda environment (and to be uninstalled). Alternatively, do
-
-```bash
-git clone https://github.com/cta-observatory/ctapipe_io_magic.git
-cd ctapipe_io_magic
-python setup.py install --user
-```
-
-In all cases, using *pip* will check if the version of *ctapipe* and *uproot* is compatible with the requested version of *ctapipe_io_magic*.
-
-#### Usage
-
-```python
-import ctapipe
-from ctapipe_io_magic import MAGICEventSource
-
-with MAGICEventSource(input_url=file_name) as event_source:
-    for event in event_source:
-        ...some processing...
-```
-
-With more recent versions of *ctapipe*, only one file at a time can be read. However, by default if a subrun of calibrated data is given as input, `MAGICEventSource` will read the events from all the subruns from the run to which the data file belongs. To suppress this behavior, set `process_run=False` No matching of the events is performed at this level (if stereo data).
-
-Starting from v0.4.7, `MAGICEventSource` will automatically recognize the type of data contained in the calibrated ROOT files (stereo or mono; std trigger or SumT). For MC data, in the case stereo MC data are to be used for mono analysis, one can set to True the `use_mc_mono_events` option of the `MAGICEventSource` to use also mono triggered events.
-
-Pedestal events (trigger pattern = 8) can be generated as well.
-
-The reader is able to handle real data or Monte Carlo files, which are automatically recognized. Note that the names of input files have to follow the convention:
--   `*_M[1-2]_RUNNUMBER.SUBRUNNR_Y_*.root` for real data
--   `*_M[1-2]_za??to??_?_RUNNUMBER_Y_*.root` for simulated data.
-
-However, the information which can be extracted from the file names is read directly from within the ROOT files.
-
-##### More usage
-
-Select a single run:
-
-```python
-run = event_source._set_active_run(event_source.run_numbers[0])
-# run is an object of type MarsCalibratedRun
-# assuming we are reading data from a file from M1
-for n in range(run['data'].n_mono_events_m1):
-    run['data'].get_mono_event_data(n, 'M1')
-
-for n in range(run['data'].n_pedestal_events_m1):
-    run['data'].get_pedestal_event_data(n, 'M1')
-```
-
-Select events triggering in stereo and pedestal events from a single telescope (recognized automatically) over event generator:
-
-```python
-# select (stereo) cosmic events from all subruns of a given run (the one to which file_name belongs)
-event_generator = MAGICEventSource(input_url=file_name)
-for cosmic_event in event_generator:
-    ...some processing...
-
-# select (stereo) cosmic events from a single subrun
-event_generator = MAGICEventSource(input_url=file_name, process_run=False)
-for cosmic_event in event_generator:
-    ...some processing...
-
-# select pedestal events
-pedestal_event_generator = MAGICEventSource(input_url=file_name, use_pedestals=True)
-for pedestal_event in pedestal_event_generator:
-    ...some processing...
-```
-
-#### Features
-
-##### Drive reports interpolation
-
-By default, when all subruns from a given run are processed, the drive reports are collected from all subruns so that the telescope pointing position for each event can be computed. Also in the case that only one subrun is processed (`process_run=False`), all drive reports from the subruns belonging to the same run will be used. This ensures that interpolation is performed correctly.
-
-##### Monitoring data
-
-Monitoring data are saved in `run['data'].monitoring_data` and can also accessed event-wise via the `event.mon` container. Available information is:
--   dead pixels: `event.mon.tel[tel_id].pixel_status.hardware_failing_pixels[0]`
--   hot pixels:  `event.mon.tel[tel_id].pixel_status.pedestal_failing_pixels[i_ped_type]`, where `i_ped_type` is an index indicating which pedestal type to use (0 is `PedestalFundamental`, 1 is `PedestalFromExtractor` and 2 is `PedestalFromExtractorRndm`)
-
-Dead and hot pixels are used in `magic-cta-pipe` for the MAGIC cleaning.
-
-##### Simulation Configuration Data
-Some general information about the simulated data, useful for IRF calculation, are read from the root files and stored in data.simulation container.
-
-#### Changelog
-
--   v0.1: Initial version
--   v0.2.0: Unification of data and MC reading
--   v0.2.1: Monitoring data (Dead pixel and pedestal information)
--   v0.2.2: Added MC Header info
--   v0.2.3: Solve issue when interpolating information from drive reports, causing crashes when using pointing information in astropy SkyCoord objects. Make the reader faster when searching for ids of mono and stereo events
--   v0.2.4: fixes in mono_event_generator; fix to allow the use of relative paths as `input_url`
--   v0.3.0: update uproot to v4, since v3 is deprecated
--   v0.4.0: version compatible with ctapipe v0.12
--   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
--   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
--   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
--   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
--   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
--   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
--   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
+## *ctapipe* MAGIC event source
+
+EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.17.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
+
+#### Installation
+
+If *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
+
+```bash
+pip install ctapipe_io_magic
+```
+
+Alternatively, you can always clone the repository and install like in the following:
+
+```bash
+git clone https://github.com/cta-observatory/ctapipe_io_magic.git
+cd ctapipe_io_magic
+conda env create -n ctapipe-io_magic -f environment.yml
+conda activate ctapipe-io_magic
+pip install .
+```
+
+#### Usage
+
+```python
+import ctapipe
+from ctapipe_io_magic import MAGICEventSource
+
+with MAGICEventSource(input_url=file_name) as event_source:
+    for event in event_source:
+        ...some processing...
+```
+
+With more recent versions of *ctapipe*, only one file at a time can be read. However, by default if a subrun of calibrated data is given as input, `MAGICEventSource` will read the events from all the subruns from the run to which the data file belongs. To suppress this behavior, set `process_run=False` No matching of the events is performed at this level (if stereo data).
+
+Starting from v0.4.7, `MAGICEventSource` will automatically recognize the type of data contained in the calibrated ROOT files (stereo or mono; std trigger or SumT). For MC data, in the case stereo MC data are to be used for mono analysis, one can set to True the `use_mc_mono_events` option of the `MAGICEventSource` to use also mono triggered events.
+
+Pedestal events (trigger pattern = 8) can be generated as well.
+
+The reader is able to handle real data or Monte Carlo files, which are automatically recognized. Note that the names of input files have to follow the convention:
+-   `*_M[1-2]_RUNNUMBER.SUBRUNNR_Y_*.root` for real data
+-   `*_M[1-2]_za??to??_?_RUNNUMBER_Y_*.root` for simulated data.
+
+However, the information which can be extracted from the file names is read directly from within the ROOT files.
+
+##### More usage
+
+Select a single run:
+
+```python
+run = event_source._set_active_run(event_source.run_numbers[0])
+# run is an object of type MarsCalibratedRun
+# assuming we are reading data from a file from M1
+for n in range(run['data'].n_mono_events_m1):
+    run['data'].get_mono_event_data(n, 'M1')
+
+for n in range(run['data'].n_pedestal_events_m1):
+    run['data'].get_pedestal_event_data(n, 'M1')
+```
+
+Select events triggering in stereo and pedestal events from a single telescope (recognized automatically) over event generator:
+
+```python
+# select (stereo) cosmic events from all subruns of a given run (the one to which file_name belongs)
+event_generator = MAGICEventSource(input_url=file_name)
+for cosmic_event in event_generator:
+    ...some processing...
+
+# select (stereo) cosmic events from a single subrun
+event_generator = MAGICEventSource(input_url=file_name, process_run=False)
+for cosmic_event in event_generator:
+    ...some processing...
+
+# select pedestal events
+pedestal_event_generator = MAGICEventSource(input_url=file_name, use_pedestals=True)
+for pedestal_event in pedestal_event_generator:
+    ...some processing...
+```
+
+#### Features
+
+##### Drive reports interpolation
+
+By default, when all subruns from a given run are processed, the drive reports are collected from all subruns so that the telescope pointing position for each event can be computed. Also in the case that only one subrun is processed (`process_run=False`), all drive reports from the subruns belonging to the same run will be used. This ensures that interpolation is performed correctly.
+
+##### Monitoring data
+
+Monitoring data are saved in `run['data'].monitoring_data` and can also accessed event-wise via the `event.mon` container. Available information is:
+-   dead pixels: `event.mon.tel[tel_id].pixel_status.hardware_failing_pixels[0]`
+-   hot pixels:  `event.mon.tel[tel_id].pixel_status.pedestal_failing_pixels[i_ped_type]`, where `i_ped_type` is an index indicating which pedestal type to use (0 is `PedestalFundamental`, 1 is `PedestalFromExtractor` and 2 is `PedestalFromExtractorRndm`)
+
+Dead and hot pixels are used in `magic-cta-pipe` for the MAGIC cleaning.
+
+##### Simulation Configuration Data
+Some general information about the simulated data, useful for IRF calculation, are read from the root files and stored in data.simulation container.
+
+#### Changelog
+
+-   v0.1: Initial version
+-   v0.2.0: Unification of data and MC reading
+-   v0.2.1: Monitoring data (Dead pixel and pedestal information)
+-   v0.2.2: Added MC Header info
+-   v0.2.3: Solve issue when interpolating information from drive reports, causing crashes when using pointing information in astropy SkyCoord objects. Make the reader faster when searching for ids of mono and stereo events
+-   v0.2.4: fixes in mono_event_generator; fix to allow the use of relative paths as `input_url`
+-   v0.3.0: update uproot to v4, since v3 is deprecated
+-   v0.4.0: version compatible with ctapipe v0.12
+-   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
+-   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
+-   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
+-   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
+-   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
+-   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
+-   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
+-   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the correct value used in MAGIC simulations (i.e. 16.97 meters)
```

### Comparing `ctapipe_io_magic-0.4.7/ctapipe_io_magic.egg-info/SOURCES.txt` & `ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 download_test_data.sh
 environment.yml
+eventsource_subclasses.py
 example_stage1_config.json
 pyproject.toml
 setup.cfg
 setup.py
 ctapipe_io_magic/__init__.py
 ctapipe_io_magic/_version.py
 ctapipe_io_magic/constants.py
```

### Comparing `ctapipe_io_magic-0.4.7/download_test_data.sh` & `ctapipe_io_magic-0.5.0/download_test_data.sh`

 * *Files 3% similar despite different names*

```diff
@@ -9,41 +9,39 @@
 
 echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M1_za35to50_8_824318_Y_w0.root" >  test_data_simulated.txt
 echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M1_za35to50_8_824319_Y_w0.root" >> test_data_simulated.txt
 echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M2_za35to50_8_824318_Y_w0.root" >> test_data_simulated.txt
 echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M2_za35to50_8_824319_Y_w0.root" >> test_data_simulated.txt
 
 if [ -z "$TEST_DATA_USER" ]; then
-    echo -n "Username: "
-    read TEST_DATA_USER
+    read -p "Username: " TEST_DATA_USER
     echo
 fi
 
 if [ -z "$TEST_DATA_PASSWORD" ]; then
-    echo -n "Password: "
-    read -s TEST_DATA_PASSWORD
+    read -sr -p "Password: " TEST_DATA_PASSWORD
     echo
 fi
 
 if ! wget \
     -i test_data_real.txt \
     --user="$TEST_DATA_USER" \
     --password="$TEST_DATA_PASSWORD" \
     --no-check-certificate \
     --no-verbose \
     --timestamping \
     --directory-prefix=test_data/real/calibrated; then
-    echo "Problem in downloading the test data set for real data."
+    echo "Problem in downloading the test data set (calibrated) for real data."
 fi
 
 if ! wget \
     -i test_data_simulated.txt \
     --user="$TEST_DATA_USER" \
     --password="$TEST_DATA_PASSWORD" \
     --no-check-certificate \
     --no-verbose \
     --timestamping \
     --directory-prefix=test_data/simulated/calibrated; then
-    echo "Problem in downloading the test data set for simulated data."
+    echo "Problem in downloading the test data set (calibrated) for simulated data."
 fi
 
 rm -f test_data_real.txt test_data_simulated.txt
```

