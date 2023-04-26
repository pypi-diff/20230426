# Comparing `tmp/Acquirers-0.0.6.tar.gz` & `tmp/Acquirers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Acquirers-0.0.6.tar", last modified: Thu Jun  9 04:14:41 2022, max compression
+gzip compressed data, was "Acquirers-0.0.7.tar", last modified: Tue Apr 25 21:16:00 2023, max compression
```

## Comparing `Acquirers-0.0.6.tar` & `Acquirers-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2022-06-09 04:14:41.286723 Acquirers-0.0.6/
-drwxrwxr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2022-06-09 04:14:41.282723 Acquirers-0.0.6/Acquirers/
-drwxrwxr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2022-06-09 04:14:41.286723 Acquirers-0.0.6/Acquirers/Rocketpay/
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1407 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/Rocketpay/__init__.py
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)      560 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/Rocketpay/exceptions.py
-drwxrwxr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2022-06-09 04:14:41.286723 Acquirers-0.0.6/Acquirers/Tinkoff/
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)    13839 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/Tinkoff/__init__.py
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1267 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/Tinkoff/exceptions.py
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1614 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/Tinkoff/receipt.py
-drwxrwxr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2022-06-09 04:14:41.286723 Acquirers-0.0.6/Acquirers/Yandexcheckout/
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1876 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/Yandexcheckout/__init__.py
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       67 2022-05-27 17:50:03.000000 Acquirers-0.0.6/Acquirers/__init__.py
-drwxrwxr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2022-06-09 04:14:41.286723 Acquirers-0.0.6/Acquirers.egg-info/
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     2016 2022-06-09 04:14:41.000000 Acquirers-0.0.6/Acquirers.egg-info/PKG-INFO
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)      406 2022-06-09 04:14:41.000000 Acquirers-0.0.6/Acquirers.egg-info/SOURCES.txt
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)        1 2022-06-09 04:14:41.000000 Acquirers-0.0.6/Acquirers.egg-info/dependency_links.txt
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       25 2022-06-09 04:14:41.000000 Acquirers-0.0.6/Acquirers.egg-info/requires.txt
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       10 2022-06-09 04:14:41.000000 Acquirers-0.0.6/Acquirers.egg-info/top_level.txt
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)    35149 2022-05-27 17:50:03.000000 Acquirers-0.0.6/LICENSE
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     2016 2022-06-09 04:14:41.286723 Acquirers-0.0.6/PKG-INFO
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1498 2022-06-09 04:13:31.000000 Acquirers-0.0.6/README.md
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       38 2022-06-09 04:14:41.286723 Acquirers-0.0.6/setup.cfg
--rw-rw-r--   0 vanzhiganov  (1000) vanzhiganov  (1000)      883 2022-06-09 04:14:39.000000 Acquirers-0.0.6/setup.py
+drwxr-xr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2023-04-25 21:16:00.971577 Acquirers-0.0.7/
+drwxr-xr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2023-04-25 21:16:00.968577 Acquirers-0.0.7/Acquirers/
+drwxr-xr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2023-04-25 21:16:00.969576 Acquirers-0.0.7/Acquirers/Rocketpay/
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1407 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/Rocketpay/__init__.py
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)      560 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/Rocketpay/exceptions.py
+drwxr-xr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2023-04-25 21:16:00.970576 Acquirers-0.0.7/Acquirers/Tinkoff/
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)    14358 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/Tinkoff/__init__.py
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1267 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/Tinkoff/exceptions.py
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1614 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/Tinkoff/receipt.py
+drwxr-xr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2023-04-25 21:16:00.970576 Acquirers-0.0.7/Acquirers/Yandexcheckout/
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1876 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/Yandexcheckout/__init__.py
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       67 2023-04-25 21:15:39.000000 Acquirers-0.0.7/Acquirers/__init__.py
+drwxr-xr-x   0 vanzhiganov  (1000) vanzhiganov  (1000)        0 2023-04-25 21:16:00.969576 Acquirers-0.0.7/Acquirers.egg-info/
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1962 2023-04-25 21:16:00.000000 Acquirers-0.0.7/Acquirers.egg-info/PKG-INFO
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)      406 2023-04-25 21:16:00.000000 Acquirers-0.0.7/Acquirers.egg-info/SOURCES.txt
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)        1 2023-04-25 21:16:00.000000 Acquirers-0.0.7/Acquirers.egg-info/dependency_links.txt
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       25 2023-04-25 21:16:00.000000 Acquirers-0.0.7/Acquirers.egg-info/requires.txt
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       10 2023-04-25 21:16:00.000000 Acquirers-0.0.7/Acquirers.egg-info/top_level.txt
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)    35149 2023-04-25 21:15:39.000000 Acquirers-0.0.7/LICENSE
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1962 2023-04-25 21:16:00.970576 Acquirers-0.0.7/PKG-INFO
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)     1498 2023-04-25 21:15:39.000000 Acquirers-0.0.7/README.md
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)       38 2023-04-25 21:16:00.971577 Acquirers-0.0.7/setup.cfg
+-rw-r--r--   0 vanzhiganov  (1000) vanzhiganov  (1000)      883 2023-04-25 21:15:39.000000 Acquirers-0.0.7/setup.py
```

### Comparing `Acquirers-0.0.6/Acquirers/Rocketpay/__init__.py` & `Acquirers-0.0.7/Acquirers/Rocketpay/__init__.py`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/Acquirers/Rocketpay/exceptions.py` & `Acquirers-0.0.7/Acquirers/Rocketpay/exceptions.py`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/Acquirers/Tinkoff/__init__.py` & `Acquirers-0.0.7/Acquirers/Tinkoff/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,27 @@
         else:
             return language.lower()
 
     @staticmethod
     def _is_recurrent(is_recurrent: bool) -> str:
         return 'y' if is_recurrent else 'n'
 
+    @staticmethod
+    def _proccess_data_key(data: dict) -> dict:
+        allowed_items = [
+            'Phone'
+        ]
+        result = {}
+        for item in data:
+            if item not in allowed_items:
+                continue
+            result[item] = data[item]
+        return result
+
+
     def init(self, order_id, amount, ip=None, description=None, currency=None, language=None,
              customer_key=None, recurrent=False, redirect_due_date=None, data=None, receipt=None, sign_request=False):
         """Init - создание заказа
 
         :param:
         {
             'Success': True,
@@ -62,42 +75,44 @@
         {
             'Success': False,
             'ErrorCode': '9999',
             'Message': 'Неверные параметры.',
             'Details': 'Неверный токен. Проверьте пару TerminalKey/SecretKey.'
         }
         """
-        data = dict()
-        data['TerminalKey'] = self.terminal_id
-        data['Amount'] = amount
-        data['OrderId'] = order_id
+        request_data = dict()
+        request_data['TerminalKey'] = self.terminal_id
+        request_data['Amount'] = amount
+        request_data['OrderId'] = order_id
 
         if ip:
-            data['IP'] = ip
+            request_data['IP'] = ip
         if description:
-            data['Description'] = description
+            request_data['Description'] = description
         if language:
-            data['Language'] = self._get_language(language)
+            request_data['Language'] = self._get_language(language)
         if customer_key:
-            data['CustomerKey'] = customer_key
+            request_data['CustomerKey'] = customer_key
         if recurrent:
-            data['Recurrent'] = self._is_recurrent(recurrent)
+            request_data['Recurrent'] = self._is_recurrent(recurrent)
             #
-            if not data['CustomerKey']:
+            if not request_data['CustomerKey']:
                 raise TinkoffSimplePaymentInitParameterRequiredException('customer_key')
+        if data:
+            request_data['DATA'] = self._proccess_data_key(data)
         if sign_request:
-            data['Token'] = self.get_signature(data)
+            request_data['Token'] = self.get_signature(request_data)
 
-        request = requests.post('https://securepay.tinkoff.ru/v2/Init', json=data)
-        data = request.json()
+        request = requests.post('https://securepay.tinkoff.ru/v2/Init', json=request_data)
+        resopnse_data = request.json()
 
-        if not data.get('Success'):
-            raise TinkoffException(data)
+        if not resopnse_data.get('Success'):
+            raise TinkoffException(resopnse_data)
 
-        return data
+        return resopnse_data
     
     def finish_authorize(self,):
         """подтверждения платежа
         Данный метод используется, если магазин обладает сертификацией PCI DSS и использует свою
         собственную платёжную форму вместо формы банка. Метод FinishAuthorize подтверждает
         инициированный платёж передачей карточных данных. При использовании одностадийного
         проведения осуществляет списание денежных средств с карты покупателя. При двухстадийном
```

### Comparing `Acquirers-0.0.6/Acquirers/Tinkoff/exceptions.py` & `Acquirers-0.0.7/Acquirers/Tinkoff/exceptions.py`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/Acquirers/Tinkoff/receipt.py` & `Acquirers-0.0.7/Acquirers/Tinkoff/receipt.py`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/Acquirers/Yandexcheckout/__init__.py` & `Acquirers-0.0.7/Acquirers/Yandexcheckout/__init__.py`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/Acquirers.egg-info/PKG-INFO` & `Acquirers-0.0.7/Acquirers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: Acquirers
-Version: 0.0.6
-Summary: UNKNOWN
+Version: 0.0.7
 Home-page: https://github.com/vanzhiganov/acquirers/
 Author: Vyacheslav Anzhiganov
 Author-email: vanzhiganov@yandex.com
-License: UNKNOWN
 Project-URL: Source, https://github.com/vanzhiganov/acquirers/
 Project-URL: Tracker, https://github.com/vanzhiganov/acquirers/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Acquirers
 
@@ -84,9 +81,7 @@
 
 Инициируем платёж
 
 ```python
 rp.init(order_id="example", amount="1.0")
 ```
 
-
-
```

### Comparing `Acquirers-0.0.6/LICENSE` & `Acquirers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/PKG-INFO` & `Acquirers-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: Acquirers
-Version: 0.0.6
-Summary: UNKNOWN
+Version: 0.0.7
 Home-page: https://github.com/vanzhiganov/acquirers/
 Author: Vyacheslav Anzhiganov
 Author-email: vanzhiganov@yandex.com
-License: UNKNOWN
 Project-URL: Source, https://github.com/vanzhiganov/acquirers/
 Project-URL: Tracker, https://github.com/vanzhiganov/acquirers/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Acquirers
 
@@ -84,9 +81,7 @@
 
 Инициируем платёж
 
 ```python
 rp.init(order_id="example", amount="1.0")
 ```
 
-
-
```

### Comparing `Acquirers-0.0.6/README.md` & `Acquirers-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Acquirers-0.0.6/setup.py` & `Acquirers-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='Acquirers',
-    version='0.0.6',
+    version='0.0.7',
     author="Vyacheslav Anzhiganov",
     author_email="vanzhiganov@yandex.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vanzhiganov/acquirers/",
     project_urls={
         "Source": "https://github.com/vanzhiganov/acquirers/",
```

