# Comparing `tmp/pydhcp3-0.0.1.tar.gz` & `tmp/pydhcp3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydhcp3-0.0.1.tar", last modified: Mon Apr 24 00:17:26 2023, max compression
+gzip compressed data, was "pydhcp3-0.0.2.tar", last modified: Wed Apr 26 00:57:16 2023, max compression
```

## Comparing `pydhcp3-0.0.1.tar` & `pydhcp3-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-24 00:15:16.000000 pydhcp3-0.0.1/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      249 2023-04-24 00:07:53.000000 pydhcp3-0.0.1/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.561128 pydhcp3-0.0.1/pydhcp/
--rw-r--r--   0 andrew    (1000) andrew    (1000)       37 2023-04-21 08:22:54.000000 pydhcp3-0.0.1/pydhcp/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2334 2023-04-23 01:51:49.000000 pydhcp3-0.0.1/pydhcp/base.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2023-04-20 03:29:25.000000 pydhcp3-0.0.1/pydhcp/enum.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1549 2023-04-22 23:15:15.000000 pydhcp3-0.0.1/pydhcp/exceptions.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/pydhcp/v4/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      653 2023-04-21 08:21:55.000000 pydhcp3-0.0.1/pydhcp/v4/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7975 2023-04-23 23:22:58.000000 pydhcp3-0.0.1/pydhcp/v4/enum.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5168 2023-04-23 23:33:10.000000 pydhcp3-0.0.1/pydhcp/v4/message.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4477 2023-04-23 23:23:41.000000 pydhcp3-0.0.1/pydhcp/v4/options.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/pydhcp/v4/server/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      155 2023-04-23 02:15:39.000000 pydhcp3-0.0.1/pydhcp/v4/server/__init__.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/pydhcp/v4/server/backend/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2324 2023-04-23 23:56:13.000000 pydhcp3-0.0.1/pydhcp/v4/server/backend/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2612 2023-04-23 23:40:22.000000 pydhcp3-0.0.1/pydhcp/v4/server/backend/cache.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7750 2023-04-24 00:03:37.000000 pydhcp3-0.0.1/pydhcp/v4/server/server.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/pydhcp/v6/
--rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-04-21 00:36:00.000000 pydhcp3-0.0.1/pydhcp/v6/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2354 2023-04-21 07:58:15.000000 pydhcp3-0.0.1/pydhcp/v6/duid.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1452 2023-04-21 08:20:56.000000 pydhcp3-0.0.1/pydhcp/v6/enum.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4381 2023-04-21 08:16:49.000000 pydhcp3-0.0.1/pydhcp/v6/message.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5065 2023-04-21 08:20:18.000000 pydhcp3-0.0.1/pydhcp/v6/options.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/pydhcp3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-04-24 00:17:26.000000 pydhcp3-0.0.1/pydhcp3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      559 2023-04-24 00:17:26.000000 pydhcp3-0.0.1/pydhcp3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-24 00:17:26.000000 pydhcp3-0.0.1/pydhcp3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       41 2023-04-24 00:17:26.000000 pydhcp3-0.0.1/pydhcp3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-04-24 00:17:26.000000 pydhcp3-0.0.1/pydhcp3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-24 00:17:26.565127 pydhcp3-0.0.1/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      777 2023-04-24 00:17:03.000000 pydhcp3-0.0.1/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-24 00:15:16.000000 pydhcp3-0.0.2/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      249 2023-04-24 00:07:53.000000 pydhcp3-0.0.2/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       37 2023-04-21 08:22:54.000000 pydhcp3-0.0.2/pydhcp/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2334 2023-04-26 00:55:45.000000 pydhcp3-0.0.2/pydhcp/base.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2023-04-20 03:29:25.000000 pydhcp3-0.0.2/pydhcp/enum.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1549 2023-04-22 23:15:15.000000 pydhcp3-0.0.2/pydhcp/exceptions.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/v4/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      672 2023-04-26 00:40:44.000000 pydhcp3-0.0.2/pydhcp/v4/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7975 2023-04-23 23:22:58.000000 pydhcp3-0.0.2/pydhcp/v4/enum.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5180 2023-04-26 00:49:02.000000 pydhcp3-0.0.2/pydhcp/v4/message.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4486 2023-04-26 00:47:50.000000 pydhcp3-0.0.2/pydhcp/v4/options.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/v4/server/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      155 2023-04-23 02:15:39.000000 pydhcp3-0.0.2/pydhcp/v4/server/__init__.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/v4/server/backend/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2324 2023-04-23 23:56:13.000000 pydhcp3-0.0.2/pydhcp/v4/server/backend/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2612 2023-04-23 23:40:22.000000 pydhcp3-0.0.2/pydhcp/v4/server/backend/cache.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8039 2023-04-26 00:39:20.000000 pydhcp3-0.0.2/pydhcp/v4/server/server.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/pydhcp/v6/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-04-21 00:36:00.000000 pydhcp3-0.0.2/pydhcp/v6/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2354 2023-04-21 07:58:15.000000 pydhcp3-0.0.2/pydhcp/v6/duid.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1452 2023-04-21 08:20:56.000000 pydhcp3-0.0.2/pydhcp/v6/enum.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4381 2023-04-21 08:16:49.000000 pydhcp3-0.0.2/pydhcp/v6/message.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5065 2023-04-21 08:20:18.000000 pydhcp3-0.0.2/pydhcp/v6/options.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/pydhcp3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      559 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       41 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      777 2023-04-26 00:56:58.000000 pydhcp3-0.0.2/setup.py
```

### Comparing `pydhcp3-0.0.1/LICENSE` & `pydhcp3-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/PKG-INFO` & `pydhcp3-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydhcp3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Python DHCP Library. DHCP Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydhcp
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydhcp3-0.0.1/pydhcp/base.py` & `pydhcp3-0.0.2/pydhcp/base.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/enum.py` & `pydhcp3-0.0.2/pydhcp/enum.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/exceptions.py` & `pydhcp3-0.0.2/pydhcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v4/__init__.py` & `pydhcp3-0.0.2/pydhcp/v4/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     'OptionCode',
 
     'Message',
 
     'Option',
     'OptionList',
     'OptEnd',
+    'OptServerId',
     'OptSubnetMask',
     'OptRouter',
     'OptDNS',
     'OptRequestedAddr',
     'OptIPLeaseTime',
     'OptMessageType',
     'OptParamRequestList',
```

### Comparing `pydhcp3-0.0.1/pydhcp/v4/enum.py` & `pydhcp3-0.0.2/pydhcp/v4/enum.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v4/message.py` & `pydhcp3-0.0.2/pydhcp/v4/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ipaddress import IPv4Address
 from typing import Union, List, Optional
 from typing_extensions import Self
 
 from pystructs import *
 
 from .enum import MessageType, OpCode, OptionCode
-from .options import OptionList, read_option
+from .options import OptionList, read_option, write_option
 from ..enum import HwType
 
 #** Variables **#
 __all__ = ['Message']
 
 #: magic cookie to include in DHCP message
 MAGIC_COOKIE = bytes([0x63, 0x82, 0x53, 0x63])
@@ -118,31 +118,31 @@
         serialize DHCP Message as bytes to send via socket
         """
         ctx   = Context()
         data  = bytearray()
         data += Header(
             opcode=self.op,
             hw_type=self.hw_type,
-            hw_length=6, #TODO: this might need to be dynamic somehow
+            hw_length=len(self.client_hw),
             hops=self.hops,
             message_id=self.id,
             seconds=self.seconds,
             flags=self.flags,
             client_addr=self.client_addr,
             your_addr=self.your_addr,
             server_addr=self.server_addr,
             gateway_addr=self.gateway_addr,
             hw_addr=self.client_hw,
             server_name=self.server_name,
             boot_file=self.boot_file,
         ).encode(ctx)
         for option in self.options:
-            data += option.encode(ctx)
+            data += write_option(ctx, option)
         if not any(opt.opcode == OptionCode.End for opt in self.options):
-            data += b'\x00'
+            data += bytes((OptionCode.End, ))
         return bytes(data)
 
     @classmethod
     def decode(cls, raw: bytes) -> Self:
         """
         deserialize encoded DHCP Message into Message object
         """
```

### Comparing `pydhcp3-0.0.1/pydhcp/v4/options.py` & `pydhcp3-0.0.2/pydhcp/v4/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #** Variables **#
 __all__ = [
     'read_option',
 
     'Option',
     'OptionList',
     'OptEnd',
+    'OptServerId',
     'OptSubnetMask',
     'OptRouter',
     'OptDNS',
     'OptRequestedAddr',
     'OptStatusCode',
     'OptIPLeaseTime',
     'OptMessageType',
@@ -56,15 +57,15 @@
     # parse option w/ it's own sub-context
     subctx = Context()
     option = oclass.decode(subctx, opt.value)
     if oclass is Option:
         oclass.opcode = opt.code
     return option
 
-def write_option(ctx: Context, option: 'Option') -> bytes:
+def write_option(ctx: Context, option) -> bytes:
     """
     write and serialize option-class into raw-bytes
     
     :param ctx: serialization context
     :param raw: option object to serialize
     :return:    serialized bytes
     """
```

### Comparing `pydhcp3-0.0.1/pydhcp/v4/server/backend/__init__.py` & `pydhcp3-0.0.2/pydhcp/v4/server/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v4/server/backend/cache.py` & `pydhcp3-0.0.2/pydhcp/v4/server/backend/cache.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v4/server/server.py` & `pydhcp3-0.0.2/pydhcp/v4/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 PyServe Session DHCPv4 Implementation
 """
 from abc import ABC, abstractmethod
+from ipaddress import IPv4Address
 from logging import Logger, getLogger
 from dataclasses import dataclass, field
 from typing import Optional
 
 from pyserve import Address, Writer
 from pyserve import Session as BaseSession
 
@@ -28,16 +29,17 @@
     """translate hardware address to mac"""
     return ':'.join(f'{c:02x}' for c in hwaddr)
 
 #** Classes **#
 
 @dataclass
 class Session(BaseSession, ABC):
-    backend: Backend
-    logger:  Logger = field(default_factory=lambda: getLogger('pydhcp'))
+    backend:   Backend
+    logger:    Logger = field(default_factory=lambda: getLogger('pydhcp'))
+    server_id: Optional[IPv4Address] = None
 
     ## Overrides
 
     @abstractmethod
     def process_discover(self, req: Message) -> Optional[Message]:
         raise NotImplementedError 
 
@@ -70,17 +72,17 @@
             options=OptionList(),
         )
 
     ## Session Impl
 
     def connection_made(self, addr: Address, writer: Writer):
         """handle session initialization on connection-made"""
-        self.addr     = addr
-        self.writer   = writer
-        self.addr_str = '%s:%d' % self.addr
+        self.addr      = addr
+        self.writer    = writer
+        self.addr_str  = '%s:%d' % self.addr
 
     def data_recieved(self, data: bytes):
         """recieve DHCPv4 request and generate response"""
         self.logger.debug(f'{self.addr_str} | recieved {len(data)} bytes')
         # parse initial request message
         request      = Message.decode(data)
         message_type = request.message_type()
@@ -113,14 +115,18 @@
             response.options.extend([nak, status])
             raise e
         finally:
             if response is None:
                 self.logger.error(f'{self.addr_str} | No Response Given.')
                 self.writer.close()
             else:
+                # apply server-identifier when given
+                if self.server_id:
+                    response.options.append(OptServerId(self.server_id))
+                # encode and send response
                 data = response.encode()
                 self.logger.debug(f'{self.addr_str} | sent {len(data)} bytes')
                 self.writer.write(data, addr=(BROADCAST, self.addr.port))
 
     def connection_lost(self, err: Optional[Exception]):
         """debug log connection lost"""
         self.logger.debug(f'{self.addr_str} | connection-lost err={err}')
```

### Comparing `pydhcp3-0.0.1/pydhcp/v6/duid.py` & `pydhcp3-0.0.2/pydhcp/v6/duid.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v6/enum.py` & `pydhcp3-0.0.2/pydhcp/v6/enum.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v6/message.py` & `pydhcp3-0.0.2/pydhcp/v6/message.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp/v6/options.py` & `pydhcp3-0.0.2/pydhcp/v6/options.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/pydhcp3.egg-info/PKG-INFO` & `pydhcp3-0.0.2/pydhcp3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydhcp3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Python DHCP Library. DHCP Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydhcp
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydhcp3-0.0.1/pydhcp3.egg-info/SOURCES.txt` & `pydhcp3-0.0.2/pydhcp3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.1/setup.py` & `pydhcp3-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pydhcp3',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pydhcp',
     description="Simple Python DHCP Library. DHCP Packet-Parsing/Client/Server",
     long_description=readme,
     long_description_content_type="text/markdown",
```

