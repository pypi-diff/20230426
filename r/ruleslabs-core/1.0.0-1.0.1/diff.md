# Comparing `tmp/ruleslabs-core-1.0.0.tar.gz` & `tmp/ruleslabs-core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruleslabs-core-1.0.0.tar", last modified: Wed Apr 26 08:59:19 2023, max compression
+gzip compressed data, was "ruleslabs-core-1.0.1.tar", last modified: Wed Apr 26 09:10:50 2023, max compression
```

## Comparing `ruleslabs-core-1.0.0.tar` & `ruleslabs-core-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.645408 ruleslabs-core-1.0.0/
--rw-r--r--   0 charleslanier   (501) staff       (20)      195 2022-09-02 14:09:10.000000 ruleslabs-core-1.0.0/.gitignore
--rw-r--r--   0 charleslanier   (501) staff       (20)       31 2022-06-30 14:47:19.000000 ruleslabs-core-1.0.0/MANIFEST.in
--rw-r--r--   0 charleslanier   (501) staff       (20)     7780 2023-04-26 08:59:19.645740 ruleslabs-core-1.0.0/PKG-INFO
--rw-r--r--   0 charleslanier   (501) staff       (20)     7423 2022-07-12 08:20:16.000000 ruleslabs-core-1.0.0/README.md
--rw-r--r--   0 charleslanier   (501) staff       (20)      186 2022-06-30 14:49:01.000000 ruleslabs-core-1.0.0/pyproject.toml
--rw-r--r--   0 charleslanier   (501) staff       (20)       49 2023-01-29 20:42:33.000000 ruleslabs-core-1.0.0/requirements.txt
--rw-r--r--   0 charleslanier   (501) staff       (20)      746 2023-04-26 08:59:19.647202 ruleslabs-core-1.0.0/setup.cfg
--rw-r--r--   0 charleslanier   (501) staff       (20)      511 2023-04-26 08:58:55.000000 ruleslabs-core-1.0.0/setup.py
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.617333 ruleslabs-core-1.0.0/src/
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.622217 ruleslabs-core-1.0.0/src/ruleslabs/
--rw-r--r--   0 charleslanier   (501) staff       (20)    11822 2023-04-26 08:26:47.000000 ruleslabs-core-1.0.0/src/ruleslabs/Rules.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)      272 2022-06-30 14:52:08.000000 ruleslabs-core-1.0.0/src/ruleslabs/__init__.py
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.624399 ruleslabs-core-1.0.0/src/ruleslabs/interfaces/
--rw-r--r--   0 charleslanier   (501) staff       (20)      342 2023-04-26 08:58:17.000000 ruleslabs-core-1.0.0/src/ruleslabs/interfaces/IRules.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)      350 2023-04-26 08:56:57.000000 ruleslabs-core-1.0.0/src/ruleslabs/interfaces/IRulesCards.cairo
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.630103 ruleslabs-core-1.0.0/src/ruleslabs/libraries/
--rw-r--r--   0 charleslanier   (501) staff       (20)     5270 2023-04-23 22:10:04.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/AccessControl.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     4360 2023-04-25 11:49:15.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/Cards.cairo
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.632302 ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/
--rw-r--r--   0 charleslanier   (501) staff       (20)    15088 2023-04-25 21:24:19.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/ERC1155.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     1957 2023-04-23 18:02:32.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/ERC1155ContractURI.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)      955 2023-04-23 16:58:55.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/IERC1155Receiver.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     1277 2023-04-23 18:03:53.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/Ownable.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     6164 2023-04-25 11:35:08.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/Packs.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     1522 2023-04-23 18:09:02.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/Scarcity.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     1227 2023-04-23 19:26:15.000000 ruleslabs-core-1.0.0/src/ruleslabs/libraries/Upgradeable.cairo
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.635268 ruleslabs-core-1.0.0/src/ruleslabs/utils/
--rw-r--r--   0 charleslanier   (501) staff       (20)     4015 2023-04-24 08:09:28.000000 ruleslabs-core-1.0.0/src/ruleslabs/utils/card.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)      430 2023-04-23 21:47:18.000000 ruleslabs-core-1.0.0/src/ruleslabs/utils/constants.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)      845 2023-01-29 20:39:28.000000 ruleslabs-core-1.0.0/src/ruleslabs/utils/memset.cairo
--rw-r--r--   0 charleslanier   (501) staff       (20)     1067 2023-04-25 11:34:41.000000 ruleslabs-core-1.0.0/src/ruleslabs/utils/metadata.cairo
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.638695 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/
--rw-r--r--   0 charleslanier   (501) staff       (20)     7780 2023-04-26 08:59:18.000000 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/PKG-INFO
--rw-r--r--   0 charleslanier   (501) staff       (20)     1153 2023-04-26 08:59:19.000000 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/SOURCES.txt
--rw-r--r--   0 charleslanier   (501) staff       (20)        1 2023-04-26 08:59:18.000000 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/dependency_links.txt
--rw-r--r--   0 charleslanier   (501) staff       (20)        1 2022-06-30 14:58:40.000000 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/not-zip-safe
--rw-r--r--   0 charleslanier   (501) staff       (20)       57 2023-04-26 08:59:19.000000 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/requires.txt
--rw-r--r--   0 charleslanier   (501) staff       (20)       15 2023-04-26 08:59:19.000000 ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/top_level.txt
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.639208 ruleslabs-core-1.0.0/src/test/
--rw-r--r--   0 charleslanier   (501) staff       (20)      759 2023-01-29 20:39:28.000000 ruleslabs-core-1.0.0/src/test/upgrade.cairo
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.641750 ruleslabs-core-1.0.0/tests/
--rw-r--r--   0 charleslanier   (501) staff       (20)      173 2022-03-30 14:00:15.000000 ruleslabs-core-1.0.0/tests/build_cache.py
--rw-r--r--   0 charleslanier   (501) staff       (20)     4333 2023-04-23 18:53:20.000000 ruleslabs-core-1.0.0/tests/conftest.py
--rw-r--r--   0 charleslanier   (501) staff       (20)    43802 2023-04-25 21:28:04.000000 ruleslabs-core-1.0.0/tests/test.py
-drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 08:59:19.644570 ruleslabs-core-1.0.0/tests/utils/
--rw-r--r--   0 charleslanier   (501) staff       (20)      319 2023-01-30 08:40:16.000000 ruleslabs-core-1.0.0/tests/utils/Signer.py
--rw-r--r--   0 charleslanier   (501) staff       (20)     2751 2023-04-23 19:10:22.000000 ruleslabs-core-1.0.0/tests/utils/TransactionSender.py
--rw-r--r--   0 charleslanier   (501) staff       (20)     5823 2023-04-24 07:58:35.000000 ruleslabs-core-1.0.0/tests/utils/misc.py
--rw-r--r--   0 charleslanier   (501) staff       (20)      826 2022-06-30 14:47:34.000000 ruleslabs-core-1.0.0/tox.ini
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.775589 ruleslabs-core-1.0.1/
+-rw-r--r--   0 charleslanier   (501) staff       (20)      195 2022-09-02 14:09:10.000000 ruleslabs-core-1.0.1/.gitignore
+-rw-r--r--   0 charleslanier   (501) staff       (20)       31 2022-06-30 14:47:19.000000 ruleslabs-core-1.0.1/MANIFEST.in
+-rw-r--r--   0 charleslanier   (501) staff       (20)     7780 2023-04-26 09:10:50.775951 ruleslabs-core-1.0.1/PKG-INFO
+-rw-r--r--   0 charleslanier   (501) staff       (20)     7423 2022-07-12 08:20:16.000000 ruleslabs-core-1.0.1/README.md
+-rw-r--r--   0 charleslanier   (501) staff       (20)      186 2022-06-30 14:49:01.000000 ruleslabs-core-1.0.1/pyproject.toml
+-rw-r--r--   0 charleslanier   (501) staff       (20)       49 2023-01-29 20:42:33.000000 ruleslabs-core-1.0.1/requirements.txt
+-rw-r--r--   0 charleslanier   (501) staff       (20)      746 2023-04-26 09:10:50.777071 ruleslabs-core-1.0.1/setup.cfg
+-rw-r--r--   0 charleslanier   (501) staff       (20)      511 2023-04-26 09:10:44.000000 ruleslabs-core-1.0.1/setup.py
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.711623 ruleslabs-core-1.0.1/src/
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.716129 ruleslabs-core-1.0.1/src/ruleslabs/
+-rw-r--r--   0 charleslanier   (501) staff       (20)    11822 2023-04-26 08:26:47.000000 ruleslabs-core-1.0.1/src/ruleslabs/Rules.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)      272 2022-06-30 14:52:08.000000 ruleslabs-core-1.0.1/src/ruleslabs/__init__.py
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.717355 ruleslabs-core-1.0.1/src/ruleslabs/interfaces/
+-rw-r--r--   0 charleslanier   (501) staff       (20)      337 2023-04-26 09:10:33.000000 ruleslabs-core-1.0.1/src/ruleslabs/interfaces/IRules.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)      350 2023-04-26 08:56:57.000000 ruleslabs-core-1.0.1/src/ruleslabs/interfaces/IRulesCards.cairo
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.721855 ruleslabs-core-1.0.1/src/ruleslabs/libraries/
+-rw-r--r--   0 charleslanier   (501) staff       (20)     5270 2023-04-23 22:10:04.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/AccessControl.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     4360 2023-04-25 11:49:15.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/Cards.cairo
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.762340 ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/
+-rw-r--r--   0 charleslanier   (501) staff       (20)    15088 2023-04-25 21:24:19.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/ERC1155.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     1957 2023-04-23 18:02:32.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/ERC1155ContractURI.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)      955 2023-04-23 16:58:55.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/IERC1155Receiver.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     1277 2023-04-23 18:03:53.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/Ownable.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     6164 2023-04-25 11:35:08.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/Packs.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     1522 2023-04-23 18:09:02.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/Scarcity.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     1227 2023-04-23 19:26:15.000000 ruleslabs-core-1.0.1/src/ruleslabs/libraries/Upgradeable.cairo
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.765018 ruleslabs-core-1.0.1/src/ruleslabs/utils/
+-rw-r--r--   0 charleslanier   (501) staff       (20)     4015 2023-04-24 08:09:28.000000 ruleslabs-core-1.0.1/src/ruleslabs/utils/card.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)      430 2023-04-23 21:47:18.000000 ruleslabs-core-1.0.1/src/ruleslabs/utils/constants.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)      845 2023-01-29 20:39:28.000000 ruleslabs-core-1.0.1/src/ruleslabs/utils/memset.cairo
+-rw-r--r--   0 charleslanier   (501) staff       (20)     1067 2023-04-25 11:34:41.000000 ruleslabs-core-1.0.1/src/ruleslabs/utils/metadata.cairo
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.768650 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/
+-rw-r--r--   0 charleslanier   (501) staff       (20)     7780 2023-04-26 09:10:50.000000 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/PKG-INFO
+-rw-r--r--   0 charleslanier   (501) staff       (20)     1153 2023-04-26 09:10:50.000000 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 charleslanier   (501) staff       (20)        1 2023-04-26 09:10:50.000000 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 charleslanier   (501) staff       (20)        1 2022-06-30 14:58:40.000000 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/not-zip-safe
+-rw-r--r--   0 charleslanier   (501) staff       (20)       57 2023-04-26 09:10:50.000000 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/requires.txt
+-rw-r--r--   0 charleslanier   (501) staff       (20)       15 2023-04-26 09:10:50.000000 ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/top_level.txt
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.769097 ruleslabs-core-1.0.1/src/test/
+-rw-r--r--   0 charleslanier   (501) staff       (20)      759 2023-01-29 20:39:28.000000 ruleslabs-core-1.0.1/src/test/upgrade.cairo
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.771516 ruleslabs-core-1.0.1/tests/
+-rw-r--r--   0 charleslanier   (501) staff       (20)      173 2022-03-30 14:00:15.000000 ruleslabs-core-1.0.1/tests/build_cache.py
+-rw-r--r--   0 charleslanier   (501) staff       (20)     4333 2023-04-23 18:53:20.000000 ruleslabs-core-1.0.1/tests/conftest.py
+-rw-r--r--   0 charleslanier   (501) staff       (20)    43802 2023-04-25 21:28:04.000000 ruleslabs-core-1.0.1/tests/test.py
+drwxr-xr-x   0 charleslanier   (501) staff       (20)        0 2023-04-26 09:10:50.774805 ruleslabs-core-1.0.1/tests/utils/
+-rw-r--r--   0 charleslanier   (501) staff       (20)      319 2023-01-30 08:40:16.000000 ruleslabs-core-1.0.1/tests/utils/Signer.py
+-rw-r--r--   0 charleslanier   (501) staff       (20)     2751 2023-04-23 19:10:22.000000 ruleslabs-core-1.0.1/tests/utils/TransactionSender.py
+-rw-r--r--   0 charleslanier   (501) staff       (20)     5823 2023-04-24 07:58:35.000000 ruleslabs-core-1.0.1/tests/utils/misc.py
+-rw-r--r--   0 charleslanier   (501) staff       (20)      826 2022-06-30 14:47:34.000000 ruleslabs-core-1.0.1/tox.ini
```

### Comparing `ruleslabs-core-1.0.0/PKG-INFO` & `ruleslabs-core-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruleslabs-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Periphery smart contracts used by rules.
 Home-page: https://github.com/ruleslabs/core
 Author: 0xChqrles
 Author-email: charles@rules.art
 License: MIT
 Platform: any
 Classifier: Operating System :: OS Independent
```

### Comparing `ruleslabs-core-1.0.0/README.md` & `ruleslabs-core-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/setup.cfg` & `ruleslabs-core-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/Rules.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/Rules.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/AccessControl.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/AccessControl.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/Cards.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/Cards.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/ERC1155.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/ERC1155.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/ERC1155ContractURI.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/ERC1155ContractURI.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/ERC1155/IERC1155Receiver.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/ERC1155/IERC1155Receiver.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/Ownable.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/Ownable.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/Packs.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/Packs.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/Scarcity.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/Scarcity.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/libraries/Upgradeable.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/libraries/Upgradeable.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/utils/card.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/utils/card.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/utils/memset.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/utils/memset.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs/utils/metadata.cairo` & `ruleslabs-core-1.0.1/src/ruleslabs/utils/metadata.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/PKG-INFO` & `ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruleslabs-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Periphery smart contracts used by rules.
 Home-page: https://github.com/ruleslabs/core
 Author: 0xChqrles
 Author-email: charles@rules.art
 License: MIT
 Platform: any
 Classifier: Operating System :: OS Independent
```

### Comparing `ruleslabs-core-1.0.0/src/ruleslabs_core.egg-info/SOURCES.txt` & `ruleslabs-core-1.0.1/src/ruleslabs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/src/test/upgrade.cairo` & `ruleslabs-core-1.0.1/src/test/upgrade.cairo`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/tests/conftest.py` & `ruleslabs-core-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/tests/test.py` & `ruleslabs-core-1.0.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/tests/utils/TransactionSender.py` & `ruleslabs-core-1.0.1/tests/utils/TransactionSender.py`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/tests/utils/misc.py` & `ruleslabs-core-1.0.1/tests/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ruleslabs-core-1.0.0/tox.ini` & `ruleslabs-core-1.0.1/tox.ini`

 * *Files identical despite different names*

