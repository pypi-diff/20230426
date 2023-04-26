# Comparing `tmp/teamplify-0.8.0.tar.gz` & `tmp/teamplify-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamplify-0.8.0.tar", last modified: Tue Apr 25 13:19:42 2023, max compression
+gzip compressed data, was "teamplify-0.9.0.tar", last modified: Tue Apr 25 16:02:31 2023, max compression
```

## Comparing `teamplify-0.8.0.tar` & `teamplify-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 13:19:42.149521 teamplify-0.8.0/
--rw-r--r--   0 ipeterov   (501) staff       (20)     1066 2023-04-12 15:29:52.000000 teamplify-0.8.0/LICENSE
--rw-r--r--   0 ipeterov   (501) staff       (20)      272 2023-04-12 15:29:52.000000 teamplify-0.8.0/MANIFEST.in
--rw-r--r--   0 ipeterov   (501) staff       (20)    23437 2023-04-25 13:19:42.149624 teamplify-0.8.0/PKG-INFO
--rw-r--r--   0 ipeterov   (501) staff       (20)    23114 2023-04-25 13:03:30.000000 teamplify-0.8.0/README.md
--rw-r--r--   0 ipeterov   (501) staff       (20)       63 2023-04-18 11:09:50.000000 teamplify-0.8.0/requirements-tests.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       79 2023-04-25 13:03:30.000000 teamplify-0.8.0/requirements.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      253 2023-04-25 13:19:42.149897 teamplify-0.8.0/setup.cfg
--rw-r--r--   0 ipeterov   (501) staff       (20)     1276 2023-04-18 11:02:31.000000 teamplify-0.8.0/setup.py
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 13:19:42.147101 teamplify-0.8.0/teamplify.egg-info/
--rw-r--r--   0 ipeterov   (501) staff       (20)    23437 2023-04-25 13:19:42.000000 teamplify-0.8.0/teamplify.egg-info/PKG-INFO
--rw-r--r--   0 ipeterov   (501) staff       (20)      617 2023-04-25 13:19:42.000000 teamplify-0.8.0/teamplify.egg-info/SOURCES.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)        1 2023-04-25 13:19:42.000000 teamplify-0.8.0/teamplify.egg-info/dependency_links.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       56 2023-04-25 13:19:42.000000 teamplify-0.8.0/teamplify.egg-info/entry_points.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      152 2023-04-25 13:19:42.000000 teamplify-0.8.0/teamplify.egg-info/requires.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       17 2023-04-25 13:19:42.000000 teamplify-0.8.0/teamplify.egg-info/top_level.txt
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 13:19:42.149228 teamplify-0.8.0/teamplify_runner/
--rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-25 13:03:49.000000 teamplify-0.8.0/teamplify_runner/__init__.py
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 13:19:42.149361 teamplify-0.8.0/teamplify_runner/backup/
--rw-r--r--   0 ipeterov   (501) staff       (20)       51 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/backup/readme.txt
--rwxr-xr-x   0 ipeterov   (501) staff       (20)    14154 2023-04-25 13:03:30.000000 teamplify-0.8.0/teamplify_runner/cli.py
--rw-r--r--   0 ipeterov   (501) staff       (20)    13881 2023-04-18 11:02:31.000000 teamplify-0.8.0/teamplify_runner/configurator.py
--rw-r--r--   0 ipeterov   (501) staff       (20)     5304 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/docker-compose.yml
--rw-r--r--   0 ipeterov   (501) staff       (20)      270 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/mysql.cnf
--rw-r--r--   0 ipeterov   (501) staff       (20)       66 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/postfix.cf
--rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/redis.conf
--rw-r--r--   0 ipeterov   (501) staff       (20)     2074 2023-04-25 13:03:30.000000 teamplify-0.8.0/teamplify_runner/utils.py
--rw-r--r--   0 ipeterov   (501) staff       (20)      766 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/uwsgi_params.conf
--rw-r--r--   0 ipeterov   (501) staff       (20)      512 2023-04-12 15:29:52.000000 teamplify-0.8.0/teamplify_runner/vhost.conf
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.225680 teamplify-0.9.0/
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1066 2023-04-12 15:29:52.000000 teamplify-0.9.0/LICENSE
+-rw-r--r--   0 ipeterov   (501) staff       (20)      272 2023-04-12 15:29:52.000000 teamplify-0.9.0/MANIFEST.in
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23437 2023-04-25 16:02:31.225778 teamplify-0.9.0/PKG-INFO
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23114 2023-04-25 13:03:30.000000 teamplify-0.9.0/README.md
+-rw-r--r--   0 ipeterov   (501) staff       (20)       63 2023-04-18 11:09:50.000000 teamplify-0.9.0/requirements-tests.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       79 2023-04-25 13:03:30.000000 teamplify-0.9.0/requirements.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      253 2023-04-25 16:02:31.226109 teamplify-0.9.0/setup.cfg
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1276 2023-04-18 11:02:31.000000 teamplify-0.9.0/setup.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.223736 teamplify-0.9.0/teamplify.egg-info/
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23437 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/PKG-INFO
+-rw-r--r--   0 ipeterov   (501) staff       (20)      589 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/SOURCES.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)        1 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/dependency_links.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       56 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/entry_points.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      152 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/requires.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       17 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/top_level.txt
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.225363 teamplify-0.9.0/teamplify_runner/
+-rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/__init__.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.225530 teamplify-0.9.0/teamplify_runner/backup/
+-rw-r--r--   0 ipeterov   (501) staff       (20)       51 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/backup/readme.txt
+-rwxr-xr-x   0 ipeterov   (501) staff       (20)    14147 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/cli.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)    14340 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/configurator.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)     5349 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/docker-compose.yml
+-rw-r--r--   0 ipeterov   (501) staff       (20)      270 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/mysql.cnf
+-rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/redis.conf
+-rw-r--r--   0 ipeterov   (501) staff       (20)     2228 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/utils.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)      766 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/uwsgi_params.conf
+-rw-r--r--   0 ipeterov   (501) staff       (20)      512 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/vhost.conf
```

### Comparing `teamplify-0.8.0/LICENSE` & `teamplify-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teamplify-0.8.0/PKG-INFO` & `teamplify-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.8.0
+Version: 0.9.0
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamplify-0.8.0/README.md` & `teamplify-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `teamplify-0.8.0/setup.py` & `teamplify-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `teamplify-0.8.0/teamplify.egg-info/PKG-INFO` & `teamplify-0.9.0/teamplify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.8.0
+Version: 0.9.0
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamplify-0.8.0/teamplify.egg-info/SOURCES.txt` & `teamplify-0.9.0/teamplify.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,13 +12,12 @@
 teamplify.egg-info/requires.txt
 teamplify.egg-info/top_level.txt
 teamplify_runner/__init__.py
 teamplify_runner/cli.py
 teamplify_runner/configurator.py
 teamplify_runner/docker-compose.yml
 teamplify_runner/mysql.cnf
-teamplify_runner/postfix.cf
 teamplify_runner/redis.conf
 teamplify_runner/utils.py
 teamplify_runner/uwsgi_params.conf
 teamplify_runner/vhost.conf
 teamplify_runner/backup/readme.txt
```

### Comparing `teamplify-0.8.0/teamplify_runner/cli.py` & `teamplify-0.9.0/teamplify_runner/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 IMAGES = {
     'db': 'mysql:8.0.29-oracle',
     'redis': 'redis:6.2.6',
     'nginx': 'jwilder/nginx-proxy:latest',
     'letsencrypt': 'jrcs/letsencrypt-nginx-proxy-companion:latest',
-    'smtp': 'instrumentisto/postfix:3.1.3',
+    'smtp': 'mikenye/postfix:3.5.9',
     'app': 'public.ecr.aws/q5a3z0t4/teamplify/server',
 }
 
 
 def _root_url(env):
     port = env['WEB_PORT']
     root_url = 'http://' + env['WEB_HOST']
```

### Comparing `teamplify-0.8.0/teamplify_runner/configurator.py` & `teamplify-0.9.0/teamplify_runner/configurator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 import socket
 from collections import OrderedDict
 from configparser import ConfigParser
 from functools import partial
 
-from teamplify_runner.utils import random_string
+from teamplify_runner.utils import is_ip_address, random_string
 
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 class ConfigurationError(Exception):
     """
@@ -233,14 +233,24 @@
         # have to specify LETSENCRYPT_HOST in any case
         # to avoid warnings in the NGINX container logs
         env['LETSENCRYPT_HOST'] = env['WEB_HOST']
         env['COMPOSE_PROFILES'] = 'nossl'
         env['HTTPS_METHOD'] = 'nohttps'
         env['HTTPS_PORT'] = env['WEB_SSL_PORT']
 
+        # Postfix
+        env['ENABLE_CLAMAV'] = 'false'
+        env['POSTFIX_MYNETWORKS'] = '127.0.0.1/32 192.168.0.0/16 172.16.0.0/12 10.0.0.0/8'
+        env['POSTFIX_MYHOSTNAME'] = env['WEB_HOST']
+        if is_ip_address(env['WEB_HOST']):
+            env['POSTMASTER_EMAIL'] = f'postmaster@{env["WEB_HOST"]}'
+        else:
+            domain = env['WEB_HOST'].split('.', 1)[-1]
+            env['POSTMASTER_EMAIL'] = f'postmaster@{domain}'
+
         # The 'external' SSL mode is handled by Django
         # and does not need special configuration
         _ssl_mode = self.ssl_mode()
         if _ssl_mode == 'builtin':
             env['HTTPS_METHOD'] = 'redirect'
 
             # deploy Let's Encrypt certificates if no SSL certs
```

### Comparing `teamplify-0.8.0/teamplify_runner/docker-compose.yml` & `teamplify-0.9.0/teamplify_runner/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,19 @@
       - nginx-ssl
     profiles:
       - letsencrypt
 
   builtin_smtp:
     image: ${IMAGE_SMTP}
     container_name: teamplify_smtp
-    volumes:
-      - ./postfix.cf:/etc/postfix/main.cf.d/10-custom.cf:ro
+    environment:
+      - ENABLE_CLAMAV
+      - POSTMASTER_EMAIL
+      - POSTFIX_MYNETWORKS
+      - POSTFIX_MYHOSTNAME
     restart: always
 
   app:
     image: ${IMAGE_APP}
     container_name: teamplify_app
     depends_on:
       - builtin_db
```

### Comparing `teamplify-0.8.0/teamplify_runner/utils.py` & `teamplify-0.9.0/teamplify_runner/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import ipaddress
 import os
 import random
 import string
 import traceback
 
 import click
 import sarge
@@ -65,7 +66,15 @@
 
 def random_string(length):
     # Use /dev/urandom, see https://stackoverflow.com/a/23728630
     choice = random.SystemRandom().choice
     return ''.join(
         choice(string.ascii_letters + string.digits) for _ in range(length)
     )
+
+
+def is_ip_address(value):
+    try:
+        ipaddress.ip_address(value)
+        return True
+    except ValueError:
+        return False
```

### Comparing `teamplify-0.8.0/teamplify_runner/uwsgi_params.conf` & `teamplify-0.9.0/teamplify_runner/uwsgi_params.conf`

 * *Files identical despite different names*

### Comparing `teamplify-0.8.0/teamplify_runner/vhost.conf` & `teamplify-0.9.0/teamplify_runner/vhost.conf`

 * *Files identical despite different names*

