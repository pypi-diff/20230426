# Comparing `tmp/certbot-onion-0.1.2.tar.gz` & `tmp/certbot-onion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.2.tar", last modified: Fri Apr 21 11:38:08 2023, max compression
+gzip compressed data, was "certbot-onion-0.1.3.tar", last modified: Wed Apr 26 18:55:55 2023, max compression
```

## Comparing `certbot-onion-0.1.2.tar` & `certbot-onion-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.058534 certbot-onion-0.1.2/rust/
--rw-r--r--   0 runner    (1001) docker     (123)    17302 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/rust/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.058534 certbot-onion-0.1.2/rust/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.054533 certbot-onion-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.058534 certbot-onion-0.1.2/src/certbot_onion/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/src/certbot_onion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/src/certbot_onion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:38:07.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.444924 certbot-onion-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/src/certbot_onion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/src/certbot_onion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/src/certbot_onion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/top_level.txt
```

### Comparing `certbot-onion-0.1.2/LICENSE.md` & `certbot-onion-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.2/PKG-INFO` & `certbot-onion-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.2
+Version: 0.1.3
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -31,15 +31,16 @@
 The important arguments here are:
 
 * `--authenticator onion-csr` - Tells certbot to use this plugin for domain authentication
 * `--onion-csr-hs-dir /var/lib/tor/example_hs/` - Provides the path to the hidden service directory, this can be specified multiple times for multiple domains.
 
 ## ⚠️ WARNING ⚠️
 
-This plugin is currently non-functional, it will not work until [this PR](https://github.com/certbot/certbot/pull/9680)
-is merged into certbot.
+This plugin is currently non-functional, it will not work until Certbot version 
+2.6.0 is released.
 
-In the meantime you update certbot to a fork that will work with the following command:
+In the meantime you update Certbot to the commit incorporating the changes required for this plugin to work:
 
 ```shell 
-pip install git+https://github.com/AS207960/certbot.git@unknown-challenges
+pip install git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=certbot \
+  git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=acme
 ```
```

### Comparing `certbot-onion-0.1.2/README.md` & `certbot-onion-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 The important arguments here are:
 
 * `--authenticator onion-csr` - Tells certbot to use this plugin for domain authentication
 * `--onion-csr-hs-dir /var/lib/tor/example_hs/` - Provides the path to the hidden service directory, this can be specified multiple times for multiple domains.
 
 ## ⚠️ WARNING ⚠️
 
-This plugin is currently non-functional, it will not work until [this PR](https://github.com/certbot/certbot/pull/9680)
-is merged into certbot.
+This plugin is currently non-functional, it will not work until Certbot version 
+2.6.0 is released.
 
-In the meantime you update certbot to a fork that will work with the following command:
+In the meantime you update Certbot to the commit incorporating the changes required for this plugin to work:
 
 ```shell 
-pip install git+https://github.com/AS207960/certbot.git@unknown-challenges
+pip install git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=certbot \
+  git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=acme
 ```
```

### Comparing `certbot-onion-0.1.2/rust/src/lib.rs` & `certbot-onion-0.1.3/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.2/src/certbot_onion/__init__.py` & `certbot-onion-0.1.3/src/certbot_onion/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.2/src/certbot_onion.egg-info/PKG-INFO` & `certbot-onion-0.1.3/src/certbot_onion.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.2
+Version: 0.1.3
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -31,15 +31,16 @@
 The important arguments here are:
 
 * `--authenticator onion-csr` - Tells certbot to use this plugin for domain authentication
 * `--onion-csr-hs-dir /var/lib/tor/example_hs/` - Provides the path to the hidden service directory, this can be specified multiple times for multiple domains.
 
 ## ⚠️ WARNING ⚠️
 
-This plugin is currently non-functional, it will not work until [this PR](https://github.com/certbot/certbot/pull/9680)
-is merged into certbot.
+This plugin is currently non-functional, it will not work until Certbot version 
+2.6.0 is released.
 
-In the meantime you update certbot to a fork that will work with the following command:
+In the meantime you update Certbot to the commit incorporating the changes required for this plugin to work:
 
 ```shell 
-pip install git+https://github.com/AS207960/certbot.git@unknown-challenges
+pip install git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=certbot \
+  git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=acme
 ```
```

