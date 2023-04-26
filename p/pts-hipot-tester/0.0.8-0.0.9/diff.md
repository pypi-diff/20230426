# Comparing `tmp/pts_hipot_tester-0.0.8.tar.gz` & `tmp/pts_hipot_tester-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_hipot_tester-0.0.8.tar", last modified: Thu Jan 26 15:12:05 2023, max compression
+gzip compressed data, was "dist/pts_hipot_tester-0.0.9.tar", last modified: Wed Apr 26 11:36:31 2023, max compression
```

## Comparing `pts_hipot_tester-0.0.8.tar` & `pts_hipot_tester-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-01-26 15:11:54.000000 pts_hipot_tester-0.0.8/pts_hipot_tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20684 2023-01-26 15:11:54.000000 pts_hipot_tester-0.0.8/pts_hipot_tester/st9201_hipot_tester.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-01-26 15:11:54.000000 pts_hipot_tester-0.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-01-26 15:11:54.000000 pts_hipot_tester-0.0.8/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3114 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      298 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     2616 2023-01-26 15:11:54.000000 pts_hipot_tester-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:12:05.000000 pts_hipot_tester-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-26 11:36:20.000000 pts_hipot_tester-0.0.9/pts_hipot_tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21207 2023-04-26 11:36:20.000000 pts_hipot_tester-0.0.9/pts_hipot_tester/st9201_hipot_tester.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-04-26 11:36:20.000000 pts_hipot_tester-0.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-26 11:36:20.000000 pts_hipot_tester-0.0.9/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2023-04-26 11:36:20.000000 pts_hipot_tester-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:36:31.000000 pts_hipot_tester-0.0.9/setup.cfg
```

### Comparing `pts_hipot_tester-0.0.8/pts_hipot_tester/st9201_hipot_tester.py` & `pts_hipot_tester-0.0.9/pts_hipot_tester/st9201_hipot_tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 COMMON_TEST_MODE = ["AC", "DC", "IR"]
 CHANNEL_VALUE = ["HIGH", "LOW", "OPEN"]
 
 
 class HipotTester:
     """
-    Base class for the Sourcetronic ST9201 Hipot Tester
+    ``Base class for the Sourcetronic ST9201 Hipot Tester``
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%H:%M:%S',
                         level=logging.INFO)
 
     def __init__(self, connection_string):
         self.tic = None
@@ -22,50 +22,47 @@
         self.ser = None
         self.hipot_tester = None
         self.port = None
         self.connection_string = connection_string
 
     def open_connection(self):
         """
-        Opens a serial connection with the Hipot tester
-        :return:
+        ``Opens a serial connection with the Hipot tester`` \n
         """
         self.port = list(list_ports.comports())
         # self.hipot_tester = [str(p.device) for p in self.port if str(p).startswith("/dev/cu.usbserial")]
         self.ser = serial.Serial(self.connection_string, baudrate=19200, stopbits=serial.STOPBITS_TWO, timeout=1)
         self.tic = time.perf_counter()
         logging.info(f"Opening serial connection to port {self.ser} ...")
         # print("Opening serial connection...")
 
     def close_connection(self):
         """
-        Closes a serial connection with the Hipot tester
-        :return:
+        ``Closes a serial connection with the Hipot tester`` \n
         """
         self.ser.close()
         self.toc = time.perf_counter()
         logging.info(f"Testing time: {self.toc - self.tic:0.4f} seconds ! ")
         logging.info(f"Closing serial connection")
         # print(f"Closing serial connection")
 
     def id_number(self):
         """
-        This function returns the ID number
-        :return: str: IDN
+        ``This function returns the ID number`` \n
+        :return: `str` : IDN
         """
         idn = "*IDN? \r \n"
         self.ser.write(idn.encode())
         read_char = self.ser.read(20).decode()
         logging.info(f":IDN: {read_char}")
         return str(read_char)
 
     def system_info(self):
         """
-        Gathers system info about the serial interface
-        :return:
+        ``Gathers system info about the serial interface`` \n
         """
         sys_version = ":SYST:VERS? \r \n"
         self.ser.write(sys_version.encode())
         read_char = self.ser.read(20).decode()
         logging.info(f": SYSTEM VERSION: {read_char}")
         # print(f": SYSTEM VERSION: {read_char}")
 
@@ -116,73 +113,72 @@
         read_resp = self.ser.read(20).decode()
         logging.info(f": SYSTEM ARC: {read_resp}")
         # print(f": SYSTEM ARC: {read_resp}")
 
     # Set and get voltage for ACW/DCW/IR test
     def set_voltage(self, step, test_mode, voltage):
         """
-        This function sets the voltage for the ACW/DCW/IR test
-        :param step: The step for which the voltage is added in the range 1-49
-        :param voltage: The voltage to be set in Volts in range 50-5000 volts for ACW test
-                        and it must be set in Volts in range 50-6000 volts for DCW test
-        :param test_mode: modes being AC/DC/IR
+        ``This function sets the voltage for the ACW/DCW/IR test`` \n
+        :param step: The step for which the voltage is added in the range 1-49 \n
+        :param voltage: The voltage to be set in Volts in range 50-5000 volts for ACW test, and it must be set in Volts in range 50-6000 volts for DCW test \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: No return
         """
         # Set voltage for ACW/DCW/IR test
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_voltage = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LEV {voltage} \r \n"
             self.ser.write(set_voltage.encode())
             self.ser.read(20).decode()
             logging.info(f"Setting voltage to : {voltage}")
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def get_voltage(self, step, test_mode):
         """
-        This function checks the voltage for the ACW test
-        :param step: The step for which the voltage is added in the range 1-49
-        :param test_mode: modes being AC/DC/IR
-        :return: int: Voltage value in volts
+        ``This function checks the voltage for the ACW test`` \n
+        :param step: The step for which the voltage is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: `int` : Voltage value in volts
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             get_voltage = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LEV? \r \n"
             self.ser.write(get_voltage.encode())
             read_char = self.ser.read(20).decode()
             logging.info(f": GET {test_mode} VOLTAGE for step 1: {read_char} Volts")
             # print(f": GET AC VOLTAGE for step 1: {read_char} Volts")
             return int(read_char)
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def set_current_limits(self, step, test_mode, low_limit, high_limit):
         """
-        This functions sets the lower and upper current limits for ACW/DCW test
-        :param test_mode: modes being AC/DC
-        :param step: The step for which the current is added in the range 1-49
-        :param low_limit: Lower current limit in range 0~30.000E-3 (0 is OFF) Amps for ACW test and
-                          lower current limit in range 0~10.000E-3 (0 is OFF) Amps for DCW test
-        :param high_limit: Upper current limit in range 1.00E-6~30.000E-3 Amps for ACW test and
-                           upper current limit in range 1.00E-6~10.000E-3 Amps for DCW test.
+        ``This functions sets the lower and upper current limits for ACW/DCW test`` \n
+        :param test_mode: modes being AC/DC \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param low_limit: Lower current limit in range 0~30.000E-3 (0 is OFF) Amps for ACW test and lower current limit in range 0~10.000E-3 (0 is OFF) Amps for DCW test \n
+        :param high_limit: Upper current limit in range 1.00E-6~30.000E-3 Amps for ACW test and upper current limit in range 1.00E-6~10.000E-3 Amps for DCW test. \n
+        :return: No return
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_low_current = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LIM:LOW {low_limit} \r \n"
             self.ser.write(set_low_current.encode())
             self.ser.read(20).decode()
 
             set_high_current = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LIM:HIGH {high_limit} \r \n"
             self.ser.write(set_high_current.encode())
             self.ser.read(20).decode()
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def get_current_limits(self, step, test_mode):
         """
-        This function checks the lower and upper current limits set by the user/by default
-        :param test_mode: modes being AC/DC/IR
-        :param step: The step for which the current is added in the range 1-49
-        :return: tuple: Lower and upper current limits in Amps respectively
+        ``This function checks the lower and upper current limits set by the user/by default`` \n
+        :param test_mode: modes being AC/DC/IR \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :return: `tuple` : Lower and upper current limits in Amps respectively
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             get_low_current = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LIM:LOW? \r \n"
             self.ser.write(get_low_current.encode())
             read_char_low = self.ser.read(20).decode()
             logging.info(f": GET LOW CURRENT LIMIT for step {step}: {read_char_low} Amps")
 
@@ -192,257 +188,264 @@
             logging.info(f": GET HIGH CURRENT LIMIT for step {step}: {read_char_high} Amps")
             return float(read_char_low), float(read_char_high)
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def arc_set_current_limits(self, step, limit, test_mode):
         """
-        This functions sets the ARC current limit for ACW/DCW test
-        :param step: The step for which the current is added in the range 1-49
-        :param limit: Current limit in range 0~15.0E-3 (0 is OFF) Amps for ACW test and
-                      current limit in range 0~10.0E-3 (0 is OFF) Amps for DCW test.
-        :param test_mode: modes being AC/DC/IR
+        ``This functions sets the ARC current limit for ACW/DCW test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param limit: Current limit in range 0~15.0E-3 (0 is OFF) Amps for ACW test and current limit in range 0~10.0E-3 (0 is OFF) Amps for DCW test. \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: No return
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_arc_current = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LIM:ARC {limit} \r \n"
             self.ser.write(set_arc_current.encode())
             self.ser.read(20).decode()
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def arc_get_current_limits(self, step, test_mode):
         """
-        This functions sets the ARC current limit for ACW/DCW test
-        :param step: The step for which the current is added in the range 1-49
-        :param test_mode: modes being AC/DC
-        :return: float: ARC current limit in Amps
+        ``This functions sets the ARC current limit for ACW/DCW test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC \n
+        :return: `float` : ARC current limit in Amps
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_arc_current = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:LIM:ARC? \r \n"
             self.ser.write(set_arc_current.encode())
             read_char_arc = self.ser.read(20).decode()
             logging.info(f": GET ARC CURRENT LIMIT for step {step}: {read_char_arc} Amps")
             return float(read_char_arc)
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def set_ramp_time(self, step, ramp_time, test_mode):
         """
-        This functions sets the RISE time for ACW/DCW/IR tests
-        :param step: The step for which the current is added in the range 1-49
-        :param ramp_time: Time in range 0~999.9 (0 is OFF) seconds for ACW/DCW/IR test.
-        :param test_mode: modes being AC/DC/IR
+        ``This functions sets the RISE time for ACW/DCW/IR tests`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param ramp_time: Time in range 0~999.9 (0 is OFF) seconds for ACW/DCW/IR test. \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: No return
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_ramp = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:TIME:RAMP {ramp_time} \r \n"
             self.ser.write(set_ramp.encode())
             self.ser.read(20).decode()
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def get_ramp_time(self, step, test_mode):
         """
-        This functions sets RAMP time for ACW/DCW/IR test
-        :param step: The step for which the current is added in the range 1-49
-        :param test_mode: modes being AC/DC/IR
-        :return: float: Ramp time in seconds
+        ``This functions sets RAMP time for ACW/DCW/IR test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: `float` : Ramp time in seconds
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             get_ramp = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:TIME:RAMP? \r \n"
             self.ser.write(get_ramp.encode())
             read_char_ramp = self.ser.read(20).decode()
             logging.log(f": GET RAMP TIME for step {step}: {read_char_ramp} seconds")
             return float(read_char_ramp)
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def set_fall_time(self, step, fall_time, test_mode):
         """
-        This functions sets the FALL time for ACW/DCW/IR tests
-        :param step: The step for which the current is added in the range 1-49
-        :param fall_time: Time in range 0~999.9 (0 is OFF) seconds for ACW/DCW/IR test.
-        :param test_mode: modes being AC/DC/IR
+        ``This functions sets the FALL time for ACW/DCW/IR tests`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param fall_time: Time in range 0~999.9 (0 is OFF) seconds for ACW/DCW/IR test. \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: No return
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_fall_time = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:TIME:FALL {fall_time} \r \n"
             self.ser.write(set_fall_time.encode())
             self.ser.read(20).decode()
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def get_fall_time(self, step, test_mode):
         """
-        This functions sets the FALL time for ACW/DCW/IR test
-        :param step: The step for which the current is added in the range 1-49
-        :param test_mode: modes being AC/DC/IR
-        :return: float: Fall time in seconds
+        ``This functions sets the FALL time for ACW/DCW/IR test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: `float` : Fall time in seconds
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             get_fall_time = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:TIME:FALL? \r \n"
             self.ser.write(get_fall_time.encode())
             read_char_fall = self.ser.read(20).decode()
             logging.info(f": GET FALL TIME for step {step}: {read_char_fall} seconds")
             return float(read_char_fall)
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def set_test_time(self, step, test_time, test_mode):
         """
-        This functions sets the TEST time for ACW/DCW/IR tests
-        :param step: The step for which the current is added in the range 1-49
-        :param test_time: Time in range 0~999.9 (0 is OFF) seconds for ACW/DCW/IR test
-        :param test_mode: modes being AC/DC/IR
+        ``This functions sets the TEST time for ACW/DCW/IR tests`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_time: Time in range 0~999.9 (0 is OFF) seconds for ACW/DCW/IR test \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: No return
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             set_test_time = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:TIME:FALL {test_time} \r \n"
             self.ser.write(set_test_time.encode())
             self.ser.read(20).decode()
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def get_test_time(self, step, test_mode):
         """
-        This functions sets the TEST time for the ACW/DCW/IR test
-        :param step: The step for which the current is added in the range 1-49
-        :param test_mode: modes being AC/DC/IR
-        :return: float: TEST time in seconds
+        ``This functions sets the TEST time for the ACW/DCW/IR test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: `float` : TEST time in seconds
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             get_test_time = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:TIME:FALL? \r \n"
             self.ser.write(get_test_time.encode())
             read_char_test = self.ser.read(20).decode()
             logging.info(f": GET TEST TIME for step {step}: {read_char_test} seconds")
             return float(read_char_test)
         else:
             raise OSError(f"ERROR: not the correct Test Mode : {test_mode}")
 
     def set_channel(self, step, test_mode, channel, chan_value):
         """
-        This functions sets HIGH/LOW/OPEN for the scanner channel for ACW/DCW/IR test.
-        :param step: The step for which the current is added in the range 1-49
-        :param test_mode: modes being AC/DC/IR
-        :param channel: Channel in the range of 1-8
-        :param chan_value: Channel values being HIGH/LOW/OPEN
+        ``This functions sets HIGH/LOW/OPEN for the scanner channel for ACW/DCW/IR test.`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC/IR \n
+        :param channel: Channel in the range of 1-8 \n
+        :param chan_value: Channel values being HIGH/LOW/OPEN \n
+        :return: No return
         """
         if (str(test_mode).upper() in COMMON_TEST_MODE) and (str(chan_value).upper() in CHANNEL_VALUE):
             set_channel_value = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:CHAN {channel}:{str(chan_value).upper()} \r \n"
             self.ser.write(set_channel_value.encode())
             self.ser.read(20).decode()
         else:
             raise OSError(f"ERROR: not the correct Test Mode: {test_mode} /Channel Value {chan_value}")
 
     def get_channel(self, step, test_mode, channel):
         """
-        This functions inquires about the set channel value for ACW/DCW/IR test.
-        :param channel: Channel value set in the range for 1-8
-        :param step: The step for which the current is added in the range 1-49
-        :param test_mode: modes being AC/DC/IR
-        :return: str: Channel value in HIGH/LOW/OPEN
+        ``This functions inquires about the set channel value for ACW/DCW/IR test.`` \n
+        :param channel: Channel value set in the range for 1-8 \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param test_mode: modes being AC/DC/IR \n
+        :return: `str` : Channel value in HIGH/LOW/OPEN
         """
         if str(test_mode).upper() in COMMON_TEST_MODE:
             get_test_time = f":SOUR:SAFE:STEP {step}:{str(test_mode).upper()}:CHAN {channel}? \r \n"
             self.ser.write(get_test_time.encode())
             read_char_chan_value = self.ser.read(20).decode()
             logging.info(f": GET CHANNEL VALUE for step {step} and channel {channel}: {read_char_chan_value}")
             return str(read_char_chan_value)
         else:
             raise OSError(f"ERROR: not the correct Test Mode: {test_mode}")
 
     def set_ac_freq(self, step, freq):
         """
-        This functions sets the test frequency for ACW test
-        :param step: The step for which the current is added in the range 1-49
-        :param freq: Set value 50/60 Hz in ACW test
+        ``This functions sets the test frequency for ACW test.`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :param freq: Set value 50/60 Hz in ACW test \n
+        :return: No return
         """
         set_test_time = f":SOUR:SAFE:STEP {step}:AC:TIME:FREQ {freq}\r \n"
         self.ser.write(set_test_time.encode())
         self.ser.read(20).decode()
 
     def get_ac_freq(self, step):
         """
-        This functions checks the test frequency for ACW test.
-        :param step: The step for which the current is added in the range 1-49
-        :return: float: Value for the test FREQUENCY
+        ``This functions checks the test frequency for ACW test.`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :return: `float` : Value for the test FREQUENCY
         """
         get_test_time = f":SOUR:SAFE:STEP {step}:AC:TIME:FREQ? \r \n"
         self.ser.write(get_test_time.encode())
         read_char_ac_freq = self.ser.read(20).decode()
         logging.info(f": GET AC FREQUENCY for step {step}: {read_char_ac_freq} Hz")
         return float(read_char_ac_freq)
 
     def set_real_current(self, step, real_curr):
         """
-        This functions sets the REAL current for ACW test
-        :param real_curr: Current in range 0~30.000E-3 (0 is OFF) Amps for ACW test
-        :param step: The step for which the current is added in the range 1-49
+        ``This functions sets the REAL current for ACW test`` \n
+        :param real_curr: Current in range 0~30.000E-3 (0 is OFF) Amps for ACW test \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :return: No return
         """
         set_ac_real_curr = f":SOUR:SAFE:STEP {step}:AC:LIM:REAL {real_curr}\r \n"
         self.ser.write(set_ac_real_curr.encode())
         self.ser.read(20).decode()
 
     def get_real_current(self, step):
         """
-        This functions checks the REAL current for ACW test
-        :param step: The step for which the current is added in the range 1-49
-        :return: float: Value for the REAL current
+        ``This functions checks the REAL current for ACW test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :return: `float` : Value for the REAL current
         """
         get_test_time = f":SOUR:SAFE:STEP {step}:AC:LIM:REAL? \r \n"
         self.ser.write(get_test_time.encode())
         read_char_real_curr = self.ser.read(20).decode()
         logging.info(f": GET AC REAL CURRENT for step {step}: {read_char_real_curr} Amps")
         return float(read_char_real_curr)
 
     def set_dc_wait_time(self, step, wait):
         """
-        This functions sets the WAIT time for DCW test
-        :param wait: Wait time in seconds in range 0~999.9 (0 is OFF) for DCW test
-        :param step: The step for which the current is added in the range 1-49
+        ``This functions sets the WAIT time for DCW test`` \n
+        :param wait: Wait time in seconds in range 0~999.9 (0 is OFF) for DCW test \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :return: No return
         """
         set_dc_wait = f":SOUR:SAFE:STEP {step}:DC:TIME:DWEL {wait}\r \n"
         self.ser.write(set_dc_wait.encode())
         self.ser.read(20).decode()
 
     def get_dc_wait_time(self, step):
         """
-        This functions checks the WAIT time for DCW test
-        :param step: The step for which the current is added in the range 1-49
-        :return: float: Value for the WAIT time in seconds
+        ``This functions checks the WAIT time for DCW test`` \n
+        :param step: The step for which the current is added in the range 1-49 \n
+        :return: `float` : Value for the WAIT time in seconds
         """
         get_dc_wait = f":SOUR:SAFE:STEP {step}:DC:TIME:DWEL? \r \n"
         self.ser.write(get_dc_wait.encode())
         read_char_wait = self.ser.read(20).decode()
         logging.info(f": GET DC WAIT TIME for step {step}: {read_char_wait} seconds")
         return float(read_char_wait)
 
     def set_ir_resistance(self, step, low_limit, high_limit):
         """
-        This functions sets the lower and upper resistance for IR test
-        :param step: The step for which the resistance is added in the range 1-49
-        :param low_limit: Lower Resistance in range 1.0E5~5.0E10 Ohms for IR test
-        :param high_limit: Upper Resistance in range 0~5E10 (0 is OFF) Ohms for IR test
+        ``This functions sets the lower and upper resistance for IR test`` \n
+        :param step: The step for which the resistance is added in the range 1-49 \n
+        :param low_limit: Lower Resistance in range 1.0E5~5.0E10 Ohms for IR test \n
+        :param high_limit: Upper Resistance in range 0~5E10 (0 is OFF) Ohms for IR test \n
+        :return: No return
         """
         set_low_resistance = f":SOUR:SAFE:STEP {step}:IR:LIM:LOW {low_limit} \r \n"
         self.ser.write(set_low_resistance.encode())
         self.ser.read(20).decode()
 
         set_high_resistance = f":SOUR:SAFE:STEP {step}:IR:LIM:HIGH {high_limit} \r \n"
         self.ser.write(set_high_resistance.encode())
         self.ser.read(20).decode()
 
     def get_ir_resistance(self, step):
         """
-        This function checks the lower and upper resistance set by the user/by default
-        :param step: The step for which the resistance is added in the range 1-49
-        :return: tuple: Lower and upper resistance limits in Ohms respectively
+        ``This function checks the lower and upper resistance set by the user/by default`` \n
+        :param step: The step for which the resistance is added in the range 1-49 \n
+        :return: `tuple` : Lower and upper resistance limits in Ohms respectively
         """
         get_low_resistance = f":SOUR:SAFE:STEP {step}:IR:LIM:LOW? \r \n"
         self.ser.write(get_low_resistance.encode())
         read_char_low = self.ser.read(20).decode()
         logging.info(f": GET LOW RESISTANCE for step {step}: {read_char_low} Ohms")
 
         get_high_resistance = f":SOUR:SAFE:STEP {step}:IR:LIM:HIGH? \r \n"
         self.ser.write(get_high_resistance.encode())
         read_char_high = self.ser.read(20).decode()
         logging.info(f": GET HIGH RESISTANCE for step {step}: {read_char_high} Ohms")
         return float(read_char_low), float(read_char_high)
 
-
```

### Comparing `pts_hipot_tester-0.0.8/PKG-INFO` & `pts_hipot_tester-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_hipot_tester
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hipot Tester Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/st9201-hipot-tester
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_hipot_tester-0.0.8/setup.py` & `pts_hipot_tester-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_hipot_tester",
-    version="0.0.8",
+    version="0.0.9",
     author="Pass testing Solutions GmbH",
     description="Hipot Tester Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/st9201-hipot-tester",
     license="MIT",
```

### Comparing `pts_hipot_tester-0.0.8/LICENSE.txt` & `pts_hipot_tester-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_hipot_tester-0.0.8/pts_hipot_tester.egg-info/PKG-INFO` & `pts_hipot_tester-0.0.9/pts_hipot_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-hipot-tester
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hipot Tester Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/st9201-hipot-tester
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_hipot_tester-0.0.8/README.md` & `pts_hipot_tester-0.0.9/README.md`

 * *Files identical despite different names*

