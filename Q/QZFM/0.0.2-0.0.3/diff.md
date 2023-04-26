# Comparing `tmp/QZFM-0.0.2.tar.gz` & `tmp/QZFM-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QZFM-0.0.2.tar", last modified: Mon Mar 27 16:12:18 2023, max compression
+gzip compressed data, was "QZFM-0.0.3.tar", last modified: Wed Apr 26 20:35:28 2023, max compression
```

## Comparing `QZFM-0.0.2.tar` & `QZFM-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-03-27 16:12:18.160475 QZFM-0.0.2/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.2/LICENSE
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     7817 2023-03-27 16:12:18.160475 QZFM-0.0.2/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     7231 2023-03-27 16:09:12.000000 QZFM-0.0.2/README.md
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      800 2023-03-27 16:11:58.000000 QZFM-0.0.2/pyproject.toml
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-03-27 16:12:18.160475 QZFM-0.0.2/setup.cfg
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-03-27 16:12:18.160475 QZFM-0.0.2/src/
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-03-27 16:12:18.160475 QZFM-0.0.2/src/QZFM.egg-info/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     7817 2023-03-27 16:12:18.000000 QZFM-0.0.2/src/QZFM.egg-info/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-03-27 16:12:18.000000 QZFM-0.0.2/src/QZFM.egg-info/SOURCES.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-03-27 16:12:18.000000 QZFM-0.0.2/src/QZFM.egg-info/dependency_links.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-03-27 16:12:18.000000 QZFM-0.0.2/src/QZFM.egg-info/requires.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-03-27 16:12:18.000000 QZFM-0.0.2/src/QZFM.egg-info/top_level.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    35199 2023-03-27 15:48:26.000000 QZFM-0.0.2/src/QZFM.py
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.2/src/__init__.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-04-26 20:35:28.988318 QZFM-0.0.3/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.3/LICENSE
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1659 2023-04-26 20:35:28.988318 QZFM-0.0.3/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1073 2023-04-20 19:39:56.000000 QZFM-0.0.3/README.md
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      799 2023-04-26 20:34:44.000000 QZFM-0.0.3/pyproject.toml
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-04-26 20:35:28.988318 QZFM-0.0.3/setup.cfg
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-04-26 20:35:28.988318 QZFM-0.0.3/src/
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-04-26 20:35:28.988318 QZFM-0.0.3/src/QZFM.egg-info/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1659 2023-04-26 20:35:28.000000 QZFM-0.0.3/src/QZFM.egg-info/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-04-26 20:35:28.000000 QZFM-0.0.3/src/QZFM.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-04-26 20:35:28.000000 QZFM-0.0.3/src/QZFM.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-04-26 20:35:28.000000 QZFM-0.0.3/src/QZFM.egg-info/requires.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-04-26 20:35:28.000000 QZFM-0.0.3/src/QZFM.egg-info/top_level.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    33750 2023-04-26 20:30:56.000000 QZFM-0.0.3/src/QZFM.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.3/src/__init__.py
```

### Comparing `QZFM-0.0.2/LICENSE` & `QZFM-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `QZFM-0.0.2/pyproject.toml` & `QZFM-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QZFM"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Derek Fujimoto", email="dfujimoto@triumf.ca" },
 ]
 description = "Python class for serial communication with QuSpin Zero Field Magnetometer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = [
-    "QZFM", 
+    "QZFM",
     "QuSpin",
     "Magnetometer",
     "Zero Field"
 ]
 dependencies = [
     "numpy",
     "matplotlib",
```

### Comparing `QZFM-0.0.2/src/QZFM.py` & `QZFM-0.0.3/src/QZFM.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Read data from, and send signals to QuSpin via QZFM commands
-# Derek Fujimoto
-# Mar 2023
-
-# see https://quspin.com/products-qzfm-gen2-arxiv/qzfm-command-list/
-# for serial commands
-
-# see also https://quspin.com/products-qzfm-gen2-arxiv/qzfm-quick-start-guide/
-# for general usage and setup
+"""
+Read data from, and send signals to QuSpin via QZFM commands
+Derek Fujimoto
+Mar 2023
+
+see https://quspin.com/products-qzfm-gen2-arxiv/qzfm-command-list/
+for serial commands
+
+see also https://quspin.com/products-qzfm-gen2-arxiv/qzfm-quick-start-guide/
+for general usage and setup
+"""
 
 import numpy as np
 import pandas as pd
 import matplotlib
 import matplotlib.pyplot as plt
 import serial
 from tqdm import tqdm
@@ -18,55 +20,55 @@
 from serial.tools import list_ports
 from time import time
 from datetime import datetime
 
 matplotlib.use('TkAgg')
 
 class QZFM(object):
-    """
-        Low-level control of QuSpin magnetic sensor via QZFM serial commands via USB
+    """Low-level control of QuSpin magnetic sensor via QZFM serial commands via USB
 
-        Attributes: 
+    Attributes:
 
-            axis_mode:          str, readback mode for daq
-            field:              np.array of magnetic fields (pT)
-            gain:               float, V/nT from setting analog gain
-            is_calibrated:      True if calibration is ok
-            is_data_streaming:  True if data streaming mode   
-            is_field_zeroed:    True if field zeroing is maintained
-            is_xyz_zeroing:     True if field zeroing applied to all axes, else only y and z
-            led:                dict of led status on/off
-            messages:           list of tuples (message, epoch time)
-            nbytes_status:      serial read chunk size in bytes for status updates
-            read_axis:          str, axis for readback
-            sensor_par:         dict of sensor parameter readback values
-            ser:                serial.Serial object for connection
-            status_last_updated:epoch time last updated status (led, sensor_par, messages)
-            time:               np.array of epoch times corresponding to field measurements 
+        axis_mode (str):            readback mode for daq
+        data_read_rate (int):       readback rate in Hz
+        field (np.array):           magnetic fields (pT)
+        gain (float):               V/nT from setting analog gain
+        is_calibrated (bool):       True if calibration is ok
+        is_data_streaming (bool):   True if data streaming mode
+        is_field_zeroed (bool):     True if field zeroing is maintained
+        is_xyz_zeroing (bool):      True if field zeroing applied to all axes, else only y and z
+        led (dict):                 led status on/off
+        messages (list):            (message, epoch time)
+        nbytes_status (int):        serial read chunk size in bytes for status updates
+        read_axis (str):            axis for readback
+        sensor_par (dict):          sensor parameter readback values
+        ser (serial.Serial):        object for connection
+        serial_settings (dict):     default settings. See https://pyserial.readthedocs.io/en/latest/pyserial_api.html#serial.Serial
+        status_last_updated (int):  epoch time last updated status (led, sensor_par, messages)
+        time (np.array):            epoch times corresponding to field measurements
     """
 
-    # see https://pyserial.readthedocs.io/en/latest/pyserial_api.html#serial.Serial
     serial_settings = { 'baudrate':     115200,
                         'bytesize':     8,
                         'parity':       serial.PARITY_NONE,
                         'stopbits':     1,
                         'write_timeout':10,     # seconds
                         'xonxoff':      False,
                         'rtscts':       False,
                         'dsrdtr':       False,
                         }
 
     data_read_rate = 200 # Hz
 
-    def __init__(self, device_name=None, nbytes_status=1000): 
-        """
-            device_name:    str, name of device to look for (connection)
-                            for windows this is likely COM3 or COM5
-                            for linux, search Z3T0 or similar    
-            nbytes_status: serial read chunk size in bytes for status updates
+    def __init__(self, device_name=None, nbytes_status=1000):
+        """Args:
+            device_name (str): name of device to look for (connection)
+                                for windows this is likely COM3 or COM5
+                                for linux, search Z3T0 or similar
+            nbytes_status (int): serial read chunk size in bytes for status updates
         """
 
         # bytes to read
         self.nbytes_status = nbytes_status
 
         # initialize data fields
         self.field = np.array([], dtype=float)
@@ -78,56 +80,64 @@
                     'cell temp lock (LED2)':False,
                     'laser lock (LED3)':    False,
                     'field zeroed (LED4)':  False,
                     'is master':            False,
                     }
         self.sensor_par = { 'cell temp error':      np.nan,
                             'cell temp voltage':    np.nan,
-                            'Bz field (pT)':        np.nan, 
-                            'By field (pT)':        np.nan, 
-                            'B0 field (pT)':        np.nan, 
+                            'Bz field (pT)':        np.nan,
+                            'By field (pT)':        np.nan,
+                            'B0 field (pT)':        np.nan,
                             }
         self.messages = []
         self._reset_attributes()
-        
+
         # connect
-        if device_name is not None: 
+        if device_name is not None:
             self.connect(device_name)
 
     def _get_next_message(self, timeout=1):
-        """
-            Block until for next message, as denoted by "#" first character
-            Save message to message list
-            timeout: duration in s to wait until next message
+        """Block until for next message, as denoted by "#" first character
+
+             Save message to message list
+
+        Args:
+            timeout (int): duration in seconds to wait until next message
         """
 
         # clear buffer to ensure new input
         self.ser.reset_input_buffer()
 
         # initialize
         mess = []
         t_start = time()
 
         while len(mess) == 0:
 
             # read output from sensor
             message = self._read_serial(self.nbytes_status)
             t = time()
-            
+
             mess = [(m[1:], t) for m in message if m[0] == '#']
 
             # timeout
             if time()-t_start > timeout:
                 return
 
         self.messages.extend(mess)
 
     def _read_serial(self, nbytes, clear_buffer=True):
-        """
-            Read a serial messsage and convert to utf-8, split by newlines
+        """Read a serial messsage and convert to utf-8, split by newlines
+
+        Args:
+            nbytes (int): number of bytes to read
+            clear_buffer (bool): if true, clear the buffer before read
+
+        Returns:
+            str: message from device
         """
 
         # clear buffer to ensure new input
         if clear_buffer:
             self.ser.reset_input_buffer()
 
         # read output from sensor
@@ -137,87 +147,89 @@
         message = message.decode('utf-8')
         message = message.replace('\x00', '')
         message = message.split('\r\n')[1:-1]  # first and last element likely incomplete
 
         return message
 
     def _reset_attributes(self):
-        """
-            Set attributes to default values
-        """
+        """Set attributes to default values"""
         # initialize state
         self.is_data_streaming = False
         self.is_field_zeroed = False
         self.is_xyz_zeroing = True
         self.is_calibrated = False
-        
+
         # axis readback mode
         self.axis_mode = 'z'
         self.read_axis = 'z'
 
         # set default gain
         self.gain = 2.7
 
     def _set_data_stream(self, on=True):
+        """Turns on/off the sensor digital data stream and stops updating sensor status information
+
+            Equivalent to the Print ON and Print OFF commands
+
+        Args:
+            on (bool): if True turn data stream on. Else turn off.
         """
-            Turns on/off the sensor digital data stream and stops updating sensor status information
-            equivalent to the Print ON and Print OFF commands
-        """
-        if on:      
+        if on:
             self.ser.write(b'7')
             self._get_next_message()
             self.is_data_streaming = True
-        else:       
+        else:
             self.ser.write(b'8')
             self.is_data_streaming = False
 
     def _set_read_axis(self, axis):
-        """
-            Change the axis for measurement
+        """Change the axis for measurement
 
-            axis: str, either x, y, or z
+        Args:
+            axis (str): x|y|z
         """
 
         # early end
         if self.read_axis == axis:
             return
 
+        # fix input
+        axis = axis.lower()
+
         if axis == 'x':     self.ser.write(b'G')
         elif axis == 'y':   self.ser.write(b'@')
         elif axis == 'z':   self.ser.write(b'?')
         else:
             raise RuntimeError(f'Unknown axis "{axis}"')
 
         self.read_axis = axis
         self._get_next_message()
 
-    def auto_start(self, block=True, show=True):   
-        """
-         	Initiate the automated sensor startup routines
-             
-            if block, wait until laser is locked and 
-            temperature stabilized before unblocking
-            
-            if show, monitor status
+    def auto_start(self, block=True, show=True):
+        """Initiate the automated sensor startup routines
+
+        Args:
+            block (bool): if True, wait until laser is locked and temperature stabilized before unblocking
+            show (boo): print status continuously to screen until finished
         """
         self.ser.write(b'>')
         self.update_status()
         self.print_status(overwrite_last=False)
 
         if block:
             while not self.led["laser lock (LED3)"] or not self.led["cell temp lock (LED2)"]:
                 self.update_status()
-                if show: 
+                if show:
                     self.print_status(overwrite_last=True)
 
     def calibrate(self, show=True):
-        """
-            Calibrate the response (field to voltage) of the magnetometer with an internal signal reference
+        """Calibrate the response (field to voltage) of the magnetometer with an internal signal reference
 
-            show: if true, print to screen
+        Args:
+            show (bool): if true, print to screen
         """
 
         # check for field zeroing
         if not self.is_field_zeroed:
 
             # double check sensor light
             if not self.field_zeroed:
@@ -231,105 +243,89 @@
         self._get_next_message(timeout=100)
 
         # print
         if show:
             self.print_messages(1)
 
     def connect(self, device_name):
-        """
-            Connect to the QuSpin
+        """Connect to the QuSpin device
 
-            device_name: str, name of device (ex: "Z3T0-AAL9"), or 
-                         partial name (ex: "Z3T0")
+        Args:
+            device_name (str): name of device (ex: "Z3T0-AAL9"), or partial name (ex: "Z3T0")
         """
-        
-        # list all serial ports 
+
+        # list all serial ports
         ports = [str(p) for p in list_ports.grep(device_name)]
 
         # error check
-        if len(ports) > 1: 
+        if len(ports) > 1:
             raise RuntimeError(f'Too many serial ports found. We found {ports}')
 
         # open serial connection
         self.ser = serial.Serial(ports[0].split()[0], **self.serial_settings)
 
     def disconnect(self):
-        """
-            Disconnect from QuSpin
-        """
+        """Disconnect from QuSpin"""
         self._set_data_stream(False)
         self.reboot()
         self.ser.close()
 
     def draw_data(self):
-        """
-            Draw data to window
-        """
-    
+        """Draw data to window"""
+
         # plot
         plt.figure(figsize=(10,6))
         plt.plot(self.time-self.time[0], self.field)
-        
+
         # plot elements
         plt.ylabel(f'$B_{self.read_axis}$ (pT)')
         plt.xlabel(f'Time Elapsed Since {datetime.fromtimestamp(self.time[0])} (s)',
                     fontsize='small')
         plt.tight_layout()
         plt.show(block=False)
 
     def field_reset(self):
-        """
-            Sets the internal coil field values to zero
-        """
+        """Sets the internal coil field values to zero"""
         self.ser.write(b'V')
         self._get_next_message()
         self.sensor_par['Bz field (pT)'] = 0
         self.sensor_par['By field (pT)'] = 0
         self.sensor_par['B0 field (pT)'] = 0
 
         # track state
         self.is_calibrated = False
         self.is_field_zeroed = False
 
-    def field_zero(self, on=True, axes_xyz=True, dBz=np.inf, dBy=np.inf, dB0=np.inf, dT=np.inf, show=True):
-        """
-            Run field zeroing procedure
-
-            if on: 
-                Start sensor field zeroing procedure to apply a compensation field using the internal sensor coils to null background fields 
-            
-            if axes_xyz: Field Zeroing is applied to all three axes (default)
-            else:        Field Zeroing is applied only to Y & Z axes
-
-            dBz, dBy, dB0:  field step thresholds in pT. 
-                            if step is smaller than this, stop zeroing procedure.
-                            All conditions must be satisfied for field zero stop
-                            Set to inf to disable
+    def field_zero(self, on=True, axes_xyz=True, show=True):
+        """Run field zeroing procedure
 
-            dT:             similar to above fields, but for cell temperature
+        Args:
+            on (bool): if True, start sensor field zeroing procedure to apply a compensation field using the internal sensor coils to null background fields.
+                        If False, stop zeroing procedure.
 
-            show: if true write diagnostic to stdout
+            axes_xyz (bool): If True, field zeroing is applied to all three axes (default). If False, field zeroing is applied only to Y & Z axes
+            show (float): if True write diagnostic to stdout
         """
 
         # calibration no longer valid
         self.is_calibrated = False
 
         # set axes for zeroing
-        if axes_xyz:    
+        if axes_xyz:
             self.ser.write(b'i')
             self.is_xyz_zeroing = True
-        else:           
+        else:
             self.ser.write(b'h')
             self.is_xyz_zeroing = False
 
         # set field zero status
-        if on:  
+        if on:
             self.ser.write(b'D')
             self.is_field_zeroed = False
-        else:   
+        else:
             self.ser.write(b'E')
             self.is_field_zeroed = True
             self.update_status()
 
         if on:
 
             # setup last setting
@@ -339,22 +335,18 @@
 
             # get current setting
             self.update_status()
             Bz_now = self.sensor_par['Bz field (pT)']
             By_now = self.sensor_par['By field (pT)']
             B0_now = self.sensor_par['B0 field (pT)']
             T_now = self.sensor_par['cell temp error']
-            
-            if not (np.isinf(dBz) and np.isinf(dBy) and np.isinf(dB0) and np.isinf(dT)):
-                print('\n'*5)
 
             try:
-                while (abs(Bz_now - Bz_last) > dBz) or (abs(By_now - By_last) > dBy) or \
-                    (abs(B0_now - B0_last) > dB0) or (abs(T_now) > dT):
-                    
+                while True:
+
                     # track
                     Bz_last = Bz_now
                     By_last = By_now
                     B0_last = B0_now
 
                     # get new values
                     self.update_status()
@@ -371,41 +363,38 @@
                                  '',
                                  f'T error = {T_now:.4f} (thresh: {dT})',
                                 ]
                         print("\033[F"*5 + '\n'.join(lines))
             except KeyboardInterrupt:
                 print()
 
-            if not (np.isinf(dBz) and np.isinf(dBy) and np.isinf(dB0) and np.isinf(dT)):
-                self.field_zero(on=False)
-
             self.update_status()
-    
+
     def monitor_cell_T_error(self, window_s=20, figsize=(10, 6)):
-        """
-            Continuously stream cell temperature to window
-            
-            window_s: show the last window_s seconds of data on the stream
-            figsize:  size of display
+        """Continuously stream cell temperature to figure
 
             See https://matplotlib.org/stable/tutorials/advanced/blitting.html
+
+        Args:
+            window_s (int): show the last window_s seconds of data on the stream
+            figsize (tuple): size of display
         """
 
         # get initial point
         self.update_status()
 
-        # make figure 
+        # make figure
         fig, ax = plt.subplots(figsize=figsize)
 
         # draw initial window
         x = np.array([self.status_last_updated])
         y = np.array([self.sensor_par['cell temp error']])
-        
+
         (line,) = plt.plot(np.zeros(1), y, animated=True, marker='o', fillstyle='none')
-        
+
         # plot elements
         plt.ylabel(f'Cell Temperature Error')
         plt.xlabel(f'Time (s)')
         plt.tight_layout()
 
         # render
         plt.show(block=False)
@@ -426,97 +415,96 @@
         # get bounds
         ylim = ax.get_ylim()
         xlim = ax.get_xlim()
 
         try:
             # draw forever
             while True:
-                
+
                 # get data
                 self.update_status(clear_buffer=True)
                 T = self.sensor_par['cell temp error']
                 t = self.status_last_updated
-                
+
                 x = np.append(x, t)
                 y = np.append(y, T)
                 dx = x-t
-                
+
                 # check data limits
                 idx = np.abs(dx) < window_s
                 x = x[idx]
                 y = y[idx]
-                dx = dx[idx] 
+                dx = dx[idx]
 
                 # check for figure
                 if not plt.fignum_exists(fig.number):
                     break
 
                 # if out of bounds, redraw
                 if not (max(y) < ylim[1] and min(y) > ylim[0]) or not (max(dx) < xlim[1] and min(dx) > xlim[0]):
                     plt.cla()
                     (line,) = plt.plot(dx, y, animated=True, marker='o', fillstyle='none')
-                    
+
                     # plot elements
                     plt.ylabel(f'Cell Temperature Error')
                     plt.xlabel(f'Time (s)')
                     plt.tight_layout()
-                    
+
                     # redraw
                     plt.pause(0.05)
                     bg = fig.canvas.copy_from_bbox(fig.bbox)
                     ax.draw_artist(line)
                     fig.canvas.blit(fig.bbox)
-                
-                else:                
+
+                else:
                     # reset background
                     fig.canvas.restore_region(bg)
 
                     # set data
                     line.set_xdata(dx)
                     line.set_ydata(y)
                     ax.draw_artist(line)
 
                 # update screen
                 fig.canvas.blit(fig.bbox)
                 fig.canvas.flush_events()
 
                 # print n events in buffer
-                print(f'N events remaining in buffer: {self.ser.in_waiting}', 
+                print(f'N events remaining in buffer: {self.ser.in_waiting}',
                       flush=True, end='\r')
 
         except KeyboardInterrupt:
             print()
-    
-    def monitor_data(self, axis='z', window_s=10, figsize=(10, 6)):
-        """
-            Continuously stream data to window
 
-            axis:     axis to read from
-            window_s: show the last window_s seconds of data on the stream
-            figsize:  size of display
+    def monitor_data(self, axis='z', window_s=10, figsize=(10, 6)):
+        """Continuously stream data to window
 
             See https://matplotlib.org/stable/tutorials/advanced/blitting.html
+
+        Args:
+            axis (str): x|y|z
+            window_s (int): show the last window_s seconds of data on the stream
+            figsize (tuple):  size of display
         """
 
         # get npts to show
         npts = self.data_read_rate * window_s
-        nticks = 5
 
         # set data to stream
         if not self.is_data_streaming:
             self._set_data_stream()
 
-        # make figure 
+        # make figure
         fig, ax = plt.subplots(figsize=figsize)
 
         # draw initial window
         x = (-np.arange(npts)/self.data_read_rate)[::-1]
         t, y = self.read_data(window_s, axis=axis, clear_buffer=True)
         (line,) = plt.plot(x, y, animated=True)
-        
+
         # plot elements
         plt.ylabel(f'$B_{self.read_axis}$ (pT)')
         plt.xlabel(f'Time (s)')
         plt.tight_layout()
 
         # render
         plt.show(block=False)
@@ -526,32 +514,32 @@
         bg = fig.canvas.copy_from_bbox(fig.bbox)
 
         # draw
         ax.draw_artist(line)
 
         # show
         fig.canvas.blit(fig.bbox)
-        
+
         # get bounds
         ylim = ax.get_ylim()
 
         try:
             # draw forever
             while True:
-                
+
                 # get data
                 tnew, data = self.read_data(0.1, axis=axis, clear_buffer=False)
                 y = np.append(y, data)[-npts:]
                 t = np.append(t, tnew)[-npts:]
 
                 # check bounds: redraw
                 if not (max(data) < ylim[1] and min(data) > ylim[0]):
                     plt.cla()
                     (line,) = plt.plot(x, y, animated=True)
-            
+
                     # plot elements
                     plt.ylabel(f'$B_{self.read_axis}$ (pT)')
                     plt.xlabel(f'Time (s)')
                     plt.tight_layout()
 
                     # render
                     bg = fig.canvas.copy_from_bbox(fig.bbox)
@@ -574,75 +562,71 @@
                 ax.draw_artist(line)
 
                 # update screen
                 fig.canvas.blit(fig.bbox)
                 fig.canvas.flush_events()
 
                 # print n events in buffer
-                print(f'N events remaining in buffer: {self.ser.in_waiting}', 
+                print(f'N events remaining in buffer: {self.ser.in_waiting}',
                       flush=True, end='\r')
-                      
+
         except KeyboardInterrupt:
             # save data
             self.time = t
             self.field = y
             print()
 
     def monitor_status(self):
-        """
-            Continuously update and print status
-        """
+        """Continuously update and print status"""
 
         # do first update
         self.update_status()
         self.print_status()
 
         # continuous
         try:
             while True:
                 self.update_status(clear_buffer=False)
                 self.print_status(overwrite_last=True)
         except KeyboardInterrupt:
             print()
 
     def print_messages(self, last_n=None):
-        """
-            Print messages to screen
+        """Print messages to screen
 
-            last_n: print the last number of messages
+        Args:
+            last_n (float|None): print the last_n number of messages. If None, print all.
         """
 
         messages = self.messages
-        
+
         if last_n is not None:
             messages = messages[-last_n:]
 
         for m, t in messages:
             print(f'{datetime.fromtimestamp(t)}  {m}')
 
     def print_state(self):
-        """
-            Print state of the python object
-        """
+        """Print state of the python object"""
         lines = [f'is_data_streaming:   {self.is_data_streaming}',
                  f'is_field_zeroed:     {self.is_field_zeroed}',
                  f'is_xyz_zeroing:      {self.is_xyz_zeroing}',
                  f'is_calibrated:       {self.is_calibrated}',
                  f'axis_mode:           {self.axis_mode}',
                  f'read_axis:           {self.read_axis}',
                  f'gain:                {self.gain} V/nT',
                  ]
         print('\n'.join(lines), flush=True)
 
     def print_status(self, update=False, overwrite_last=False):
-        """
-            Print status of QuSpin in a nicely formatted message
+        """Print status of QuSpin in a nicely formatted message
 
-            update: if true, update before printing
-            overwrite_last: if true, overwrite the last message. Used in monitor_status
+        Args:
+            update (bool): if True, update before printing. Otherwise, print prior saved values.
+            overwrite_last (bool): if True, overwrite the last message. Used in monitor_status
         """
 
         # look for print before update
         if update or self.status_last_updated is None:
             self.update_status()
 
         # format output
@@ -656,82 +640,82 @@
                  '',
                  f'Cell T error:    {self.sensor_par["cell temp error"]:.5g}',
                  #f'Cell T voltage:  {self.sensor_par["cell temp voltage"]}',
                  f'Bz field:        {self.sensor_par["Bz field (pT)"]:.4f} pT',
                  f'By field:        {self.sensor_par["By field (pT)"]:.4f} pT',
                  f'B0 field:        {self.sensor_par["B0 field (pT)"]:.4f} pT',
                  ]
-        
+
         # add white space incase overwrite has fewer characters
         lines = [line+' '*10 for line in lines]
-    
+
         # do print
         if overwrite_last:
             print("\033[F"*(len(lines)) + '\n'.join(lines))
         else:
             print('\n'.join(lines), flush=True)
 
     def read_data(self, seconds, axis='z', clear_buffer=True):
-        """
-            Read data from the device 
+        """Read data from the device
 
-            seconds:        float, duration of measurement npts= seconds*200Hz
-            axis:           str, which axis to read from (x, y, or z)
-            clear_buffer:   bool, if true, clear buffer and wait for new
-
-            assumed readback rate based on comments from QuSpin
-            time[0] is the time immediately after clearing the buffer. 
-                Note that there is often an incomplete word after clear, we ignore this
-                As a result the error in time is at most 1/self.data_read_rate
+        Assumed readback rate based on comments from QuSpin:
+            time[0] is the time immediately after clearing the buffer.
+            Note that there is often an incomplete word after clear, we ignore this
+            As a result the error in time is at most 1/self.data_read_rate
+
+        Args:
+            seconds (float): duration of measurement npts= seconds*200Hz
+            axis (str): x|y|z
+            clear_buffer (bool): If true, clear buffer and wait for new
 
-            returns (time, field)
+        Returns:
+            tuple: np arrays (time, field)
         """
-        
 
         # get npts
         npts = int(seconds*self.data_read_rate)
 
         # switch axis
         self._set_read_axis(axis)
-        
+
         # start data stream
         if not self.is_data_streaming:
             self._set_data_stream()
 
-        
+
         # get number of bytes to read
         # +2 bytes for \r and \n
         # +2 points since first and last are often partial
         nbytes = (self.serial_settings['bytesize']+2) * (npts+2)
 
         # clear buffer
         if clear_buffer:
             self.ser.reset_input_buffer()
-        
+
         # take data
         time_start = time()
         message = self.ser.read(nbytes)
         time_stop = time()
-       
+
         # clean up message to data format
         message = message.decode('utf-8')
         message = message.replace('\x00', '')
         message = message.replace('\r', '')
         message = message.replace('!', '')
         message = message.strip().split('\n')[1:-1]
-        
+
         # check for bad byte lengths in message
         good_data = (np.array([len(m) for m in message]) == self.serial_settings['bytesize']-1)
 
         # convert to numeric data
         data = np.array(message).astype(int)
         data = (data - 8388608) * 0.01
 
-        # check number of points 
-        if len(data) > npts: 
+        # check number of points
+        if len(data) > npts:
             data = data[:npts]
             good_data = good_data[:npts]
 
         assert npts == len(data), f"Readback data length incorrect: npts != len(data) ({npts} != {len(data)})"
 
         # interpolate times
         dt = (time_stop-time_start)/len(data)
@@ -741,281 +725,284 @@
         data[~good_data] = np.nan
 
         # save data
         self.time = times
         self.field = data
 
         return (self.time, self.field)
-    
+
     def read_offsets(self, npts, clear_buffer=True):
-        """
-            Read offset data from the device in field zeroing mode 
+        """Read offset data from the device in field zeroing mode
 
-            npts:           int, number of data points to read
-            clear_buffer:   bool, if true, clear initial buffer and wait for new
+        time[0] is the time immediately after clearing the buffer.
+        reads at approx 7.5 Hz
 
-            time[0] is the time immediately after clearing the buffer. 
-            
-            reads at approx 7.5 Hz
+        Args:
+            npts (int): number of data points to read
+            clear_buffer (bool): if true, clear initial buffer and wait for new
+
+        Returns:
+            pd.DataFrame: field zeroing data and timestamps
         """
-        
+
         # change to status readback
         if self.is_data_streaming:
-            self._set_data_stream(False)	
-        
+            self._set_data_stream(False)
+
         # storage for messages and data
         stream = ''
-        data = {'x':np.zeros(npts*2), 
-                'y':np.zeros(npts*2), 
+        data = {'x':np.zeros(npts*2),
+                'y':np.zeros(npts*2),
                 'z':np.zeros(npts*2)}
         nx = 0
         ny = 0
         nz = 0
-        
+
         # initialize progress bar
         progress = tqdm(leave=False, total=npts, desc='Measuring')
 
         # clear buffer
         if clear_buffer:
             self.ser.reset_input_buffer()
 
         # take data
         time_start = time()
-        
+
         while nx < npts and ny < npts and nz < npts:
-            
+
             nx_start = nx
-            
-            # read message 
+
+            # read message
             message = self.ser.read(self.nbytes_status)
 
             # clean up message to data format
             message = message.decode('utf-8')
             message = message.replace('\x00', '')
             message = message.replace('\r', '')
-            
+
             # append the old stream
             message = stream+message
-            
+
             # split into lines
             codes = message.split('\n')
-            
+
             if nx+ny+nz == 0:
                 codes = codes[1:]
-            
+
             # parse the message
-            for code in codes[:-1]: 
+            for code in codes[:-1]:
                 if code[0] == '~':
                     if code[3:].replace('.', '').isnumeric():
-                        if code[1:3] == '07':   
+                        if code[1:3] == '07':
                             data['z'][nz] = float(code[3:])-32768
                             nz += 1
-                        elif code[1:3] == '08':   
+                        elif code[1:3] == '08':
                             data['y'][ny] = float(code[3:])-32768
                             ny += 1
-                        elif code[1:3] == '09':   
+                        elif code[1:3] == '09':
                             data['x'][nx] = float(code[3:])-32768
                             nx += 1
 
             # save last point
-            stream = codes[-1]   
-            
+            stream = codes[-1]
+
             # iterate progress bar
             progress.update(nx-nx_start)
-		
-        # check number of points 
+
+        # check number of points
         data['x'] = data['x'][:npts]
         data['y'] = data['y'][:npts]
         data['z'] = data['z'][:npts]
-        
+
         # interpolate times
         times = np.arange(npts)/self.data_read_rate + time_start
-        
-        # save 
+
+        # save
         self.data_fz = pd.DataFrame(data, index=times)
         self.data_fz.index.name = 't (s)'
-        self.data_fz.rename(columns={'x':'B0 (pT)', 'y':'By (pT)', 'z':'Bz (pT)'}, 
+        self.data_fz.rename(columns={'x':'B0 (pT)', 'y':'By (pT)', 'z':'Bz (pT)'},
                                     inplace=True)
-                                    
+
         return self.data_fz
-    
+
     def reboot(self):
-        """
-            Reboot the microprocessor and reloads the firmware
-        """
+        """Reboot the microprocessor and reloads the firmware"""
         self.ser.write(b'e')
         self.update_status()
         self._reset_attributes()
 
     def set_axis_mode(self, mode='z'):
-        """
-            Change field-sensitive axis
+        """Change field-sensitive axis
 
             Note: triaxial sensors do not respond to this command
 
-            mode =  z       Operate the magnetometer in single Z axis mode
-                    y       Operate the magnetometer in single Y axis mode
-                    dual    Operate the magnetometer in dual Y and Z axis mode
+        Args:
+            mode (str): z|y|dual
         """
 
         mode = mode.lower().strip()
-        if mode == 'z':     
+        if mode == 'z':
             self.ser.write(b'C')
         elif mode == 'y':   self.ser.write(b'F')
         elif mode == 'dual':self.ser.write(b'B')
         else:
             raise RuntimeError('Bad mode: must be one of "z", "y", or "dual".')
-        
+
         self.axis_mode = mode
         self.is_calibrated = False
         self.is_field_zeroed = False
         self.update_status()
 
     def set_gain(self, mode='1x'):
-        """
-            Set analog gain (analog output only)
+        """Set analog gain (analog output only)
 
-            mode =  0.33x   Set the analog output gain to 0.33 times default (0.9 V/nT)
-                    1x      Set the analog output gain to default (2.7 V/nT)
-                    3x      Set the analog output gain to 3 times default (8.1 V/nT)
+        Args:
+            mode (str): 0.33x|1x|3x
+                    0.33x (0.9 V/nT)
+                    1x (2.7 V/nT)
+                    3x (8.1 V/nT)
         """
-        
+
         mode = mode.lower().strip()
-        if mode == '0.33x': 
+        if mode == '0.33x':
             self.ser.write(b'a')
             self.gain = 0.9     # V/nT
 
-        elif mode == '1x':  
+        elif mode == '1x':
             self.ser.write(b'`')
             self.gain = 2.7     # V/nT
 
-        elif mode == '3x':  
+        elif mode == '3x':
             self.ser.write(b'b')
             self.gain = 8.1     # V/nT
 
     def to_csv(self, filename=None, *notes):
+        """Write data to csv, if no filename, use default
+
+        Args:
+            filename (str): name of file to write
+            notes: things to add to file header
         """
-            Write data to csv, if no filename, use default
-            
-            notes: list of things to add to file header
-        """
-        
+
         # set default file name
         if filename is None:
             t = datetime.now()
             filename = f'qzfm_{datetime.strftime("%y%m%d%H%M%S")}.csv'
-        
+
         # make dataframe
         df = pd.DataFrame({'time (epoch)':self.time, f'{self.read_axis} field (pT)':self.field})
-        
+
         self.update_status()
-        
+
         # write file header
         header = [ '# QZFM (QuSpin Zero Field Monitor) data',
                    '# ',
                   f'# Field zeroed:    {self.led["field zeroed (LED4)"]}',
                   f'# Laser lock:      {self.led["laser lock (LED3)"]}',
                   f'# Cell T lock:     {self.led["cell temp lock (LED2)"]}',
                   f'# Laser on:        {self.led["laser on (LED1)"]}',
                   '#',
                   f'# Cell T error:    {self.sensor_par["cell temp error"]}',
                   f'# Bz field:        {self.sensor_par["Bz field (pT)"]:.4f} pT',
                   f'# By field:        {self.sensor_par["By field (pT)"]:.4f} pT',
                   f'# B0 field:        {self.sensor_par["B0 field (pT)"]:.4f} pT',
                    '#',
                   ]
-          
+
         if notes:
             notes = [f'#\t{note}' for note in notes]
             header.extend(['# Notes', *notes, '#'])
-            
+
         header.extend([f'# {datetime.now()}', '# \n'])
-        
+
         with open(filename, 'w') as fid:
             fid.write('\n'.join(header))
-        
+
         # write data
         df.to_csv(filename, mode='a', index=False)
-           
+
     def to_csv_fz(self, filename=None, *notes):
+        """Write field zero data to csv, if no filename, use default
+
+        Args:
+            filename (str): name of file to write
+            notes: things to add to file header
         """
-            Write field zero data to csv, if no filename, use default
-            
-            notes: list of things to add to file header
-        """
-        
+
         # set default file name
         if filename is None:
             t = datetime.now()
             filename = f'qzfm_fz_{datetime.strftime("%y%m%d%H%M%S")}.csv'
-        
+
         # make dataframe
         df = self.data_fz
-        
+
         # write file header
         header = [ '# QZFM (QuSpin Zero Field Monitor) field zeroing data',
                    '# ',
                    '#',
                   ]
-          
+
         if notes:
             notes = [f'#\t{note}' for note in notes]
             header.extend(['# Notes', *notes, '#'])
-            
+
         header.extend([f'# {datetime.now()}', '# \n'])
-        
+
         with open(filename, 'w') as fid:
             fid.write('\n'.join(header))
-        
+
         # write data
         df.to_csv(filename, mode='a', index=False)
-                 
+
     def update_status(self, clear_buffer=True):
-        """
-            Clear input buffer and read status
-            
-            updates the following attributes: 
+        """Clear input buffer and read status
+
+            updates the following attributes:
                 self.status_last_updated
                 self.led
                 self.sensor_par
                 self.messages
+
+        Args:
+            clear_buffer (bool): if True clear the buffer before read attempt
         """
 
         # change to status readback
         if self.is_data_streaming:
             self._set_data_stream(False)
 
         # set update time
         message = self._read_serial(self.nbytes_status, clear_buffer=clear_buffer)
         self.status_last_updated = time()
-        
+
         # look for unique codes starting from the end
         codes = []
         codes_uniq = []
         for m in message[::-1]:
             if m[:3] not in codes_uniq:
                 codes.append(m)
                 codes_uniq.append(m[:3])
 
         # set values based on code types
         sp = {}
         led = {}
-        for code in codes: 
-            
+        for code in codes:
+
             # code has no length
             if not code: continue
 
             # LED
             if code[0] == '|':
                 if   code[1] == '1':  led['laser on (LED1)'] = code[2] == '1'
                 elif code[1] == '2':  led['cell temp lock (LED2)'] = code[2] == '1'
                 elif code[1] == '3':  led['laser lock (LED3)'] = code[2] == '1'
                 elif code[1] == '4':  led['field zeroed (LED4)'] = code[2] == '1'
                 elif code[1] == '5':  led['is master'] = code[2] == '1'
-            
+
             # readback parameters
             elif code[0] == '~':
                 if code[3:].replace('.', '').isnumeric():
                     if   code[1:3] == '04':   sp['cell temp error'] = (float(code[3:])-8388608)/524288
                     elif code[1:3] == '05':   sp['cell temp voltage'] = int(code[3:])
                     elif code[1:3] == '07':   sp['Bz field (pT)'] = float(code[3:])-32768
                     elif code[1:3] == '08':   sp['By field (pT)'] = float(code[3:])-32768
@@ -1024,36 +1011,36 @@
             # messages
             elif code[0] == '#':
                 self.messages.append((code[1:], self.status_last_updated))
 
         # reset field dicts and update
         for k in self.led.keys():
             self.led[k] = led.get(k, False)
-        
+
         for k in self.sensor_par.keys():
             if 'field' in k:
                 self.sensor_par[k] = sp.get(k, self.sensor_par[k])
             else:
                 self.sensor_par[k] = sp.get(k, np.nan)
-        
+
     @property
     def laser_on(self):
         self.update_status()
         return self.led['laser on (LED1)']
-    
+
     @property
     def cell_Tlock(self):
         self.update_status()
         return self.led['cell temp lock (LED2)']
-    
+
     @property
     def laser_locked(self):
         self.update_status()
         return self.led['laser lock (LED3)']
-    
+
     @property
     def field_zeroed(self):
         self.update_status()
         return self.led['field zeroed (LED4)']
 
     @property
     def is_master(self):
```

