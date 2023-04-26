# Comparing `tmp/proxyport2-1.0.1.tar.gz` & `tmp/proxyport2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyport2-1.0.1.tar", last modified: Mon Mar 27 13:51:00 2023, max compression
+gzip compressed data, was "proxyport2-1.1.0.tar", last modified: Tue Apr 25 15:32:48 2023, max compression
```

## Comparing `proxyport2-1.0.1.tar` & `proxyport2-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bakhankov  (1000) bakhankov  (1000)        0 2023-03-27 13:51:00.191474 proxyport2-1.0.1/
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1066 2023-03-13 16:43:15.000000 proxyport2-1.0.1/LICENSE
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     3595 2023-03-27 13:51:00.191474 proxyport2-1.0.1/PKG-INFO
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1007 2023-03-27 12:55:44.000000 proxyport2-1.0.1/README.md
-drwxr-xr-x   0 bakhankov  (1000) bakhankov  (1000)        0 2023-03-27 13:51:00.191474 proxyport2-1.0.1/proxyport2/
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)      330 2023-03-14 15:41:04.000000 proxyport2-1.0.1/proxyport2/__init__.py
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)      264 2023-03-14 16:07:14.000000 proxyport2-1.0.1/proxyport2/__main__.py
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)       22 2023-03-27 13:48:59.000000 proxyport2-1.0.1/proxyport2/__version__.py
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     3696 2023-03-14 16:07:14.000000 proxyport2-1.0.1/proxyport2/proxyport2.py
-drwxr-xr-x   0 bakhankov  (1000) bakhankov  (1000)        0 2023-03-27 13:51:00.191474 proxyport2-1.0.1/proxyport2.egg-info/
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     3595 2023-03-27 13:51:00.000000 proxyport2-1.0.1/proxyport2.egg-info/PKG-INFO
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)      274 2023-03-27 13:51:00.000000 proxyport2-1.0.1/proxyport2.egg-info/SOURCES.txt
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)        1 2023-03-27 13:51:00.000000 proxyport2-1.0.1/proxyport2.egg-info/dependency_links.txt
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)       11 2023-03-27 13:51:00.000000 proxyport2-1.0.1/proxyport2.egg-info/top_level.txt
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1426 2023-03-27 13:03:21.000000 proxyport2-1.0.1/pyproject.toml
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)       38 2023-03-27 13:51:00.191474 proxyport2-1.0.1/setup.cfg
--rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1817 2023-03-27 13:03:09.000000 proxyport2-1.0.1/setup.py
+drwxr-xr-x   0 bakhankov  (1000) bakhankov  (1000)        0 2023-04-25 15:32:48.895969 proxyport2-1.1.0/
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1066 2023-03-13 16:43:15.000000 proxyport2-1.1.0/LICENSE
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     3595 2023-04-25 15:32:48.895969 proxyport2-1.1.0/PKG-INFO
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1007 2023-03-27 12:55:44.000000 proxyport2-1.1.0/README.md
+drwxr-xr-x   0 bakhankov  (1000) bakhankov  (1000)        0 2023-04-25 15:32:48.895969 proxyport2-1.1.0/proxyport2/
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)      330 2023-03-14 15:41:04.000000 proxyport2-1.1.0/proxyport2/__init__.py
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)      264 2023-03-14 16:07:14.000000 proxyport2-1.1.0/proxyport2/__main__.py
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)       22 2023-04-25 15:29:41.000000 proxyport2-1.1.0/proxyport2/__version__.py
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     3445 2023-04-25 15:19:49.000000 proxyport2-1.1.0/proxyport2/proxyport2.py
+drwxr-xr-x   0 bakhankov  (1000) bakhankov  (1000)        0 2023-04-25 15:32:48.895969 proxyport2-1.1.0/proxyport2.egg-info/
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     3595 2023-04-25 15:32:48.000000 proxyport2-1.1.0/proxyport2.egg-info/PKG-INFO
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)      274 2023-04-25 15:32:48.000000 proxyport2-1.1.0/proxyport2.egg-info/SOURCES.txt
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)        1 2023-04-25 15:32:48.000000 proxyport2-1.1.0/proxyport2.egg-info/dependency_links.txt
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)       11 2023-04-25 15:32:48.000000 proxyport2-1.1.0/proxyport2.egg-info/top_level.txt
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1426 2023-03-27 13:03:21.000000 proxyport2-1.1.0/pyproject.toml
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)       38 2023-04-25 15:32:48.895969 proxyport2-1.1.0/setup.cfg
+-rw-r--r--   0 bakhankov  (1000) bakhankov  (1000)     1817 2023-03-27 13:03:09.000000 proxyport2-1.1.0/setup.py
```

### Comparing `proxyport2-1.0.1/LICENSE` & `proxyport2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyport2-1.0.1/PKG-INFO` & `proxyport2-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyport2
-Version: 1.0.1
+Version: 1.1.0
 Summary: Proxy Port SDK
 Home-page: https://proxy-port.com/en/scraping-proxy
 Author: Proxy Port
 Author-email: Proxy Port <proxyportcom@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 proxyport
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proxyport2 Version: 1.0.1 Summary: Proxy Port SDK
+Metadata-Version: 2.1 Name: proxyport2 Version: 1.1.0 Summary: Proxy Port SDK
 Home-page: https://proxy-port.com/en/scraping-proxy Author: Proxy Port Author-
 email: Proxy Port
 gmail.com> License: MIT License Copyright (c) 2023 proxyport Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `proxyport2-1.0.1/README.md` & `proxyport2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `proxyport2-1.0.1/proxyport2/proxyport2.py` & `proxyport2-1.1.0/proxyport2/proxyport2.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,106 +13,100 @@
 class ProxyPort:
     last_load = None
     warned = False
     api_url = 'https://api.proxy-port.com/scraping-proxy'
     user_agent = 'py-proxyport2/{}'.format(__version__)
     headers = {'User-Agent': user_agent}
     ttl_seconds = 5 * 60
+    ttl_delta = timedelta(seconds=ttl_seconds)
 
     def __init__(self, api_key=None):
         self.log = logger
         self.new_proxy = list()
         self.known_proxy = dict()
-        self.used_proxy = dict()
         if not api_key:
             api_key = os.environ.get('PROXY_PORT_API_KEY')
         if api_key:
             self.set_api_key(api_key)
-            self.load_proxy()
+            self._load_proxy()
 
     def set_user_agent(self, user_agent):
         self.headers['User-Agent'] = '{} {}'.format(
             self.user_agent, user_agent)
 
     def set_api_key(self, api_key):
         self.headers['X-API-KEY'] = api_key
 
-    def load_proxy(self):
+    def get_proxy(self):
+        self._refresh()
+        if not self.new_proxy:
+            if not self.known_proxy:
+                self.log.warning('Proxy list is empty')
+                return
+            return choice(list(self.known_proxy.keys()))
+        proxy = self.new_proxy.pop(0)
+        return proxy
+
+    def get_proxy_list(self):
+        self._refresh()
+        return self.new_proxy
+
+    def _load_proxy(self):
         if not self.headers.get('X-API-KEY'):
             raise AuthorizationError(
                 '\nAPI key are not specified, '
                 'call `set_api_key` before usage:\n\n'
                 ' from proxyport2 import set_api_key, get_proxy\n\n'
                 ' set_api_key(<API_KEY>)\n'
                 ' print(get_proxy())\n'
             )
         try:
-            response = urlopen(self.get_proxy_list_request())
+            response = urlopen(Request(self.api_url, headers=self.headers))
             response_data = json.load(response)
         except Exception as e:
-            self.check_error(e)
+            self._check_error(e)
             return
         if response_data.get('warning') and not self.warned:
             self.log.warning(response_data.get('warning'))
             self.warned = True
-        for proxy in response_data.get('data'):
-            if not self.known_proxy.get(proxy):
-                self.new_proxy = [proxy] + self.new_proxy
-                self.known_proxy[proxy] = True
-            elif self.used_proxy.get(proxy):
-                self.used_proxy[proxy] = self.get_ttl()
-        self.proxy_list_gc()
-        self.last_load = datetime.now()
 
-    def get_proxy_list_request(self):
-        return Request(self.api_url, headers=self.headers)
+        self._proxy_list_gc()
 
-    def get_ttl(self):
-        return datetime.now() + timedelta(seconds=self.ttl_seconds)
+        new_proxy = []
+        for proxy in response_data.get('data'):
+            if not self.known_proxy.get(proxy) or proxy in self.new_proxy:
+                new_proxy.append(proxy)
+            self.known_proxy[proxy] = datetime.now() + self.ttl_delta
+        self.new_proxy = new_proxy
+        self.last_load = datetime.now()
 
-    def proxy_list_gc(self):
+    def _proxy_list_gc(self):
         now = datetime.now()
-        for address, ttl in list(self.used_proxy.items()):
+        for address, ttl in list(self.known_proxy.items()):
             if now > ttl:
-                del self.used_proxy[address]
                 del self.known_proxy[address]
 
-    def check_error(self, e):
+    def _check_error(self, e):
         auth_failed = False
         msg = str(e)
         if hasattr(e, 'code'):
             if e.code == 401:
                 auth_failed = True
                 msg = (
                     'Invalid API key, visit '
                     'https://account.proxy-port.com/scraping to obtain new key'
                 )
         self.log.error('Error on API call, {}'.format(msg))
         if auth_failed:
             raise AuthorizationError(msg)
 
-    def get_proxy(self):
-        self.refresh()
-        if not self.new_proxy:
-            if not self.used_proxy:
-                self.log.warning('Proxy list is empty')
-                return
-            return choice(list(self.used_proxy.keys()))
-        proxy = self.new_proxy.pop(0)
-        self.used_proxy[proxy] = self.get_ttl()
-        return proxy
-
-    def get_proxy_list(self):
-        self.refresh()
-        return self.new_proxy
-
-    def refresh(self):
+    def _refresh(self):
         if (not self.last_load or
                 self.last_load < datetime.now() - timedelta(seconds=60)):
-            self.load_proxy()
+            self._load_proxy()
 
 
 class AuthorizationError(Exception):
     pass
 
 
 instance = ProxyPort()
```

### Comparing `proxyport2-1.0.1/proxyport2.egg-info/PKG-INFO` & `proxyport2-1.1.0/proxyport2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyport2
-Version: 1.0.1
+Version: 1.1.0
 Summary: Proxy Port SDK
 Home-page: https://proxy-port.com/en/scraping-proxy
 Author: Proxy Port
 Author-email: Proxy Port <proxyportcom@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 proxyport
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proxyport2 Version: 1.0.1 Summary: Proxy Port SDK
+Metadata-Version: 2.1 Name: proxyport2 Version: 1.1.0 Summary: Proxy Port SDK
 Home-page: https://proxy-port.com/en/scraping-proxy Author: Proxy Port Author-
 email: Proxy Port
 gmail.com> License: MIT License Copyright (c) 2023 proxyport Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `proxyport2-1.0.1/pyproject.toml` & `proxyport2-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proxyport2-1.0.1/setup.py` & `proxyport2-1.1.0/setup.py`

 * *Files identical despite different names*

