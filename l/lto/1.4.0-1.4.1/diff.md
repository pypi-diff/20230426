# Comparing `tmp/lto-1.4.0.tar.gz` & `tmp/lto-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lto-1.4.0.tar", last modified: Thu Jul 14 18:37:59 2022, max compression
+gzip compressed data, was "lto-1.4.1.tar", last modified: Tue Apr 25 17:03:22 2023, max compression
```

## Comparing `lto-1.4.0.tar` & `lto-1.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.799588 lto-1.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2022-07-14 18:37:44.000000 lto-1.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     3742 2022-07-14 18:37:59.799588 lto-1.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3246 2022-07-14 18:37:44.000000 lto-1.4.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      103 2022-07-14 18:37:44.000000 lto-1.4.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      833 2022-07-14 18:37:59.799588 lto-1.4.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.795590 lto-1.4.0/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.795590 lto-1.4.0/src/lto/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.795590 lto-1.4.0/src/lto/accounts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1652 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/account_factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/bip39.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/brainwallet.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.795590 lto-1.4.0/src/lto/accounts/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/ecdsa/account_ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4008 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/ecdsa/account_factory_ecdsa.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.799588 lto-1.4.0/src/lto/accounts/ed25519/
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/ed25519/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      958 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/ed25519/account_ed25519.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3415 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/accounts/ed25519/account_factory_ed25519.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/binary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2556 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5209 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/ethereum_mnemonic_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3945 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/public_node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transaction.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.799588 lto-1.4.0/src/lto/transactions/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2590 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/anchor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/association.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1780 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/burn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2161 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/cancel_lease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2245 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/cancel_sponsorship.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2343 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1960 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/data_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/lease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2237 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/mapped_anchor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3115 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/mass_transfer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/register.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3517 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/revoke_association.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2527 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/set_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2236 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/sponsorship.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3266 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/statement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/transactions/transfer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21480 2022-07-14 18:37:44.000000 lto-1.4.0/src/lto/word_list.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-14 18:37:59.795590 lto-1.4.0/src/lto.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3742 2022-07-14 18:37:59.000000 lto-1.4.0/src/lto.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1354 2022-07-14 18:37:59.000000 lto-1.4.0/src/lto.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-07-14 18:37:59.000000 lto-1.4.0/src/lto.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2022-07-14 18:37:59.000000 lto-1.4.0/src/lto.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2022-07-14 18:37:59.000000 lto-1.4.0/src/lto.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.145055 lto-1.4.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-04-25 17:03:03.000000 lto-1.4.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3868 2023-04-25 17:03:22.145055 lto-1.4.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3369 2023-04-25 17:03:03.000000 lto-1.4.1/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      103 2023-04-25 17:03:03.000000 lto-1.4.1/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      830 2023-04-25 17:03:22.145055 lto-1.4.1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.093029 lto-1.4.1/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.117041 lto-1.4.1/src/lto/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.129047 lto-1.4.1/src/lto/accounts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      702 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1652 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/account_factory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      122 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/bip39.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      589 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/brainwallet.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.129047 lto-1.4.1/src/lto/accounts/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      996 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/ecdsa/account_ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4008 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/ecdsa/account_factory_ecdsa.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.129047 lto-1.4.1/src/lto/accounts/ed25519/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      219 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/ed25519/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      958 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/ed25519/account_ed25519.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3415 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/accounts/ed25519/account_factory_ed25519.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/binary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2556 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5209 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/ethereum_mnemonic_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3945 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/public_node.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2231 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transaction.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.145055 lto-1.4.1/src/lto/transactions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2590 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/anchor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4697 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/association.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1780 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/burn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2161 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/cancel_lease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2245 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/cancel_sponsorship.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2343 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1960 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/data_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/lease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2237 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/mapped_anchor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3115 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/mass_transfer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/register.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3517 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/revoke_association.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2527 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/set_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2236 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/sponsorship.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3266 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/statement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/transactions/transfer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21480 2023-04-25 17:03:03.000000 lto-1.4.1/src/lto/word_list.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-25 17:03:22.129047 lto-1.4.1/src/lto.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3868 2023-04-25 17:03:22.000000 lto-1.4.1/src/lto.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1354 2023-04-25 17:03:22.000000 lto-1.4.1/src/lto.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-25 17:03:22.000000 lto-1.4.1/src/lto.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2023-04-25 17:03:22.000000 lto-1.4.1/src/lto.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        4 2023-04-25 17:03:22.000000 lto-1.4.1/src/lto.egg-info/top_level.txt
```

### Comparing `lto-1.4.0/LICENSE` & `lto-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/PKG-INFO` & `lto-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: lto
-Version: 1.4.0
+Version: 1.4.1
 Summary: LTO Network Python API
 Home-page: https://github.com/ltonetwork/lto-api.python
-Author: Andrea
-Author-email: andrea@ltonetwork.com
+Author: LTO Network
+Author-email: info@ltonetwork.com
 Project-URL: Bug Tracker, https://github.com/ltonetwork/lto-api.python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![LTO github readme](https://user-images.githubusercontent.com/100821/196711741-96cd4ba5-932a-4e95-b420-42d4d61c21fd.png)
+
 # lto-api.python
 Python client library for interacting with LTO Network
 
 
 ## Accounts
 
 ### Create an account
```

### Comparing `lto-1.4.0/README.md` & `lto-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![LTO github readme](https://user-images.githubusercontent.com/100821/196711741-96cd4ba5-932a-4e95-b420-42d4d61c21fd.png)
+
 # lto-api.python
 Python client library for interacting with LTO Network
 
 
 ## Accounts
 
 ### Create an account
```

### Comparing `lto-1.4.0/setup.cfg` & `lto-1.4.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = lto
-version = v1.4.0
-author = Andrea
-author_email = andrea@ltonetwork.com
+version = v1.4.1
+author = LTO Network
+author_email = info@ltonetwork.com
 description = LTO Network Python API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ltonetwork/lto-api.python
 project_urls = 
 	Bug Tracker = https://github.com/ltonetwork/lto-api.python/issues
 classifiers = 
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	requests>=2.24.0, <=2.26.0
+	requests>=2.24.0, <3
 	PyNaCl
 	pyblake2~=1.1.0
 	base58~=0.2.5
 	ecdsa~=0.17.0
 	inflection~=0.5.1
 	freezegun~=1.1.0
 	mnemonic~=0.20
```

### Comparing `lto-1.4.0/src/lto/__init__.py` & `lto-1.4.1/src/lto/__init__.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/account.py` & `lto-1.4.1/src/lto/accounts/account.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/account_factory.py` & `lto-1.4.1/src/lto/accounts/account_factory.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/brainwallet.py` & `lto-1.4.1/src/lto/accounts/brainwallet.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/ecdsa/account_ecdsa.py` & `lto-1.4.1/src/lto/accounts/ecdsa/account_ecdsa.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/ecdsa/account_factory_ecdsa.py` & `lto-1.4.1/src/lto/accounts/ecdsa/account_factory_ecdsa.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/ed25519/account_ed25519.py` & `lto-1.4.1/src/lto/accounts/ed25519/account_ed25519.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/accounts/ed25519/account_factory_ed25519.py` & `lto-1.4.1/src/lto/accounts/ed25519/account_factory_ed25519.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/crypto.py` & `lto-1.4.1/src/lto/crypto.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/ethereum_mnemonic_utils.py` & `lto-1.4.1/src/lto/ethereum_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/public_node.py` & `lto-1.4.1/src/lto/public_node.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transaction.py` & `lto-1.4.1/src/lto/transaction.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/__init__.py` & `lto-1.4.1/src/lto/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/anchor.py` & `lto-1.4.1/src/lto/transactions/anchor.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/association.py` & `lto-1.4.1/src/lto/transactions/association.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/burn.py` & `lto-1.4.1/src/lto/transactions/burn.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/cancel_lease.py` & `lto-1.4.1/src/lto/transactions/cancel_lease.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/cancel_sponsorship.py` & `lto-1.4.1/src/lto/transactions/cancel_sponsorship.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/data.py` & `lto-1.4.1/src/lto/transactions/data.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/data_entry.py` & `lto-1.4.1/src/lto/transactions/data_entry.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/lease.py` & `lto-1.4.1/src/lto/transactions/lease.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/mapped_anchor.py` & `lto-1.4.1/src/lto/transactions/mapped_anchor.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/mass_transfer.py` & `lto-1.4.1/src/lto/transactions/mass_transfer.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/register.py` & `lto-1.4.1/src/lto/transactions/register.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/revoke_association.py` & `lto-1.4.1/src/lto/transactions/revoke_association.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/set_script.py` & `lto-1.4.1/src/lto/transactions/set_script.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/sponsorship.py` & `lto-1.4.1/src/lto/transactions/sponsorship.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/statement.py` & `lto-1.4.1/src/lto/transactions/statement.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/transactions/transfer.py` & `lto-1.4.1/src/lto/transactions/transfer.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto/word_list.py` & `lto-1.4.1/src/lto/word_list.py`

 * *Files identical despite different names*

### Comparing `lto-1.4.0/src/lto.egg-info/PKG-INFO` & `lto-1.4.1/src/lto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: lto
-Version: 1.4.0
+Version: 1.4.1
 Summary: LTO Network Python API
 Home-page: https://github.com/ltonetwork/lto-api.python
-Author: Andrea
-Author-email: andrea@ltonetwork.com
+Author: LTO Network
+Author-email: info@ltonetwork.com
 Project-URL: Bug Tracker, https://github.com/ltonetwork/lto-api.python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![LTO github readme](https://user-images.githubusercontent.com/100821/196711741-96cd4ba5-932a-4e95-b420-42d4d61c21fd.png)
+
 # lto-api.python
 Python client library for interacting with LTO Network
 
 
 ## Accounts
 
 ### Create an account
```

### Comparing `lto-1.4.0/src/lto.egg-info/SOURCES.txt` & `lto-1.4.1/src/lto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

