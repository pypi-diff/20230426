# Comparing `tmp/netpackAIO-0.0.4.tar.gz` & `tmp/netpackAIO-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpackAIO-0.0.4.tar", last modified: Mon Apr 24 23:43:22 2023, max compression
+gzip compressed data, was "netpackAIO-0.0.5.tar", last modified: Tue Apr 25 18:36:58 2023, max compression
```

## Comparing `netpackAIO-0.0.4.tar` & `netpackAIO-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 23:43:22.088549 netpackAIO-0.0.4/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3405 2023-04-24 23:43:22.089548 netpackAIO-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2894 2023-04-20 20:36:34.000000 netpackAIO-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 23:43:22.045551 netpackAIO-0.0.4/netpack/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.4/netpack/__init__.py
--rw-rw-rw-   0        0        0    11538 2023-04-24 23:37:13.000000 netpackAIO-0.0.4/netpack/func.py
--rw-rw-rw-   0        0        0      129 2023-04-24 21:06:39.000000 netpackAIO-0.0.4/netpack/test.py
-drwxrwxrwx   0        0        0        0 2023-04-24 23:43:22.087548 netpackAIO-0.0.4/netpackAIO.egg-info/
--rw-rw-rw-   0        0        0     3405 2023-04-24 23:43:21.000000 netpackAIO-0.0.4/netpackAIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-24 23:43:21.000000 netpackAIO-0.0.4/netpackAIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 23:43:21.000000 netpackAIO-0.0.4/netpackAIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-24 23:43:21.000000 netpackAIO-0.0.4/netpackAIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 23:43:21.000000 netpackAIO-0.0.4/netpackAIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-24 23:43:22.094551 netpackAIO-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-24 23:43:18.000000 netpackAIO-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.071283 netpackAIO-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3405 2023-04-25 18:36:58.072286 netpackAIO-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2894 2023-04-20 20:36:34.000000 netpackAIO-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.035286 netpackAIO-0.0.5/netpack/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.5/netpack/__init__.py
+-rw-rw-rw-   0        0        0    11570 2023-04-25 17:06:55.000000 netpackAIO-0.0.5/netpack/func.py
+-rw-rw-rw-   0        0        0      877 2023-04-25 17:10:17.000000 netpackAIO-0.0.5/netpack/test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.069281 netpackAIO-0.0.5/netpackAIO.egg-info/
+-rw-rw-rw-   0        0        0     3405 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-25 18:36:58.078282 netpackAIO-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-25 18:36:55.000000 netpackAIO-0.0.5/setup.py
```

### Comparing `netpackAIO-0.0.4/LICENSE` & `netpackAIO-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.4/PKG-INFO` & `netpackAIO-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netpackAIO-0.0.4/README.md` & `netpackAIO-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.4/netpack/func.py` & `netpackAIO-0.0.5/netpack/func.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import threading
+
 from bs4 import BeautifulSoup
 import requests
 import ipaddress
 import socket
 import time
 import struct
 import random
@@ -27,15 +29,15 @@
         RIPR_NCC: https://apps.db.ripe.net/docs/13.Types-of-Queries/
         LACNIC & IANA, no specific instructions
     """
     WHOIS_PORT = 43
     SOCKET_TIMEOUT = 5
 
     @staticmethod
-    def _is_valid_ipv4(ip: str) -> bool:
+    def is_valid_ipv4(ip: str) -> bool:
         try:
             ipaddress.IPv4Address(ip)
             return True
         except ipaddress.AddressValueError:
             return False
 
     @staticmethod
@@ -255,21 +257,29 @@
         else:
             # Raise an error if an unsupported protocol is given
             raise ValueError("Unsupported protocol. Please use 'icmp' or 'tcp'.")
 
     @staticmethod
     def multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
         multiping_results = {}
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            # Submit ping tasks for each host
-            ping_tasks = {executor.submit(NetPack.ping, host, packet_size, protocol, interval, timeout, packet_num): host for host in hosts}
-            for task in concurrent.futures.as_completed(ping_tasks):
-                host = ping_tasks[task]
-                try:
-                    # Get the ping result and add it to the results dictionary
-                    latency, success_rate = task.result()
-                    multiping_results[host] = {'success_rate': success_rate, 'latency': latency}
-                except Exception as e:
-                    # Handle any exceptions that occurred during the ping task
-                    print(e)
-                    multiping_results[host] = {'success_rate': 0, 'latency': None}
+
+        # Define a function to ping a host and store the result in the results dictionary
+        def ping_host(host):
+            try:
+                latency, success_rate = NetPack.ping(host, packet_size, protocol, interval, timeout, packet_num)
+                multiping_results[host] = {'success_rate': success_rate, 'latency': latency}
+            except Exception as e:
+                print(e)
+                multiping_results[host] = {'success_rate': 0, 'latency': None}
+
+        # Create a thread for each host and start them all simultaneously
+        threads = []
+        for host in hosts:
+            t = threading.Thread(target=ping_host, args=(host,))
+            threads.append(t)
+            t.start()
+
+        # Wait for all threads to finish before returning the results dictionary
+        for t in threads:
+            t.join()
+
         return multiping_results
```

### Comparing `netpackAIO-0.0.4/netpackAIO.egg-info/PKG-INFO` & `netpackAIO-0.0.5/netpackAIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netpackAIO-0.0.4/setup.py` & `netpackAIO-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netpackAIO',
-    version='0.0.4',
+    version='0.0.5',
     description='A Python package for performing network-related tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dongjie Zhang',
     author_email='crusade.ray@gmail.com',
     url='https://github.com/crusaderay/netpack',
     packages=find_packages(),
```

