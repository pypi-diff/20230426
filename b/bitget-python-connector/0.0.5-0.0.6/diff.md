# Comparing `tmp/bitget-python-connector-0.0.5.tar.gz` & `tmp/bitget-python-connector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitget-python-connector-0.0.5.tar", last modified: Tue Apr 25 14:27:29 2023, max compression
+gzip compressed data, was "bitget-python-connector-0.0.6.tar", last modified: Wed Apr 26 03:58:18 2023, max compression
```

## Comparing `bitget-python-connector-0.0.5.tar` & `bitget-python-connector-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.310550 bitget-python-connector-0.0.5/
--rw-rw-rw-   0        0        0     1076 2023-04-25 10:21:00.000000 bitget-python-connector-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      592 2023-04-25 14:27:29.310550 bitget-python-connector-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:20:16.000000 bitget-python-connector-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.261562 bitget-python-connector-0.0.5/bitget_python_connector/
--rw-rw-rw-   0        0        0      385 2023-04-25 14:23:23.000000 bitget-python-connector-0.0.5/bitget_python_connector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.284563 bitget-python-connector-0.0.5/bitget_python_connector/broker/
--rw-rw-rw-   0        0        0     4261 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/broker/account_api.py
--rw-rw-rw-   0        0        0     1668 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/broker/manage_api.py
--rw-rw-rw-   0        0        0     3076 2023-04-25 13:26:06.000000 bitget-python-connector-0.0.5/bitget_python_connector/client.py
--rw-rw-rw-   0        0        0     1535 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/consts.py
--rw-rw-rw-   0        0        0     1208 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.293549 bitget-python-connector-0.0.5/bitget_python_connector/mix/
--rw-rw-rw-   0        0        0       18 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/__init__.py
--rw-rw-rw-   0        0        0     5556 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/account_api.py
--rw-rw-rw-   0        0        0     5582 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/market_api.py
--rw-rw-rw-   0        0        0     5435 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/order_api.py
--rw-rw-rw-   0        0        0     8974 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/plan_api.py
--rw-rw-rw-   0        0        0     1306 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/position_api.py
--rw-rw-rw-   0        0        0     6103 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/mix/trace_api.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.304541 bitget-python-connector-0.0.5/bitget_python_connector/spot/
--rw-rw-rw-   0        0        0       18 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/account_api.py
--rw-rw-rw-   0        0        0     2362 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/market_api.py
--rw-rw-rw-   0        0        0     4562 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/order_api.py
--rw-rw-rw-   0        0        0     2811 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/plan_api.py
--rw-rw-rw-   0        0        0     1182 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/public_api.py
--rw-rw-rw-   0        0        0     3823 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/spot/wallet_api.py
--rw-rw-rw-   0        0        0     1625 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.305541 bitget-python-connector-0.0.5/bitget_python_connector/ws/
--rw-rw-rw-   0        0        0    10899 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/ws/bitget_ws_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.307548 bitget-python-connector-0.0.5/bitget_python_connector/ws/utils/
--rw-rw-rw-   0        0        0      485 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.5/bitget_python_connector/ws/utils/sign_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.281564 bitget-python-connector-0.0.5/bitget_python_connector.egg-info/
--rw-rw-rw-   0        0        0      592 2023-04-25 14:27:29.000000 bitget-python-connector-0.0.5/bitget_python_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-04-25 14:27:29.000000 bitget-python-connector-0.0.5/bitget_python_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 14:27:29.000000 bitget-python-connector-0.0.5/bitget_python_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 14:27:29.000000 bitget-python-connector-0.0.5/bitget_python_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-04-25 14:27:29.000000 bitget-python-connector-0.0.5/bitget_python_connector.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 14:27:29.308544 bitget-python-connector-0.0.5/examples/
--rw-rw-rw-   0        0        0      247 2023-04-25 11:01:35.000000 bitget-python-connector-0.0.5/examples/spot_example.py
--rw-rw-rw-   0        0        0      751 2023-04-25 14:23:40.000000 bitget-python-connector-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 14:27:29.311540 bitget-python-connector-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.735760 bitget-python-connector-0.0.6/
+-rw-rw-rw-   0        0        0     1076 2023-04-25 10:21:00.000000 bitget-python-connector-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3008 2023-04-26 03:58:18.735760 bitget-python-connector-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2412 2023-04-26 03:55:14.000000 bitget-python-connector-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.688761 bitget-python-connector-0.0.6/bitget_python_connector/
+-rw-rw-rw-   0        0        0      385 2023-04-25 14:23:23.000000 bitget-python-connector-0.0.6/bitget_python_connector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.708760 bitget-python-connector-0.0.6/bitget_python_connector/broker/
+-rw-rw-rw-   0        0        0     4467 2023-04-26 03:23:19.000000 bitget-python-connector-0.0.6/bitget_python_connector/broker/account_api.py
+-rw-rw-rw-   0        0        0     1728 2023-04-26 03:23:27.000000 bitget-python-connector-0.0.6/bitget_python_connector/broker/manage_api.py
+-rw-rw-rw-   0        0        0     3076 2023-04-25 13:26:06.000000 bitget-python-connector-0.0.6/bitget_python_connector/client.py
+-rw-rw-rw-   0        0        0     1535 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/consts.py
+-rw-rw-rw-   0        0        0     1208 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.718761 bitget-python-connector-0.0.6/bitget_python_connector/mix/
+-rw-rw-rw-   0        0        0       18 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/__init__.py
+-rw-rw-rw-   0        0        0     5804 2023-04-26 03:12:05.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/account_api.py
+-rw-rw-rw-   0        0        0     5894 2023-04-26 03:22:46.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/market_api.py
+-rw-rw-rw-   0        0        0     5671 2023-04-26 03:20:48.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/order_api.py
+-rw-rw-rw-   0        0        0     9404 2023-04-26 03:19:49.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/plan_api.py
+-rw-rw-rw-   0        0        0     1358 2023-04-26 03:17:54.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/position_api.py
+-rw-rw-rw-   0        0        0     6358 2023-04-26 03:17:32.000000 bitget-python-connector-0.0.6/bitget_python_connector/mix/trace_api.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.725761 bitget-python-connector-0.0.6/bitget_python_connector/spot/
+-rw-rw-rw-   0        0        0       18 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/__init__.py
+-rw-rw-rw-   0        0        0     2159 2023-04-26 03:12:16.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/account_api.py
+-rw-rw-rw-   0        0        0     2490 2023-04-26 03:12:32.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/market_api.py
+-rw-rw-rw-   0        0        0     4758 2023-04-26 03:12:52.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/order_api.py
+-rw-rw-rw-   0        0        0     2811 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/plan_api.py
+-rw-rw-rw-   0        0        0     1258 2023-04-26 03:13:03.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/public_api.py
+-rw-rw-rw-   0        0        0     4020 2023-04-26 03:13:34.000000 bitget-python-connector-0.0.6/bitget_python_connector/spot/wallet_api.py
+-rw-rw-rw-   0        0        0     1625 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.727765 bitget-python-connector-0.0.6/bitget_python_connector/ws/
+-rw-rw-rw-   0        0        0    10933 2023-04-26 03:05:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/ws/bitget_ws_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.728760 bitget-python-connector-0.0.6/bitget_python_connector/ws/utils/
+-rw-rw-rw-   0        0        0      485 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.6/bitget_python_connector/ws/utils/sign_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.706760 bitget-python-connector-0.0.6/bitget_python_connector.egg-info/
+-rw-rw-rw-   0        0        0     3008 2023-04-26 03:58:18.000000 bitget-python-connector-0.0.6/bitget_python_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-04-26 03:58:18.000000 bitget-python-connector-0.0.6/bitget_python_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 03:58:18.000000 bitget-python-connector-0.0.6/bitget_python_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 03:58:18.000000 bitget-python-connector-0.0.6/bitget_python_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-04-26 03:58:18.000000 bitget-python-connector-0.0.6/bitget_python_connector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 03:58:18.734759 bitget-python-connector-0.0.6/examples/
+-rw-rw-rw-   0        0        0     3695 2023-04-26 02:55:56.000000 bitget-python-connector-0.0.6/examples/spot_example.py
+-rw-rw-rw-   0        0        0      751 2023-04-26 03:56:57.000000 bitget-python-connector-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 03:58:18.735760 bitget-python-connector-0.0.6/setup.cfg
```

### Comparing `bitget-python-connector-0.0.5/LICENSE` & `bitget-python-connector-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/broker/account_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/broker/account_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,134 +2,135 @@
 from ..consts import *
 
 
 class AccountApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    get broker info
-    :return:
-    '''
     def info(self):
+        '''
+        ### get broker info
+        :return:
+        '''
         return self._request_without_params(GET, BROKER_ACCOUNT_V1_URL + '/info')
 
-    '''
-    broker create sub account
-    :return:
-    '''
     def sub_create(self, subName, remark):
+        '''
+        ### broker create sub account
+        :return:
+        '''
         params = {}
         if subName:
             params["subName"] = subName
             params["remark"] = remark
             return self._request_with_params(POST, BROKER_ACCOUNT_V1_URL + '/sub-create', params)
         else:
             return "pls check args "
 
-    '''
-    get sub info list
-    :return:
-    '''
     def sub_list(self, pageSize, lastEndId, status):
+        '''
+        ### get sub info list
+        :return:
+        '''
         params = {}
         params["pageSize"] = pageSize
         params["lastEndId"] = lastEndId
         params["status"] = status
         return self._request_with_params(GET, BROKER_ACCOUNT_V1_URL + '/sub-list', params)
         return "pls check args"
 
-    '''
-    modify sub info list
-    :return:
-    '''
+
     def sub_modify(self, subUid, perm, status):
+        '''
+        ### modify sub info list
+        :return:
+        '''
         params = {}
         if subUid and perm and status:
             params["subUid"] = subUid
             params["perm"] = perm
             params["status"] = status
             return self._request_with_params(POST, BROKER_ACCOUNT_V1_URL + '/sub-modify', params)
         else:
             return "pls check args "
 
-    '''
-    modify sub email
-    :return:
-    '''
     def sub_modify_email(self, subUid, subEmail):
+        '''
+        ### modify sub email
+        :return:
+        '''
         params = {}
         if subUid and subEmail:
             params["subUid"] = subUid
             params["subEmail"] = subEmail
             return self._request_with_params(POST, BROKER_ACCOUNT_V1_URL + '/sub-modify-email', params)
         else:
             return "pls check args "
 
-    '''
-    get sub spot assets
-    :return:
-    '''
     def sub_spot_assets(self, subUid):
+        '''
+        ### get sub spot assets
+        :return:
+        '''
         params = {}
         if subUid :
             params["subUid"] = subUid
             return self._request_with_params(GET, BROKER_ACCOUNT_V1_URL + '/sub-spot-assets', params)
         else:
             return "pls check args "
 
-    '''
-    get sub future assets
-    :return:
-    '''
     def sub_future_assets(self, subUid):
+        '''
+        ### get sub future assets
+        :return:
+        '''
         params = {}
         if subUid:
             params["subUid"] = subUid
             return self._request_with_params(GET, BROKER_ACCOUNT_V1_URL + '/sub-future-assets', params)
         else:
             return "pls check args "
 
-    '''
-    get sub deposit address
-    :return:
-    '''
     def sub_address(self, subUid, subEmail):
+        '''
+        ### get sub deposit address
+        :return:
+        '''
         params = {}
         if subUid and subEmail:
             params["subUid"] = subUid
             params["subEmail"] = subEmail
             return self._request_with_params(POST, BROKER_ACCOUNT_V1_URL + '/sub-address', params)
         else:
             return "pls check args "
 
-    '''
-    sub withdrawal
-    :return:
-    '''
     def sub_withdrawal(self, subUid, coin, chain, address, amount, tag, clientOid):
+        '''
+        ### sub withdrawal
+        :return:
+        '''
         params = {}
         if subUid and coin and chain and address and amount:
             params["subUid"] = subUid
             params["coin"] = coin
             params["chain"] = chain
             params["address"] = address
             params["amount"] = amount
             params["tag"] = tag
             params["clientOid"] = clientOid
             return self._request_with_params(POST, BROKER_ACCOUNT_V1_URL + '/sub-withdrawal', params)
         else:
             return "pls check args "
 
-    '''
-    sub auto transfer 
-    deposit success auto transfer future
-    :return:
-    '''
     def sub_auto_transfer(self, subUid, coin, toAccountType):
+        '''
+        ### sub auto transfer 
+        deposit success auto transfer future
+        :return:
+        '''
         params = {}
         if subUid and coin and toAccountType:
             params["subUid"] = subUid
             params["coin"] = coin
             params["toAccountType"] = toAccountType
             return self._request_with_params(POST, BROKER_ACCOUNT_V1_URL + '/sub-auto-transfer', params)
         else:
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/broker/manage_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/broker/manage_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 from ..consts import *
 
 
 class ManageApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    broker create sub apikey
-    :return:
-    '''
     def sub_create_api(self, subUid, passphrase, remark, ip, perm):
+        '''
+        ### broker create sub apikey
+        :return:
+        '''
         params = {}
         if subUid and passphrase and perm:
             params["subUid"] = subUid
             params["passphrase"] = passphrase
             params["remark"] = remark
             params["ip"] = ip
             params["perm"] = perm
             return self._request_with_params(POST, BROKER_MANAGE_V1_URL + '/sub-api-create', params)
         else:
             return "pls check args "
 
-    '''
-    get sub apikey list
-    :return:
-    '''
     def sub_list(self, subUid):
+        '''
+        ### get sub apikey list
+        :return:
+        '''
         params = {}
         if subUid:
             params["subUid"] = subUid
             return self._request_with_params(GET, BROKER_MANAGE_V1_URL + '/sub-api-list', params)
         else:
             return "pls check args"
 
-    '''
-    broker modify sub apikey
-    :return:
-    '''
     def sub_modify_api(self, subUid, apikey, remark, ip, perm):
+        '''
+        ### broker modify sub apikey
+        :return:
+        '''
         params = {}
         if subUid and apikey and perm:
             params["subUid"] = subUid
             params["apikey"] = apikey
             params["remark"] = remark
             params["ip"] = ip
             params["perm"] = perm
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/client.py` & `bitget-python-connector-0.0.6/bitget_python_connector/client.py`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/consts.py` & `bitget-python-connector-0.0.6/bitget_python_connector/consts.py`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/exceptions.py` & `bitget-python-connector-0.0.6/bitget_python_connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/mix/account_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/mix/account_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,140 +4,140 @@
 from ..consts import *
 
 
 class AccountApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Obtain user account information
-    symbol: Contract transaction pair
-    marginCoin: Deposit currency
-    :return:
-    '''
     def account(self, symbol, marginCoin):
+        '''
+        ### Obtain user account information
+        symbol: Contract transaction pair
+        marginCoin: Deposit currency
+        :return:
+        '''
         params = {}
         if symbol and marginCoin:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             return self._request_with_params(GET, MIX_ACCOUNT_V1_URL + '/account', params)
         else:
             return "pls check args"
 
-    '''
-    Adjusting lever
-    symbol: Contract transaction pair
-    marginCoin: Deposit currency
-    leverage: Leverage ratio
-    holdSide: In the position direction, long multi position short short short positions can not be transferred in case of full positions
-    :return:
-    '''
     def leverage(self, symbol, marginCoin, leverage, holdSide=''):
+        '''
+        ### Adjusting lever
+        symbol: Contract transaction pair
+        marginCoin: Deposit currency
+        leverage: Leverage ratio
+        holdSide: In the position direction, long multi position short short short positions can not be transferred in case of full positions
+        :return:
+        '''
         params = {}
         if symbol and marginCoin:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["leverage"] = leverage
             params["holdSide"] = holdSide
             return self._request_with_params(POST, MIX_ACCOUNT_V1_URL + '/setLeverage', params)
         else:
             return "pls check args"
 
-    '''
-    Adjustment margin
-    symbol: Contract transaction pair
-    marginCoin: Deposit currency
-    amount: Positive increase and negative decrease of deposit amount
-    holdSide: In the position direction, long multi position short short short positions can not be transferred in case of full positions
-    :return:
-    '''
     def margin(self, symbol, marginCoin, amount, holdSide=''):
+        '''
+        ### Adjustment margin
+        symbol: Contract transaction pair
+        marginCoin: Deposit currency
+        amount: Positive increase and negative decrease of deposit amount
+        holdSide: In the position direction, long multi position short short short positions can not be transferred in case of full positions
+        :return:
+        '''
         params = {}
         if symbol and marginCoin:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["amount"] = amount
             params["holdSide"] = holdSide
             return self._request_with_params(POST, MIX_ACCOUNT_V1_URL + '/setMargin', params)
         else:
             return "pls check args"
 
-    '''
-    Adjust margin mode
-    symbol: Contract transaction pair
-    marginCoin: Deposit currency
-    marginMode: Fixed warehouse by warehouse crossed full warehouse
-    :return:
-    '''
     def margin_mode(self, symbol, marginCoin, marginMode):
+        '''
+        ### Adjust margin mode
+        symbol: Contract transaction pair
+        marginCoin: Deposit currency
+        marginMode: Fixed warehouse by warehouse crossed full warehouse
+        :return:
+        '''
         params = {}
         if symbol and marginCoin:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["marginMode"] = marginMode
             return self._request_with_params(POST, MIX_ACCOUNT_V1_URL + '/setMarginMode', params)
         else:
             return "pls check args"
 
-    '''
-    Set position mode
-    symbol: Contract transaction pair
-    marginCoin: Deposit currency
-    holdMode: Position mode single_ Hold single position double_ Hold Bidirectional Position Default Bidirectional Position
-    :return:
-    '''
     def position_mode(self, symbol, marginCoin, holdMode):
+        '''
+        ### Set position mode
+        symbol: Contract transaction pair
+        marginCoin: Deposit currency
+        holdMode: Position mode single_ Hold single position double_ Hold Bidirectional Position Default Bidirectional Position
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and holdMode:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["holdMode"] = holdMode
             return self._request_with_params(POST, MIX_ACCOUNT_V1_URL + '/setPositionMode', params)
         else:
             return "pls check args"
 
-    '''
-    Query the number of open sheets
-    symbol: Contract transaction pair
-    marginCoin: Deposit currency
-    openPrice： Opening price
-    openAmount: Opening limit
-    leverage: Default leverage 20
-    :return:
-    '''
     def open_count(self, symbol, marginCoin, openPrice, openAmount, leverage=20):
+        '''
+        ### Query the number of open sheets
+        symbol: Contract transaction pair
+        marginCoin: Deposit currency
+        openPrice： Opening price
+        openAmount: Opening limit
+        leverage: Default leverage 20
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and openPrice and openAmount:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["openPrice"] = openPrice
             params["openAmount"] = openAmount
             params["leverage"] = leverage
             return self._request_with_params(POST, MIX_ACCOUNT_V1_URL + '/open-count', params)
         else:
             return "pls check args"
 
-    '''
-    Get account information list
-    productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
-    :return:
-    '''
     def accounts(self, productType):
+        '''
+        ### Get account information list
+        productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
+        :return:
+        '''
         params = {}
         if productType:
             params['productType'] = productType
             return self._request_with_params(GET, MIX_ACCOUNT_V1_URL + '/accounts', params)
         else:
             return "pls check args"
 
-    '''
-    Obtain the list of account flow information
-    :return:
-    '''
     def accountBill(self, symbol,marginCoin,startTime,endTime,lastEndId = '',pageSize=20,next=False):
+        '''
+        ### Obtain the list of account flow information
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and startTime and endTime:
             params['symbol'] = symbol
             params['marginCoin'] = marginCoin
             params['startTime'] = startTime
             params['endTime'] = endTime
             params['lastEndId'] = lastEndId
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/mix/market_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/mix/market_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,173 +4,173 @@
 from ..consts import *
 
 
 class MarketApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Get contract list
-    productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
-    :return:
-    '''
     def contracts(self, productType):
+        '''
+        ### Get contract list
+        productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
+        :return:
+        '''
         params = {}
         if productType:
             params['productType'] = productType
         return self._request_with_params(GET, MIX_MARKET_V1_URL + '/contracts', params)
 
-    '''
-    Get depth data
-    symbol：Contract transaction pair
-    :return:
-    '''
     def depth(self, symbol, limit='150'):
+        '''
+        ### Get depth data
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol and limit and type:
             params["symbol"] = symbol
             params["limit"] = limit
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/depth', params)
         else:
             return "pls check args"
 
-    '''
-    Get ticker information according to the currency pair
-    symbol：Contract transaction pair
-    :return:
-    '''
     def ticker(self, symbol):
+        '''
+        ### Get ticker information according to the currency pair
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/ticker', params)
         else:
             return "pls check args"
 
-    '''
-    Get all ticket information
-    productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
-    :return:
-    '''
     def tickers(self,productType):
+        '''
+        ### Get all ticket information
+        productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
+        :return:
+        '''
         params = {}
         if productType:
             params['productType'] = productType
         return self._request_with_params(GET, MIX_MARKET_V1_URL + '/tickers', params)
 
-    '''
-    Get real-time transaction
-    symbol：Contract transaction pair
-    :return:
-    '''
     def fills(self, symbol, limit=100):
+        '''
+        ### Get real-time transaction
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol and limit:
             params["symbol"] = symbol
             params["limit"] = limit
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/fills', params)
         else:
             return "pls check args"
 
-    '''
-    Obtain K line information
-    params
-    period: 60, 300, 900, 1800, 3600,14400,43200, 86400, 604800
-    startTime: start time
-    endTime: end time
-    :return:
-    '''
     def candles(self, symbol, granularity, startTime='', endTime='',limit=''):
+        '''
+        ### Obtain K line information
+        params
+        period: 60, 300, 900, 1800, 3600,14400,43200, 86400, 604800
+        startTime: start time
+        endTime: end time
+        :return:
+        '''
         params = {}
         if symbol and granularity:
             params["symbol"] = symbol
             params["granularity"] = granularity
             params["startTime"] = startTime
             params["endTime"] = endTime
             params["limit"] = limit
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/candles', params)
         else:
             return "pls check args"
 
-    '''
-    Currency index price
-    symbol：Contract transaction pair
-    :return:
-    '''
     def index(self, symbol):
+        '''
+        ### Currency index price
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/index', params)
         else:
             return "pls check args"
 
-    '''
-    Next settlement time
-    symbol：Contract transaction pair
-    :return:
-    '''
     def funding_time(self, symbol):
+        '''
+        ### Next settlement time
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/funding-time', params)
         else:
             return "pls check args"
 
-    '''
-    Contract Mark Price
-    symbol：Contract transaction pair
-    :return:
-    '''
     def market_price(self, symbol):
+        '''
+        ### Contract Mark Price
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/mark-price', params)
         else:
             return "pls check args"
 
-    '''
-    Historical fund rate
-    symbol：Contract transaction pair
-    pageSize: Number of queries
-    pageNo: Number of query pages
-    nextPage: Whether to query the next page
-    :return:F
-    '''
     def history_fund_rate(self, symbol, pageSize=20, pageNo=1, nextPage=False):
+        '''
+        ### Historical fund rate
+        symbol：Contract transaction pair
+        pageSize: Number of queries
+        pageNo: Number of query pages
+        nextPage: Whether to query the next page
+        :return:F
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             params["nextPage"] = nextPage
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/history-fundRate', params)
         else:
             return "pls check args"
 
-    '''
-    Current fund rate
-    symbol：Contract transaction pair
-    :return:F
-    '''
     def current_fund_rate(self, symbol):
+        '''
+        ### Current fund rate
+        symbol：Contract transaction pair
+        :return:F
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/current-fundRate', params)
         else:
             return "pls check args"
 
-    '''
-    Obtain the total position of the platform
-    symbol：Contract transaction pair
-    :return:
-    '''
     def open_interest(self, symbol):
+        '''
+        ### Obtain the total position of the platform
+        symbol：Contract transaction pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/open-interest', params)
         else:
             return "pls check args"
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/mix/order_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/mix/order_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from ..consts import *
 
 
 class OrderApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    place an order
-    price: Mandatory in case of price limit
-    marginCoin: Deposit currency
-    size: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
-    side：open_long open_short close_long close_short
-    orderType: limit(fixed price)  market(market price)
-    timeInForceValue: normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
-    presetTakeProfitPrice: Default stop profit price
-    presetStopLossPrice：Preset stop loss price
-    :return:
-    '''
     def place_order(self, symbol, marginCoin, size, side, orderType, clientOrderId=None, price='', timeInForceValue='normal', presetTakeProfitPrice='', presetStopLossPrice=''):
+        '''
+        ### Place an order
+        price: Mandatory in case of price limit
+        marginCoin: Deposit currency
+        size: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
+        side：open_long open_short close_long close_short
+        orderType: limit(fixed price)  market(market price)
+        timeInForceValue: normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
+        presetTakeProfitPrice: Default stop profit price
+        presetStopLossPrice：Preset stop loss price
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and side and orderType and marginCoin:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["price"] = price
             params["size"] = size
             params["side"] = side
@@ -33,105 +33,105 @@
             params["clientOid"] = clientOrderId
             params["presetTakeProfitPrice"] = presetTakeProfitPrice
             params["presetStopLossPrice"] = presetStopLossPrice
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/placeOrder', params)
         else:
             return "pls check args "
 
-    '''
-    Place orders in batches
-    price: Mandatory in case of price limit
-    marginCoin: Deposit currency
-    order_data: 
-    size: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
-    side：open_long open_short close_long close_short
-    orderType: limit(fixed price)  market(market price)
-    timeInForceValue: normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
-    presetTakeProfitPrice: Default stop profit price
-    presetStopLossPrice： Preset stop loss price
-    :return:
-    '''
     def batch_orders(self, symbol, marginCoin, order_data):
+        '''
+        ### Place orders in batches
+        price: Mandatory in case of price limit
+        marginCoin: Deposit currency
+        order_data: 
+        size: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
+        side：open_long open_short close_long close_short
+        orderType: limit(fixed price)  market(market price)
+        timeInForceValue: normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
+        presetTakeProfitPrice: Default stop profit price
+        presetStopLossPrice： Preset stop loss price
+        :return:
+        '''
         params = {'symbol': symbol, 'marginCoin': marginCoin, 'orderDataList': order_data}
         return self._request_with_params(POST, MIX_ORDER_V1_URL + '/batch-orders', params)
 
-    '''
-    cancel the order
-    :return:
-    '''
     def cancel_orders(self, symbol, marginCoin, orderId):
+        '''
+        ### Cancel the order
+        :return:
+        '''
         params = {}
         if symbol and orderId:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["orderId"] = orderId
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/cancel-order', params)
         else:
             return "pls check args "
 
-    '''
-    Batch cancellation
-    orderIds: List 
-    :return:
-    '''
     def cancel_batch_orders(self, symbol, marginCoin, orderIds):
+        '''
+        ### Batch cancellation
+        orderIds: List 
+        :return:
+        '''
         if symbol and orderIds:
             params = {'symbol': symbol, 'marginCoin':marginCoin, 'orderIds': orderIds}
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/cancel-batch-orders', params)
         else:
             return "pls check args "
 
-    '''
-    Get order information
-    :return:
-    '''
     def detail(self, symbol, orderId):
+        '''
+        ### Get order information
+        :return:
+        '''
         params = {}
         if symbol and orderId:
             params["symbol"] = symbol
             params["orderId"] = orderId
             return self._request_with_params(GET, MIX_ORDER_V1_URL + '/detail', params)
         else:
             return "pls check args "
 
-    '''
-    Get the current order
-    :return:
-    '''
     def current(self, symbol):
+        '''
+        ### Get the current order
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, MIX_ORDER_V1_URL + '/current', params)
         else:
             return "pls check args "
 
-    '''
-    Get Historical Delegation
-    isPre： Whether to query the previous page
-    :return:
-    '''
     def history(self, symbol, startTime, endTime, pageSize, lastEndId='', isPre=False):
+        '''
+        ### Get Historical Delegation
+        isPre： Whether to query the previous page
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["startTime"] = startTime
             params["endTime"] = endTime
             params["pageSize"] = pageSize
             params["lastEndId"] = lastEndId
             params["isPre"] = isPre
             return self._request_with_params(GET, MIX_ORDER_V1_URL + '/history', params)
         else:
             return "pls check args "
 
-    '''
-    Obtain transaction details
-    :return:
-    '''
     def fills(self, symbol='', orderId=''):
+        '''
+        ### Obtain transaction details
+        :return:
+        '''
         params = {}
         if symbol and orderId:
             params["symbol"] = symbol
             params["orderId"] = orderId
             return self._request_with_params(GET, MIX_ORDER_V1_URL + '/fills', params)
         else:
             return "pls check args "
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/mix/plan_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/mix/plan_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 from ..consts import *
 
 
 class PlanApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Plan Entrusted Order
-    triggerPrice: Trigger Price
-    executePrice: Execution price
-    triggerType: Trigger Type fill_price market_price 
-    marginCoin: Deposit currency
-    size: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
-    side：open_long open_short close_long close_short
-    orderType: limit(fixed price)  market(market price)
-    timeInForceValue: normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
-    presetTakeProfitPrice: Default stop profit price
-    presetStopLossPrice： Preset stop loss price
-    :return:
-    '''
-
     def place_plan(self, symbol, marginCoin, size, side, orderType, triggerPrice, triggerType, executePrice='',
                    clientOrderId='', timeInForceValue='normal', presetTakeProfitPrice='', presetStopLossPrice=''):
+        '''
+        ### Plan Entrusted Order
+        triggerPrice: Trigger Price
+        executePrice: Execution price
+        triggerType: Trigger Type fill_price market_price 
+        marginCoin: Deposit currency
+        size: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
+        side：open_long open_short close_long close_short
+        orderType: limit(fixed price)  market(market price)
+        timeInForceValue: normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
+        presetTakeProfitPrice: Default stop profit price
+        presetStopLossPrice： Preset stop loss price
+        :return:
+        '''        
         params = {}
         if symbol and marginCoin and side and orderType and triggerPrice and triggerType:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["triggerPrice"] = triggerPrice
             params["executePrice"] = executePrice
             params["triggerType"] = triggerType
@@ -39,192 +38,184 @@
             params["clientOrderId"] = clientOrderId
             params["presetTakeProfitPrice"] = presetTakeProfitPrice
             params["presetStopLossPrice"] = presetStopLossPrice
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/placePlan', params)
         else:
             return "pls check args "
 
-    '''
-    Modify Plan Delegation
-    triggerPrice: Trigger Price
-    executePrice: Execution price
-    triggerType: Trigger Type fill_price market_price 
-    marginCoin: Deposit currency
-    orderType: limit(fixed price)  market(market price)
-    :return:
-    '''
-
     def modify_plan(self, symbol, marginCoin, orderId, orderType, triggerPrice, triggerType, executePrice=''):
+        '''
+        ### Modify Plan Delegation
+        triggerPrice: Trigger Price
+        executePrice: Execution price
+        triggerType: Trigger Type fill_price market_price 
+        marginCoin: Deposit currency
+        orderType: limit(fixed price)  market(market price)
+        :return:
+        '''        
         params = {}
         if symbol and marginCoin and orderType and orderId and triggerType:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["orderId"] = orderId
             params["triggerPrice"] = triggerPrice
             params["executePrice"] = executePrice
             params["triggerType"] = triggerType
             params["orderType"] = orderType
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/modifyPlan', params)
         else:
             return "pls check args "
 
-    '''
-    Modify the preset profit and loss stop of plan entrustment
-    orderId：orderId
-    triggerType: Trigger Type 
-    marginCoin: Deposit currency
-    planType: Plan delegation type normal_ Plan general plan_ Plan profit stop plan loss_ Plan stop loss plan
-    presetTakeProfitPrice: Default stop profit price
-    presetStopLossPrice： Preset stop loss price
-    :return:
-    '''
-
     def modify_plan_preset(self, symbol, marginCoin, orderId, planType='normal_plan', presetTakeProfitPrice='',
                            presetStopLossPrice=''):
+        '''
+        ### Modify the preset profit and loss stop of plan entrustment
+        orderId：orderId
+        triggerType: Trigger Type 
+        marginCoin: Deposit currency
+        planType: Plan delegation type normal_ Plan general plan_ Plan profit stop plan loss_ Plan stop loss plan
+        presetTakeProfitPrice: Default stop profit price
+        presetStopLossPrice： Preset stop loss price
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and orderId and planType:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["planType"] = planType
             params["orderId"] = orderId
             params["presetTakeProfitPrice"] = presetTakeProfitPrice
             params["presetStopLossPrice"] = presetStopLossPrice
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/modifyPlanPreset', params)
         else:
             return "pls check args "
 
-    '''
-    Modify the preset profit and loss stop of plan entrustment
-    orderId：orderId
-    triggerPrice: Trigger Price
-    marginCoin: Deposit currency
-    :return:
-    '''
-
     def modify_tpsl_plan(self, symbol, marginCoin, orderId, triggerPrice):
+        '''
+        ### Modify the preset profit and loss stop of plan entrustment
+        orderId：orderId
+        triggerPrice: Trigger Price
+        marginCoin: Deposit currency
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and orderId and triggerPrice:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["orderId"] = orderId
             params["triggerPrice"] = triggerPrice
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/modifyTPSLPlan', params)
         else:
             return "pls check args "
 
-    '''
-    Stop profit and stop loss Order
-    At present, only the market price trigger type is transaction price when placing an order with profit stop and loss stop
-    symbol: Trading pair name
-    marginCoin: Deposit currency
-    orderId: orderId
-    planType: Order type prof it_ Plan profit stop plan loss_ Plan stop loss plan
-    holdSide: Long long short short short position in position direction
-    :return:
-    '''
-
     def place_tpsl(self, symbol, marginCoin, triggerPrice, planType, holdSide):
+        '''
+        ### Stop profit and stop loss Order
+        At present, only the market price trigger type is transaction price when placing an order with profit stop and loss stop
+        symbol: Trading pair name
+        marginCoin: Deposit currency
+        orderId: orderId
+        planType: Order type prof it_ Plan profit stop plan loss_ Plan stop loss plan
+        holdSide: Long long short short short position in position direction
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and planType and holdSide and triggerPrice:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["planType"] = planType
             params["holdSide"] = holdSide
             params["triggerPrice"] = triggerPrice
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/placeTPSL', params)
         else:
             return "pls check args "
 
-    '''
-    place trail stop order
-    symbol
-    marginCoin
-    triggerPrice
-    triggerType
-    side
-    size
-    rangeRate: 
-    reduceOnly: only one-way mode
-    :return:
-    '''
     def place_trail_stop(self, params=None):
+        '''
+        ### Place trail stop order
+        symbol
+        marginCoin
+        triggerPrice
+        triggerType
+        side
+        size
+        rangeRate: 
+        reduceOnly: only one-way mode
+        :return:
+        '''
         if params is None:
             params = {}
         return self._request_with_params(POST, MIX_PLAN_V1_URL + '/placeTrailStop', params)
 
-    '''
-    place positions tpsl order
-    symbol
-    marginCoin
-    triggerPrice
-    triggerType
-    side
-    size
-    rangeRate: 
-    reduceOnly: only one-way mode
-    :return:
-    '''
     def place_positions_tpsl(self, params=None):
+        '''
+        ### Place positions tpsl order
+        symbol
+        marginCoin
+        triggerPrice
+        triggerType
+        side
+        size
+        rangeRate: 
+        reduceOnly: only one-way mode
+        :return:
+        '''
         if params is None:
             params = {}
         return self._request_with_params(POST, MIX_PLAN_V1_URL + '/placePositionsTPSL', params)
 
-
-    '''
-    cancel all trigger order
-    :return:
-    '''
     def cancel_all_plan(self, params=None):
+        '''
+        ### Cancel all trigger order
+        :return:
+        '''
         if params is None:
             params = {}
         return self._request_with_params(POST, MIX_PLAN_V1_URL + '/cancelAllPlan', params)
 
-    '''
-    Planned entrustment (profit and loss stop) cancellation
-    symbol: Trading pair name
-    marginCoin: Deposit currency
-    orderId: orderId 
-    planType: Order type normal_ Plan plan entrustment prof it_ Plan profit stop plan loss_ Plan stop loss plan
-    :return:
-    '''
-
     def cancel_plan(self, symbol, marginCoin, orderId, planType):
+        '''
+        ### Planned entrustment (profit and loss stop) cancellation
+        symbol: Trading pair name
+        marginCoin: Deposit currency
+        orderId: orderId 
+        planType: Order type normal_ Plan plan entrustment prof it_ Plan profit stop plan loss_ Plan stop loss plan
+        :return:
+        '''
         params = {}
         if symbol and marginCoin and planType and orderId:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             params["planType"] = planType
             params["orderId"] = orderId
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/cancelPlan', params)
         else:
             return "pls check args "
 
-    '''
-    Get the current plan delegation
-    isPlan: Query plan delegation plan delegation profile_ Loss Stop Profit Stop Loss
-    :return:
-    '''
-
     def current_plan(self, symbol, isPlan='plan'):
+        '''
+        ### Get the current plan delegation
+        isPlan: Query plan delegation plan delegation profile_ Loss Stop Profit Stop Loss
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["isPlan"] = isPlan
             return self._request_with_params(GET, MIX_PLAN_V1_URL + '/currentPlan', params)
         else:
             return "pls check args "
 
-    '''
-    Get historical plan delegation
-    isPre： Whether to query the previous page
-    isPlan: Query plan delegation plan delegation profile_ Loss Stop Profit Stop Loss
-    :return:
-    '''
-
     def history_plan(self, symbol, startTime, endTime, pageSize, lastEndId='', isPre=False, isPlan='plan'):
+        '''
+        ### Get historical plan delegation
+        isPre： Whether to query the previous page
+        isPlan: Query plan delegation plan delegation profile_ Loss Stop Profit Stop Loss
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["startTime"] = startTime
             params["endTime"] = endTime
             params["pageSize"] = pageSize
             params["lastEndId"] = lastEndId
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/mix/position_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/mix/position_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from ..consts import *
 
 
 class PositionApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Obtain the user's single position information
-    :return:
-    '''
     def single_position(self, symbol, marginCoin):
+        '''
+        ### Obtain the user's single position information
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
             return self._request_with_params(GET, MIX_POSITION_V1_URL + '/singlePosition', params)
         else:
             return "pls check args"
-
-    '''
-    Obtain all position information of the user
-    productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
-    :return:
-    '''
+        
     def all_position(self, productType, marginCoin):
+        '''
+        ### Obtain all position information of the user
+        productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
+        :return:
+        '''
         params = {}
         if productType:
             params["productType"] = productType
             params["marginCoin"] = marginCoin
             return self._request_with_params(GET, MIX_POSITION_V1_URL + '/allPosition', params)
         else:
             return "pls check args"
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/mix/trace_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/mix/trace_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,186 +4,173 @@
 from ..consts import *
 
 
 class TraceApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Dealers close positions
-    symbol： Trading pair name
-    trackingNo: Tracking order No
-    :return:
-    '''
-
     def close_track_order(self, symbol, trackingNo):
+        '''
+        ### Dealers close positions
+        symbol： Trading pair name
+        trackingNo: Tracking order No
+        :return:
+        '''
         params = {}
         if symbol and trackingNo:
             params["symbol"] = symbol
             params["trackingNo"] = trackingNo
             return self._request_with_params(POST, MIX_TRACE_V1_URL + '/closeTrackOrder', params)
         else:
             return "pls check args "
 
-    '''
-    The trader obtains the current order
-    symbol: Trading pair name
-    productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
-    pageNo： Start at 1
-    :return:
-    '''
-
     def current_track(self, symbol, productType, pageSize=20, pageNo=1):
+        '''
+        ### The trader obtains the current order
+        symbol: Trading pair name
+        productType: Umcbl (USDT professional contract) dmcbl (mixed contract) sumcbl (USDT professional contract simulation disk) sdmcbl (mixed contract simulation disk)
+        pageNo： Start at 1
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["productType"] = productType
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             return self._request_with_params(GET, MIX_TRACE_V1_URL + '/currentTrack', params)
         else:
             return "pls check args "
 
-    '''
-    The trader obtains the current order
-    symbol: Trading pair name
-    startTime: start time
-    endTime: end time
-    pageSize: Number of queries
-    pageNo: Number of query pages
-    :return:
-    '''
-
     def history_track(self, startTime, endTime, pageSize=100, pageNo=1):
+        '''
+        ### The trader obtains the current order
+        symbol: Trading pair name
+        startTime: start time
+        endTime: end time
+        pageSize: Number of queries
+        pageNo: Number of query pages
+        :return:
+        '''
         params = {}
         if startTime and endTime:
             params["startTime"] = startTime
             params["endTime"] = endTime
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             return self._request_with_params(GET, MIX_TRACE_V1_URL + '/historyTrack', params)
         else:
             return "pls check args "
 
-    '''
-    Summary of traders' profit sharing
-    :return:
-    '''
-
     def summary(self):
+        '''
+        ### Summary of traders' profit sharing
+        :return:
+        '''
         return self._request_without_params(GET, MIX_TRACE_V1_URL + '/summary')
 
-    '''
-    Summary of traders' profit sharing (by settlement currency)
-    :return:
-    '''
-
     def profit_settle_margin_coin(self):
+        '''
+        ### Summary of traders' profit sharing (by settlement currency)
+        :return:
+        '''
         return self._request_without_params(GET, MIX_TRACE_V1_URL + '/profitSettleTokenIdGroup')
 
-    '''
-    Summary of traders' profit sharing (by date)
-    :return:
-    '''
-
     def profit_date_group(self, pageSize, pageNo):
+        '''
+        ### Summary of traders' profit sharing (by date)
+        :return:
+        '''
         params = {}
         if pageSize and pageNo:
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             return self._request_with_params(GET, MIX_TRACE_V1_URL + '/profitDateGroupList', params)
         else:
             return "pls check args "
 
-    '''
-    Historical profit distribution details of traders
-    :return:
-    '''
-
     def profit_date_detail(self, marginCoin, date, pageSize, pageNo):
+        '''
+        ### Historical profit distribution details of traders
+        :return:
+        '''
         params = {}
         if marginCoin and date and pageSize and pageNo:
             params["marginCoin"] = marginCoin
             params["date"] = date
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             return self._request_with_params(GET, MIX_TRACE_V1_URL + '/profitDateList', params)
         else:
             return "pls check args "
 
-    '''
-    Details of traders to be distributed
-    :return:
-    '''
-
     def wait_profit_detail(self, pageSize, pageNo):
+        '''
+        ### Details of traders to be distributed
+        :return:
+        '''
         params = {}
         if pageSize and pageNo:
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             return self._request_with_params(GET, MIX_TRACE_V1_URL + '/waitProfitDateList', params)
         else:
             return "pls check args "
 
-    '''
-    Followers obtain information on opening and closing orders
-    :return:
-    '''
-
     def follower_history_orders(self, page_size, page_no, start_time, end_time):
+        '''
+        ### Followers obtain information on opening and closing orders
+        :return:
+        '''
         params = {}
         if page_size and page_no:
             params["pageSize"] = page_size
             params["pageNo"] = page_no
 
         if start_time and end_time:
             params["startTime"] = start_time
             params["endTime"] = end_time
 
         return self._request_with_params(GET, MIX_TRACE_V1_URL + '/followerHistoryOrders', params)
 
-    '''
-    get trader copytrader symbol
-    '''
-
     def trader_symbols(self):
+        '''
+        ### Get trader copytrader symbol
+        '''
         return self._request_without_params(GET, MIX_TRACE_V1_URL + '/traderSymbols')
 
-    '''
-    set trader copytrader symbol
-   '''
-
     def set_trder_symbol(self, symbol):
+        '''
+        ### Set trader copytrader symbol
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(POST, MIX_TRACE_V1_URL + '/setUpCopySymbols', params)
         else:
             return "pls check args "
 
-    '''
-      trader modify tpsl order
-    '''
-
     def trader_modify_tpsl_order(self, symbol, trackingNo, stopProfitPrice, stopLossPrice):
+        '''
+        ### Trader modify tpsl order
+        '''
         params = {}
         if symbol and trackingNo:
             params["symbol"] = symbol
             params["trackingNo"] = trackingNo
             params["stopProfitPrice"] = stopProfitPrice
             params["stopLossPrice"] = stopLossPrice
             return self._request_with_params(POST, MIX_TRACE_V1_URL + '/modifyTPSL', params)
         else:
             return "pls check args "
 
-    '''
-      followerOrder
-    '''
-
     def followerOrder(self, symbol, productType, pageSize=100, pageNo=1):
+        '''
+        ### FollowerOrder
+        '''
         params = {}
         if symbol and productType:
             params["symbol"] = symbol
             params["productType"] = productType
             params["pageSize"] = pageSize
             params["pageNo"] = pageNo
             return self._request_with_params(GET, MIX_TRACE_V1_URL + '/followerOrder', params)
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/spot/account_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/spot/account_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 from ..consts import *
 
 
 class AccountApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Obtain all asset currency information of the user
-    :return:
-    '''
+
     def assets(self, coin=''):
+        '''
+        ### Obtain all asset currency information of the user
+        :return:
+        '''
         params = {}
         if coin:
             params["coin"] = coin
         return self._request_with_params(GET, SPOT_ACCOUNT_V1_URL + '/assets-lite', params)
 
-    '''
-    Obtain all asset currency information of the user
-    
-    groupType: Deposit, withdraw, transaction, transfer, other
-    bizType：Dispose, withdraw, buy, sell, transfer in, transfer out
-    after: Pass in billId, the data before this billId
-    before: Incoming billId data after this billId
-    :return:
-    '''
     def bills(self, coinId='', groupType='', bizType='', after='', before='', limit=100):
+        '''
+        ### Obtain all asset currency information of the user
+        groupType: Deposit, withdraw, transaction, transfer, other
+        bizType：Disposit, withdraw, buy, sell, transfer in, transfer out
+        after: Pass in billId, the data before this billId
+        before: Incoming billId data after this billId
+        :return:
+        '''
         params = {}
 
         if coinId:
             params["coinId"] = coinId
         if groupType:
             params["groupType"] = groupType
         if bizType:
@@ -41,22 +41,20 @@
         if before:
             params["before"] = before
 
 
         params["limit"] = limit
         return self._request_with_params(POST, SPOT_ACCOUNT_V1_URL + '/bills', params)
 
-
-
-    '''
-    query transfer records
-    fromType: exchange(spot)   USD_MIX(coin future) USDT_MIX(usdt future)
-    :return:
-    '''
     def transfer_records(self, coinId='', fromType='', after='', before='', limit=100):
+        '''
+        ### Query transfer records
+        fromType: exchange(spot)   USD_MIX(coin future) USDT_MIX(usdt future)
+        :return:
+        '''
         params = {}
 
         if coinId:
             params["coinId"] = coinId
         if fromType:
             params["fromType"] = fromType
         if after:
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/spot/market_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/spot/market_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,73 +5,73 @@
 
 
 class MarketApi(Client):
 
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Get real-time transaction
-    :return:
-    '''
     def fills(self, symbol, limit=100):
+        '''
+        ### Get real-time transaction
+        :return:
+        '''
         params = {}
         if symbol and limit:
             params["symbol"] = symbol
             params["limit"] = limit
             return self._request_with_params(GET, SPOT_MARKET_V1_URL + '/fills', params)
         else:
             return "pls check args"
 
-    '''
-    Get depth data
-    Depth Merge Type
-    type: step0(default) step1 step2 step3 step4 step5
-    :return:
-    '''
     def depth(self, symbol, limit='150', type='step0'):
+        '''
+        ### Get depth data
+        Depth Merge Type
+        type: step0(default) step1 step2 step3 step4 step5
+        :return:
+        '''
         params = {}
         if symbol and limit and type:
             params["symbol"] = symbol
             params["limit"] = limit
             params["type"] = type
             return self._request_with_params(GET, SPOT_MARKET_V1_URL + '/depth', params)
         else:
             return "pls check args"
 
-    '''
-    Get ticker information according to the currency pair
-    :return:
-    '''
     def ticker(self, symbol):
+        '''
+        ### Get ticker information according to the currency pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, SPOT_MARKET_V1_URL + '/ticker', params)
         else:
             return "pls check args"
 
-    '''
-    Get all transaction pair ticker information
-    :return:
-    '''
-    def tickers(self):
 
+    def tickers(self):
+        '''
+        ### Get all transaction pair ticker information
+        :return:
+        '''
         return self._request_without_params(GET, SPOT_MARKET_V1_URL + '/tickers')
 
-    '''
-    Obtain K line information
-    params
-    
-    period: 1min, 5min, 15min, 30min, 1h,4h,12h, 1day, 1week
-    after: time before
-    before: time after
-    :return:
-    '''
     def candles(self, symbol, period, after='', before='', limit=100):
+        '''
+        ### Obtain K line information
+        params
+        
+        period: 1min, 5min, 15min, 30min, 1h,4h,12h, 1day, 1week
+        after: time before
+        before: time after
+        :return:
+        '''
         params = {}
         if symbol and period:
             params["symbol"] = symbol
             params["period"] = period
             params["after"] = after
             params["before"] = before
             params["limit"] = limit
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/spot/order_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/spot/order_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,123 +3,123 @@
 from ..consts import *
 
 
 class OrderApi(Client):
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    place an order
-    price: Mandatory in case of price limit
-    quantity: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
-    side：buy sell
-    orderType: limit(fixed price)  market(market price)
-    force:normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
-    :return:
-    '''
     def orders(self, symbol, quantity, side, orderType, force, price='', clientOrderId=''):
+        '''
+        ### Place an order
+        price: Mandatory in case of price limit
+        quantity: It is quantity when the price is limited. The market price is the limit. The sales is the quantity
+        side：buy sell
+        orderType: limit(fixed price)  market(market price)
+        force:normal(Ordinary price limit order)   postOnly(It is only a maker. The market price is not allowed to use this)  ioc(Close immediately and cancel the remaining)  fok(Complete transaction or immediate cancellation)
+        :return:
+        '''
         params = {}
 
         if symbol and quantity and side and orderType and force:
             params["symbol"] = symbol
             params["price"] = price
             params["quantity"] = quantity
             params["side"] = side
             params["orderType"] = orderType
             params["force"] = force
             params["clientOrderId"] = clientOrderId
             return self._request_with_params(POST, SPOT_ORDER_V1_URL + '/orders', params)
         else:
             return "pls check args "
 
-    '''
-    Place orders in batches
-    '''
     def batch_orders(self, symbol, order_data):
+        '''
+        ### Place orders in batches
+        '''
         params = {'symbol': symbol, 'orderList': order_data}
         return self._request_with_params(POST, SPOT_ORDER_V1_URL + "/batch-orders", params)
 
-    '''
-    cancel the order
-    :return:
-    '''
     def cancel_orders(self, symbol, orderId):
+        '''
+        ### Cancel the order
+        :return:
+        '''
         params = {}
         if symbol and orderId:
             params["symbol"] = symbol
             params["orderId"] = orderId
             return self._request_with_params(POST, SPOT_ORDER_V1_URL + '/cancel-order', params)
         else:
             return "pls check args "
 
-    '''
-    Batch cancellation
-    orderIds: List 
-    :return:
-    '''
     def cancel_batch_orders(self, symbol, orderIds):
+        '''
+        ### Batch cancellation
+        orderIds: List 
+        :return:
+        '''
         if symbol and orderIds:
             params = {'symbol': symbol, 'orderIds': orderIds}
             return self._request_with_params(POST, SPOT_ORDER_V1_URL + '/cancel-batch-orders', params)
         else:
             return "pls check args "
 
-    '''
-    Get order information
-    :return:
-    '''
     def order_info(self, symbol, orderId='', clientOrderId=''):
+        '''
+        ### Get order information
+        :return:
+        '''
         params = {}
         if clientOrderId:
             params["clientOrderId"] = clientOrderId
         if symbol:
             params["symbol"] = symbol
 
         if orderId:
             params["orderId"] = orderId
             return self._request_with_params(POST, SPOT_ORDER_V1_URL + '/orderInfo', params)
         else:
             return "pls check args "
 
-    '''
-    Get the current order
-    :return:
-    '''
     def open_order(self, symbol):
+        '''
+        ### Get the current order
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(POST, SPOT_ORDER_V1_URL + '/open-orders', params)
         else:
             return "pls check args "
 
-    '''
-    Get Historical Delegation
-    after: The orderId is passed in. The data before the orderId desc
-    before: Pass in the data after the orderId asc
-    :return:
-    '''
     def history(self, symbol, after='', before='', limit=100):
+        '''
+        ### Get Historical Delegation
+        after: The orderId is passed in. The data before the orderId desc
+        before: Pass in the data after the orderId asc
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             params["after"] = after
             params["before"] = before
             params["limit"] = limit
             return self._request_with_params(POST, SPOT_ORDER_V1_URL + '/history', params)
         else:
             return "pls check args "
 
-    '''
-    Obtain transaction details
-    after: Only the data before the fillId can be passed in
-    before: Only data passing in the fillId after this fillId is supported
-    :return:
-    '''
     def fills(self, symbol='', orderId='', after='', before='', limit=100):
+        '''
+        ### Obtain transaction details
+        after: Only the data before the fillId can be passed in
+        before: Only data passing in the fillId after this fillId is supported
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
         if orderId:
             params["orderId"] = orderId
         if after:
             params["after"] = after
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/spot/plan_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/spot/plan_api.py`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/spot/public_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/spot/public_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,42 +5,40 @@
 
 
 class PublicApi(Client):
 
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    Get Timestamp
-    :return:
-    '''
     def times(self):
+        '''
+        ### Get Timestamp
+        :return:
+        '''
         return self._request_without_params(GET, SPOT_PUBLIC_V1_URL + '/time')
 
-    '''
-    Get all currencies
-    :return:
-    '''
     def currencies(self):
-
+        '''
+        ### Get all currencies
+        :return:
+        '''
         return self._request_without_params(GET, SPOT_PUBLIC_V1_URL + '/currencies')
 
-    '''
-    Get all transaction pair information
-    :return:
-    '''
     def products(self):
-
+        '''
+        ### Get all transaction pair information
+        :return:
+        '''
         return self._request_without_params(GET, SPOT_PUBLIC_V1_URL+'/products')
 
-    '''
-    Obtain single currency pair information according to the transaction pair
-    :return:
-    '''
     def product(self, symbol):
+        '''
+        ### Obtain single currency pair information according to the transaction pair
+        :return:
+        '''
         params = {}
         if symbol:
             params["symbol"] = symbol
             return self._request_with_params(GET, SPOT_PUBLIC_V1_URL+'/product', params)
         else:
             return "pls check args"
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/spot/wallet_api.py` & `bitget-python-connector-0.0.6/bitget_python_connector/spot/wallet_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,61 +5,61 @@
 
 
 class WalletApi(Client):
 
     def __init__(self, api_key, api_secret_key, passphrase, use_server_time=False, first=False):
         Client.__init__(self, api_key, api_secret_key, passphrase, use_server_time, first)
 
-    '''
-    inner transfer 
-    fromType： spot, mix_usdt, mix_usd
-    toType: spot, mix_usdt, mix_usd
-    amount: transfer amount
-    coin: crypto currency
-   :return:
-    '''
     def transfer(self, fromType, toType, amount, coin):
+        '''
+        ### Inner transfer 
+        fromType： spot, mix_usdt, mix_usd
+        toType: spot, mix_usdt, mix_usd
+        amount: transfer amount
+        coin: crypto currency
+        :return:
+        '''
         params = {}
         if fromType and toType and amount and coin :
             params["fromType"] = fromType
             params["toType"] = toType
             params["amount"] = amount
             params["coin"] = coin
             return self._request_with_params(POST, SPOT_WALLET_V1_URL + '/transfer', params)
         else:
             return "pls check args "
 
-    '''
-    GET deposit address
-    coin： btc usdt
-    chain: trc20  erc20
-    :return:
-    '''
     def depositAddress(self, coin, chain):
+        '''
+        ### GET deposit address
+        coin： btc usdt
+        chain: trc20  erc20
+        :return:
+        '''
         params = {}
         if coin:
             params["coin"] = coin
             params["chain"] = chain
             return self._request_with_params(GET, SPOT_WALLET_V1_URL + '/deposit-address', params)
         else:
             return "pls check args "
 
-    '''
-    withdrawal
-    coin： btc usdt
-    address: withdrawal address
-    tag: exit? 
-    chain: trc20  erc20
-    amount: withdrawal amount
-    ip: required 
-    remark: 
-    clientOid:
-    :return:
-    '''
     def withdrawal(self, coin, address, chain, amount, remark, clientOid=None,tag=None):
+        '''
+        ### Withdrawal
+        coin： btc usdt
+        address: withdrawal address
+        tag: exit? 
+        chain: trc20  erc20
+        amount: withdrawal amount
+        ip: required 
+        remark: 
+        clientOid:
+        :return:
+        '''
         params = {}
         if coin:
             params["coin"] = coin
             params["address"] = address
 
             params["chain"] = chain
             params["amount"] = amount
@@ -68,56 +68,56 @@
                 params["tag"] = tag
             if clientOid:
                 params["clientOid"] = clientOid
             return self._request_with_params(POST, SPOT_WALLET_V1_URL + '/withdrawal', params)
         else:
             return "pls check args "
 
-    '''
-    withdrawalInner
-    coin： btc usdt
-    toUid: 
-    amount: withdrawal amount
-    ip: required 
-    clientOid:
-    :return:
-    '''
     def withdrawalInner(self, coin, toUid, amount, clientOid):
+        '''
+        ### WithdrawalInner
+        coin： btc usdt
+        toUid: 
+        amount: withdrawal amount
+        ip: required 
+        clientOid:
+        :return:
+        '''
         params = {}
         if coin:
             params["coin"] = coin
             params["toUid"] = toUid
             params["amount"] = amount
             if clientOid:
                 params["clientOid"] = clientOid
             return self._request_with_params(POST, SPOT_WALLET_V1_URL + '/withdrawal-inner', params)
         else:
             return "pls check args "
 
-    '''
-    withdrawal list
-    :return:
-    '''
     def withdrawalList(self, coin, startTime, endTime, pageNo='1', pageSize='20'):
+        '''
+        ### Withdrawal list
+        :return:
+        '''
         params = {}
         if coin:
             params["coin"] = coin
             params["startTime"] = startTime
             params["endTime"] = endTime
             params["pageNo"] = pageNo
             params["pageSize"] = pageSize
             return self._request_with_params(GET, SPOT_WALLET_V1_URL + '/withdrawal-list', params)
         else:
             return "pls check args "
 
-    '''
-    deposit list
-    :return:
-    '''
     def depositList(self, coin, startTime, endTime, pageNo='1', pageSize='20'):
+        '''
+        ### Deposit list
+        :return:
+        '''
         params = {}
         if coin:
             params["coin"] = coin
             params["startTime"] = startTime
             params["endTime"] = endTime
             params["pageNo"] = pageNo
             params["pageSize"] = pageSize
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/utils.py` & `bitget-python-connector-0.0.6/bitget_python_connector/utils.py`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector/ws/bitget_ws_client.py` & `bitget-python-connector-0.0.6/bitget_python_connector/ws/bitget_ws_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import time
 import traceback
 from threading import Timer
 from zlib import crc32
 
 import websocket
 
-from bitget.consts import GET, REQUEST_PATH
-from bitget.ws.utils import sign_utils
+from bitget_python_connector.consts import GET, REQUEST_PATH
+from bitget_python_connector.ws.utils import sign_utils
 
 WS_OP_LOGIN = 'login'
 WS_OP_SUBSCRIBE = "subscribe"
 WS_OP_UNSUBSCRIBE = "unsubscribe"
 
 
 def handle(message):
```

### Comparing `bitget-python-connector-0.0.5/bitget_python_connector.egg-info/SOURCES.txt` & `bitget-python-connector-0.0.6/bitget_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.5/pyproject.toml` & `bitget-python-connector-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitget-python-connector"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Cheng, Chuan-Yi", email="parker178912.en08@nycu.edu.tw" },
 ]
 description = "A tool to easily connect to bitget api."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

