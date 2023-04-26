# Comparing `tmp/pts_fug_hvpsu-0.1.1.tar.gz` & `tmp/pts_fug_hvpsu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fug_hvpsu-0.1.1.tar", last modified: Tue Apr  4 10:23:31 2023, max compression
+gzip compressed data, was "dist/pts_fug_hvpsu-0.1.2.tar", last modified: Wed Apr 26 11:38:02 2023, max compression
```

## Comparing `pts_fug_hvpsu-0.1.1.tar` & `pts_fug_hvpsu-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     3077 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-04 10:23:20.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-04-04 10:23:20.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu/fug_hvpsu.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-04-04 10:23:20.000000 pts_fug_hvpsu-0.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-04 10:23:20.000000 pts_fug_hvpsu-0.1.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-04 10:23:20.000000 pts_fug_hvpsu-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3077 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/pts_fug_hvpsu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 10:23:31.000000 pts_fug_hvpsu-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-26 11:37:52.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-26 11:37:52.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu/fug_hvpsu.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-04-26 11:37:52.000000 pts_fug_hvpsu-0.1.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-26 11:37:52.000000 pts_fug_hvpsu-0.1.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-26 11:37:52.000000 pts_fug_hvpsu-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/pts_fug_hvpsu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:38:02.000000 pts_fug_hvpsu-0.1.2/setup.cfg
```

### Comparing `pts_fug_hvpsu-0.1.1/PKG-INFO` & `pts_fug_hvpsu-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fug_hvpsu
-Version: 0.1.1
+Version: 0.1.2
 Summary: FUG HV PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/fug-power-supply
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fug_hvpsu-0.1.1/pts_fug_hvpsu/fug_hvpsu.py` & `pts_fug_hvpsu-0.1.2/pts_fug_hvpsu/fug_hvpsu.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import socket
 import os
 
 
 class FugHVPsu:
     """
-    Base class for the FUG HV PSU
+    ``Base class for the FUG HV PSU``
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%Y-%m-%d %H:%M:%S',
                         level=logging.INFO)
 
     def __init__(self, connection_string = None, port = 2101):
         if not connection_string:
@@ -18,139 +18,139 @@
         else:
             self.connection_string = connection_string
         self.port = port
         self.sock = None
 
     def open_connection(self):
         """
-        Opens a TCP/IP connection to connect to the FUG HV PSU
+        ``Opens a TCP/IP connection to connect to the FUG HV PSU``
         """
         try:
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.connect((self.connection_string, self.port))
             logging.info(f": Opening FUG HV PSU connection at {self.connection_string} and port {self.port}")
         except Exception as e:
             raise Exception(f": ERROR {e}: Could not open connection")
 
     def close_connection(self):
         """
-        Closes the TCP/IP connection to the FUG HV PSU
+        ``Closes the TCP/IP connection to the FUG HV PSU``
         """
         self.sock.close()
         logging.info(": Closing TCP/IP connection!")
 
     def query_data(self):
         """
-        This command queries the FuG PSU identity data
-        :return: str: PSU Data
+        ``This command queries the FuG PSU identity data`` \n
+        :return: `str` : PSU Data
         """
         self.sock.send(b'? \n')
         time.sleep(0.3)
         query_data = self.sock.recv(1024)
         logging.info(f": Data: {query_data.decode()}")
         return str(query_data.decode())
 
     def clear_device(self):
         """
-        This command clears the initialization data.
-        :return: str: Error code for the command
+        ``This command clears the initialization data.`` \n
+        :return: `str` : Error code for the command
         """
         self.sock.send(b'= \n')
         time.sleep(0.3)
         clr = self.sock.recv(1024).decode().rstrip()
         if clr == 'E0':
             logging.info(f": Cleared Device: {clr}")
             return str(clr)
         else:
             raise Exception(f": ERROR {clr}: Clearing device ")
 
     def identification_number(self):
         """
-        This command checks the identification number
-        :return: str: Identification number
+        ``This command checks the identification number`` \n
+        :return: `str` : Identification number
         """
         self.sock.send(b'*IDN? \n')
         time.sleep(0.3)
         idn = self.sock.recv(1024)
         logging.info(f": Identification number: {idn.decode()}")
         return str(idn.decode())
 
     def enable_output(self):
         """
-        This command enables the output
-        :return: str: Error code for the command
+        ``This command enables the output`` \n
+        :return: `str` : Error code for the command
         """
         self.sock.send(b'F1 \n')
         time.sleep(0.3)
         op_on = str(self.sock.recv(1024).decode().rstrip())
         if op_on == 'E0':
             logging.info(f": Output Enabled: {op_on}")
             return str(op_on)
         else:
             raise Exception(f": ERROR {op_on}: Enabling output ")
 
     def disable_output(self):
         """
-        This command disables the output
-        :return: str: Error code for the command
+        ``This command disables the output`` \n
+        :return: `str` : Error code for the command
         """
         self.sock.send(b'F0 \n')
         time.sleep(0.3)
         op_off = self.sock.recv(1024).decode().rstrip()
         if op_off == 'E0':
             logging.info(f": Output Disabled: {op_off}")
             return str(op_off)
         else:
             raise Exception(f": ERROR {op_off}: Disabling output")
 
     def set_voltage(self, volt):
         """
-        This command will set the output voltage in Volts
-        :param volt: output voltage in Volts
-        :return: str: Error code for the command
+        ``This command will set the output voltage in Volts`` \n
+        :param: `float`: volt: output voltage in Volts \n
+        :return: `str` : Error code for the command
         """
         b_volt = 'U'+str(volt)
         self.sock.send(b_volt.encode()+b'\n')
         time.sleep(0.3)
         voltage = self.sock.recv(1024).decode().rstrip()
         if voltage == 'E0':
             logging.info(f": Voltage set: {voltage}")
             return str(voltage)
         else:
             raise Exception(f": ERROR {voltage}: Setting Voltage ")
 
     def set_current(self, curr_limit):
         """
-        This command will set the output current in milliAmps
-        :param curr_limit: current limit in milliAmps
-        :return: str: Error code for the command
+        ``This command will set the output current in milliAmps`` \n
+        :param: `float` : curr_limit: current limit in Amps \n
+        :return: `str` : Error code for the command
         """
         b_curr = 'I'+str(curr_limit)
         self.sock.send(b_curr.encode()+b'\n')
         time.sleep(0.3)
         current = self.sock.recv(1024).decode().rstrip()
         if current == 'E0':
             logging.info(f": Current limit set: {current}")
             return str(current)
         else:
             raise Exception(f": ERROR {current}: Setting Current limit ")
 
     def measure_voltage(self):
         """
-        This function measures output voltage
-        :return: float: Programmed output voltage in Volts
+        ``This function measures output voltage`` \n
+        :return: `float` : Programmed output voltage in Volts
         """
         self.sock.send(b'>M0? \n')
         meas_volt = self.sock.recv(1024).decode().rstrip().split(":")[-1]
         logging.info(f": Output Voltage: {meas_volt} Volts")
         return float(meas_volt)
 
     def measure_current(self):
         """
-        This function measures output current
-        :return: float: Programmed output Current in milliAmps
+        ``This function measures output current`` \n
+        :return: `float` : Programmed output Current in milliAmps
         """
         self.sock.send(b'>M1? \n')
         meas_curr = self.sock.recv(1024).decode().rstrip().split(":")[-1]
         logging.info(f": Output Current: {meas_curr} Amps")
         return float(meas_curr)
```

### Comparing `pts_fug_hvpsu-0.1.1/setup.py` & `pts_fug_hvpsu-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fug_hvpsu",
-    version='0.1.1',
+    version='0.1.2',
     author="Pass testing Solutions GmbH",
     description="FUG HV PSU Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/fug-power-supply",
     license="MIT",
```

### Comparing `pts_fug_hvpsu-0.1.1/LICENSE.txt` & `pts_fug_hvpsu-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fug_hvpsu-0.1.1/README.md` & `pts_fug_hvpsu-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pts_fug_hvpsu-0.1.1/pts_fug_hvpsu.egg-info/PKG-INFO` & `pts_fug_hvpsu-0.1.2/pts_fug_hvpsu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fug-hvpsu
-Version: 0.1.1
+Version: 0.1.2
 Summary: FUG HV PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/fug-power-supply
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

