# Comparing `tmp/ebyte-lora-e22-0.0.2.tar.gz` & `tmp/ebyte-lora-e22-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebyte-lora-e22-0.0.2.tar", last modified: Tue Apr 18 14:12:54 2023, max compression
+gzip compressed data, was "ebyte-lora-e22-0.0.3.tar", last modified: Tue Apr 25 17:08:09 2023, max compression
```

## Comparing `ebyte-lora-e22-0.0.2.tar` & `ebyte-lora-e22-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:12:54.829271 ebyte-lora-e22-0.0.2/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e22-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0    28200 2023-04-18 14:12:54.830234 ebyte-lora-e22-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    25296 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/README.md
--rw-rw-rw-   0        0        0     1521 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      844 2023-04-18 14:12:54.833238 ebyte-lora-e22-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1514 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:12:54.800404 ebyte-lora-e22-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 14:12:54.816160 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/
--rw-rw-rw-   0        0        0    28200 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-18 14:12:54.000000 ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    28688 2023-04-18 14:11:21.000000 ebyte-lora-e22-0.0.2/src/lora_e22.py
--rw-rw-rw-   0        0        0    12924 2023-04-18 14:04:15.000000 ebyte-lora-e22-0.0.2/src/lora_e22_constants.py
--rw-rw-rw-   0        0        0     3615 2023-03-22 16:19:56.000000 ebyte-lora-e22-0.0.2/src/lora_e22_operation_constant.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:08:09.059065 ebyte-lora-e22-0.0.3/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e22-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0    28252 2023-04-25 17:08:09.059065 ebyte-lora-e22-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    25348 2023-04-25 17:07:29.000000 ebyte-lora-e22-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1521 2023-04-25 17:07:29.000000 ebyte-lora-e22-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      844 2023-04-25 17:08:09.061076 ebyte-lora-e22-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1514 2023-04-25 17:07:29.000000 ebyte-lora-e22-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:08:09.035899 ebyte-lora-e22-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:08:09.057335 ebyte-lora-e22-0.0.3/src/ebyte_lora_e22.egg-info/
+-rw-rw-rw-   0        0        0    28252 2023-04-25 17:08:08.000000 ebyte-lora-e22-0.0.3/src/ebyte_lora_e22.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-25 17:08:08.000000 ebyte-lora-e22-0.0.3/src/ebyte_lora_e22.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:08:08.000000 ebyte-lora-e22-0.0.3/src/ebyte_lora_e22.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-25 17:08:08.000000 ebyte-lora-e22-0.0.3/src/ebyte_lora_e22.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    28727 2023-04-25 17:07:29.000000 ebyte-lora-e22-0.0.3/src/lora_e22.py
+-rw-rw-rw-   0        0        0    12924 2023-04-18 14:04:15.000000 ebyte-lora-e22-0.0.3/src/lora_e22_constants.py
+-rw-rw-rw-   0        0        0     3615 2023-03-22 16:19:56.000000 ebyte-lora-e22-0.0.3/src/lora_e22_operation_constant.py
```

### Comparing `ebyte-lora-e22-0.0.2/LICENSE.md` & `ebyte-lora-e22-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e22-0.0.2/PKG-INFO` & `ebyte-lora-e22-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e22
-Version: 0.0.2
+Version: 0.0.3
 Summary: MicroPython LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266, esp32, Raspberry, rp2040 and STM32. sx1262/sx1268
 Home-page: https://github.com/xreef/EByte_LoRa_E22_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -58,14 +58,15 @@
 </div>
 
 #
 # EBYTE LoRa E22 devices micropython library (SX1262, SX1268)
 
 
 ### Changelog
+ - 2023-04-25 0.0.3 Minor fix on set configuration
  - 2023-04-18 0.0.2 Fix regular expression and better constant management
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.2 Summary: MicroPython
+Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.3 Summary: MicroPython
 LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266,
 esp32, Raspberry, rp2040 and STM32. sx1262/sx1268 Home-page: https://
 github.com/xreef/EByte_LoRa_E22_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -33,26 +33,27 @@
 Pico,rp2040,MicroPython,sx1262,sx1268,e22 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Programming Language :: Python :: Implementation
 :: MicroPython Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
 [Support_forum_EByte_e32_English]
 [Forum_supporto_EByte_e32_italiano]
 # # EBYTE LoRa E22 devices micropython library (SX1262, SX1268) ### Changelog -
-2023-04-18 0.0.2 Fix regular expression and better constant management - 2023-
-03-21 0.0.1 Fully functional library ### Library usage Here an example of
-constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. ### Installation To install the library
-execute the following command: ```bash pip install ebyte-lora-e22 ``` ####
-Initialization ```python from lora_e22 import LoRaE22 from machine import UART
-uart2 = UART(2) lora = LoRaE22('400T22D', uart2, aux_pin=15, m0_pin=21,
-m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
-print("Initialization: {}", ResponseStatusCode.get_description(code)) ``` ####
-Get Configuration ```python from lora_e22 import LoRaE22, print_configuration
-from lora_e22_operation_constant import ResponseStatusCode code, configuration
-= lora.get_configuration() print("Retrieve configuration: {}",
+2023-04-25 0.0.3 Minor fix on set configuration - 2023-04-18 0.0.2 Fix regular
+expression and better constant management - 2023-03-21 0.0.1 Fully functional
+library ### Library usage Here an example of constructor, you must pass the
+UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
+### Installation To install the library execute the following command: ```bash
+pip install ebyte-lora-e22 ``` #### Initialization ```python from lora_e22
+import LoRaE22 from machine import UART uart2 = UART(2) lora = LoRaE22
+('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
+transmission ```python code = lora.begin() print("Initialization: {}",
+ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
+from lora_e22 import LoRaE22, print_configuration from
+lora_e22_operation_constant import ResponseStatusCode code, configuration =
+lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` # ---------------------------------------- # HEAD : 0xc1 0x0
 0x9 # # AddH : 0x0 # AddL : 0x0 # # Chan : 23 -> 433 # # SpeedParityBit : 0b0 -
 > 8N1 (Default) # SpeedUARTDatte : 0b11 -> 9600bps (default) # SpeedAirDataRate
 : 0b10 -> 2.4kbps (default) # # OptionSubPacketSett: 0b0 -> 240bytes (default)
 # OptionTranPower : 0b0 -> 22dBm (Default) # OptionRSSIAmbientNo: 0b0 -
 > Disabled (default) # # TransModeWORPeriod : 0b11 -> 2000ms (default) #
```

### Comparing `ebyte-lora-e22-0.0.2/README.md` & `ebyte-lora-e22-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 </div>
 
 #
 # EBYTE LoRa E22 devices micropython library (SX1262, SX1268)
 
 
 ### Changelog
+ - 2023-04-25 0.0.3 Minor fix on set configuration
  - 2023-04-18 0.0.2 Fix regular expression and better constant management
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
 [Support_forum_EByte_e32_English]
 [Forum_supporto_EByte_e32_italiano]
 # # EBYTE LoRa E22 devices micropython library (SX1262, SX1268) ### Changelog -
-2023-04-18 0.0.2 Fix regular expression and better constant management - 2023-
-03-21 0.0.1 Fully functional library ### Library usage Here an example of
-constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. ### Installation To install the library
-execute the following command: ```bash pip install ebyte-lora-e22 ``` ####
-Initialization ```python from lora_e22 import LoRaE22 from machine import UART
-uart2 = UART(2) lora = LoRaE22('400T22D', uart2, aux_pin=15, m0_pin=21,
-m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
-print("Initialization: {}", ResponseStatusCode.get_description(code)) ``` ####
-Get Configuration ```python from lora_e22 import LoRaE22, print_configuration
-from lora_e22_operation_constant import ResponseStatusCode code, configuration
-= lora.get_configuration() print("Retrieve configuration: {}",
+2023-04-25 0.0.3 Minor fix on set configuration - 2023-04-18 0.0.2 Fix regular
+expression and better constant management - 2023-03-21 0.0.1 Fully functional
+library ### Library usage Here an example of constructor, you must pass the
+UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
+### Installation To install the library execute the following command: ```bash
+pip install ebyte-lora-e22 ``` #### Initialization ```python from lora_e22
+import LoRaE22 from machine import UART uart2 = UART(2) lora = LoRaE22
+('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
+transmission ```python code = lora.begin() print("Initialization: {}",
+ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
+from lora_e22 import LoRaE22, print_configuration from
+lora_e22_operation_constant import ResponseStatusCode code, configuration =
+lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` # ---------------------------------------- # HEAD : 0xc1 0x0
 0x9 # # AddH : 0x0 # AddL : 0x0 # # Chan : 23 -> 433 # # SpeedParityBit : 0b0 -
 > 8N1 (Default) # SpeedUARTDatte : 0b11 -> 9600bps (default) # SpeedAirDataRate
 : 0b10 -> 2.4kbps (default) # # OptionSubPacketSett: 0b0 -> 240bytes (default)
 # OptionTranPower : 0b0 -> 22dBm (Default) # OptionRSSIAmbientNo: 0b0 -
 > Disabled (default) # # TransModeWORPeriod : 0b11 -> 2000ms (default) #
```

### Comparing `ebyte-lora-e22-0.0.2/pyproject.toml` & `ebyte-lora-e22-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2265 6279 7465 2d6c 6f72 612d 6532  = "ebyte-lora-e2
 00000020: 3222 0d0a 7665 7273 696f 6e20 3d20 2230  2"..version = "0
-00000030: 2e30 2e32 220d 0a61 7574 686f 7273 203d  .0.2"..authors =
+00000030: 2e30 2e33 220d 0a61 7574 686f 7273 203d  .0.3"..authors =
 00000040: 205b 0d0a 2020 7b20 6e61 6d65 3d22 5265   [..  { name="Re
 00000050: 6e7a 6f20 4d69 7363 6869 616e 7469 222c  nzo Mischianti",
 00000060: 2065 6d61 696c 3d22 7265 6e7a 6f40 6d69   email="renzo@mi
 00000070: 7363 6869 616e 7469 2e6f 7267 2220 7d2c  schianti.org" },
 00000080: 0d0a 5d0d 0a6d 6169 6e74 6169 6e65 7273  ..]..maintainers
 00000090: 203d 205b 0d0a 2020 7b20 6e61 6d65 3d22   = [..  { name="
 000000a0: 5265 6e7a 6f20 4d69 7363 6869 616e 7469  Renzo Mischianti
```

### Comparing `ebyte-lora-e22-0.0.2/setup.cfg` & `ebyte-lora-e22-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6279 7465 2d6c 6f72 612d 6532   = ebyte-lora-e2
 00000020: 320d 0a76 6572 7369 6f6e 203d 2030 2e30  2..version = 0.0
-00000030: 2e32 0d0a 6175 7468 6f72 203d 2052 656e  .2..author = Ren
+00000030: 2e33 0d0a 6175 7468 6f72 203d 2052 656e  .3..author = Ren
 00000040: 7a6f 204d 6973 6368 6961 6e74 690d 0a64  zo Mischianti..d
 00000050: 6573 6372 6970 7469 6f6e 203d 2022 4d69  escription = "Mi
 00000060: 6372 6f50 7974 686f 6e20 4c6f 5261 2045  croPython LoRa E
 00000070: 4259 5445 2045 3232 2064 6576 6963 6520  BYTE E22 device 
 00000080: 6c69 6272 6172 7920 636f 6d70 6c65 7465  library complete
 00000090: 2061 6e64 2074 6573 7465 6420 7769 7468   and tested with
 000000a0: 2041 7264 7569 6e6f 2053 414d 442c 2065   Arduino SAMD, e
```

### Comparing `ebyte-lora-e22-0.0.2/setup.py` & `ebyte-lora-e22-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="micropython-lora-e22",
     package_dir={'': 'src'},
     py_modules=["lora_e22", "lora_e22_constants", "lora_e22_operation_constant"],
-    version="0.0.2",
+    version="0.0.3",
     description="MicroPython LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266, esp32, Raspberry, rp2040 and STM32. sx1262/sx1268",
     long_description="MicroPython Ebyte E22 LoRa (Long Range) library device very cheap and very long range (from 4Km to 10Km). LoRa EBYTE E22 device library complete and tested with  Arduino SAMD, esp8266, esp32 and STM32. sx1262/sx1268",
     keywords="LoRa, UART, EByte, esp32, esp8266, stm32, SAMD, Arduino, Raspberry Pi Pico, rp2040, MicroPython,sx1262, sx1268, e22",
     url="https://github.com/xreef/EByte_LoRa_E22_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `ebyte-lora-e22-0.0.2/src/ebyte_lora_e22.egg-info/PKG-INFO` & `ebyte-lora-e22-0.0.3/src/ebyte_lora_e22.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e22
-Version: 0.0.2
+Version: 0.0.3
 Summary: MicroPython LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266, esp32, Raspberry, rp2040 and STM32. sx1262/sx1268
 Home-page: https://github.com/xreef/EByte_LoRa_E22_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -58,14 +58,15 @@
 </div>
 
 #
 # EBYTE LoRa E22 devices micropython library (SX1262, SX1268)
 
 
 ### Changelog
+ - 2023-04-25 0.0.3 Minor fix on set configuration
  - 2023-04-18 0.0.2 Fix regular expression and better constant management
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.2 Summary: MicroPython
+Metadata-Version: 2.1 Name: ebyte-lora-e22 Version: 0.0.3 Summary: MicroPython
 LoRa EBYTE E22 device library complete and tested with Arduino SAMD, esp8266,
 esp32, Raspberry, rp2040 and STM32. sx1262/sx1268 Home-page: https://
 github.com/xreef/EByte_LoRa_E22_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -33,26 +33,27 @@
 Pico,rp2040,MicroPython,sx1262,sx1268,e22 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Programming Language :: Python :: Implementation
 :: MicroPython Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
 [Support_forum_EByte_e32_English]
 [Forum_supporto_EByte_e32_italiano]
 # # EBYTE LoRa E22 devices micropython library (SX1262, SX1268) ### Changelog -
-2023-04-18 0.0.2 Fix regular expression and better constant management - 2023-
-03-21 0.0.1 Fully functional library ### Library usage Here an example of
-constructor, you must pass the UART interface and (if you want, but It's
-reccomended) the AUX pin, M0 and M1. ### Installation To install the library
-execute the following command: ```bash pip install ebyte-lora-e22 ``` ####
-Initialization ```python from lora_e22 import LoRaE22 from machine import UART
-uart2 = UART(2) lora = LoRaE22('400T22D', uart2, aux_pin=15, m0_pin=21,
-m1_pin=19) ``` #### Start the module transmission ```python code = lora.begin()
-print("Initialization: {}", ResponseStatusCode.get_description(code)) ``` ####
-Get Configuration ```python from lora_e22 import LoRaE22, print_configuration
-from lora_e22_operation_constant import ResponseStatusCode code, configuration
-= lora.get_configuration() print("Retrieve configuration: {}",
+2023-04-25 0.0.3 Minor fix on set configuration - 2023-04-18 0.0.2 Fix regular
+expression and better constant management - 2023-03-21 0.0.1 Fully functional
+library ### Library usage Here an example of constructor, you must pass the
+UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
+### Installation To install the library execute the following command: ```bash
+pip install ebyte-lora-e22 ``` #### Initialization ```python from lora_e22
+import LoRaE22 from machine import UART uart2 = UART(2) lora = LoRaE22
+('400T22D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
+transmission ```python code = lora.begin() print("Initialization: {}",
+ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
+from lora_e22 import LoRaE22, print_configuration from
+lora_e22_operation_constant import ResponseStatusCode code, configuration =
+lora.get_configuration() print("Retrieve configuration: {}",
 ResponseStatusCode.get_description(code)) print_configuration(configuration)
 ``` The result ``` # ---------------------------------------- # HEAD : 0xc1 0x0
 0x9 # # AddH : 0x0 # AddL : 0x0 # # Chan : 23 -> 433 # # SpeedParityBit : 0b0 -
 > 8N1 (Default) # SpeedUARTDatte : 0b11 -> 9600bps (default) # SpeedAirDataRate
 : 0b10 -> 2.4kbps (default) # # OptionSubPacketSett: 0b0 -> 240bytes (default)
 # OptionTranPower : 0b0 -> 22dBm (Default) # OptionRSSIAmbientNo: 0b0 -
 > Disabled (default) # # TransModeWORPeriod : 0b11 -> 2000ms (default) #
```

### Comparing `ebyte-lora-e22-0.0.2/src/lora_e22.py` & `ebyte-lora-e22-0.0.3/src/lora_e22.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #############################################################################################
 # EBYTE LoRa E22 Series for MicroPython
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.2
+# VERSION: 0.0.3
 #
 # This library is based on the work of:
 # https://www.mischianti.org/category/my-libraries/lora-e22-devices/
 #
 # This library implements the EBYTE LoRa E22 Series for MicroPython.
 #
 # The MIT License (MIT)
@@ -493,15 +493,17 @@
             self.set_mode(prev_mode)
             return code, None
 
         code = self.set_mode(prev_mode)
         if code != ResponseStatusCode.E22_SUCCESS:
             return code, None
 
-        data = self.uart.read()
+        self.managed_delay(100)
+
+        data = self.uart.read_all()
         logger.debug("data: {}".format(data))
         logger.debug("data len: {}".format(len(data)))
 
         if data is None or len(data) != PacketLength.PL_CONFIGURATION+3:
             code = ResponseStatusCode.ERR_E22_DATA_SIZE_NOT_MATCH
             return code, None
```

### Comparing `ebyte-lora-e22-0.0.2/src/lora_e22_constants.py` & `ebyte-lora-e22-0.0.3/src/lora_e22_constants.py`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e22-0.0.2/src/lora_e22_operation_constant.py` & `ebyte-lora-e22-0.0.3/src/lora_e22_operation_constant.py`

 * *Files identical despite different names*

