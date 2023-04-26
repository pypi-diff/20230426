# Comparing `tmp/alicat-0.4.1.tar.gz` & `tmp/alicat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicat-0.4.1.tar", last modified: Tue Feb 28 21:18:54 2023, max compression
+gzip compressed data, was "alicat-0.5.0.tar", last modified: Tue Apr 25 18:14:39 2023, max compression
```

## Comparing `alicat-0.4.1.tar` & `alicat-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 21:18:54.316367 alicat-0.4.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       43 2022-01-04 06:44:03.000000 alicat-0.4.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2021-09-30 16:03:53.000000 alicat-0.4.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5139 2023-02-28 21:18:54.316449 alicat-0.4.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4531 2022-04-04 13:28:47.000000 alicat-0.4.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 21:18:54.315509 alicat-0.4.1/alicat/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2698 2023-02-27 03:43:06.000000 alicat-0.4.1/alicat/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1534 2023-02-27 03:43:06.000000 alicat-0.4.1/alicat/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    21517 2023-02-28 21:16:40.000000 alicat-0.4.1/alicat/serial.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 21:18:54.316230 alicat-0.4.1/alicat.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5139 2023-02-28 21:18:54.000000 alicat-0.4.1/alicat.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      280 2023-02-28 21:18:54.000000 alicat-0.4.1/alicat.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-02-28 21:18:54.000000 alicat-0.4.1/alicat.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       38 2023-02-28 21:18:54.000000 alicat-0.4.1/alicat.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        9 2023-02-28 21:18:54.000000 alicat-0.4.1/alicat.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-02-28 21:18:54.000000 alicat-0.4.1/alicat.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      152 2023-02-28 21:18:54.316663 alicat-0.4.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)      980 2023-02-28 21:18:15.000000 alicat-0.4.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.202353 alicat-0.5.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-04-12 17:39:23.000000 alicat-0.5.0/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2023-04-12 01:08:23.000000 alicat-0.5.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5725 2023-04-25 18:14:39.202454 alicat-0.5.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4894 2023-04-12 17:39:23.000000 alicat-0.5.0/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.201067 alicat-0.5.0/alicat/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4570 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18579 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2881 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     7932 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.202090 alicat-0.5.0/alicat.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5725 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      332 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      126 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      136 2023-04-25 18:14:39.202704 alicat-0.5.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1536 2023-04-25 18:10:43.000000 alicat-0.5.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.202218 alicat-0.5.0/tests/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2142 2023-04-25 18:10:19.000000 alicat-0.5.0/tests/test_driver.py
```

### Comparing `alicat-0.4.1/LICENSE` & `alicat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicat-0.4.1/PKG-INFO` & `alicat-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: alicat
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python driver for Alicat mass flow controllers.
 Home-page: https://github.com/numat/alicat/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 alicat
 ======
 
-Serial driver and command line tool for
+TCP/Serial driver and command line tool for
 [Alicat mass flow controllers](http://www.alicat.com/products/mass-flow-meters-and-controllers/mass-flow-controllers/).
 
 <p align="center">
   <img src="http://www.alicat.com/wpinstall/wp-content/uploads/2012/01/gas-mass-flow-controller1.jpg" height="400" />
 </p>
 
 *If you are using Analyt-MTC flow controllers, go to [this repository](https://github.com/schlenzmeister/AnalytMTC/wiki) for more info.*
@@ -31,14 +36,15 @@
 ===================
 
 | Type | Usage |
 | --- | --- |
 | The standard [DB9 cable](http://www.alicat.com/wpinstall/wp-content/uploads/2013/07/MD8DB9.jpg) connected directly to a computer (unix: `/dev/ttyS0`, windows: `COM1`). | Good with older computers that still have the connector. |
 | The cable connected to a computer through a [USB converter](https://www.amazon.com/gp/product/B0007T27H8) (unix: `/dev/ttyUSB0`, windows: `COM1`). | Good for newer computers and maker boards such as Raspberry Pis. |
 | Multiple cables connected to one port via a [splitter](https://www.amazon.com/gp/product/B007F2E188) and Alicat's addressing (`A`-`Z`). | Good when number of ports is limited. |
+| Cables routed through a [TCP device server](https://www.usconverters.com/serial-rs232-ethernet-converter) (`192.168.1.100:23`).
 
 Installation
 ============
 
 ```
 pip install alicat
 ```
@@ -52,21 +58,25 @@
 for more.
 
 ```
 alicat --help
 ```
 
 ## Python
-
-For more complex projects, use python to automate your workflow.
+This uses Python ≥3.5's async/await syntax to asynchronously communicate with an Alicat. For example:
 
 ```python
+import asyncio
 from alicat import FlowController
-flow_controller = FlowController(port='/dev/ttyUSB0')
-print(flow_controller.get())
+
+async def get():
+    async with FlowController('ip-address:port') as flow_controller:
+        print(await flow_controller.get())
+
+asyncio.run(get())
 ```
 
 If the flow controller is communicating on the specified port, this should
 return a dictionary of the form:
 
 ```python
 {
@@ -80,83 +90,82 @@
   'volumetric_flow': 0.0   # Volumetric flow (in units specified at time of purchase)
 }
 ```
 
 On flow controllers, you can set the flow or pressure setpoints.
 
 ```python
-flow_controller.set_flow_rate(1.0)
-flow_controller.set_pressure(20)
+await flow_controller.set_flow_rate(1.0)
+await flow_controller.set_pressure(20)
 ```
 
 ### Gas Type
 
 You can set the gas type by name or by index. For more on setting by index, see the gas table in your Alicat's manual.
 
 ```python
-flow_controller.set_gas('N2')
-flow_controller.set_gas(8)
+await flow_controller.set_gas('N2')
+await flow_controller.set_gas(8)
 ```
 
 For firmware 5v and greater, you can create and set gas mixes. Mixes can contain up to five gases and are stored in gas indices 236-255.
 
 ```python
-flow_controller.create_mix(mix_no=236, name="Mix1", gases={'N2': 50, 'O2': 30, 'CO2': 20})
-flow_controller.set_gas(236)
-flow_controller.delete_mix(236)
+await flow_controller.create_mix(mix_no=236, name="Mix1", gases={'N2': 50, 'O2': 30, 'CO2': 20})
+await flow_controller.set_gas(236)
+await flow_controller.delete_mix(236)
 ```
 
 ### PID Parameters
 
 For flow controllers, read and write PID loop settings for device tuning.
 
 ```python
-flow_controller.set_pid(p=4000, i=4000, d=10, loop_type='PD2I')
-print(flow_controller.get_pid())
+await flow_controller.set_pid(p=4000, i=4000, d=10, loop_type='PD2I')
+print(await flow_controller.get_pid())
 {
     'loop_type': 'PD2I',
     'P': '4000',
     'I': '4000',
     'D': '10',
 }
 ```
 
 ### Other Features
 
 Additional features include override commands to increase device functionality.
 
 ```python
-flow_controller.lock()            # Lock the front display.
-flow_controller.unlock()          # Unlock the front display.
-flow_controller.hold()            # Hold the valve in its current position.
-flow_controller.cancel_hold()     # Cancel the valve hold.
-flow_controller.tare_volumetric() # Tare volumetric flow.
-flow_controller.tare_pressure()   # Tare pressure.
-flow_controller.reset_totalizer() # Reset totalizer, if totalizer functionality included.
+await flow_controller.lock()            # Lock the front display.
+await flow_controller.unlock()          # Unlock the front display.
+await flow_controller.hold()            # Hold the valve in its current position.
+await flow_controller.cancel_hold()     # Cancel the valve hold.
+await flow_controller.tare_volumetric() # Tare volumetric flow.
+await flow_controller.tare_pressure()   # Tare pressure.
+await flow_controller.reset_totalizer() # Reset totalizer, if totalizer functionality included.
 ```
 
 ### Addressing
 
 You can have multiple controllers on the same port by using Alicat's `A`-`Z` addresses
 and an [RS-232 splitter](https://www.amazon.com/gp/product/B007F2E188).
 
 ```python
 flow_controller_1 = FlowController(address='A')
 flow_controller_2 = FlowController(address='B')
 
-flow_controller_1.set_flow_rate(1.0)
-flow_controller_2.set_flow_rate(0.5)
+await flow_controller_1.set_flow_rate(1.0)
+await flow_controller_2.set_flow_rate(0.5)
 
-flow_controller_1.close() # /dev/ttyUSB0 is still open!
-flow_controller_2.close()
+await flow_controller_1.close() # /dev/ttyUSB0 is still open!
+await flow_controller_2.close()
 ```
 
-TCP Support
-===
+### Breaking changes
 
-The last version with working TCP support is [here](https://github.com/numat/alicat/tree/8af92647cb396401c0d604d83fb95a49d9a82be9) and can be installed with:
-
-```
-pip install alicat==0.3.1
-```
+`0.5.0`
+- Support only `asyncio`.  The last version with synchronous code was `0.4.1`.
+- Rename `address`/`-a` to `unit`/`-u` to match Alicat's documentation
+- Rename `-u` to `-ul` (for `--unlock`)
 
-If you use the TCP driver, please let us know and we'll add it back to the current version.
+`0.4.1`
+Remove TCP support.  Use `pip install alicat==0.3.1` if needed
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alicat-0.4.1/README.md` & `alicat-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 alicat
 ======
 
-Serial driver and command line tool for
+TCP/Serial driver and command line tool for
 [Alicat mass flow controllers](http://www.alicat.com/products/mass-flow-meters-and-controllers/mass-flow-controllers/).
 
 <p align="center">
   <img src="http://www.alicat.com/wpinstall/wp-content/uploads/2012/01/gas-mass-flow-controller1.jpg" height="400" />
 </p>
 
 *If you are using Analyt-MTC flow controllers, go to [this repository](https://github.com/schlenzmeister/AnalytMTC/wiki) for more info.*
@@ -14,14 +14,15 @@
 ===================
 
 | Type | Usage |
 | --- | --- |
 | The standard [DB9 cable](http://www.alicat.com/wpinstall/wp-content/uploads/2013/07/MD8DB9.jpg) connected directly to a computer (unix: `/dev/ttyS0`, windows: `COM1`). | Good with older computers that still have the connector. |
 | The cable connected to a computer through a [USB converter](https://www.amazon.com/gp/product/B0007T27H8) (unix: `/dev/ttyUSB0`, windows: `COM1`). | Good for newer computers and maker boards such as Raspberry Pis. |
 | Multiple cables connected to one port via a [splitter](https://www.amazon.com/gp/product/B007F2E188) and Alicat's addressing (`A`-`Z`). | Good when number of ports is limited. |
+| Cables routed through a [TCP device server](https://www.usconverters.com/serial-rs232-ethernet-converter) (`192.168.1.100:23`).
 
 Installation
 ============
 
 ```
 pip install alicat
 ```
@@ -35,21 +36,25 @@
 for more.
 
 ```
 alicat --help
 ```
 
 ## Python
-
-For more complex projects, use python to automate your workflow.
+This uses Python ≥3.5's async/await syntax to asynchronously communicate with an Alicat. For example:
 
 ```python
+import asyncio
 from alicat import FlowController
-flow_controller = FlowController(port='/dev/ttyUSB0')
-print(flow_controller.get())
+
+async def get():
+    async with FlowController('ip-address:port') as flow_controller:
+        print(await flow_controller.get())
+
+asyncio.run(get())
 ```
 
 If the flow controller is communicating on the specified port, this should
 return a dictionary of the form:
 
 ```python
 {
@@ -63,83 +68,82 @@
   'volumetric_flow': 0.0   # Volumetric flow (in units specified at time of purchase)
 }
 ```
 
 On flow controllers, you can set the flow or pressure setpoints.
 
 ```python
-flow_controller.set_flow_rate(1.0)
-flow_controller.set_pressure(20)
+await flow_controller.set_flow_rate(1.0)
+await flow_controller.set_pressure(20)
 ```
 
 ### Gas Type
 
 You can set the gas type by name or by index. For more on setting by index, see the gas table in your Alicat's manual.
 
 ```python
-flow_controller.set_gas('N2')
-flow_controller.set_gas(8)
+await flow_controller.set_gas('N2')
+await flow_controller.set_gas(8)
 ```
 
 For firmware 5v and greater, you can create and set gas mixes. Mixes can contain up to five gases and are stored in gas indices 236-255.
 
 ```python
-flow_controller.create_mix(mix_no=236, name="Mix1", gases={'N2': 50, 'O2': 30, 'CO2': 20})
-flow_controller.set_gas(236)
-flow_controller.delete_mix(236)
+await flow_controller.create_mix(mix_no=236, name="Mix1", gases={'N2': 50, 'O2': 30, 'CO2': 20})
+await flow_controller.set_gas(236)
+await flow_controller.delete_mix(236)
 ```
 
 ### PID Parameters
 
 For flow controllers, read and write PID loop settings for device tuning.
 
 ```python
-flow_controller.set_pid(p=4000, i=4000, d=10, loop_type='PD2I')
-print(flow_controller.get_pid())
+await flow_controller.set_pid(p=4000, i=4000, d=10, loop_type='PD2I')
+print(await flow_controller.get_pid())
 {
     'loop_type': 'PD2I',
     'P': '4000',
     'I': '4000',
     'D': '10',
 }
 ```
 
 ### Other Features
 
 Additional features include override commands to increase device functionality.
 
 ```python
-flow_controller.lock()            # Lock the front display.
-flow_controller.unlock()          # Unlock the front display.
-flow_controller.hold()            # Hold the valve in its current position.
-flow_controller.cancel_hold()     # Cancel the valve hold.
-flow_controller.tare_volumetric() # Tare volumetric flow.
-flow_controller.tare_pressure()   # Tare pressure.
-flow_controller.reset_totalizer() # Reset totalizer, if totalizer functionality included.
+await flow_controller.lock()            # Lock the front display.
+await flow_controller.unlock()          # Unlock the front display.
+await flow_controller.hold()            # Hold the valve in its current position.
+await flow_controller.cancel_hold()     # Cancel the valve hold.
+await flow_controller.tare_volumetric() # Tare volumetric flow.
+await flow_controller.tare_pressure()   # Tare pressure.
+await flow_controller.reset_totalizer() # Reset totalizer, if totalizer functionality included.
 ```
 
 ### Addressing
 
 You can have multiple controllers on the same port by using Alicat's `A`-`Z` addresses
 and an [RS-232 splitter](https://www.amazon.com/gp/product/B007F2E188).
 
 ```python
 flow_controller_1 = FlowController(address='A')
 flow_controller_2 = FlowController(address='B')
 
-flow_controller_1.set_flow_rate(1.0)
-flow_controller_2.set_flow_rate(0.5)
+await flow_controller_1.set_flow_rate(1.0)
+await flow_controller_2.set_flow_rate(0.5)
 
-flow_controller_1.close() # /dev/ttyUSB0 is still open!
-flow_controller_2.close()
+await flow_controller_1.close() # /dev/ttyUSB0 is still open!
+await flow_controller_2.close()
 ```
 
-TCP Support
-===
+### Breaking changes
 
-The last version with working TCP support is [here](https://github.com/numat/alicat/tree/8af92647cb396401c0d604d83fb95a49d9a82be9) and can be installed with:
-
-```
-pip install alicat==0.3.1
-```
+`0.5.0`
+- Support only `asyncio`.  The last version with synchronous code was `0.4.1`.
+- Rename `address`/`-a` to `unit`/`-u` to match Alicat's documentation
+- Rename `-u` to `-ul` (for `--unlock`)
 
-If you use the TCP driver, please let us know and we'll add it back to the current version.
+`0.4.1`
+Remove TCP support.  Use `pip install alicat==0.3.1` if needed
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alicat-0.4.1/alicat/__init__.py` & `alicat-0.5.0/alicat/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Python driver for Alicat mass flow controllers.
 
 Distributed under the GNU General Public License v2
-Copyright (C) 2019 NuMat Technologies
+Copyright (C) 2023 NuMat Technologies
 """
-from alicat.serial import FlowController, FlowMeter, command_line  # noqa
+from typing import Any
 
+from alicat.driver import FlowController, FlowMeter  # noqa
 
-def run():
+
+def command_line(args: Any = None) -> None:
     """CLI interface, accessible when installed through pip."""
     import argparse
-
+    import asyncio
+    import json
+    from time import time
     parser = argparse.ArgumentParser(description="Control an Alicat mass "
                                      "flow controller from the command line.")
-    parser.add_argument('port', nargs='?', default='/dev/ttyUSB0', help="The "
-                        "target serial port. Default '/dev/ttyUSB0'.")
-    parser.add_argument('--address', '-a', default='A', type=str, help="The "
-                        "device address, A-Z. Should only be used if multiple "
+    parser.add_argument('address', type=str, default='/dev/ttyUSB0', help="The "
+                        "target serial port (or TCP address:port). Default '/dev/ttyUSB0'.")
+    parser.add_argument('--unit', '-u', default='A', type=str, help="The "
+                        "device unit ID, A-Z. Should only be used if multiple "
                         "flow controllers are connected to one port or if"
                         "device ID is not A.")
     parser.add_argument('--set-gas', '-g', default=None, type=str,
                         help="Sets the gas type. Supported gas types are: "
                              "'Air', 'Ar', 'CH4', 'CO', 'CO2', 'C2H6', 'H2', "
                              "'He', 'N2', 'N2O', 'Ne', 'O2', 'C3H8', "
                              "'n-C4H10', 'C2H2', 'C2H4', 'i-C2H10', 'Kr', "
@@ -31,22 +35,58 @@
     parser.add_argument('--set-pressure', '-p', default=None, type=float,
                         help="Sets the target pressure of the controller.")
     parser.add_argument('--stream', '-s', action='store_true',
                         help="Sends a constant stream of flow controller "
                              "data, formatted as a tab-separated table.")
     parser.add_argument("--lock", "-l", action="store_true",
                         help="Locks device display.")
-    parser.add_argument("--unlock", "-u", action="store_true",
+    parser.add_argument("--unlock", "-ul", action="store_true",
                         help="Unlocks device display.")
     parser.add_argument("--hold", "-hd", action="store_true",
                         help="Holds the valve at the present value.")
     parser.add_argument("--cancel-hold", "-c", action="store_true",
                         help="Cancel valve hold.")
     parser.add_argument("--reset-totalizer", "-r", action="store_true",
                         help="Reset current value of totalizer to zero.")
-    args = parser.parse_args()
+    args = parser.parse_args(args)
+    async def get() -> None:
+        async with FlowController(address=args.address, unit=args.unit) as flow_controller:
+            if args.set_gas:
+                await flow_controller.set_gas(args.set_gas)
+            if args.set_flow_rate is not None and args.set_pressure is not None:
+                raise ValueError("Cannot set both flow rate and pressure.")
+            if args.set_flow_rate is not None:
+                await flow_controller.set_flow_rate(args.set_flow_rate)
+            if args.set_pressure is not None:
+                await flow_controller.set_pressure(args.set_pressure)
+            if args.lock:
+                await flow_controller.lock()
+            if args.unlock:
+                await flow_controller.unlock()
+            if args.hold:
+                await flow_controller.hold()
+            if args.cancel_hold:
+                await flow_controller.cancel_hold()
+            if args.reset_totalizer:
+                await flow_controller.reset_totalizer()
+            state = await flow_controller.get()
+            if args.stream:
+                try:
+                    print('time\t' + '\t'.join(flow_controller.keys))
+                    t0 = time()
+                    while True:
+                        state = await flow_controller.get()
+                        print(f'{time() - t0:.2f}\t' +
+                              '\t\t'.join(f'{state[key]:.2f}'
+                                          for key in flow_controller.keys[:-1]) +
+                              '\t\t' + state['gas'])
+                except KeyboardInterrupt:
+                    pass
+            else:
+                print(json.dumps(state, indent=2, sort_keys=True))
+            await flow_controller.close()
 
-    command_line(args)
+    asyncio.run(get())
 
 
 if __name__ == '__main__':
-    run()
+    command_line()
```

### Comparing `alicat-0.4.1/alicat.egg-info/PKG-INFO` & `alicat-0.5.0/alicat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: alicat
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python driver for Alicat mass flow controllers.
 Home-page: https://github.com/numat/alicat/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 alicat
 ======
 
-Serial driver and command line tool for
+TCP/Serial driver and command line tool for
 [Alicat mass flow controllers](http://www.alicat.com/products/mass-flow-meters-and-controllers/mass-flow-controllers/).
 
 <p align="center">
   <img src="http://www.alicat.com/wpinstall/wp-content/uploads/2012/01/gas-mass-flow-controller1.jpg" height="400" />
 </p>
 
 *If you are using Analyt-MTC flow controllers, go to [this repository](https://github.com/schlenzmeister/AnalytMTC/wiki) for more info.*
@@ -31,14 +36,15 @@
 ===================
 
 | Type | Usage |
 | --- | --- |
 | The standard [DB9 cable](http://www.alicat.com/wpinstall/wp-content/uploads/2013/07/MD8DB9.jpg) connected directly to a computer (unix: `/dev/ttyS0`, windows: `COM1`). | Good with older computers that still have the connector. |
 | The cable connected to a computer through a [USB converter](https://www.amazon.com/gp/product/B0007T27H8) (unix: `/dev/ttyUSB0`, windows: `COM1`). | Good for newer computers and maker boards such as Raspberry Pis. |
 | Multiple cables connected to one port via a [splitter](https://www.amazon.com/gp/product/B007F2E188) and Alicat's addressing (`A`-`Z`). | Good when number of ports is limited. |
+| Cables routed through a [TCP device server](https://www.usconverters.com/serial-rs232-ethernet-converter) (`192.168.1.100:23`).
 
 Installation
 ============
 
 ```
 pip install alicat
 ```
@@ -52,21 +58,25 @@
 for more.
 
 ```
 alicat --help
 ```
 
 ## Python
-
-For more complex projects, use python to automate your workflow.
+This uses Python ≥3.5's async/await syntax to asynchronously communicate with an Alicat. For example:
 
 ```python
+import asyncio
 from alicat import FlowController
-flow_controller = FlowController(port='/dev/ttyUSB0')
-print(flow_controller.get())
+
+async def get():
+    async with FlowController('ip-address:port') as flow_controller:
+        print(await flow_controller.get())
+
+asyncio.run(get())
 ```
 
 If the flow controller is communicating on the specified port, this should
 return a dictionary of the form:
 
 ```python
 {
@@ -80,83 +90,82 @@
   'volumetric_flow': 0.0   # Volumetric flow (in units specified at time of purchase)
 }
 ```
 
 On flow controllers, you can set the flow or pressure setpoints.
 
 ```python
-flow_controller.set_flow_rate(1.0)
-flow_controller.set_pressure(20)
+await flow_controller.set_flow_rate(1.0)
+await flow_controller.set_pressure(20)
 ```
 
 ### Gas Type
 
 You can set the gas type by name or by index. For more on setting by index, see the gas table in your Alicat's manual.
 
 ```python
-flow_controller.set_gas('N2')
-flow_controller.set_gas(8)
+await flow_controller.set_gas('N2')
+await flow_controller.set_gas(8)
 ```
 
 For firmware 5v and greater, you can create and set gas mixes. Mixes can contain up to five gases and are stored in gas indices 236-255.
 
 ```python
-flow_controller.create_mix(mix_no=236, name="Mix1", gases={'N2': 50, 'O2': 30, 'CO2': 20})
-flow_controller.set_gas(236)
-flow_controller.delete_mix(236)
+await flow_controller.create_mix(mix_no=236, name="Mix1", gases={'N2': 50, 'O2': 30, 'CO2': 20})
+await flow_controller.set_gas(236)
+await flow_controller.delete_mix(236)
 ```
 
 ### PID Parameters
 
 For flow controllers, read and write PID loop settings for device tuning.
 
 ```python
-flow_controller.set_pid(p=4000, i=4000, d=10, loop_type='PD2I')
-print(flow_controller.get_pid())
+await flow_controller.set_pid(p=4000, i=4000, d=10, loop_type='PD2I')
+print(await flow_controller.get_pid())
 {
     'loop_type': 'PD2I',
     'P': '4000',
     'I': '4000',
     'D': '10',
 }
 ```
 
 ### Other Features
 
 Additional features include override commands to increase device functionality.
 
 ```python
-flow_controller.lock()            # Lock the front display.
-flow_controller.unlock()          # Unlock the front display.
-flow_controller.hold()            # Hold the valve in its current position.
-flow_controller.cancel_hold()     # Cancel the valve hold.
-flow_controller.tare_volumetric() # Tare volumetric flow.
-flow_controller.tare_pressure()   # Tare pressure.
-flow_controller.reset_totalizer() # Reset totalizer, if totalizer functionality included.
+await flow_controller.lock()            # Lock the front display.
+await flow_controller.unlock()          # Unlock the front display.
+await flow_controller.hold()            # Hold the valve in its current position.
+await flow_controller.cancel_hold()     # Cancel the valve hold.
+await flow_controller.tare_volumetric() # Tare volumetric flow.
+await flow_controller.tare_pressure()   # Tare pressure.
+await flow_controller.reset_totalizer() # Reset totalizer, if totalizer functionality included.
 ```
 
 ### Addressing
 
 You can have multiple controllers on the same port by using Alicat's `A`-`Z` addresses
 and an [RS-232 splitter](https://www.amazon.com/gp/product/B007F2E188).
 
 ```python
 flow_controller_1 = FlowController(address='A')
 flow_controller_2 = FlowController(address='B')
 
-flow_controller_1.set_flow_rate(1.0)
-flow_controller_2.set_flow_rate(0.5)
+await flow_controller_1.set_flow_rate(1.0)
+await flow_controller_2.set_flow_rate(0.5)
 
-flow_controller_1.close() # /dev/ttyUSB0 is still open!
-flow_controller_2.close()
+await flow_controller_1.close() # /dev/ttyUSB0 is still open!
+await flow_controller_2.close()
 ```
 
-TCP Support
-===
+### Breaking changes
 
-The last version with working TCP support is [here](https://github.com/numat/alicat/tree/8af92647cb396401c0d604d83fb95a49d9a82be9) and can be installed with:
-
-```
-pip install alicat==0.3.1
-```
+`0.5.0`
+- Support only `asyncio`.  The last version with synchronous code was `0.4.1`.
+- Rename `address`/`-a` to `unit`/`-u` to match Alicat's documentation
+- Rename `-u` to `-ul` (for `--unlock`)
 
-If you use the TCP driver, please let us know and we'll add it back to the current version.
+`0.4.1`
+Remove TCP support.  Use `pip install alicat==0.3.1` if needed
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

