# Comparing `tmp/cloudcheck-2.0.0.34.tar.gz` & `tmp/cloudcheck-2.0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcheck-2.0.0.34.tar", max compression
+gzip compressed data, was "cloudcheck-2.0.0.36.tar", max compression
```

## Comparing `cloudcheck-2.0.0.34.tar` & `cloudcheck-2.0.0.36.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1340 2023-04-05 18:33:48.324203 cloudcheck-2.0.0.34/README.md
--rw-r--r--   0        0        0       74 2023-04-05 18:33:48.328203 cloudcheck-2.0.0.34/cloudcheck/__init__.py
--rw-r--r--   0        0        0      772 2023-04-05 18:33:48.328203 cloudcheck-2.0.0.34/cloudcheck/cidr.py
--rw-r--r--   0        0        0     3054 2023-04-05 18:33:48.328203 cloudcheck-2.0.0.34/cloudcheck/cloudcheck.py
--rw-r--r--   0        0        0      365 2023-04-05 18:33:48.328203 cloudcheck-2.0.0.34/cloudcheck/helpers.py
--rw-r--r--   0        0        0     4685 2023-04-05 18:33:48.328203 cloudcheck-2.0.0.34/cloudcheck/providers.py
--rw-r--r--   0        0        0      496 2023-04-05 18:33:48.404204 cloudcheck-2.0.0.34/pyproject.toml
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 cloudcheck-2.0.0.34/PKG-INFO
+-rw-r--r--   0        0        0     1389 2023-04-26 11:31:08.069953 cloudcheck-2.0.0.36/README.md
+-rw-r--r--   0        0        0       74 2023-04-26 11:31:08.069953 cloudcheck-2.0.0.36/cloudcheck/__init__.py
+-rw-r--r--   0        0        0      772 2023-04-26 11:31:08.069953 cloudcheck-2.0.0.36/cloudcheck/cidr.py
+-rw-r--r--   0        0        0     3159 2023-04-26 11:31:08.073953 cloudcheck-2.0.0.36/cloudcheck/cloudcheck.py
+-rw-r--r--   0        0        0      365 2023-04-26 11:31:08.073953 cloudcheck-2.0.0.36/cloudcheck/helpers.py
+-rw-r--r--   0        0        0     5216 2023-04-26 11:31:08.073953 cloudcheck-2.0.0.36/cloudcheck/providers.py
+-rw-r--r--   0        0        0      496 2023-04-26 11:31:08.129953 cloudcheck-2.0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     2089 1970-01-01 00:00:00.000000 cloudcheck-2.0.0.36/PKG-INFO
```

### Comparing `cloudcheck-2.0.0.34/README.md` & `cloudcheck-2.0.0.36/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,7 +34,8 @@
 - Amazon ([source](https://ip-ranges.amazonaws.com/ip-ranges.json)) 
 - Azure ([source](https://www.microsoft.com/en-us/download/confirmation.aspx?id=56519))
 - Google ([source](https://www.gstatic.com/ipranges/cloud.json))
 - Oracle Cloud ([source](https://docs.cloud.oracle.com/en-us/iaas/tools/public_ip_ranges.json))
 - DigitalOcean ([source](http://digitalocean.com/geo/google.csv))
 - Cloudflare ([source](https://api.cloudflare.com/client/v4/ips))
 - Akamai ([source](https://techdocs.akamai.com/property-manager/pdfs/akamai_ipv4_ipv6_CIDRs-txt.zip))
+- Github ([source](https://api.github.com/meta))
```

### Comparing `cloudcheck-2.0.0.34/cloudcheck/cidr.py` & `cloudcheck-2.0.0.36/cloudcheck/cidr.py`

 * *Files identical despite different names*

### Comparing `cloudcheck-2.0.0.34/cloudcheck/cloudcheck.py` & `cloudcheck-2.0.0.36/cloudcheck/cloudcheck.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import json
 import traceback
 from threading import Lock
 from datetime import datetime
+from collections import OrderedDict
 from concurrent.futures import ThreadPoolExecutor
 
 from .providers import *
 from .helpers import ip_network_parents
 
 import logging
 
@@ -25,14 +26,15 @@
         except Exception:
             self.json = {}
         provider_classes = CloudProvider.__subclasses__()
         self.now = datetime.now().isoformat()
         with ThreadPoolExecutor(max_workers=len(provider_classes)) as e:
             for p in provider_classes:
                 e.submit(self._get_provider, p, *args, **kwargs)
+        self.providers = OrderedDict(sorted(self.providers.items()))
 
     def _get_provider(self, p, *args, **kwargs):
         try:
             provider = p(*args, **kwargs)
             self.providers[provider.name] = provider
             # if we successfully got CIDR ranges, then update the JSON
             if not provider.name in self.json:
```

### Comparing `cloudcheck-2.0.0.34/cloudcheck/providers.py` & `cloudcheck-2.0.0.36/cloudcheck/providers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import csv
 import logging
 import zipfile
 import requests
+import ipaddress
 import traceback
 from pathlib import Path
 from requests_cache import CachedSession
 from requests_cache.backends import SQLiteCache
 
 from .cidr import CidrRanges
 
@@ -145,7 +146,25 @@
             for filename in ("akamai_ipv4_CIDRs.txt", "akamai_ipv6_CIDRs.txt"):
                 with zip_file.open(filename) as f:
                     for line in f.read().splitlines():
                         line = line.decode(errors="ignore").strip()
                         if line:
                             ranges.add(line)
         return ranges
+
+
+class Github(CloudProvider):
+    main_url = "https://api.github.com/meta"
+    provider_type = "cdn"
+
+    def parse_response(self, response):
+        ranges = set()
+        response_json = response.json()
+        for k, v in response_json.items():
+            if isinstance(v, list):
+                for n in v:
+                    try:
+                        ipaddress.ip_network(n)
+                        ranges.add(n)
+                    except ValueError:
+                        pass
+        return ranges
```

### Comparing `cloudcheck-2.0.0.34/PKG-INFO` & `cloudcheck-2.0.0.36/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcheck
-Version: 2.0.0.34
+Version: 2.0.0.36
 Summary: Check whether an IP address belongs to a cloud provider
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -52,8 +52,9 @@
 - Amazon ([source](https://ip-ranges.amazonaws.com/ip-ranges.json)) 
 - Azure ([source](https://www.microsoft.com/en-us/download/confirmation.aspx?id=56519))
 - Google ([source](https://www.gstatic.com/ipranges/cloud.json))
 - Oracle Cloud ([source](https://docs.cloud.oracle.com/en-us/iaas/tools/public_ip_ranges.json))
 - DigitalOcean ([source](http://digitalocean.com/geo/google.csv))
 - Cloudflare ([source](https://api.cloudflare.com/client/v4/ips))
 - Akamai ([source](https://techdocs.akamai.com/property-manager/pdfs/akamai_ipv4_ipv6_CIDRs-txt.zip))
+- Github ([source](https://api.github.com/meta))
```

