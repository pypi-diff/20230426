# Comparing `tmp/pts_keysight_dmm-0.0.7.tar.gz` & `tmp/pts_keysight_dmm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_keysight_dmm-0.0.7.tar", last modified: Thu Jan 26 15:11:19 2023, max compression
+gzip compressed data, was "dist/pts_keysight_dmm-0.0.8.tar", last modified: Wed Apr 26 12:43:17 2023, max compression
```

## Comparing `pts_keysight_dmm-0.0.7.tar` & `pts_keysight_dmm-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:11:19.000000 pts_keysight_dmm-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-01-26 15:11:19.000000 pts_keysight_dmm-0.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:11:19.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-01-26 15:11:18.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      291 2023-01-26 15:11:18.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:11:18.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-26 15:11:18.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-01-26 15:11:18.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-01-26 15:11:09.000000 pts_keysight_dmm-0.0.7/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-01-26 15:11:09.000000 pts_keysight_dmm-0.0.7/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-01-26 15:11:09.000000 pts_keysight_dmm-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:11:19.000000 pts_keysight_dmm-0.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:11:19.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-26 15:11:09.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7623 2023-01-26 15:11:09.000000 pts_keysight_dmm-0.0.7/pts_keysight_dmm/keysight_dmm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:43:17.000000 pts_keysight_dmm-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-26 12:43:17.000000 pts_keysight_dmm-0.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:43:17.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-26 12:43:16.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-26 12:43:16.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:43:16.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-26 12:43:16.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-26 12:43:16.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-26 12:43:05.000000 pts_keysight_dmm-0.0.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-26 12:43:05.000000 pts_keysight_dmm-0.0.8/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-26 12:43:05.000000 pts_keysight_dmm-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:43:17.000000 pts_keysight_dmm-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:43:16.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-26 12:43:05.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7786 2023-04-26 12:43:05.000000 pts_keysight_dmm-0.0.8/pts_keysight_dmm/keysight_dmm.py
```

### Comparing `pts_keysight_dmm-0.0.7/PKG-INFO` & `pts_keysight_dmm-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_keysight_dmm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Keysight DMM 34465A Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/keysight34465a-interface
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_keysight_dmm-0.0.7/pts_keysight_dmm.egg-info/PKG-INFO` & `pts_keysight_dmm-0.0.8/pts_keysight_dmm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-keysight-dmm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Keysight DMM 34465A Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/keysight34465a-interface
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_keysight_dmm-0.0.7/setup.py` & `pts_keysight_dmm-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_keysight_dmm",
-    version="0.0.7",
+    version="0.0.8",
     author="Pass testing Solutions GmbH",
     description="Keysight DMM 34465A Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/keysight34465a-interface",
     license="MIT",
```

### Comparing `pts_keysight_dmm-0.0.7/LICENSE.txt` & `pts_keysight_dmm-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_keysight_dmm-0.0.7/README.md` & `pts_keysight_dmm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pts_keysight_dmm-0.0.7/pts_keysight_dmm/keysight_dmm.py` & `pts_keysight_dmm-0.0.8/pts_keysight_dmm/keysight_dmm.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,50 +4,50 @@
 import logging
 
 RANGE = 'AUTO'
 
 
 class KeySight34465A:
     """
-    Base class for the Keysight 34465A DMM
+    ``Base class for the Keysight 34465A DMM``
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%H:%M:%S',
                         level=logging.INFO)
 
     def __init__(self, connection_string):
         self.dmm = None
         self.connection_string = connection_string
         self.resource_manager = None
 
     def open_connection(self):
         """
-        Opens a TCP/IP connection to connect to the Keysight DMM 34465A
+        ``Opens a TCP/IP connection to connect to the Keysight DMM 34465A`` \n
         """
         self.resource_manager = pyvisa.ResourceManager()
         self.connection_string = os.getenv("DMM_CONNECTION_STRING", default='TCPIP0::192.168.123.200::INSTR')
         try:
             logging.info(f": Opening KeysightDMM 34465A Resource at {self.connection_string}")
             self.dmm = self.resource_manager.open_resource(self.connection_string)
             self.dmm.read_termination = '\n'
             self.dmm.write_termination = '\n'
             time.sleep(3)
         except Exception as err:
             raise Exception(f": ERROR {err}: Could not open connection! ")
 
     def close_connection(self):
         """
-        Closes the TCP/IP connection to the Keysight DMM 34465A
+        ``Closes the TCP/IP connection to the Keysight DMM 34465A`` \n
         """
         self.resource_manager.close()
 
     def self_test(self):
         """
-        Performs the self-test and checks for system errors
-        :return: Boolean: True or Error
+        ``Performs the self-test and checks for system errors`` \n
+        :return: `bool` : True or Error
         """
         sys_err = self.dmm.query(f'SYST:ERR?', delay=1)
         if sys_err == '+0,"No error"':
             try:
                 selftest = self.dmm.query(f'TEST:ALL?', delay=1)
                 if selftest == "+0":
                     logging.info("PASS: SELF-TEST PASSED!")
@@ -59,26 +59,26 @@
                 raise Exception(f": ERROR: {e} One or more self-test has FAILED")
         else:
             logging.error(f": SYSTEM_ERROR: {sys_err}")
             raise Exception(f": {sys_err}")
 
     def id_number(self):
         """
-        This function returns the ID number on query in string
-        :return: str: ID number
+        ``This function returns the ID number on query in string`` \n
+        :return: `str` : ID number
         """
         time.sleep(5)
         idn = self.dmm.query(f'*IDN?', delay=1)
         logging.info(f": IDN: {idn} \n")
         return str(idn)
 
     def system_info(self):
         """
-        This function gets all the system info for the Keysight DMM 34465A
-        :return: information in logs
+        ``This function gets all the system info for the Keysight DMM 34465A`` \n
+        :return: Information in logs
         """
 
         sys_ver = self.dmm.query(f'SYST:VERS?', delay=1)
         logging.info(f": System Version: {sys_ver}")
 
         is_dhcp = self.dmm.query(f'SYST:COMM:LAN:DHCP?', delay=1)
         logging.info(f": DHCP Setting: {is_dhcp} \n")
@@ -99,20 +99,20 @@
         logging.info(f": DNS Setting: {dns_setting} \n")
 
         gateway = self.dmm.query(f'SYST:COMM:LAN:GAT?', delay=1)
         logging.info(f": Default Gateway: {gateway} \n")
 
     # def configure_current(self):
     #     """
-    #     This function sets all the measurement parameters and trigger parameters to their default values with specified
-    #     range and resolution
-    #     :param test_mode: AC/DC
-    #     :param ranges: {100µA | 1mA | 10mA | 100mA | 1A | 3A | 10A }. Default: AUTO
-    #     :param resolution: AC: optional and ignored, fixed to 6 1/2 digits; DC default 10 PLC
-    #     :return: Success or failure
+    #     ``This function sets all the measurement parameters and trigger parameters to their default values with specified
+    #     range and resolution`` \n
+    #     :param: `str` : test_mode: AC/DC \n
+    #     :param: ranges: {100µA | 1mA | 10mA | 100mA | 1A | 3A | 10A }. Default: AUTO \n
+    #     :param: `str` : resolution: AC: optional and ignored, fixed to 6 1/2 digits; DC default 10 PLC \n
+    #     :return: `bool` : Success or failure
     #     """
     #     sys_err = self.dmm.query(f'SYST:ERR?')
     #     time.sleep(2)
     #     if sys_err == '+0,"No error"':
     #         time.sleep(2)
     #         self.dmm.write(f'CONF:CURR:DC AUTO')
     #         self.dmm.write(f'TRIG:SOUR EXT;SLOP POS')
@@ -124,53 +124,53 @@
     #         return True
     #     else:
     #         logging.info(f" SYSTEM ERROR: {sys_err}")
     #         raise Exception(f": ERROR: {sys_err}")
 
     def get_current(self, test_mode):
         """
-        This function reads a current measurement
-        :param test_mode: AC/DC
-        :return: float: Current in Amps
+        ``This function reads a current measurement`` \n
+        :param test_mode: `str` : AC/DC \n
+        :return: `float` : Current in Amps
         """
         current = self.dmm.query(f'MEAS:CURR:{test_mode}?', delay=1)
         logging.info(f": {str(test_mode)} Current: {current} Amps \n")
         return float(current)
 
     # def configure_voltage(self, test_mode, ranges, resolution):
     #     """
-    #     This function sets all the measurement parameters and trigger parameters to their default values with specified
-    #     range and resolution
-    #     :param test_mode: AC/DC
-    #     :param ranges: {100 mV | 1 V | 10 V | 100 V | 1000 V}. Default: AUTO
-    #     :param resolution: AC: optional and ignored, fixed to 6 1/2 digits; DC default 10 PLC
+    #     ``This function sets all the measurement parameters and trigger parameters to their default values with specified
+    #     range and resolution`` \n
+    #     :param: `str` :  test_mode: AC/DC \n
+    #     :param: ranges: {100 mV | 1 V | 10 V | 100 V | 1000 V}. Default: AUTO \n
+    #     :param: resolution: AC: optional and ignored, fixed to 6 1/2 digits; DC default 10 PLC \n
     #     :return: Success or failure
     #     """
     #     sys_err = self.dmm.query(f'SYST:ERR?')
     #     if sys_err == '+0,"No error"':
     #         conf_volt = self.dmm.query(f'CONF:VOLT:{str(test_mode).upper()} {ranges}, {float(resolution)}')
     #         logging.info(f": {str(test_mode).upper()} Voltage: {conf_volt} Volts \n")
     #         return True
     #     else:
     #         logging.info(f" SYSTEM ERROR: {sys_err}")
     #         raise Exception(f": ERROR: {sys_err}")
 
     def get_voltage(self, test_mode):
         """
-        This function reads a voltage measurement
-        :param test_mode: AC/DC
-        :return: float: Current in Amps
+        ``This function reads a voltage measurement`` \n
+        :param test_mode: `str` : AC/DC \n
+        :return: `float` : Current in Amps
         """
         voltage = self.dmm.query(f'MEAS:VOLT:{test_mode}?', delay=1)
         logging.info(f": {str(test_mode)} Voltage: {voltage} Volts \n")
         return float(voltage)
 
     def measurements(self):
         """
-        This function takes all the necessary measurements from the DMM
+        ``This function takes all the necessary measurements from the DMM`` \n
         :return: Values in logs
         """
         frequency = self.dmm.query(f'MEAS:FREQ?', delay=1)
         logging.info(f": Frequency: {frequency} \n")
 
         period = self.dmm.query(f'MEAS:PER?', delay=1)
         logging.info(f": Period: {period} \n")
```

