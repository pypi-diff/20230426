# Comparing `tmp/aiosc-0.1.4.tar.gz` & `tmp/aiosc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiosc-0.1.4.tar", last modified: Sat Oct  5 22:46:32 2019, max compression
+gzip compressed data, was "aiosc-0.1.5.tar", last modified: Wed Apr 26 19:19:32 2023, max compression
```

## Comparing `aiosc-0.1.4.tar` & `aiosc-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2019-10-05 22:46:32.000000 aiosc-0.1.4/
--rw-r--r--   0 art       (1000) art       (1000)     6614 2019-09-28 08:54:41.000000 aiosc-0.1.4/aiosc.py
--rw-r--r--   0 art       (1000) art       (1000)      832 2019-10-05 22:41:25.000000 aiosc-0.1.4/setup.py
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2019-10-05 22:46:32.000000 aiosc-0.1.4/examples/
--rwxr-xr-x   0 art       (1000) art       (1000)      386 2017-10-07 14:16:38.000000 aiosc-0.1.4/examples/server.py
--rwxr-xr-x   0 art       (1000) art       (1000)      666 2017-10-07 14:16:38.000000 aiosc-0.1.4/examples/echo_server.py
--rwxr-xr-x   0 art       (1000) art       (1000)      349 2017-10-07 14:16:38.000000 aiosc-0.1.4/examples/ordering.py
--rwxr-xr-x   0 art       (1000) art       (1000)      168 2019-09-28 08:52:31.000000 aiosc-0.1.4/examples/hello.py
--rw-r--r--   0 art       (1000) art       (1000)     2583 2017-12-05 09:42:38.000000 aiosc-0.1.4/README.rst
--rw-r--r--   0 art       (1000) art       (1000)       38 2019-10-05 22:46:32.000000 aiosc-0.1.4/setup.cfg
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2019-10-05 22:46:32.000000 aiosc-0.1.4/aiosc.egg-info/
--rw-r--r--   0 art       (1000) art       (1000)        1 2019-10-05 22:46:32.000000 aiosc-0.1.4/aiosc.egg-info/dependency_links.txt
--rw-r--r--   0 art       (1000) art       (1000)      246 2019-10-05 22:46:32.000000 aiosc-0.1.4/aiosc.egg-info/SOURCES.txt
--rw-r--r--   0 art       (1000) art       (1000)        6 2019-10-05 22:46:32.000000 aiosc-0.1.4/aiosc.egg-info/top_level.txt
--rw-r--r--   0 art       (1000) art       (1000)     3911 2019-10-05 22:46:32.000000 aiosc-0.1.4/aiosc.egg-info/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)     1096 2014-07-20 12:07:47.000000 aiosc-0.1.4/LICENSE
--rw-r--r--   0 art       (1000) art       (1000)     3911 2019-10-05 22:46:32.000000 aiosc-0.1.4/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)       57 2014-07-26 10:42:56.000000 aiosc-0.1.4/MANIFEST.in
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-04-26 19:19:32.389401 aiosc-0.1.5/
+-rw-r--r--   0 art       (1000) art       (1000)     1096 2023-04-14 19:17:39.000000 aiosc-0.1.5/LICENSE
+-rw-r--r--   0 art       (1000) art       (1000)       57 2023-04-14 19:17:39.000000 aiosc-0.1.5/MANIFEST.in
+-rw-r--r--   0 art       (1000) art       (1000)     4047 2023-04-26 19:19:32.388401 aiosc-0.1.5/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)     3456 2023-04-26 19:18:28.000000 aiosc-0.1.5/README.rst
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-04-26 19:19:32.388401 aiosc-0.1.5/aiosc.egg-info/
+-rw-r--r--   0 art       (1000) art       (1000)     4047 2023-04-26 19:19:32.000000 aiosc-0.1.5/aiosc.egg-info/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)      246 2023-04-26 19:19:32.000000 aiosc-0.1.5/aiosc.egg-info/SOURCES.txt
+-rw-r--r--   0 art       (1000) art       (1000)        1 2023-04-26 19:19:32.000000 aiosc-0.1.5/aiosc.egg-info/dependency_links.txt
+-rw-r--r--   0 art       (1000) art       (1000)        6 2023-04-26 19:19:32.000000 aiosc-0.1.5/aiosc.egg-info/top_level.txt
+-rw-r--r--   0 art       (1000) art       (1000)     6724 2023-04-14 19:17:39.000000 aiosc-0.1.5/aiosc.py
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-04-26 19:19:32.388401 aiosc-0.1.5/examples/
+-rwxr-xr-x   0 art       (1000) art       (1000)      703 2023-04-14 19:17:39.000000 aiosc-0.1.5/examples/echo_server.py
+-rwxr-xr-x   0 art       (1000) art       (1000)      154 2023-04-14 19:17:39.000000 aiosc-0.1.5/examples/hello.py
+-rwxr-xr-x   0 art       (1000) art       (1000)      349 2023-04-14 19:17:39.000000 aiosc-0.1.5/examples/ordering.py
+-rwxr-xr-x   0 art       (1000) art       (1000)      425 2023-04-26 19:15:27.000000 aiosc-0.1.5/examples/server.py
+-rw-r--r--   0 art       (1000) art       (1000)       38 2023-04-26 19:19:32.389401 aiosc-0.1.5/setup.cfg
+-rw-r--r--   0 art       (1000) art       (1000)      832 2023-04-26 19:18:28.000000 aiosc-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiosc-0.1.4/aiosc.py` & `aiosc-0.1.5/aiosc.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,17 @@
     for t in type_tag[1:]:
         if t == 'i':
             len = 4
             value, tail = struct.unpack('>i', tail[:len])[0], tail[len:]
         elif t == 'f':
             len = 4
             value, tail = struct.unpack('>f', tail[:len])[0], tail[len:]
+        elif t == 'h':
+            len = 8
+            value, tail = struct.unpack('>q', tail[:len])[0], tail[len:]
         elif t == 's':
             value, tail = read_string(tail)
         elif t == 'b':
             value, tail = read_blob(tail)
         elif t == 'T':
             value = True
         elif t == 'F':
@@ -191,11 +194,11 @@
             if pattern_re.match(path):
                 handler(addr, path, *args)
 
     def send(self, path, *args, addr=None):
         return self.transport.sendto(pack_message(path, *args), addr=addr)
 
 async def send(target, path, *args, loop=None):
-    loop = loop or asyncio.get_event_loop()
+    loop = asyncio.get_running_loop()
     transport, protocol = await loop.create_datagram_endpoint(OSCProtocol, remote_addr=target)
     protocol.send(path, *args)
     transport.close()
```

### Comparing `aiosc-0.1.4/setup.py` & `aiosc-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
     name='aiosc',
     author='Artem Popov',
     author_email='artfwo@gmail.com',
     url='https://github.com/artfwo/aiosc',
     description='Minimalistic Open Sound Control (OSC) communication module using asyncio',
     long_description=long_description,
-    version='0.1.4',
+    version='0.1.5',
     py_modules=['aiosc'],
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `aiosc-0.1.4/examples/echo_server.py` & `aiosc-0.1.5/examples/echo_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,13 +14,15 @@
         asyncio.get_event_loop().stop()
 
     def echo(self, addr, path, *args):
         print("incoming message from {}: {} {}".format(addr, path, args))
         # echo the message
         self.send(path, *args, addr=addr)
 
-loop = asyncio.get_event_loop()
+async def main():
+    loop = asyncio.get_running_loop()
+    transport, protocol = await loop.create_datagram_endpoint(EchoServer,
+        local_addr=('127.0.0.1', 9000))
 
-coro = loop.create_datagram_endpoint(EchoServer, local_addr=('127.0.0.1', 9000))
-transport, protocol = loop.run_until_complete(coro)
+    await loop.create_future()
 
-loop.run_forever()
+asyncio.run(main())
```

### Comparing `aiosc-0.1.4/README.rst` & `aiosc-0.1.5/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,89 @@
 =====
 aiosc
 =====
 
-This is an experimental minimalistic Open Sound Control (OSC) communication
-module which uses asyncio for network operations and is compatible with the
+aiosc is a minimalistic Open Sound Control (OSC) communication module
+which uses asyncio for network operations and is compatible with the
 asyncio event loop.
 
 Installation
 ============
 
-aiosc requires at least Python 3.5. It can be installed using pip::
+aiosc requires at least Python 3.7. It can be installed using pip::
 
     pip3 install aiosc
 
-Or use `--user` option to install aiosc locally::
+Alternatively, use ``--user`` option to install aiosc only for the current user::
 
     pip3 install --user aiosc
 
 Usage
 =====
 
-To send an OSC message just use ``aiosc.send``:
+To send OSC messages with ``aiosc``, create an asyncio datagram connection
+endpoint using ``aiosc.OSCProtocol`` as the protocol factory.
+
+A datagram connection can be created with the ``create_datagram_endpoint``
+method of the asyncio event loop. Use the argument ``remote_addr`` to specify
+the OSC server address and port as follows:
 
 .. code-block:: python
 
     import asyncio
     import aiosc
 
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(
-        aiosc.send(('127.0.0.1', 9000), '/hello', 'world')
-    )
-
-To implement an OSC server with ``aiosc`` you should create an UDP endpoint
-using ``aiosc.OSCProtocol`` as the protocol. ``OSCProtocol`` can be subclassed
-or directly constructed with a dictionary mapping OSC address patterns to
-handler methods for incoming messages:
+    async def main():
+        loop = asyncio.get_running_loop()
+        
+        transport, osc = await loop.create_datagram_endpoint(aiosc.OSCProtocol,
+            remote_addr=('127.0.0.1', 8000))
+
+        osc.send('/hello/world')
+        osc.send('/a/b/cde', 1000, -1, 'hello', 1.234, 5.678)
+
+    asyncio.run(main())
+
+For an OSC server implementation, ``aiosc.OSCProtocol`` can be subclassed
+or directly constructed with a dictionary which maps OSC address patterns to
+handler methods for incoming messages.
+
+When creating datagram connection for an OSC server with
+``create_datagram_endpoint``, use the argument ``local_addr`` to specify
+the interface (address) and listening port for the server.
+
+In a typical case, local address can look like ``('0.0.0.0', 9000)`` where
+``9000`` is the port number and ``0.0.0.0`` address designates that the server
+will be listening on all available network interfaces.
 
 .. code-block:: python
 
+    import asyncio
+    import aiosc
+    import sys
+
     class EchoServer(aiosc.OSCProtocol):
         def __init__(self):
             super().__init__(handlers={
                 '/sys/exit': lambda addr, path, *args: sys.exit(0),
                 '//*': self.echo,
             })
 
         def echo(self, addr, path, *args):
             print("incoming message from {}: {} {}".format(addr, path, args))
 
-    loop = asyncio.get_event_loop()
-    coro = loop.create_datagram_endpoint(EchoServer, local_addr=('127.0.0.1', 9000))
-    transport, protocol = loop.run_until_complete(coro)
+    async def main():
+        loop = asyncio.get_running_loop()
+
+        transport, osc = await loop.create_datagram_endpoint(EchoServer,
+            local_addr=('0.0.0.0', 8000))
+
+        await loop.create_future()
 
-    loop.run_forever()
+    asyncio.run(main())
 
 For more examples, see ``examples/``.
 
 OSC address patterns
 ====================
 
 ``aiosc`` dispatches messages to handler methods using glob-style address
@@ -72,18 +98,18 @@
 * ``//*`` matches any address.
 
 Notes
 =====
 
 Bundles are not yet supported.
 
-Contrary to most OSC implementations, OSC data types are picked from the
-preliminary spec documented in Features and Future of Open Sound Control
-version 1.1 for NIME paper. For example, 'I' typetag is decoded to Impulse
-(aka "bang") which is passed around as ``aiosc.Impulse`` singleton.
+OSC data types are picked from the preliminary spec documented in Features
+and Future of Open Sound Control version 1.1 for NIME paper. For example,
+``I`` typetag is decoded to Impulse (aka "bang") which is passed around
+as ``aiosc.Impulse`` singleton.
 
 Suggestions, bug reports, issues and/or pull requests are, of course, welcome.
 
 License
 =======
 
 Copyright (c) 2014 Artem Popov <artfwo@gmail.com>
```

### Comparing `aiosc-0.1.4/LICENSE` & `aiosc-0.1.5/LICENSE`

 * *Files identical despite different names*

