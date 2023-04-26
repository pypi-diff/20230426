# Comparing `tmp/adc_socketx-0.1.0.tar.gz` & `tmp/adc_socketx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adc_socketx-0.1.0.tar", max compression
+gzip compressed data, was "adc_socketx-0.1.1.tar", max compression
```

## Comparing `adc_socketx-0.1.0.tar` & `adc_socketx-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2023-03-27 19:35:20.131806 adc_socketx-0.1.0/LICENSE
--rw-r--r--   0        0        0     1613 2023-03-27 22:37:39.395225 adc_socketx-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-27 21:01:55.029199 adc_socketx-0.1.0/adc_socketx/__init__.py
--rw-r--r--   0        0        0     5577 2023-03-27 21:29:14.593364 adc_socketx-0.1.0/adc_socketx/commands.py
--rw-r--r--   0        0        0     2119 2023-03-27 20:12:39.551595 adc_socketx-0.1.0/adc_socketx/config.py
--rw-r--r--   0        0        0      766 2023-03-27 20:01:55.113352 adc_socketx-0.1.0/adc_socketx/data_models.py
--rw-r--r--   0        0        0     3460 2023-03-27 22:21:22.108754 adc_socketx-0.1.0/adc_socketx/main.py
--rw-r--r--   0        0        0      601 2023-03-27 22:10:47.576162 adc_socketx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 adc_socketx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-03-31 19:26:13.433935 adc_socketx-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2480 2023-04-26 02:07:58.109929 adc_socketx-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 21:01:55.029199 adc_socketx-0.1.1/adc_socketx/__init__.py
+-rw-r--r--   0        0        0     5622 2023-04-26 01:56:19.082727 adc_socketx-0.1.1/adc_socketx/commands.py
+-rw-r--r--   0        0        0     2186 2023-04-26 00:37:52.344844 adc_socketx-0.1.1/adc_socketx/config.py
+-rw-r--r--   0        0        0      766 2023-03-27 20:01:55.113352 adc_socketx-0.1.1/adc_socketx/data_models.py
+-rw-r--r--   0        0        0     5537 2023-04-26 01:55:33.662441 adc_socketx-0.1.1/adc_socketx/main.py
+-rw-r--r--   0        0        0      602 2023-04-26 02:00:05.269196 adc_socketx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 adc_socketx-0.1.1/PKG-INFO
```

### Comparing `adc_socketx-0.1.0/LICENSE` & `adc_socketx-0.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Pavel Russu (GTLAB Diagnostics, LLC)
+Copyright (c) 2023 Pavel Russu (GTLAB Diagnostic, LLC)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `adc_socketx-0.1.0/adc_socketx/commands.py` & `adc_socketx-0.1.1/adc_socketx/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import pathlib
 import socket
 import struct
 import time
-
-from adc_socketx import config
+from pathlib import Path
 
 import numpy as np
 import typer
 from rich.progress import track
 from soundfile import SoundFile
 
+from adc_socketx import config
+
 
 class SocketX:
     def __init__(
             self,
             host: str = config.SOCKET_HOST,
             port: str = config.SOCKET_PORT
     ) -> None:
-        self._host = host
-        self._port = port
+        self.host = host
+        self.port = port
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.settimeout(2)
 
     def connect(self) -> None:
         try:
-            self.sock.connect((self._host, self._port))
+            self.sock.connect((self.host, self.port))
         except socket.error as e:
             msg = (
                 f'err: {e}. Check settings: '
-                f'{config.SOCKET_HOST}:{config.SOCKET_PORT}'
+                f'{self.host}:{self.port}'
             )
             typer.secho(msg, fg=typer.colors.BRIGHT_RED)
             raise typer.Exit(1)
 
     def disconnect(self) -> None:
         self.sock.close()
 
@@ -60,21 +60,14 @@
     data = sock.receive(config.COMMAND_GET_INFO['response_len'])
     unpacked_data = struct.unpack(
         config.COMMAND_GET_INFO['struct_unpack_str'], data
     )
     return unpacked_data
 
 
-def adc_get_mode():
-    """Get mode from ADC."""
-    sock.send(config.COMMAND_GET_MODE['h_text'])
-    data = sock.receive(config.COMMAND_GET_MODE['response_len'])
-    print(data)
-
-
 def adc_set_mode(num_of_channels: bool, ch1: bool, ch2: bool) -> bool:
     """Set mode to ADC.
 
     Args:
         num_of_channels (bool):  True = 2, False = 1
         ch1 (bool): True = IEPE, False = AC
         ch2 (bool): True = IEPE, False = AC
@@ -113,39 +106,45 @@
     data = b''
     while data != config.COMMAND_ADC_OFF['response_ok']:
         sock.send(config.COMMAND_ADC_OFF['h_text'])
         data = sock.receive(8008)
     return True
 
 
-def record_to_wav(num_of_frames: int, num_of_channels: int) -> bool:
+def record_to_wav(
+    num_of_frames: int,
+    num_of_channels: int,
+    output_file_name: Path
+) -> bool:
     """Record the ADC data."""
     adc_off()
     data_frame = bytearray()
     sock.send(config.COMMAND_ADC_ON['h_text'])
-
-    p = pathlib.Path(config.FILE_PATH)
-    p.mkdir(parents=True, exist_ok=True)
-    file_name = time.strftime(config.FIlE_FORMAT)
-    path_filename = p / file_name
+    if sock.receive(3) != config.COMMAND_ADC_ON['response_ok']:
+        raise ValueError('ADC start failed')
+    if output_file_name is None:
+        p = Path(config.FILE_PATH)
+        p.mkdir(parents=True, exist_ok=True)
+        file_name = time.strftime(config.FIlE_FORMAT)
+        output_file_name = p / file_name
 
     with SoundFile(
-        path_filename, 'w', 96000, num_of_channels, subtype='PCM_24'
+        output_file_name, 'w', 96000, num_of_channels, subtype='PCM_24'
     ) as sf:
         for frame in track(
             range(1, num_of_frames + 1), description='Recording...'
         ):
             while len(data_frame) != 8008:
                 data_frame.extend(sock.receive(8008))
 
             unpacked_head = struct.unpack('<6c 2b 2I', data_frame[:16])
 
             if unpacked_head[-1] != frame:
                 adc_off()
-                path_filename.unlink()
+                output_file_name.unlink()
                 raise ValueError('Data frame is lost')
 
             data = data_frame[16:]
 
             if len(data) % 3 != 0:
                 adc_off()
                 raise ValueError('Size of data must be a multiple of 3 bytes')
@@ -154,20 +153,20 @@
 
             for _ in range(0, len(data), 3):
                 # Add 1 byte (\x00) to each chain
                 temp.append(0)
                 temp.extend(data[_:_ + 3])
 
             sig = np.frombuffer(temp, dtype='i4').reshape(-1, num_of_channels)
-            sf.write(sig)
+            sf.write(sig)  # add exceptions at v0.1.1
             data_frame.clear()
         adc_off()
 
     if unpacked_head[-1] == num_of_frames:
-        print(f'File is written to: {path_filename}')
+        print(f'File is written to: {output_file_name.absolute()}')
         return True
 
     return False
 
 
 def adc_reboot() -> bool:
     """Reboot ADC."""
```

### Comparing `adc_socketx-0.1.0/adc_socketx/config.py` & `adc_socketx-0.1.1/adc_socketx/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Socket connection
 SOCKET_HOST = '192.168.0.50'
+SOCKET_GATEWAY = '192.168.0.1'
 SOCKET_PORT = 5000
 
 # Default number of channels in (1, 2) __(used for recording)__
 NUM_OF_CHANNELS_DEFAULT = 1
 
 # Record's filename format
 FIlE_FORMAT = '__%Y-%m-%d__%H-%M-%S.wav'
 FILE_PATH = 'waves/'  # creates a file in the same place if empty
 
 # Byte frames (7992) settings
-FRAMES_1CH_PER_SECOND = 30.036
+FRAMES_1CH_PER_SECOND = 30.036 * 1.2
 FRAMES_2CH_PER_SECOND = 72.072
 
 # Commands
 COMMAND_GET_INFO = {
     'h_text': '47 45 54 5F 49 4E 46 4F 00',
     'response_len': 45,
     'struct_unpack_str': '<3i 8f x',
@@ -71,14 +72,15 @@
     'response_ok': b'OK\x00',
 }
 
 COMMAND_ADC_ON = {
     'h_text': '41 44 43 5F 4F 4E 00',
     'response_len': 3,
     'struct_pack_str': '<6c 2b 2I',
+    'response_ok': b'OK\x00',
 }
 
 COMMAND_ADC_OFF = {
     'h_text': '41 44 43 5F 4F 46 46 00',
     'response_len': 3,
     'response_ok': b'OK\x00',
 }
```

### Comparing `adc_socketx-0.1.0/adc_socketx/data_models.py` & `adc_socketx-0.1.1/adc_socketx/data_models.py`

 * *Files identical despite different names*

### Comparing `adc_socketx-0.1.0/pyproject.toml` & `adc_socketx-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "adc-socketx"
-version = "0.1.0"
+version = "0.1.1"
 description = "ADC socket data eXchange"
 authors = ["Pavel Russu <pavlucho@gmail.com>"]
-license = "GTLAB Diagnostic LLC"
+license = "GTLAB Diagnostic, LLC"
 readme = "README.md"
 
 [tool.poetry.scripts]
 adcx = "adc_socketx.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `adc_socketx-0.1.0/PKG-INFO` & `adc_socketx-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 Metadata-Version: 2.1
 Name: adc-socketx
-Version: 0.1.0
+Version: 0.1.1
 Summary: ADC socket data eXchange
-License: GTLAB Diagnostic LLC
+License: GTLAB Diagnostic, LLC
 Author: Pavel Russu
 Author-email: pavlucho@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
-# `adcx` <sup>0.1.0</sup>
+# `adcx` <sup>_v0.1.1_</sup>
 
 **ADC** socket data e**X**change py-script.
 
-GTLAB Diagnostic LLC, 2023
+_[GTLAB Diagnostic LLC](http://gtlab.pro), 2023_
 
 **Usage**:
 
 ```console
 $ adcx [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 **Commands**:
 
-* `get-info`: Get the ADC information.
-* `get-lan`: Get lan configuration and exit.
+* `get-info`: Get the ADC information (s/n, frequency, channels, calibration).
+* `get-lan`: Get lan configuration (port, ip, netmask, gateway, MAC).
 * `get-wav`: Record a signal from the ADC to a .wav file.
 * `reboot`: Reboot the ADC.
-* `set-ip`: Change the ipv4 address setting.
+* `set-lan`: Set lan (ipv4) settings (ip/netmask, gateway).
 
 ## `adcx get-info`
 
-Get the ADC information.
-(serial number, frequency, channels, calibration)
+Get the ADC information (s/n, frequency, channels, calibration).
 
 **Usage**:
 
 ```console
 $ adcx get-info [OPTIONS]
 ```
+**Options**:
+
+* `--ip TEXT`: IPv4 connection address  [default: 192.168.0.50]
+* `--help`: Show this message and exit.
 
 ## `adcx get-lan`
 
-Get lan configuration and exit.
+Get lan configuration (port, ip, netmask, gateway, MAC).
 
 **Usage**:
 
 ```console
 $ adcx get-lan [OPTIONS]
 ```
 
+**Options**:
+
+* `--ip TEXT`: IPv4 connection address  [default: 192.168.0.50]
+* `--help`: Show this message and exit.
+
 ## `adcx get-wav`
 
 Record a signal from the ADC to a .wav file.
 
 **Usage**:
 
 ```console
@@ -74,37 +82,50 @@
 
 * `SECONDS`: [required]
 
 **Options**:
 
 * `--ch INTEGER RANGE`: Set the number of channels to record  [default: 1; 1<=x<=2]
 * `--iepe / --no-iepe`: [default: iepe]
+* `--ip TEXT`: IPv4 connection address  [default: 192.168.0.50]
+* `--out FILE`: Path and name (only .wav extension!) of the file to be written
 * `--help`: Show this message and exit.
 
 ## `adcx reboot`
 
 Reboot the ADC.
 
 **Usage**:
 
 ```console
 $ adcx reboot [OPTIONS]
 ```
 
-## `adcx set-ip`
+**Options**:
 
-Change the ipv4 address setting.
+* `--ip TEXT`: IPv4 connection address  [default: 192.168.0.50]
+* `--help`: Show this message and exit.
+
+## `adcx set-lan`
+
+Set lan (ipv4) settings (ip/netmask, gateway).
 
 **Usage**:
 
 ```console
-$ adcx set-ip [OPTIONS] IPV4
+$ set-lan [OPTIONS] IPV4 [GATEWAY]
 ```
 
 **Arguments**:
 
-* `IPV4`: [required]
+* `IPV4`: New IPv4 address/netmask. Example: 192.168.0.50/24  [required]
+* `[GATEWAY]`: New IPv4 Gateway  [default: 192.168.0.1]
+
+**Options**:
+
+* `--ip TEXT`: IPv4 connection address  [default: 192.168.0.50]
+* `--help`: Show this message and exit.
 
 # `Contacts`
 [![Telegram Badge](https://img.shields.io/badge/-pavelrus-blue?style=social&logo=telegram&link=https://t.me/pavelrus)](https://t.me/pavelrus)<br>
 [![Gmail Badge](https://img.shields.io/badge/-pavlucho@gmail.com-c14438?style=flat&logo=Gmail&logoColor=white&link=mailto:pavlucho@gmail.com)](mailto:pavlucho@gmail.com)
```

