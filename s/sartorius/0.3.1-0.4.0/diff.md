# Comparing `tmp/sartorius-0.3.1.tar.gz` & `tmp/sartorius-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sartorius-0.3.1.tar", last modified: Mon Mar  6 23:08:21 2023, max compression
+gzip compressed data, was "sartorius-0.4.0.tar", last modified: Wed Apr 26 21:17:17 2023, max compression
```

## Comparing `sartorius-0.3.1.tar` & `sartorius-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 23:08:21.498524 sartorius-0.3.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       64 2023-03-06 23:05:10.000000 sartorius-0.3.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18092 2021-07-02 17:04:12.000000 sartorius-0.3.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3060 2023-03-06 23:08:21.498607 sartorius-0.3.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2216 2021-07-02 17:04:12.000000 sartorius-0.3.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 23:08:21.497734 sartorius-0.3.1/sartorius/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1328 2022-08-23 20:25:06.000000 sartorius-0.3.1/sartorius/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3259 2022-08-23 19:16:34.000000 sartorius-0.3.1/sartorius/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1192 2021-07-02 17:04:12.000000 sartorius-0.3.1/sartorius/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3914 2023-03-06 23:06:40.000000 sartorius-0.3.1/sartorius/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 23:08:21.498423 sartorius-0.3.1/sartorius.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3060 2023-03-06 23:08:21.000000 sartorius-0.3.1/sartorius.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      325 2023-03-06 23:08:21.000000 sartorius-0.3.1/sartorius.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-03-06 23:08:21.000000 sartorius-0.3.1/sartorius.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       53 2023-03-06 23:08:21.000000 sartorius-0.3.1/sartorius.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       93 2023-03-06 23:08:21.000000 sartorius-0.3.1/sartorius.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       10 2023-03-06 23:08:21.000000 sartorius-0.3.1/sartorius.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      241 2023-03-06 23:08:21.498834 sartorius-0.3.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1384 2023-03-06 23:07:36.000000 sartorius-0.3.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:17:17.524237 sartorius-0.4.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       74 2023-04-25 18:54:02.000000 sartorius-0.4.0/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18092 2021-07-02 17:04:12.000000 sartorius-0.4.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3011 2023-04-26 21:17:17.524309 sartorius-0.4.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2216 2021-07-02 17:04:12.000000 sartorius-0.4.0/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:17:17.523247 sartorius-0.4.0/sartorius/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1375 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3504 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1282 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4022 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:17:17.524127 sartorius-0.4.0/sartorius.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3011 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      344 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       53 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       84 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       10 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      283 2023-04-26 21:17:17.524572 sartorius-0.4.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1370 2023-04-26 21:17:07.000000 sartorius-0.4.0/setup.py
```

### Comparing `sartorius-0.3.1/LICENSE` & `sartorius-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sartorius-0.3.1/PKG-INFO` & `sartorius-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: sartorius
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python driver for Sartorius and Minebea Intec scales.
-Home-page: http://github.com/numat/sartorius/
+Home-page: https://github.com/numat/sartorius/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `sartorius-0.3.1/README.md` & `sartorius-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sartorius-0.3.1/sartorius/__init__.py` & `sartorius-0.4.0/sartorius/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Python driver for Sartorius and Minebea Intec scales.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2019 NuMat Technologies
 """
+from typing import Any
+
 from sartorius.driver import Scale
 
 
-def command_line(args=None):
+def command_line(args: Any = None) -> None:
     """Command line tool exposed through package install."""
     import argparse
     import asyncio
     import json
 
     parser = argparse.ArgumentParser(description="Read scale status.")
     parser.add_argument('address', help="The IP address of the scale.")
@@ -19,15 +21,15 @@
                         type=int, default=49155)
     parser.add_argument('-n', '--no-info', action='store_true', help="Exclude "
                         "scale information. Reduces communication overhead.")
     parser.add_argument('-z', '--zero', action='store_true', help="Tares and "
                         "zeroes the scale.")
     args = parser.parse_args(args)
 
-    async def get():
+    async def get() -> None:
         async with Scale(args.address, args.port) as scale:
             if args.zero:
                 await scale.zero()
             d = await scale.get()
             if not args.no_info and d.get('on', True):
                 d['info'] = await scale.get_info()
             print(json.dumps(d, indent=4))
```

### Comparing `sartorius-0.3.1/sartorius/driver.py` & `sartorius-0.4.0/sartorius/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,48 +14,52 @@
 class Scale(TcpClient):
     """Driver for Sartorius and Minebea Intec ethernet scales.
 
     This implements a version of the Scale Manufacturers Association
     standardized communications protocol.
     """
 
-    def __init__(self, ip: str, port: int = 49155):
+    def __init__(self, ip: str, port: int = 49155) -> None:
         """Set up connection parameters, IP address and port."""
-        self.units = None
+        self.units: str = ""
         if ":" in ip:
             port = int(ip.split(":")[1])
             ip = ip.split(':')[0]
         super().__init__(ip, port)
 
-    async def get(self):
+    async def get(self) -> dict:
         """Get scale reading."""
         response = await self._write_and_read('\x1bP')
+        if not response:
+            raise OSError("Unable to get reading from scale.")
         return self._parse(response)
 
-    async def get_info(self):
+    async def get_info(self) -> dict:
         """Get scale model, serial, and software version numbers."""
-        model = (await self._write_and_read('\x1bx1_')).strip()
-        serial = (await self._write_and_read('\x1bx2_')).strip()
-        software = (await self._write_and_read('\x1bx3_')).strip()
+        model = await self._write_and_read('\x1bx1_')
+        serial = await self._write_and_read('\x1bx2_')
+        software = await self._write_and_read('\x1bx3_')
+        if not (model and serial and software):
+            raise OSError("Unable to get information from scale.")
         response = {
-            'model': model,
-            'serial': serial,
-            'software': software,
+            'model': model.strip(),
+            'serial': serial.strip(),
+            'software': software.strip(),
         }
         for item in response.values():
             if (' + ' in item or ' kg' in item):
                 logger.error(f"Received malformed data: {response}")
                 return {}
         return response
 
-    async def zero(self):
+    async def zero(self) -> None:
         """Tare and zero the scale."""
         await self._write_and_read('\x1bT')
 
-    def _parse(self, response):
+    def _parse(self, response: str) -> dict:
         """Parse a scale response.
 
         Scale weight is returned according to the SMA communication standard:
             K K K K K K + * A A A A A A A A * E E E CR LF
         K: ID code character
         +: plus or minus
         *: space
```

### Comparing `sartorius-0.3.1/sartorius/mock.py` & `sartorius-0.4.0/sartorius/mock.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Contains mocks for driver objects for offline testing."""
 
 import asyncio
-from random import random, choice
+from random import choice, random
+from typing import Any
 from unittest.mock import MagicMock
 
 
 class Scale(MagicMock):
     """Mocks the Scale driver for offline testing."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Set up connection parameters with default scale port."""
         super().__init__(*args, **kwargs)
         self.info = {"model": "SIWADCP-1-",
                      "serial": "37454321",
                      "software": "00-37-09"}
 
-    async def __aenter__(self, *args):
+    async def __aenter__(self, *args: Any) -> Any:
         """Set up connection."""
         return self
 
-    async def __aexit__(self, *args):
+    async def __aexit__(self, *args: Any) -> None:
         """Close connection."""
         pass
 
-    async def get(self):
+    async def get(self) -> dict:
         """Get scale reading."""
         await asyncio.sleep(random() * 0.25)
         return {'stable': True,
                 'units': choice(['kg', 'lb']),
                 'mass': random() * 100.0}
 
-    async def get_info(self):
+    async def get_info(self) -> dict:
         """Get scale model, serial, and software version numbers."""
         await asyncio.sleep(random() * 0.1)
         return self.info
 
-    async def zero(self):
+    async def zero(self) -> None:
         """Tare and zero the scale."""
         await asyncio.sleep(random() * 0.1)
```

### Comparing `sartorius-0.3.1/sartorius/util.py` & `sartorius-0.4.0/sartorius/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 """Base functionality for async TCP communication.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2019 NuMat Technologies
 """
-try:
-    import asyncio
-except ImportError:
-    raise ImportError("TCP connections require python >=3.5.")
+
+import asyncio
 import logging
+from typing import Any, Dict, Optional
 
 logger = logging.getLogger('sartorius')
 
 
 class TcpClient():
     """A generic reconnecting asyncio TCP client.
 
     This base functionality can be used by any industrial control device
     communicating over TCP.
     """
 
-    def __init__(self, ip, port, eol='\r\n'):
+    def __init__(self, ip: str, port: int, eol: str = '\r\n'):
         """Set connection parameters.
 
         Connection is handled asynchronously, either using `async with` or
         behind the scenes on the first `await` call.
         """
         self.ip = ip
         self.port = port
         self.eol = eol.encode()
         self.open = False
         self.reconnecting = False
         self.timeouts = 0
         self.max_timeouts = 10
-        self.connection = {}
-        self.lock = None
+        self.connection: Dict[str, Any] = {}
+        self.lock: Optional[asyncio.Lock] = None
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> Any:
         """Provide async entrance to context manager.
 
         Contrasting synchronous access, this will connect on initialization.
         """
         await self._handle_connection()
         return self
 
-    def __exit__(self, *args):
+    def __exit__(self, *args: Any) -> None:
         """Provide exit to context manager."""
         self.close()
 
-    async def __aexit__(self, *args):
+    async def __aexit__(self, *args: Any) -> None:
         """Provide async exit to context manager."""
         self.close()
 
-    def close(self):
+    def close(self) -> None:
         """Close the TCP connection."""
         if self.open:
             self.connection['writer'].close()
         self.open = False
 
-    async def _connect(self):
+    async def _connect(self) -> None:
         """Asynchronously open a TCP connection with the server."""
         self.close()
         reader, writer = await asyncio.open_connection(self.ip, self.port)
         self.connection = {'reader': reader, 'writer': writer}
         self.open = True
 
-    async def _write_and_read(self, command):
+    async def _write_and_read(self, command: str) -> Optional[str]:
         """Write a command and read a response.
 
         As industrial devices are commonly unplugged, this has been expanded to
         handle recovering from disconnects.  A lock is used to queue multiple requests.
         """
         if not self.lock:
             # lock initialized here so the loop exists.
@@ -76,31 +75,31 @@
         async with self.lock:  # lock releases on CancelledError
             await self._handle_connection()
             if self.open:
                 try:
                     response = await self._handle_communication(command)
                 except asyncio.exceptions.IncompleteReadError:
                     logger.error('IncompleteReadError.  Are there multiple connections?')
-                    return {}
+                    return None
             else:
                 response = None
         return response
 
-    async def _handle_connection(self):
+    async def _handle_connection(self) -> None:
         """Automatically maintain TCP connection."""
         try:
             if not self.open:
                 await asyncio.wait_for(self._connect(), timeout=0.5)
             self.reconnecting = False
         except (asyncio.TimeoutError, OSError):
             if not self.reconnecting:
                 logger.error(f'Connecting to {self.ip} timed out.')
             self.reconnecting = True
 
-    async def _handle_communication(self, command):
+    async def _handle_communication(self, command: str) -> Optional[str]:
         """Manage communication, including timeouts and logging."""
         try:
             self.connection['writer'].write(command.encode() + self.eol)
             future = self.connection['reader'].readuntil(self.eol)
             line = await asyncio.wait_for(future, timeout=0.5)
             result = line.decode()
             self.timeouts = 0
```

### Comparing `sartorius-0.3.1/sartorius.egg-info/PKG-INFO` & `sartorius-0.4.0/sartorius.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: sartorius
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python driver for Sartorius and Minebea Intec scales.
-Home-page: http://github.com/numat/sartorius/
+Home-page: https://github.com/numat/sartorius/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `sartorius-0.3.1/setup.py` & `sartorius-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """Package manager setup for Sartorius driver."""
 from setuptools import setup
 
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="sartorius",
-    version="0.3.1",
+    version="0.4.0",
     description="Python driver for Sartorius and Minebea Intec scales.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="http://github.com/numat/sartorius/",
+    url="https://github.com/numat/sartorius/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     packages=['sartorius'],
+    package_data={'sartorius': ['py.typed']},
     extras_require={
-        'test': ['pytest>=6,<8',
-                 'pytest-cov>=2,<4',
-                 'pytest-asyncio==0.*',
-                 'flake8>=5.*',
-                 'flake8-docstrings==1.*']
+        'test': [
+            'mypy==1.2.0',
+            'pytest>=6,<8',
+            'pytest-cov>=4,<5',
+            'pytest-asyncio==0.*',
+            'ruff==0.0.263'
+        ]
     },
     entry_points={
         'console_scripts': [('sartorius = sartorius:command_line')]
     },
     license='GPLv2',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Human Machine Interfaces'
     ]
 )
```

