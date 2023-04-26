# Comparing `tmp/pts_hmp4040_psu-0.0.3.tar.gz` & `tmp/pts_hmp4040_psu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_hmp4040_psu-0.0.3.tar", last modified: Thu Jan 26 15:11:52 2023, max compression
+gzip compressed data, was "dist/pts_hmp4040_psu-0.0.4.tar", last modified: Wed Apr 26 11:39:31 2023, max compression
```

## Comparing `pts_hmp4040_psu-0.0.3.tar` & `pts_hmp4040_psu-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     6741 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6741 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      283 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-01-26 15:11:41.000000 pts_hmp4040_psu-0.0.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-01-26 15:11:41.000000 pts_hmp4040_psu-0.0.3/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-01-26 15:11:41.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10955 2023-01-26 15:11:41.000000 pts_hmp4040_psu-0.0.3/pts_hmp4040_psu/hmp4040_psu.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2023-01-26 15:11:41.000000 pts_hmp4040_psu-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:11:52.000000 pts_hmp4040_psu-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     6741 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6741 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      283 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-26 11:39:20.000000 pts_hmp4040_psu-0.0.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-26 11:39:20.000000 pts_hmp4040_psu-0.0.4/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-26 11:39:20.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11258 2023-04-26 11:39:20.000000 pts_hmp4040_psu-0.0.4/pts_hmp4040_psu/hmp4040_psu.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-04-26 11:39:20.000000 pts_hmp4040_psu-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:39:31.000000 pts_hmp4040_psu-0.0.4/setup.cfg
```

### Comparing `pts_hmp4040_psu-0.0.3/PKG-INFO` & `pts_hmp4040_psu-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_hmp4040_psu
-Version: 0.0.3
+Version: 0.0.4
 Summary: Rohde & Schwarz HMP4040 PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/fug-power-supply
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_hmp4040_psu-0.0.3/pts_hmp4040_psu.egg-info/PKG-INFO` & `pts_hmp4040_psu-0.0.4/pts_hmp4040_psu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-hmp4040-psu
-Version: 0.0.3
+Version: 0.0.4
 Summary: Rohde & Schwarz HMP4040 PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/fug-power-supply
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_hmp4040_psu-0.0.3/setup.py` & `pts_hmp4040_psu-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_hmp4040_psu",
-    version="0.0.3",
+    version="0.0.4",
     author="Pass testing Solutions GmbH",
     description="Rohde & Schwarz HMP4040 PSU Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/fug-power-supply",
     license="MIT",
```

### Comparing `pts_hmp4040_psu-0.0.3/LICENSE.txt` & `pts_hmp4040_psu-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_hmp4040_psu-0.0.3/pts_hmp4040_psu/hmp4040_psu.py` & `pts_hmp4040_psu-0.0.4/pts_hmp4040_psu/hmp4040_psu.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 import pyvisa
 import os
 import logging
 
 
 class HMP4040_Psu:
     """
-    Base class for the Rohde & Schwarz HMP4040 PSU
+    ``Base class for the Rohde & Schwarz HMP4040 PSU``
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%H:%M:%S',
                         level=logging.INFO)
 
     def __init__(self, connection_string=None):
         if not connection_string:
             self.connection_string = os.getenv("HMP_CONNECTION_STRING", default="TCPIP::192.168.1.128::5025::SOCKET")
         else:
             self.connection_string = connection_string
         self.resource_manager = None
 
     def open_connection(self):
         """
-        Opens a TCP/IP connection to connect to the Rohde & Schwarz HMP4040 PSU
+         ``Opens a TCP/IP connection to connect to the Rohde & Schwarz HMP4040 PSU`` \n
         """
         self.resource_manager = pyvisa.ResourceManager()
         try:
             self.hmp = self.resource_manager.open_resource(self.connection_string)
             self.hmp.read_termination = '\n'
             self.hmp.write_termination = '\n'
             logging.info(f": Opening PSU Resource at {self.connection_string}")
         except Exception as e:
             raise Exception(f": ERROR {e}: Could not open Resource")
 
     def close_connection(self):
         """
-        Closes the TCP/IP connection to the R&S HMP4040 PSU
+        ``Closes the TCP/IP connection to the R&S HMP4040 PSU`` \n
         """
         logging.info(f": Closing connection")
         self.resource_manager.close()
 
     def self_test(self):
         """
-        Performs the self-test and checks for system errors
-        :return: bool: True or Error
+        ``Performs the self-test and checks for system errors`` \n
+        :return: `bool` : True or Error
         """
         sys_err = str(self.hmp.query(f'SYST:ERR?', delay=1))
         if sys_err == '0, "No error"':
             try:
                 selftest = self.hmp.query(f'*TST?', delay=1)
                 if selftest == "0":
                     logging.info(": PASS: SELF-TEST PASSED!")
@@ -58,60 +58,60 @@
                 raise Exception(f": ERROR: {e} One or more self-test has FAILED")
         else:
             logging.error(f": SYSTEM_ERROR: {sys_err}")
             raise Exception(f": {sys_err}")
 
     def id_number(self):
         """
-        This function returns the ID number of the device
-        :return: str: ID number
+        ``This function returns the ID number of the device`` \n
+        :return: `str` : ID number
         """
         time.sleep(5)
         idn = self.hmp.query(f'*IDN?', delay=2)
         logging.info(f": IDN: {idn} \n")
         return str(idn)
 
     def scpi_version(self):
         """
-        This function gets the SCPI version info for the R&S HMP4040 PSU
-        :return: str: SCPI version number
+        ``This function gets the SCPI version info for the R&S HMP4040 PSU`` \n
+        :return: `str` : SCPI version number
         """
         scpi_ver = self.hmp.query(f'SYST:VERS?', delay=1)
         logging.info(f": SCPI Version: {scpi_ver}")
         return str(scpi_ver)
 
     def set_remote(self):
         """
-        This function set the R&S HMP4040 PSU to a remote status
+        ``This function set the R&S HMP4040 PSU to a remote status`` \n
         :return: None
         """
         self.hmp.write(f'SYST:REM')
         logging.info(f": System is set to REMOTE")
 
     def channel_selection(self, channel):
         """
-        This function selects the output channel
-        :param: channel: int: selected output channel out of 4
-        :return: bool: True or False
+        ``This function selects the output channel`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :return: `bool` : True or False
         """
         self.hmp.write(f'INST:NSEL {channel}')
         channel_selection = self.hmp.query(f'INST:NSEL?')
         if channel_selection == str(channel):
             logging.info(f": Channel {channel} is selected.")
             return True
         else:
             logging.info(f": ERROR: Failed to select channel {channel} ")
             return False
 
     def set_voltage(self, channel, volt_in):
         """
-        This function sets the output voltage for the R&S HMP4040 PSU
-        :param volt_in: int: Voltage in the range of 0-1200 Volts
-        :param channel: int: Output channel out of 4 (OUT1, OUT2, OUT3, OUT4)
-        :return: True or raises Error
+        ``This function sets the output voltage for the R&S HMP4040 PSU`` \n
+        :param volt_in: `int` : Voltage in the range of 0-1200 Volts \n
+        :param channel: `int` : Output channel out of 4 (OUT1, OUT2, OUT3, OUT4) \n
+        :return: `bool` : True or raises Error
         """
         # Enables PSU output setting
         sys_err = str(self.hmp.query(f'SYST:ERR?', delay=1))
         if sys_err == '0, "No error"':
             try:
                 if self.channel_selection(channel):
                     self.hmp.write(f'VOLT {volt_in}')
@@ -123,96 +123,96 @@
                         logging.error(f"ERROR: Could not set voltage")
                         return False
             except Exception as e:
                 raise Exception(f"FAIL: to set Voltage : {e}")
 
     def get_voltage(self, channel):
         """
-        This function returns the output voltage of a channel
-        :param: channel: int: selected output channel out of 4
-        :return: float: Output Voltage in Volts
-                 str  : System Error code
+        ``This function returns the output voltage of a channel`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :returns: - `float` : Output Voltage in Volts \n
+                  - `str` : System Error code
         """
         if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
             if self.channel_selection(channel):
                 get_volt = self.hmp.query(f':VOLT?')
                 logging.info(f": Output Voltage: {get_volt} V on channel: {channel}")
                 return float(get_volt)
         else:
             logging.info(f": System Errors: {self.hmp.query(f'SYST:ERR?')}")
             return str(self.hmp.query(f'SYST:ERR?'))
 
     def set_max_voltage(self, channel):
         """
-        Sets the voltage to maximum voltage
-        :param: channel: int: selected output channel out of 4
-        :return: bool: True or False
+        ``Sets the voltage to maximum voltage`` \n
+        :param channel: `int` : selected output channel out of 4 \n
+        :return: `bool` : True or False
         """
         if self.channel_selection(channel):
             self.hmp.write(f'VOLT MAX')
             if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
                 logging.info(f": Output set to MAX voltage")
                 return True
             else:
                 logging.info(f": ERROR: Failed to set MAX voltage")
                 return False
 
     def set_min_voltage(self, channel):
         """
-        Sets the voltage to minimum voltage
-        :param: channel: int: selected output channel out of 4
-        :return: bool: True or False
+        ``Sets the voltage to minimum voltage`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :return: `bool` : True or False
         """
         if self.channel_selection(channel):
             self.hmp.write(f'VOLT MIN')
             if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
                 logging.info(f": Output set to MIN voltage")
                 return True
             else:
                 logging.info(f": ERROR: Failed to set MIN voltage")
                 return False
 
     def get_max_voltage(self, channel):
         """
-        Queries the upper limit of the output voltage
-        :param channel: int: selected output channel out of 4
-        :return: float: Maximum Voltage in Volts
-                 str  : System Error code
+        ``Queries the upper limit of the output voltage`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :returns: - `float` : Maximum Voltage in Volts \n
+                  - `str` : System Error code
         """
         if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
             if self.channel_selection(channel):
                 max_volt = self.hmp.query(f'VOLT? MAX')
                 logging.info(f": Max Voltage: {max_volt} V on channel: {channel}")
                 return float(max_volt)
         else:
             logging.info(f": System Errors: {self.hmp.query(f'SYST:ERR?')}")
             return str(self.hmp.query(f'SYST:ERR?'))
 
     def get_min_voltage(self, channel):
         """
-        Queries the lower limit of the output voltage
-        :param channel: int: selected output channel out of 4
-        :return: float: Minimum Voltage in Volts
-                 str  : System Error code
+        ``Queries the lower limit of the output voltage`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :returns: - `float`: Minimum Voltage in Volts \n
+                  - `str` : System Error code
         """
         if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
             if self.channel_selection(channel):
                 min_volt = self.hmp.query(f'VOLT? MIN')
                 logging.info(f": Min Voltage: {min_volt} V on channel: {channel}")
                 return float(min_volt)
         else:
             logging.info(f": System Errors: {self.hmp.query(f'SYST:ERR?')}")
             return str(self.hmp.query(f'SYST:ERR?'))
 
     def set_current(self, channel, curr_in):
         """
-        This function selects a channel and sets the current for the R&S HMP4040 PSU
-        :param curr_in: int: Current in the range of 0-10 Amps
-        :param channel: int: Output channel out of 4 (OUT1, OUT2, OUT3, OUT4)
-        :return: True or raises Error
+        ``This function selects a channel and sets the current for the R&S HMP4040 PSU`` \n
+        :param curr_in: `int` : Current in the range of 0-10 Amps \n
+        :param channel: `int` : Output channel out of 4 (OUT1, OUT2, OUT3, OUT4) \n
+        :returns: `bool` : True or raises Error
         """
         # Enables PSU output setting
         sys_err = str(self.hmp.query(f'SYST:ERR?', delay=1))
         if sys_err == '0, "No error"':
             try:
                 if self.channel_selection(channel):
                     self.hmp.write(f'CURR {curr_in}')
@@ -224,50 +224,50 @@
                         logging.error(f"FAIL: Could not set Current")
                         return False
             except Exception as e:
                 raise Exception(f"ERROR: {e}")
 
     def get_current(self, channel):
         """
-        This function queries the current of a selected channel
-        :param: channel: int: selected output channel out of 4
-        :return: float: Output current in Amps
-                 str  : System Error code
+        ``This function queries the current of a selected channel`` \n
+        :param channel: Selected output channel out of 4 \n
+        :returns: - `float` : Output current in Amps \n
+                  - `str` : System Error code
         """
         if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
             if self.channel_selection(channel):
                 get_curr = self.hmp.query(f':CURR?')
                 logging.info(f": Output current: {get_curr} A on channel: {channel}")
                 return float(get_curr)
         else:
             logging.info(f": System Errors: {self.hmp.query(f'SYST:ERR?')}")
             return str(self.hmp.query(f'SYST:ERR?'))
 
     def get_max_current(self, channel):
         """
-        Queries the upper limit of the output current
-        :param channel: int: selected output channel out of 4
-        :return: float: Maximum current in Amps
-                 str  : System Error code
+        ``Queries the upper limit of the output current`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :returns: - `float` : Maximum current in Amps \n
+                  - `str` : System Error code
         """
         if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
             if self.channel_selection(channel):
                 max_curr = self.hmp.query(f'CURR? MAX')
                 logging.info(f": Max current: {max_curr} A on channel: {channel}")
                 return float(max_curr)
         else:
             logging.info(f": System Errors: {self.hmp.query(f'SYST:ERR?')}")
             return str(self.hmp.query(f'SYST:ERR?'))
 
     def get_min_current(self, channel):
         """
-        Queries the lower limit of the output current
-        :param channel: int: selected output channel out of 4
-        :return: float: Minimum current in Amps
-                 str  : System Error code
+        ``Queries the lower limit of the output current`` \n
+        :param channel: `int` : Selected output channel out of 4 \n
+        :returns: - `float` : Minimum current in Amps \n
+                  - `str` : System Error code
         """
         if self.hmp.query(f'SYST:ERR?') == '0, "No error"':
             if self.channel_selection(channel):
                 min_curr = self.hmp.query(f'VOLT? MIN')
                 logging.info(f": Min current: {min_curr} A on channel: {channel}")
                 return float(min_curr)
         else:
```

### Comparing `pts_hmp4040_psu-0.0.3/README.md` & `pts_hmp4040_psu-0.0.4/README.md`

 * *Files identical despite different names*

