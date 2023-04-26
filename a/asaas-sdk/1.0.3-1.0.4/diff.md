# Comparing `tmp/asaas-sdk-1.0.3.tar.gz` & `tmp/asaas-sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaas-sdk-1.0.3.tar", last modified: Wed Apr 26 05:59:30 2023, max compression
+gzip compressed data, was "asaas-sdk-1.0.4.tar", last modified: Wed Apr 26 06:02:13 2023, max compression
```

## Comparing `asaas-sdk-1.0.3.tar` & `asaas-sdk-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 05:59:30.959368 asaas-sdk-1.0.3/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-1.0.3/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-26 05:59:30.959368 asaas-sdk-1.0.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-20 02:28:32.000000 asaas-sdk-1.0.3/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 05:59:30.956035 asaas-sdk-1.0.3/asaas/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13085 2023-04-26 05:59:02.000000 asaas-sdk-1.0.3/asaas/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-26 05:13:01.000000 asaas-sdk-1.0.3/asaas/customers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      107 2023-04-19 02:53:26.000000 asaas-sdk-1.0.3/asaas/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-26 05:29:32.000000 asaas-sdk-1.0.3/asaas/payments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-19 23:28:03.000000 asaas-sdk-1.0.3/asaas/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 05:59:30.956035 asaas-sdk-1.0.3/asaas_sdk.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-26 05:59:30.000000 asaas-sdk-1.0.3/asaas_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-26 05:59:30.000000 asaas-sdk-1.0.3/asaas_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-26 05:59:30.000000 asaas-sdk-1.0.3/asaas_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-26 05:59:30.000000 asaas-sdk-1.0.3/asaas_sdk.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-26 05:59:30.000000 asaas-sdk-1.0.3/asaas_sdk.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-26 05:59:09.000000 asaas-sdk-1.0.3/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-26 05:59:30.959368 asaas-sdk-1.0.3/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 06:02:13.335963 asaas-sdk-1.0.4/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-1.0.4/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-26 06:02:13.332630 asaas-sdk-1.0.4/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-20 02:28:32.000000 asaas-sdk-1.0.4/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 06:02:13.332630 asaas-sdk-1.0.4/asaas/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13104 2023-04-26 06:01:35.000000 asaas-sdk-1.0.4/asaas/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-26 05:13:01.000000 asaas-sdk-1.0.4/asaas/customers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      107 2023-04-19 02:53:26.000000 asaas-sdk-1.0.4/asaas/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-26 05:29:32.000000 asaas-sdk-1.0.4/asaas/payments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-19 23:28:03.000000 asaas-sdk-1.0.4/asaas/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 06:02:13.332630 asaas-sdk-1.0.4/asaas_sdk.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-26 06:02:01.000000 asaas-sdk-1.0.4/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-26 06:02:13.335963 asaas-sdk-1.0.4/setup.cfg
```

### Comparing `asaas-sdk-1.0.3/LICENSE` & `asaas-sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.3/PKG-INFO` & `asaas-sdk-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaas-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary:  Biblioteca não oficial de comunicação com a API de pagamento do ASAAS
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/asaas-sdk
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/asaas-sdk/issues
 Keywords: asaas,sdk,payment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asaas-sdk-1.0.3/README.md` & `asaas-sdk-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.3/asaas/__init__.py` & `asaas-sdk-1.0.4/asaas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,21 +171,21 @@
         )
 
         return Payment(**customer)
 
     def new(self,
             customer: Customer,
             billingType: payments.BillingType,
-            value: float,
             dueDate: date,
+            value: Optional[float] = None,
+            totalValue: Optional[float] = None, 
             description: Optional[str] = None,
             externalReference: Optional[str] = None,
             installmentCount: Optional[str] = None,
             installmentValue: Optional[str] = None, 
-            totalValue: Optional[str] = None, 
             discount: Optional[payments.Discount] = None,
             interest: Optional[payments.Interest] = None,
             fine: Optional[payments.Fine] = None,
             postalService: Optional[bool] = None,
             split: Optional[List[payments.Split]] = None,
             creditCard: Optional[payments.CreditCard] = None,
             creditCardHolderInfo: Optional[payments.CreditCardHolderInfo] = None,
```

### Comparing `asaas-sdk-1.0.3/asaas/customers.py` & `asaas-sdk-1.0.4/asaas/customers.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.3/asaas/payments.py` & `asaas-sdk-1.0.4/asaas/payments.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.3/asaas_sdk.egg-info/PKG-INFO` & `asaas-sdk-1.0.4/asaas_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaas-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary:  Biblioteca não oficial de comunicação com a API de pagamento do ASAAS
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/asaas-sdk
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/asaas-sdk/issues
 Keywords: asaas,sdk,payment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asaas-sdk-1.0.3/pyproject.toml` & `asaas-sdk-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asaas-sdk"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Gabriel Niziolek", email="ganiziolek@gmail.com" },
 ]
 description = " Biblioteca não oficial de comunicação com a API de pagamento do ASAAS"
 keywords = ["asaas", "sdk", "payment"]
 readme = "README.md"
 requires-python = ">=3.10"
```

