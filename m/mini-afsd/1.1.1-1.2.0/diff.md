# Comparing `tmp/mini_afsd-1.1.1.tar.gz` & `tmp/mini_afsd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\shsde\Documents\Python Scripts\MiniAFSDCode\dist\.tmp-g_c6_kpi\mini_afsd-1.1.1.tar", last modified: Tue Mar 14 18:24:52 2023, max compression
+gzip compressed data, was "C:\Users\shsde\Documents\Python Scripts\MiniAFSDCode\dist\.tmp-sttr7yvt\mini_afsd-1.2.0.tar", last modified: Wed Apr 26 16:17:47 2023, max compression
```

## Comparing `mini_afsd-1.1.1.tar` & `mini_afsd-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 18:24:52.740811 mini_afsd-1.1.1/
--rw-rw-rw-   0        0        0      527 2022-09-07 17:45:49.000000 mini_afsd-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      346 2022-09-07 17:45:49.000000 mini_afsd-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5823 2023-03-14 18:24:52.741807 mini_afsd-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4750 2023-01-25 20:53:55.000000 mini_afsd-1.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-14 18:24:52.688948 mini_afsd-1.1.1/mini_afsd/
--rw-rw-rw-   0        0        0      436 2023-03-14 18:23:19.000000 mini_afsd-1.1.1/mini_afsd/__init__.py
--rw-rw-rw-   0        0        0     2994 2022-11-10 15:57:17.000000 mini_afsd-1.1.1/mini_afsd/__main__.py
--rw-rw-rw-   0        0        0    14974 2022-11-04 19:34:21.000000 mini_afsd-1.1.1/mini_afsd/controller.py
--rw-rw-rw-   0        0        0    38584 2023-01-27 16:07:59.000000 mini_afsd-1.1.1/mini_afsd/gui.py
--rw-rw-rw-   0        0        0     8346 2023-01-27 15:57:02.000000 mini_afsd-1.1.1/mini_afsd/labjack_handler.py
--rw-rw-rw-   0        0        0    22848 2023-01-26 21:06:07.000000 mini_afsd-1.1.1/mini_afsd/serial_processor.py
-drwxrwxrwx   0        0        0        0 2023-03-14 18:24:52.739811 mini_afsd-1.1.1/mini_afsd.egg-info/
--rw-rw-rw-   0        0        0     5823 2023-03-14 18:24:52.000000 mini_afsd-1.1.1/mini_afsd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-03-14 18:24:52.000000 mini_afsd-1.1.1/mini_afsd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 18:24:52.000000 mini_afsd-1.1.1/mini_afsd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-04 19:43:09.000000 mini_afsd-1.1.1/mini_afsd.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2023-03-14 18:24:52.000000 mini_afsd-1.1.1/mini_afsd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-14 18:24:52.000000 mini_afsd-1.1.1/mini_afsd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2022-09-07 17:45:49.000000 mini_afsd-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1625 2023-03-14 18:24:52.754772 mini_afsd-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:47.769534 mini_afsd-1.2.0/
+-rw-rw-rw-   0        0        0      527 2022-09-07 17:45:49.000000 mini_afsd-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      346 2022-09-07 17:45:49.000000 mini_afsd-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5610 2023-04-26 16:17:47.770789 mini_afsd-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4537 2023-04-18 19:34:45.000000 mini_afsd-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:47.698102 mini_afsd-1.2.0/mini_afsd/
+-rw-rw-rw-   0        0        0      436 2023-04-26 16:16:07.000000 mini_afsd-1.2.0/mini_afsd/__init__.py
+-rw-rw-rw-   0        0        0     2994 2022-11-10 15:57:17.000000 mini_afsd-1.2.0/mini_afsd/__main__.py
+-rw-rw-rw-   0        0        0    14974 2022-11-04 19:34:21.000000 mini_afsd-1.2.0/mini_afsd/controller.py
+-rw-rw-rw-   0        0        0    39925 2023-04-26 16:12:11.000000 mini_afsd-1.2.0/mini_afsd/gui.py
+-rw-rw-rw-   0        0        0     8346 2023-01-27 15:57:02.000000 mini_afsd-1.2.0/mini_afsd/labjack_handler.py
+-rw-rw-rw-   0        0        0    22848 2023-01-26 21:06:07.000000 mini_afsd-1.2.0/mini_afsd/serial_processor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:47.761472 mini_afsd-1.2.0/mini_afsd.egg-info/
+-rw-rw-rw-   0        0        0     5610 2023-04-26 16:17:47.000000 mini_afsd-1.2.0/mini_afsd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-04-26 16:17:47.000000 mini_afsd-1.2.0/mini_afsd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:17:47.000000 mini_afsd-1.2.0/mini_afsd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-04 19:43:09.000000 mini_afsd-1.2.0/mini_afsd.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-04-26 16:17:47.000000 mini_afsd-1.2.0/mini_afsd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 16:17:47.000000 mini_afsd-1.2.0/mini_afsd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2022-09-07 17:45:49.000000 mini_afsd-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1625 2023-04-26 16:17:47.778239 mini_afsd-1.2.0/setup.cfg
```

### Comparing `mini_afsd-1.1.1/LICENSE.txt` & `mini_afsd-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mini_afsd-1.1.1/PKG-INFO` & `mini_afsd-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini_afsd
-Version: 1.1.1
+Version: 1.2.0
 Summary: A program for controlling a miniturized additive friction stir deposition (AFSD) machine.
 Home-page: https://github.com/RyTheGuy355/MiniAFSDCode
 Author: Ryan Gottwald
 Maintainer: Donald Erb
 Maintainer-email: derb15@vt.edu
 Project-URL: Source Code, https://github.com/RyTheGuy355/MiniAFSDCode
 Project-URL: Documentation, https://mini_afsd.readthedocs.io
@@ -26,15 +26,14 @@
 =========
 mini_afsd
 =========
 
 mini_afsd is a program for controlling a miniturized additive friction stir deposition (AFSD) machine.
 
 * For Python 3.7+
-* Open Source: BSD 3-Clause License
 * Source Code: https://github.com/RyTheGuy355/MiniAFSDCode
 
 
 .. contents:: **Contents**
     :depth: 1
 
 
@@ -104,15 +103,15 @@
 ~~~~~~~~~~~~~~
 
 mini_afsd can be installed from `pypi <https://pypi.org/project/mini_afsd>`_
 using `pip <https://pip.pypa.io>`_, by running the following command in the terminal:
 
 .. code-block:: console
 
-    pip install mini_afsd
+    pip install -U mini_afsd
 
 
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 The sources for mini_afsd can be downloaded from the `GitHub repo`_.
 To install the current version of mini_afsd from GitHub, run:
@@ -166,22 +165,14 @@
 Contributions are welcomed and greatly appreciated. For information on
 submitting bug reports, pull requests, or general feedback, please refer
 to the `contributing guide`_.
 
 .. _contributing guide: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/docs/contributing.rst
 
 
-Changelog
----------
-
-Refer to the changelog_ for information on mini_afsd's changes.
-
-.. _changelog: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/CHANGELOG.rst
-
-
 License
 -------
 
 mini_afsd is all rights reserved. For more information, refer to the license_.
 
 .. _license: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/LICENSE.txt
```

### Comparing `mini_afsd-1.1.1/README.rst` & `mini_afsd-1.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 =========
 mini_afsd
 =========
 
 mini_afsd is a program for controlling a miniturized additive friction stir deposition (AFSD) machine.
 
 * For Python 3.7+
-* Open Source: BSD 3-Clause License
 * Source Code: https://github.com/RyTheGuy355/MiniAFSDCode
 
 
 .. contents:: **Contents**
     :depth: 1
 
 
@@ -79,15 +78,15 @@
 ~~~~~~~~~~~~~~
 
 mini_afsd can be installed from `pypi <https://pypi.org/project/mini_afsd>`_
 using `pip <https://pip.pypa.io>`_, by running the following command in the terminal:
 
 .. code-block:: console
 
-    pip install mini_afsd
+    pip install -U mini_afsd
 
 
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 The sources for mini_afsd can be downloaded from the `GitHub repo`_.
 To install the current version of mini_afsd from GitHub, run:
@@ -141,22 +140,14 @@
 Contributions are welcomed and greatly appreciated. For information on
 submitting bug reports, pull requests, or general feedback, please refer
 to the `contributing guide`_.
 
 .. _contributing guide: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/docs/contributing.rst
 
 
-Changelog
----------
-
-Refer to the changelog_ for information on mini_afsd's changes.
-
-.. _changelog: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/CHANGELOG.rst
-
-
 License
 -------
 
 mini_afsd is all rights reserved. For more information, refer to the license_.
 
 .. _license: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/LICENSE.txt
```

### Comparing `mini_afsd-1.1.1/mini_afsd/__main__.py` & `mini_afsd-1.2.0/mini_afsd/__main__.py`

 * *Files identical despite different names*

### Comparing `mini_afsd-1.1.1/mini_afsd/controller.py` & `mini_afsd-1.2.0/mini_afsd/controller.py`

 * *Files identical despite different names*

### Comparing `mini_afsd-1.1.1/mini_afsd/gui.py` & `mini_afsd-1.2.0/mini_afsd/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,26 @@
             bg="#91ceff",
             fg="black",
             relief="raised",
             command=lambda: self.sendCode(b"$H", False)
         )
         homeAllBut.grid(column=4, row=5, in_=posFrame, pady=5, rowspan=2, sticky=tk.NS)
 
+        resetOffsetBut = tk.Button(
+            text="Reset &\nOffset",
+            font=("Times New Roman", 12),
+            width=7,
+            pady=5,
+            bg="#91ceff",
+            fg="black",
+            relief="raised",
+            command=self.reset_and_offset,
+        )
+        resetOffsetBut.grid(column=3, row=5, in_=posFrame, pady=5, rowspan=2, sticky=tk.NS)
+
         self.cancelJogBut = tk.Button(
             text="Cancel Jog",
             font=("Times New Roman bold", 12),
             bg="#8efa8e",
             fg="black",
             command=lambda: self.sendCode(b'\x85', False),
         )
@@ -1066,7 +1078,27 @@
         Parameters
         ----------
         axis : {b'X', b'Y', b'Z', b'A'}
             The byte designating which axis to zero.
         """
         if self.controller.serial_processor.esp is not None:
             self.controller.serial_processor.zeroCord(axis)
+
+    def reset_and_offset(self):
+        """Resets the mill and then reapplies the current offsets.
+
+        Needed since FluidNC will reset the offsets when the mill is reset, so use
+        this to not lose the old offsets.
+        """
+        if self.controller.serial_processor.esp is not None:
+            # copy so that the values do not update while using
+            current_offsets = self.controller.serial_processor.work_offsets.copy()
+            current_position = (
+                float(self.xAbsVar.get()) - current_offsets[0],
+                float(self.yAbsVar.get()) - current_offsets[1],
+                float(self.zAbsVar.get()) - current_offsets[2],
+                float(self.aAbsVar.get()) - current_offsets[3],
+            )
+
+            self.sendCode(b'\x18', False),
+            self.sendCode(b'$X', False),
+            self.sendCode('G92 X{0} Y{1} Z{2} A{3}'.format(*current_position).encode(), False)
```

### Comparing `mini_afsd-1.1.1/mini_afsd/labjack_handler.py` & `mini_afsd-1.2.0/mini_afsd/labjack_handler.py`

 * *Files identical despite different names*

### Comparing `mini_afsd-1.1.1/mini_afsd/serial_processor.py` & `mini_afsd-1.2.0/mini_afsd/serial_processor.py`

 * *Files identical despite different names*

### Comparing `mini_afsd-1.1.1/mini_afsd.egg-info/PKG-INFO` & `mini_afsd-1.2.0/mini_afsd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-afsd
-Version: 1.1.1
+Version: 1.2.0
 Summary: A program for controlling a miniturized additive friction stir deposition (AFSD) machine.
 Home-page: https://github.com/RyTheGuy355/MiniAFSDCode
 Author: Ryan Gottwald
 Maintainer: Donald Erb
 Maintainer-email: derb15@vt.edu
 Project-URL: Source Code, https://github.com/RyTheGuy355/MiniAFSDCode
 Project-URL: Documentation, https://mini_afsd.readthedocs.io
@@ -26,15 +26,14 @@
 =========
 mini_afsd
 =========
 
 mini_afsd is a program for controlling a miniturized additive friction stir deposition (AFSD) machine.
 
 * For Python 3.7+
-* Open Source: BSD 3-Clause License
 * Source Code: https://github.com/RyTheGuy355/MiniAFSDCode
 
 
 .. contents:: **Contents**
     :depth: 1
 
 
@@ -104,15 +103,15 @@
 ~~~~~~~~~~~~~~
 
 mini_afsd can be installed from `pypi <https://pypi.org/project/mini_afsd>`_
 using `pip <https://pip.pypa.io>`_, by running the following command in the terminal:
 
 .. code-block:: console
 
-    pip install mini_afsd
+    pip install -U mini_afsd
 
 
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 The sources for mini_afsd can be downloaded from the `GitHub repo`_.
 To install the current version of mini_afsd from GitHub, run:
@@ -166,22 +165,14 @@
 Contributions are welcomed and greatly appreciated. For information on
 submitting bug reports, pull requests, or general feedback, please refer
 to the `contributing guide`_.
 
 .. _contributing guide: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/docs/contributing.rst
 
 
-Changelog
----------
-
-Refer to the changelog_ for information on mini_afsd's changes.
-
-.. _changelog: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/CHANGELOG.rst
-
-
 License
 -------
 
 mini_afsd is all rights reserved. For more information, refer to the license_.
 
 .. _license: https://github.com/RyTheGuy355/MiniAFSDCode/tree/main/LICENSE.txt
```

### Comparing `mini_afsd-1.1.1/setup.cfg` & `mini_afsd-1.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 696e 695f 6166 7364 0d0a 7665   = mini_afsd..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 310d 0a61  rsion = 1.1.1..a
+00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
 00000030: 7574 686f 7220 3d20 5279 616e 2047 6f74  uthor = Ryan Got
 00000040: 7477 616c 640d 0a6d 6169 6e74 6169 6e65  twald..maintaine
 00000050: 7220 3d20 446f 6e61 6c64 2045 7262 0d0a  r = Donald Erb..
 00000060: 6d61 696e 7461 696e 6572 5f65 6d61 696c  maintainer_email
 00000070: 203d 2064 6572 6231 3540 7674 2e65 6475   = derb15@vt.edu
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 4120 7072 6f67 7261 6d20 666f 7220 636f  A program for co
```

