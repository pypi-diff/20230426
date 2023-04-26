# Comparing `tmp/testvault-0.1.0.tar.gz` & `tmp/testvault-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testvault-0.1.0.tar", max compression
+gzip compressed data, was "testvault-0.2.0.tar", max compression
```

## Comparing `testvault-0.1.0.tar` & `testvault-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      436 2023-04-26 11:13:35.030598 testvault-0.1.0/README.md
--rw-r--r--   0        0        0      382 2023-04-26 11:06:04.396354 testvault-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 10:51:59.192865 testvault-0.1.0/testvault/__init__.py
--rw-r--r--   0        0        0     1817 2023-04-26 11:11:00.029169 testvault-0.1.0/testvault/client.py
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 testvault-0.1.0/setup.py
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 testvault-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      436 2023-04-26 11:13:35.030598 testvault-0.2.0/README.md
+-rw-r--r--   0        0        0      382 2023-04-26 11:17:05.058824 testvault-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1817 2023-04-26 11:16:27.643358 testvault-0.2.0/testvault/__init__.py
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 testvault-0.2.0/setup.py
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 testvault-0.2.0/PKG-INFO
```

### Comparing `testvault-0.1.0/testvault/client.py` & `testvault-0.2.0/testvault/__init__.py`

 * *Files identical despite different names*

### Comparing `testvault-0.1.0/setup.py` & `testvault-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0', 'structlog>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'testvault',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '# testvault-python-sdk\n\nA Python SDK for TestVault. TestVault is a sample service used to demonstrate building Common Fate Access Providers to automate entitlements. TestVault is a fictional password management service similar to 1Password or Lastpass.\n\nCommon Fate hosts the TestVault service at `https://prod.testvault.granted.run`.\n\nThe source code for the TestVault service can be found at https://github.com/common-fate/testvault.\n',
     'author': 'Common Fate',
     'author_email': 'hello@commonfate.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `testvault-0.1.0/PKG-INFO` & `testvault-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testvault
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Common Fate
 Author-email: hello@commonfate.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

