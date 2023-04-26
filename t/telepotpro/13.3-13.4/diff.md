# Comparing `tmp/telepotpro-13.3.tar.gz` & `tmp/telepotpro-13.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telepotpro-13.3.tar", last modified: Sun May 23 08:19:39 2021, max compression
+gzip compressed data, was "telepotpro-13.4.tar", last modified: Wed Apr 26 20:08:58 2023, max compression
```

## Comparing `telepotpro-13.3.tar` & `telepotpro-13.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 08:19:39.945735 telepotpro-13.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-05-23 08:19:31.000000 telepotpro-13.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-05-23 08:19:39.945735 telepotpro-13.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-05-23 08:19:31.000000 telepotpro-13.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-23 08:19:39.945735 telepotpro-13.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2021-05-23 08:19:31.000000 telepotpro-13.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 08:19:39.945735 telepotpro-13.3/telepotpro/
--rw-r--r--   0 runner    (1001) docker     (121)    55319 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 08:19:39.945735 telepotpro-13.3/telepotpro/aio/
--rw-r--r--   0 runner    (1001) docker     (121)    39799 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/delegate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/hack.py
--rw-r--r--   0 runner    (1001) docker     (121)    13392 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7310 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/aio/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5086 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13513 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/delegate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/hack.py
--rw-r--r--   0 runner    (1001) docker     (121)    41205 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/loop.py
--rw-r--r--   0 runner    (1001) docker     (121)    31684 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     7293 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2021-05-23 08:19:31.000000 telepotpro-13.3/telepotpro/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 08:19:39.945735 telepotpro-13.3/telepotpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-05-23 08:19:39.000000 telepotpro-13.3/telepotpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-05-23 08:19:39.000000 telepotpro-13.3/telepotpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-23 08:19:39.000000 telepotpro-13.3/telepotpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-05-23 08:19:39.000000 telepotpro-13.3/telepotpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-05-23 08:19:39.000000 telepotpro-13.3/telepotpro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 20:08:42.000000 telepotpro-13.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-26 20:08:58.696465 telepotpro-13.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-26 20:08:42.000000 telepotpro-13.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:08:58.696465 telepotpro-13.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-26 20:08:42.000000 telepotpro-13.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/telepotpro/
+-rw-r--r--   0 runner    (1001) docker     (123)    55319 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/telepotpro/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)    39799 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/aio/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41205 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-26 20:08:42.000000 telepotpro-13.4/telepotpro/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:58.696465 telepotpro-13.4/telepotpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:08:58.000000 telepotpro-13.4/telepotpro.egg-info/top_level.txt
```

### Comparing `telepotpro-13.3/LICENSE.md` & `telepotpro-13.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/PKG-INFO` & `telepotpro-13.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: telepotpro
-Version: 13.3
+Version: 13.4
 Summary: Python framework for Telegram Bot API
 Home-page: https://github.com/pesaventofilippo/telepotpro
 Author: Filippo Pesavento
 Author-email: pesaventofilippo@gmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: telegram bot api python wrapper
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -21,7 +19,8 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.md
```

### Comparing `telepotpro-13.3/README.md` & `telepotpro-13.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 - [x] Fixed requests crashing with urllib3 >= 1.24.2
 - [x] Added "deleted" text format option in HTML and MD
 - [x] Fixed bot crashing when receiving a poll
 - [x] Fully implemented polls (incoming)
 - [x] Added support for dice messages
 - [x] Fix urllib connections pooling
 - [x] Fix requests to telegram servers timeout
-- [ ] Update api.py to latest Telegram v4.9 APIs
-  - [ ] Fully implement polls (outgoing, from bot)
 
 
 ## Original links & description
 telepot - Python framework for Telegram Bot API
 
 - [Original Repo »](https://github.com/nickoala/telepot)
 - [Introduction »](http://telepot.readthedocs.io/en/latest/)
```

### Comparing `telepotpro-13.3/setup.py` & `telepotpro-13.4/setup.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/__init__.py` & `telepotpro-13.4/telepotpro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Patch urllib3 for sending unicode filename
 from . import hack
 
 from . import exception
 
 
-__version_info__ = (13, 3)
+__version_info__ = (13, 4)
 __version__ = '.'.join(map(str, __version_info__))
 
 
 def flavor(msg):
     """
     Return flavor of message or event.
```

### Comparing `telepotpro-13.3/telepotpro/aio/__init__.py` & `telepotpro-13.4/telepotpro/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/aio/api.py` & `telepotpro-13.4/telepotpro/aio/api.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/aio/delegate.py` & `telepotpro-13.4/telepotpro/aio/delegate.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/aio/hack.py` & `telepotpro-13.4/telepotpro/aio/hack.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/aio/helper.py` & `telepotpro-13.4/telepotpro/aio/helper.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/aio/loop.py` & `telepotpro-13.4/telepotpro/aio/loop.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/aio/routing.py` & `telepotpro-13.4/telepotpro/aio/routing.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/api.py` & `telepotpro-13.4/telepotpro/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 from . import exception, _isstring
 
 # Suppress InsecurePlatformWarning
 urllib3.disable_warnings()
 
 
+_API_BASE_URL = 'https://api.telegram.org'
 _default_pool_params = dict(num_pools=3, maxsize=10, retries=3, timeout=10)
 _onetime_pool_params = dict(num_pools=1, maxsize=1, retries=3, timeout=30)
 
+
 _pools = {
     'default': urllib3.PoolManager(**_default_pool_params)
 }
 
 _onetime_pool_spec = (urllib3.PoolManager, _onetime_pool_params)
 
 
@@ -34,21 +36,34 @@
         h = urllib3.make_headers(proxy_basic_auth=':'.join(basic_auth))
         _pools['default'] = urllib3.ProxyManager(url, proxy_headers=h, **_default_pool_params)
         _onetime_pool_spec = (urllib3.ProxyManager, dict(proxy_url=url, proxy_headers=h, **_onetime_pool_params))
     else:
         _pools['default'] = urllib3.ProxyManager(url, **_default_pool_params)
         _onetime_pool_spec = (urllib3.ProxyManager, dict(proxy_url=url, **_onetime_pool_params))
 
+def set_api_url(url):
+    """
+    Set Telegram API base url. Defaults to ``https://api.telegram.org``.
+
+    :param url: API Base URL
+    """
+    global _API_BASE_URL
+    if not url:
+        _API_BASE_URL = 'https://api.telegram.org'
+    else:
+        _API_BASE_URL = url.rstrip('/')
+
 def _create_onetime_pool():
     cls, kw = _onetime_pool_spec
     return cls(**kw)
 
 def _methodurl(req, **user_kw):
     token, method, params, files = req
-    return 'https://api.telegram.org/bot%s/%s' % (token, method)
+    return f"{_API_BASE_URL}/bot{token}/{method}"
+
 
 def _which_pool(req, **user_kw):
     # token, method, params, files = req
     # return None if files else 'default'
     return None
 
 def _guess_filename(obj):
@@ -152,13 +167,13 @@
 def request(req, **user_kw):
     fn, args, kwargs = _transform(req, **user_kw)
     r = fn(*args, **kwargs)  # `fn` must be thread-safe
     return _parse(r)
 
 def _fileurl(req):
     token, path = req
-    return 'https://api.telegram.org/file/bot%s/%s' % (token, path)
+    return f"{_API_BASE_URL}/file/bot{token}/{path}"
 
 def download(req, **user_kw):
     pool = _create_onetime_pool()
     r = pool.request('GET', _fileurl(req), **user_kw)
     return r
```

### Comparing `telepotpro-13.3/telepotpro/delegate.py` & `telepotpro-13.4/telepotpro/delegate.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/exception.py` & `telepotpro-13.4/telepotpro/exception.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/filtering.py` & `telepotpro-13.4/telepotpro/filtering.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/helper.py` & `telepotpro-13.4/telepotpro/helper.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/loop.py` & `telepotpro-13.4/telepotpro/loop.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/namedtuple.py` & `telepotpro-13.4/telepotpro/namedtuple.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/routing.py` & `telepotpro-13.4/telepotpro/routing.py`

 * *Files identical despite different names*

### Comparing `telepotpro-13.3/telepotpro/text.py` & `telepotpro-13.4/telepotpro/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,21 +48,23 @@
         a list of `MessageEntity <https://core.telegram.org/bots/api#messageentity>`_ objects
     """
     escapes = {'*': '\\*',
                '_': '\\_',
                '[': '\\[',
                '`': '\\`',}
 
-    formatters = {'bold':         lambda s,e: '*'+s+'*',
-                  'italic':       lambda s,e: '_'+s+'_',
-                  'text_link':    lambda s,e: '['+s+']('+e['url']+')',
-                  'text_mention': lambda s,e: '['+s+'](tg://user?id='+str(e['user']['id'])+')',
-                  'code':         lambda s,e: '`'+s+'`',
-                  'pre':          lambda s,e: '```text\n'+s+'```',
-                  'del':          lambda s,e: '~'+s+'~'}
+    formatters = {'bold':          lambda s,e: '*'+s+'*',
+                  'italic':        lambda s,e: '_'+s+'_',
+                  'underline':     lambda s, e: '__' + s + '__',
+                  'strikethrough': lambda s, e: '~' + s + '~',
+                  'spoiler': lambda s, e: '||' + s + '||',
+                  'text_link':     lambda s,e: '['+s+']('+e['url']+')',
+                  'text_mention':  lambda s,e: '['+s+'](tg://user?id='+str(e['user']['id'])+')',
+                  'code':          lambda s,e: '`'+s+'`',
+                  'pre':           lambda s,e: '```text\n'+s+'```'}
 
     return _apply_entities(text, entities, escapes, formatters)
 
 
 def apply_entities_as_html(text, entities):
     """
     Format text as HTML. Also take care of escaping special characters.
@@ -75,16 +77,18 @@
     :param entities:
         a list of `MessageEntity <https://core.telegram.org/bots/api#messageentity>`_ objects
     """
     escapes = {'<': '&lt;',
                '>': '&gt;',
                '&': '&amp;',}
 
-    formatters = {'bold':         lambda s,e: '<b>'+s+'</b>',
-                  'italic':       lambda s,e: '<i>'+s+'</i>',
-                  'text_link':    lambda s,e: '<a href="'+e['url']+'">'+s+'</a>',
-                  'text_mention': lambda s,e: '<a href="tg://user?id='+str(e['user']['id'])+'">'+s+'</a>',
-                  'code':         lambda s,e: '<code>'+s+'</code>',
-                  'pre':          lambda s,e: '<pre>'+s+'</pre>',
-                  'del':          lambda s,e: '<del>'+s+'</del>'}
+    formatters = {'bold':          lambda s,e: '<b>'+s+'</b>',
+                  'italic':        lambda s,e: '<i>'+s+'</i>',
+                  'underline':     lambda s,e: '<u>'+s+'</u>',
+                  'strikethrough': lambda s,e: '<s>'+s+'</s>',
+                  'spoiler':       lambda s,e: '<tg-spoiler>'+s+'</tg-spoiler>',
+                  'text_link':     lambda s,e: '<a href="'+e['url']+'">'+s+'</a>',
+                  'text_mention':  lambda s,e: '<a href="tg://user?id='+str(e['user']['id'])+'">'+s+'</a>',
+                  'code':          lambda s,e: '<code>'+s+'</code>',
+                  'pre':           lambda s,e: '<pre>'+s+'</pre>'}
 
     return _apply_entities(text, entities, escapes, formatters)
```

### Comparing `telepotpro-13.3/telepotpro.egg-info/PKG-INFO` & `telepotpro-13.4/telepotpro.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: telepotpro
-Version: 13.3
+Version: 13.4
 Summary: Python framework for Telegram Bot API
 Home-page: https://github.com/pesaventofilippo/telepotpro
 Author: Filippo Pesavento
 Author-email: pesaventofilippo@gmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: telegram bot api python wrapper
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -21,7 +19,8 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.md
```

### Comparing `telepotpro-13.3/telepotpro.egg-info/SOURCES.txt` & `telepotpro-13.4/telepotpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

