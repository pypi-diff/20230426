# Comparing `tmp/promsoft_pecom_interface-0.1.1.tar.gz` & `tmp/promsoft_pecom_interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_pecom_interface-0.1.1.tar", max compression
+gzip compressed data, was "promsoft_pecom_interface-0.1.2.tar", max compression
```

## Comparing `promsoft_pecom_interface-0.1.1.tar` & `promsoft_pecom_interface-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      236 2023-04-25 07:23:26.403577 promsoft_pecom_interface-0.1.1/README.md
--rw-r--r--   0        0        0      496 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.1/promsoft_pecom_interface/__init__.py
--rw-r--r--   0        0        0     7757 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.1/promsoft_pecom_interface/cargopickup.py
--rw-r--r--   0        0        0      357 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.1/promsoft_pecom_interface/common.py
--rw-r--r--   0        0        0     5121 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.1/promsoft_pecom_interface/preregistration.py
--rw-r--r--   0        0        0      528 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 promsoft_pecom_interface-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      278 2023-04-26 10:02:58.776966 promsoft_pecom_interface-0.1.2/README.md
+-rw-r--r--   0        0        0      496 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.2/promsoft_pecom_interface/__init__.py
+-rw-r--r--   0        0        0     7757 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.2/promsoft_pecom_interface/cargopickup.py
+-rw-r--r--   0        0        0      357 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.2/promsoft_pecom_interface/common.py
+-rw-r--r--   0        0        0     5121 2023-04-25 07:23:26.407577 promsoft_pecom_interface-0.1.2/promsoft_pecom_interface/preregistration.py
+-rw-r--r--   0        0        0      528 2023-04-26 12:30:00.376901 promsoft_pecom_interface-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 promsoft_pecom_interface-0.1.2/PKG-INFO
```

### Comparing `promsoft_pecom_interface-0.1.1/promsoft_pecom_interface/cargopickup.py` & `promsoft_pecom_interface-0.1.2/promsoft_pecom_interface/cargopickup.py`

 * *Files identical despite different names*

### Comparing `promsoft_pecom_interface-0.1.1/promsoft_pecom_interface/preregistration.py` & `promsoft_pecom_interface-0.1.2/promsoft_pecom_interface/preregistration.py`

 * *Files identical despite different names*

### Comparing `promsoft_pecom_interface-0.1.1/pyproject.toml` & `promsoft_pecom_interface-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promsoft-pecom-interface"
-version = "0.1.1"
+version = "0.1.2"
 description = "Интерфейс HTTP API для транспортной компании PECOM "
 authors = ["Promsoft <info@promsoft.ru>"]
 readme = "README.md"
 packages = [{include = "promsoft_pecom_interface"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `promsoft_pecom_interface-0.1.1/PKG-INFO` & `promsoft_pecom_interface-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: promsoft-pecom-interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: Интерфейс HTTP API для транспортной компании PECOM 
 Author: Promsoft
 Author-email: info@promsoft.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
+# promsoft_pecom_interface
+
 Interfaces for HTTP API <a href="https://kabinet.pecom.ru/api/v1">PECOM</a> transport company.
 Usage:
 
+```python
 from promsoft_pecom_interface import IdentityCard
 
 
 ic = IdentityCard(series='1234', numbers='567890')
 print(f"As dict: {ic.dict()}")
+```
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: promsoft-pecom-interface Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: promsoft-pecom-interface Version: 0.1.2 Summary:
 ÐÐ½ÑÐµÑÑÐµÐ¹Ñ HTTP API Ð´Ð»Ñ ÑÑÐ°Ð½ÑÐ¿Ð¾ÑÑÐ½Ð¾Ð¹ ÐºÐ¾Ð¼Ð¿Ð°Ð½Ð¸Ð¸
 PECOM Author: Promsoft Author-email: info@promsoft.ru Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: pydantic (>=1.10.7,<2.0.0) Description-Content-
-Type: text/markdown Interfaces for HTTP API PECOM transport company. Usage:
-from promsoft_pecom_interface import IdentityCard ic = IdentityCard
-(series='1234', numbers='567890') print(f"As dict: {ic.dict()}")
+Type: text/markdown # promsoft_pecom_interface Interfaces for HTTP API PECOM
+transport company. Usage: ```python from promsoft_pecom_interface import
+IdentityCard ic = IdentityCard(series='1234', numbers='567890') print(f"As
+dict: {ic.dict()}") ```
```

