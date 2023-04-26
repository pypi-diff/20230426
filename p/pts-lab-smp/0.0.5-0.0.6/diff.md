# Comparing `tmp/pts_lab_smp-0.0.5.tar.gz` & `tmp/pts_lab_smp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_lab_smp-0.0.5.tar", last modified: Thu Jan 26 15:12:25 2023, max compression
+gzip compressed data, was "dist/pts_lab_smp-0.0.6.tar", last modified: Wed Apr 26 12:56:22 2023, max compression
```

## Comparing `pts_lab_smp-0.0.5.tar` & `pts_lab_smp-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-01-26 15:12:15.000000 pts_lab_smp-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/pts_lab_smp/
--rw-rw-rw-   0 root         (0) root         (0)    10172 2023-01-26 15:12:15.000000 pts_lab_smp-0.0.5/pts_lab_smp/lab_smp.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-01-26 15:12:15.000000 pts_lab_smp-0.0.5/pts_lab_smp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-01-26 15:12:15.000000 pts_lab_smp-0.0.5/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/pts_lab_smp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/pts_lab_smp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/pts_lab_smp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/pts_lab_smp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/pts_lab_smp.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2573 2023-01-26 15:12:15.000000 pts_lab_smp-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:12:25.000000 pts_lab_smp-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-04-26 12:56:11.000000 pts_lab_smp-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/pts_lab_smp/
+-rw-rw-rw-   0 root         (0) root         (0)    10429 2023-04-26 12:56:11.000000 pts_lab_smp-0.0.6/pts_lab_smp/lab_smp.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-04-26 12:56:11.000000 pts_lab_smp-0.0.6/pts_lab_smp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-26 12:56:11.000000 pts_lab_smp-0.0.6/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/pts_lab_smp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/pts_lab_smp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/pts_lab_smp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/pts_lab_smp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/pts_lab_smp.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2023-04-26 12:56:11.000000 pts_lab_smp-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:56:22.000000 pts_lab_smp-0.0.6/setup.cfg
```

### Comparing `pts_lab_smp-0.0.5/PKG-INFO` & `pts_lab_smp-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_lab_smp
-Version: 0.0.5
+Version: 0.0.6
 Summary: LAB-SMP PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/lab-smp-psu
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_lab_smp-0.0.5/setup.py` & `pts_lab_smp-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_lab_smp",
-    version="0.0.5",
+    version="0.0.6",
     author="Pass testing Solutions GmbH",
     description="LAB-SMP PSU Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/lab-smp-psu",
     license="MIT",
```

### Comparing `pts_lab_smp-0.0.5/pts_lab_smp/lab_smp.py` & `pts_lab_smp-0.0.6/pts_lab_smp/lab_smp.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,119 +16,119 @@
         self.ls_psu = None
         self.resource_manager = None
         self.connection_string = connection_string
         self.port = port
 
     def open_connection(self):
         """
-        Opens a TCP/IP connection to connect to the LAB SMP PSU
+        ``Opens a TCP/IP connection to connect to the LAB SMP PSU`` \n
         """
         try:
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.connect((self.connection_string, self.port))
             logging.info(f": Opening LAB-SMP Resource at {self.connection_string} and port {self.port}")
         except Exception as e:
             raise Exception(f": ERROR {e}: Could not open Resource")
 
     def close_connection(self):
         """
-        Closes the TCP/IP connection to the TDK Lambda PSU
+        ``Closes the TCP/IP connection to the TDK Lambda PSU`` \n
         """
         self.sock.close()
         print(f": Closing serial connection!")
 
     def clear_status(self):
         """
-        This command deletes the status byte
+        ``This command deletes the status byte`` \n
         :return: No return
         """
         self.sock.send(f'CLS')
         time.sleep(0.3)
         logging.info(f": CLEAR STATUS")
         print(f"CLEAR STATUS")
 
     def clear_device(self):
         """
-        This command resets the initialization data.
+        ``This command resets the initialization data.`` \n
         :return: No return value.
         """
         self.sock.send(f'DCL')
         time.sleep(0.3)
         logging.info(": CLEAR DEVICE")
         print(": CLEAR DEVICE")
 
     def identification_number(self):
         """
-        This command checks the identification number
-        :return: str: Identification number
+        ``This command checks the identification number`` \n
+        :return: `str` : Identification number
         """
         self.sock.send(b'ID \n')
         time.sleep(0.3)
         idn = self.sock.recv(1024)
         logging.info(f": Identification number: {idn.decode()}")
         print(f": Identification number: {idn.decode()}")
         return str(idn.decode())
 
     def optical_idn(self):
         """
-        This command checks the optical identification number
-        :return: str: optical idn
+        ``This command checks the optical identification number`` \n
+        :return: `str` : optical idn
         """
         self.sock.send(b'*OPT? \n')
         time.sleep(0.3)
         optical_idn = self.sock.recv(1024)
         logging.info(f": Optical Identification Query: {optical_idn.decode()}")
         print(f": Optical Identification Query: {optical_idn.decode()}")
         return str(optical_idn.decode())
 
     def interface_status(self):
         """
-        This command checks the interface status
-        :return: str: Interface status
+        ``This command checks the interface status`` \n
+        :return: `str` : Interface status
         """
         self.sock.send(b'*STB? \n')
         time.sleep(0.3)
         interface_status = self.sock.recv(1024)
         logging.info(f": Interface Status: {interface_status.decode()}")
         print(f": Interface Status: {interface_status.decode()}")
         return str(interface_status.decode())
 
     def local_lockout(self):
         """
-        This command deactivates the LOCAL button
+        ``This command deactivates the LOCAL button`` \n
         :return: None return
         """
         self.sock.send(b'LLO \n')
         logging.info(": LOCAL button Deactivated")
         print(f": LOCAL button deactivated")
 
     def activate_remote(self):
         """
-        This command activates the front panel operation and also resets Local lockout button
+        ``This command activates the front panel operation and also resets Local lockout button`` \n
         :return: None return
         """
         self.sock.send(b'GTR \n')
         logging.info(": Remote mode activated")
         print(f": Remote mode activated")
 
     def activate_local(self):
         """
-        This command activates the front panel operation and also resets Local lockout button
+        ``This command activates the front panel operation and also resets Local lockout button`` \n
         :return: None return
         """
         self.sock.send(b'GTL \n')
         logging.info(": Front panel activated")
         print(f": Front panel activated")
 
     def toggle_device_output(self, state):
         """
-        This function enables/disables the LAB SMP output setting -
+        ``This function enables/disables the LAB SMP output setting -
         S|1: puts the unit in Standby, Output is disabled
-        R|0: disables Standby mode, Output is enabled
-        :param state: the required output state
+        R|0: disables Standby mode, Output is enabled`` \n
+        :param: `str` : state: the required output state \n
         :return: Success or failure
         """
         states = {'R': 'ENABLED', 'S': 'DISABLED'}
         self.sock.send(b'SB \n')
         resp = self.sock.recv(1024)
         check_standby = resp.decode().rstrip().split(",")[-1]
         if check_standby != str(state):
@@ -146,135 +146,135 @@
         else:
             logging.info(f": PSU Output is already: {states[str(state)]}")
             print(f": PSU Output is already: {states[str(state)]}")
         return True
 
     def get_interface(self, interface_id):
         """
-        This command will query the three interface parameters (possibly only one available)
-        :param interface_id: PC1 - Serial, PC2 - LAN, PC3 - GPIB (Empty)
-        :return: list: Interface Parameters
+        ``This command will query the three interface parameters (possibly only one available)`` \n
+        :param: `str` : interface_id: PC1 - Serial, PC2 - LAN, PC3 - GPIB (Empty) \n
+        :return: `list` : Interface Parameters
         """
         self.sock.send(str(interface_id+'\n').encode())
         time.sleep(0.3)
         comm_intf = self.sock.recv(1024)
         logging.info(f": Query of the interface: {comm_intf.decode()}")
         print(f": Query of the interface: {comm_intf.decode()}")
         return str(comm_intf.decode())
 
     def set_voltage(self, volt):
         """
-        This command will query the three interface parameters (possibly only one available)
-        :param volt: output voltage in Volts
-        :return: list: Interface Parameters
+        ``This command will query the three interface parameters (possibly only one available)`` \n
+        :param: `float` : volt: output voltage in Volts \n
+        :return: `list` : Interface Parameters
         """
         b_volt = 'UA,'+str(volt)
         self.sock.send(b_volt.encode()+b'\n')
         time.sleep(0.3)
         logging.info(f": Voltage set to: {volt} ")
 
     def set_current_limit(self, curr_limit):
         """
-        This command will query the three interface parameters (possibly only one available)
-        :param curr_limit: current limit in Amps
-        :return: list: Interface Parameters
+        ``This command will query the three interface parameters (possibly only one available)`` \n
+        :param: `float` : curr_limit: current limit in Amps \n
+        :return: `list` : Interface Parameters
         """
         b_curr_lim = 'IA,'+str(curr_limit)
         self.sock.send(b_curr_lim.encode()+b'\n')
         time.sleep(0.3)
         logging.info(f": Current limit set to: {curr_limit}")
 
     def set_interface_params(self):
         """
-        This command will set the different interface parameters
-        ONLY TO BE USED WITH SERIAL RS232 CONNECTION - PC1
+        ``This command will set the different interface parameters
+        ONLY TO BE USED WITH SERIAL RS232 CONNECTION - PC1`` \n
         :return: No return value
         """
         self.sock.send(b'PC1,9600,N,8,2,N,E \n')
         time.sleep(0.3)
         self.sock.send(b'SS \n')
         logging.info(f": Interface Arguments changed")
         print(f": Interface Arguments changed")
 
     def check_voltage_limit(self):
         """
-        This function reads maximum adjustable voltage limitation
-        :return: float: Voltage limit in Volts
+        ``This function reads maximum adjustable voltage limitation`` \n
+        :return: `float` : Voltage limit in Volts
         """
         self.sock.send(b'LIMU \n')
         volt_limit = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Maximum adjustable voltage limit : {volt_limit} Volts")
         print(f": Maximum adjustable voltage limit : {volt_limit} Volts")
         return str(volt_limit)
 
     def check_current_limit(self):
         """
-        This function reads maximum adjustable current limitation
-        :return: float: Current limit in Amps
+        ``This function reads maximum adjustable current limitation`` \n
+        :return: `float` : Current limit in Amps
         """
         self.sock.send(b'LIMI \n')
         curr_limit = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Maximum adjustable current limit : {curr_limit} Amps")
         print(f": Maximum adjustable current limit : {curr_limit} Amps")
         return str(curr_limit)
 
     def check_unit_output(self):
         """
-        This function reads maximum unit output
-        :return: float: Unit output in Watts
+        ``This function reads maximum unit output`` \n
+        :return: `float` : Unit output in Watts
         """
         self.sock.send(b'LIMP \n')
         unit_out = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Maximum unit output : {unit_out} Watts")
         print(f": Maximum unit output : {unit_out} Watts")
         return str(unit_out)
 
     def check_resistance_range(self):
         """
-        This function reads the adjustable range for Ri in UIR mode
-        :return: tuple: Resistance in Ohms
+        ``This function reads the adjustable range for Ri in UIR mode`` \n
+        :return: `tuple` : Resistance in Ohms
         """
         self.sock.send(b'LIMR \n')
         r_limit = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Limit of Ri in UIR mode : {r_limit} Ohms")
         print(f": Limit of Ri in UIR mode : {r_limit} Ohms")
         return str(r_limit)
 
     def measure_output_voltage(self):
         """
-        This function measures present output voltage
-        :return: float: Programmed output voltage in Volts
+        ``This function measures present output voltage`` \n
+        :return: `float` : Programmed output voltage in Volts
         """
         self.sock.send(b'MU \n')
         meas_volt = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Present Output Voltage: {meas_volt} Volts")
         print(f": Present Output Voltage: {meas_volt} Volts")
         return str(meas_volt)
 
     def get_ovp_limit(self):
         """
-        This command displays the present set over-voltage protection point.
-        :return: Over-voltage range
+        ``This command displays the present set over-voltage protection point.`` \n
+        :return: `str` : Over-voltage range
         """
         self.sock.send(b'OVP \n')
         ovp = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Over-voltage protection point: {ovp} Volts")
         print(f": Over-voltage protection point: {ovp} Volts")
         return str(ovp)
 
     def measure_output_current(self):
         """
-        This function measures present output current
-        :return: float: Programmed output Current in Amps
+        ``This function measures present output current`` \n
+        :return: `float` : Programmed output Current in Amps
         """
         self.sock.send(b'MI \n')
         meas_curr = self.sock.recv(1024).decode().rstrip().split(",")[-1]
         logging.info(f": Present Output Current: {meas_curr} Amps")
         print(f": Present Output Current: {meas_curr} Amps")
         return str(meas_curr)
 
     def reset(self):
         """
-        This function Resets hardware/Instrument
+        ``This function Resets hardware/Instrument`` \n
         :return: (no return value)
         """
         self.sock.send(b'*RST \n')
```

### Comparing `pts_lab_smp-0.0.5/LICENSE.txt` & `pts_lab_smp-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_lab_smp-0.0.5/pts_lab_smp.egg-info/PKG-INFO` & `pts_lab_smp-0.0.6/pts_lab_smp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-lab-smp
-Version: 0.0.5
+Version: 0.0.6
 Summary: LAB-SMP PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/lab-smp-psu
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_lab_smp-0.0.5/README.md` & `pts_lab_smp-0.0.6/README.md`

 * *Files identical despite different names*

