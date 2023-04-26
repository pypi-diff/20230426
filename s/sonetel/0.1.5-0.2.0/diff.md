# Comparing `tmp/sonetel-0.1.5.tar.gz` & `tmp/sonetel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonetel-0.1.5.tar", last modified: Fri Aug 12 04:39:55 2022, max compression
+gzip compressed data, was "sonetel-0.2.0.tar", last modified: Wed Apr 26 12:39:07 2023, max compression
```

## Comparing `sonetel-0.1.5.tar` & `sonetel-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-08-12 04:39:55.339630 sonetel-0.1.5/
--rw-rw-rw-   0        0        0     1096 2022-07-25 10:32:18.000000 sonetel-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     7169 2022-08-12 04:39:55.339630 sonetel-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6531 2022-07-26 04:12:36.000000 sonetel-0.1.5/README.md
--rw-rw-rw-   0        0        0      154 2022-07-25 10:32:18.000000 sonetel-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      826 2022-08-12 04:39:55.344631 sonetel-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-12 04:39:55.285630 sonetel-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2022-08-12 04:39:55.311629 sonetel-0.1.5/src/sonetel/
--rw-rw-rw-   0        0        0       26 2022-07-25 10:32:18.000000 sonetel-0.1.5/src/sonetel/__init__.py
--rw-rw-rw-   0        0        0    12333 2022-08-12 04:34:05.000000 sonetel-0.1.5/src/sonetel/api.py
-drwxrwxrwx   0        0        0        0 2022-08-12 04:39:55.335632 sonetel-0.1.5/src/sonetel.egg-info/
--rw-rw-rw-   0        0        0     7169 2022-08-12 04:39:55.000000 sonetel-0.1.5/src/sonetel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2022-08-12 04:39:55.000000 sonetel-0.1.5/src/sonetel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-12 04:39:55.000000 sonetel-0.1.5/src/sonetel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-08-12 04:39:55.000000 sonetel-0.1.5/src/sonetel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-12 04:39:55.000000 sonetel-0.1.5/src/sonetel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 12:39:07.019193 sonetel-0.2.0/
+-rw-rw-rw-   0        0        0     1096 2023-04-26 12:20:53.000000 sonetel-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     8458 2023-04-26 12:39:07.020194 sonetel-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7532 2023-04-26 12:14:14.000000 sonetel-0.2.0/README.md
+-rw-rw-rw-   0        0        0      154 2022-08-31 06:56:53.000000 sonetel-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1000 2023-04-26 12:39:07.022192 sonetel-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      329 2022-09-12 10:27:57.000000 sonetel-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:39:06.995193 sonetel-0.2.0/sonetel/
+-rw-rw-rw-   0        0        0      197 2022-09-12 09:51:10.000000 sonetel-0.2.0/sonetel/__init__.py
+-rw-rw-rw-   0        0        0     1158 2023-04-26 09:51:09.000000 sonetel-0.2.0/sonetel/_constants.py
+-rw-rw-rw-   0        0        0     2928 2023-04-23 05:14:17.000000 sonetel-0.2.0/sonetel/account.py
+-rw-rw-rw-   0        0        0     4718 2023-04-26 11:50:52.000000 sonetel-0.2.0/sonetel/auth.py
+-rw-rw-rw-   0        0        0     3379 2023-04-26 09:14:29.000000 sonetel-0.2.0/sonetel/calls.py
+-rw-rw-rw-   0        0        0      674 2022-09-09 02:17:51.000000 sonetel-0.2.0/sonetel/exceptions.py
+-rw-rw-rw-   0        0        0     6098 2023-04-23 05:39:34.000000 sonetel-0.2.0/sonetel/phonenumber.py
+-rw-rw-rw-   0        0        0     2602 2023-04-23 05:44:46.000000 sonetel-0.2.0/sonetel/recording.py
+-rw-rw-rw-   0        0        0     3856 2023-04-26 03:06:09.000000 sonetel-0.2.0/sonetel/users.py
+-rw-rw-rw-   0        0        0     4022 2023-04-26 09:36:28.000000 sonetel-0.2.0/sonetel/utilities.py
+-rw-rw-rw-   0        0        0      973 2023-04-26 12:06:42.000000 sonetel-0.2.0/sonetel/voiceapps.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:39:07.015195 sonetel-0.2.0/sonetel.egg-info/
+-rw-rw-rw-   0        0        0     8458 2023-04-26 12:39:06.000000 sonetel-0.2.0/sonetel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-26 12:39:06.000000 sonetel-0.2.0/sonetel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 12:39:06.000000 sonetel-0.2.0/sonetel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-26 12:39:06.000000 sonetel-0.2.0/sonetel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 12:39:06.000000 sonetel-0.2.0/sonetel.egg-info/top_level.txt
```

### Comparing `sonetel-0.1.5/LICENSE` & `sonetel-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Sonetel AB (publ)
+Copyright (c) 2023 Sonetel AB (publ)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sonetel-0.1.5/PKG-INFO` & `sonetel-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,204 +1,246 @@
 Metadata-Version: 2.1
 Name: sonetel
-Version: 0.1.5
-Summary: A simple Python wrapper for Sonetel REST APIs.
+Version: 0.2.0
+Summary: A simple python wrapper for using Sonetel's REST APIs
 Home-page: https://github.com/Sonetel/sonetel-python
-Author: Aashish
+Author: aashish
 Author-email: dev.support@sonetel.com
+License: MIT
 Project-URL: Bug Tracker, https://github.com/Sonetel/sonetel-python/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Telephony
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <br />
 <div align="center">
   <a href="https://github.com/Sonetel/sonetel-python">
     <img src="https://dl.dropboxusercontent.com/s/hn4o0v378od1aoo/logo_white_background.png" alt="Logo" width="80" height="80">
   </a>
 
-<h3 align="center">Sonetel API Python Wrapper</h3>
+<h3 align="center">Sonetel Python SDK</h3>
 
 <p align="center">
-    A simple Python wrapper for using Sonetel's REST API endpoints.
+    Python package for using Sonetel's REST API endpoints.
     <br />
     <br />
     <a href="https://sonetel.com/en/developer/">Sonetel Developer Home</a>
     .
     <a href="https://sonetel.com/en/developer/api-documentation/">API Documentation</a>
     .
     <a href="https://app.sonetel.com/register?tag=api-developer&simple=true">Get Free Account</a>
   </p>
 </div>
 
-## Introduction
+## 1. Introduction
 The Sonetel API is a REST based web-service that enables you to manage your Sonetel account from your own platform or service. You can manage your account, your phone numbers and make callback calls etc.
 
-This is a simple python wrapper to use Sonetel's communication APIs. For more information about the API, please see the [documentation](https://docs.sonetel.com/).
+This Python package provides an easy-to-use interface to integrate Sonetel's APIs with your service. For more information about the API, please see the [documentation](https://docs.sonetel.com/).
 
-## Getting Started
+## 2. Get Started
 
-To use the module, you need a Sonetel account. If you don't already have one, get a free account from <a href="https://app.sonetel.com/register?tag=api-developer&simple=true">sonetel.com</a>.
+To use the package, you need a Sonetel account. If you don't already have one, get a free account from <a href="https://app.sonetel.com/register?tag=api-developer&simple=true">sonetel.com</a>.
 
-### Installation
+### 2.1 Installation
 
-#### PIP
-Run the following command to install from pip.
+#### 2.1.1 PIP
+
+This is the recommended way to install the module. It installs the latest stable version from the Python Package Index.
 
 `pip install sonetel`
 
-#### Git
-To get the latest features, clone a specific [tag](https://github.com/Sonetel/sonetel-python/tags) and [follow these instructions](https://packaging.python.org/en/latest/tutorials/packaging-projects/) to build the module locally.
+#### 2.1.2 Git
+
+To get the latest features, clone [the repository](https://github.com/Sonetel/sonetel-python) and [follow these instructions](https://packaging.python.org/en/latest/tutorials/packaging-projects/) to build the SDK locally.
+
+### 2.2 Usage
 
-## Functions
+To use the package, add the following line to the top of your Python program.
 
-The following functions are support at the moment. More will be added in the future.
+`import sonetel`
 
-- `get_balance()` - Get the prepaid balance of the account (e.g. '10'). Pass the argument `currency=True` to get the balance with the currency appended (e.g. '10 USD')
-- `get_token()` - Get the access token being used.
-- `get_accountid()` - Returns your Sonetel account ID.
-- `get_username()` - Returns the email address of the user that was used to create the token.
-- `get_voiceapps()` - get a list of all the voice apps in the account.
-- `get_refreshtoken()` - get the refresh token used to regenerate the access token when it expires.
-- `account_info()` - Fetch information about your account such as company name, balance, country, timezone, daily limit and so on.
-- `account_users()` - Details of all the users in your account.
-- `callback()` - Use our Callback API to make a callback call.
-- `create_token()` - Create a new access token. A new access token is automatically created when you call the Account resource the first time.
-- `subscription_buynum()` - Purchase a phone number. Requires a phone number to be passed. Use the `/availablephonenumber` API endpoint to see a list of phone numbers available for purchase from a country and area.
-- `subscription_listnums()` - See the details of all the phone numbers purchased by you. Pass the parameter `e164only=True` to only get a list of E.164 numbers without any metadata.
+Here's a description of the various modules and the methods available with each.
+#### 2.2.1 Auth
 
-## Examples
+The Auth module is used to generate and manage access tokens.
 
-### 1. Create an access token
+To instantiate it, you need to pass your Sonetel username and password to it. It supports the following methods:
+
+1. `create_token()` - create a new access token. Called automatically when a new instance is created.
+2. `get_access_token()` - fetch the current access token.
+3. `get_refresh_token()` - get the refresh token, used to refresh the access token.
+4. `get_decoded_token()` - return the decoded JWT value. Returns a dict.
+
+##### Generate an access token
 
 ```python
 import os
-from sonetel import api
+import sonetel as sntl
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sntl.Auth(username=user, password=pswd)
 
-print(s.get_token())
+print(s.get_access_token())
 ```
 
-### 2. Print your Sonetel account ID and the current prepaid balance. 
+#####  Refresh access token
+
+When your access token has expired, you can use the `create_token()` method to get a new `access_token` & `refresh_token`.
+
+This automatically updates the Account object to use the newly generated access and refresh tokens.
 
 ```python
 import os
-from sonetel import api
+import sonetel as sntl
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sntl.Auth(username=user, password=pswd)
 
-print(f"Your account ID is {s.get_accountid()} and your prepaid balance is {s.get_balance()}.")
+print(s.get_access_token())
+
+# Generate the refresh token and update the Account object
+response = s.create_token(refresh="yes", grant_type="refresh_token")
+
+print(response)
 ```
 
-### 3. List the phone numbers available in your account
+##### Get decoded JWT token
+
+Get the decoded JWT token.
 
 ```python
 import os
-from sonetel import api
+import sonetel as sntl
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sntl.Auth(username=user, password=pswd)
+
+print(s.get_decoded_token())
 
-print(s.subscription_listnums(e164only=True))
 ```
 
-### 4. Make a callback call
+#### 2.2.2 Account
 
-When making a callback call, `num1` is the destination where you will first answer the call before we call `num2`. This can be your mobile number, a SIP address or your Sonetel email address. 
+The Account module provides you information about your Sonetel account. For example, the prepaid balance, address and so on.
 
-If you set `num1` as your Sonetel email address, then the call will be handled as per your incoming call settings.
+It supports the following methods:
+
+1. `get()` - Get information about the account. Return a dict with an overview of the information such as account ID, currency, prepaid balance, country and so on.
+2. `update()` - Update basic information about your account.
+3. `get_balance()` - Returns the prepaid balance. Pass the parameter `currency` = `True` to include the currency with the returned value.
+4. `get_accountid()` - Fetch the account ID.
+
+##### Print your Sonetel account ID and the current prepaid balance. 
 
 ```python
 import os
-from sonetel import api
+from sonetel import Auth
+from sonetel import Account
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = Auth(username=user,password=pswd)
 
-result = s.callback(
-    num1="YOUR_NUMBER_OR_ADDRESS",
-    num2="NUMBER_TO_CALL",
-)
-print(result)
+a = Account(s.get_access_token())
+
+print(f"Your account ID is {a.get_accountid()} and your prepaid balance is {a.get_balance()}.")
 ```
 
-### 5. Refresh access token
+#### 2.2.3 Call
 
-When your access token has expired, you can use the `create_token()` method to get a new `access_token` & `refresh_token`.
+Use this to make callback calls with your Sonetel account.
 
-This automatically updates the Account object to use the newly generated access and refresh tokens.
+It supports the `callback()` method which requires your mobile number and the number of the person you wish to speak to. In a callback call, our system will first call you and when you answer, call the other number you provided. When the second call has been answered successfully, the calls will be connected together.
+
+##### Make a callback call
+
+When making a callback call, `num1` is the destination where you will first answer the call before we call `num2`. This can be your mobile number, a SIP address or your Sonetel email address. 
+
+If you set `num1` as your Sonetel email address, then the call will be handled as per your incoming call settings.
 
 ```python
 import os
-from sonetel import api
+import sonetel
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
-
-print(s.get_token())
+s = sonetel.Auth(username=user,password=pswd)
 
-# Generate the refresh token and update the Account object
-response = s.create_token(refresh="yes", grant_type="refresh_token")
+c = sonetel.Call(s.get_access_token())
 
-print(response)
+result = c.callback(
+    num1="YOUR_NUMBER_OR_ADDRESS",
+    num2="NUMBER_TO_CALL",
+)
+print(result)
 ```
 
-### 6. Get decoded JWT token
+#### 2.2.4 Phone Number
 
-Get the decoded JWT token.
+The `Phonenumber` module allows you to manage phone numbers in your Sonetel account.
+
+It supports the following methods:
+
+1. `get()` - get a list of phone numbers in your account. By default only returns a list of the E164 numbers. Set the parameter `e164only` equal to `False` to get detailed information.
+2. `add()` - buy a new phone number.
+3. `update()` - update the call forwarding settings for a phone number.
+4. `delete()` - remove a phone number from your Sonetel account.
+
+##### List the phone numbers available in your account
 
 ```python
 import os
-from sonetel import api
+import sonetel
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sonetel.Auth(username=user,password=pswd)
 
-print(s.get_decodedtoken())
+ph = sonetel.PhoneNumber(s.get_access_token())
+print(ph.get())
 
 ```
 
 ## Storing your credentials
 
-Please keep your credentials safe to avoid any misuse of your account. Do not hard code them into scripts or save them in files that are saved in any form of version control.
+Please keep your Sonetel login credentials safe to avoid any misuse of your account. Do not hard code them into scripts or save them in files that are saved in any form of version control.
 
 You can add them to your operating system's environment variables and use Python's `os` module to fetch them.
 
-Assuming the username and password are stored in environment variables named `sonetelUserName` and `sonetelPassword` respectively, here's how you can access them from a script:
+Assuming the username and password are stored in environment variables named `sonetelUsername` and `sonetelPassword` respectively, here's how you can access them from a script:
 
 ```python
 import os
-from sonetel import api
+import sonetel
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sonetel.Auth(username=user,password=pswd)
 
-print(s.get_accountid())
+print(s.get_access_token())
 ```
 
 ## Help
 
 For help with the Sonetel API, have a look at the <a href="https://docs.sonetel.com">API documentation</a>.
 
 If you have an issue with the module, please [report an issue](https://github.com/Sonetel/sonetel-python/issues/issues) on GitHub.
```

#### html2text {}

```diff
@@ -1,86 +1,103 @@
-Metadata-Version: 2.1 Name: sonetel Version: 0.1.5 Summary: A simple Python
-wrapper for Sonetel REST APIs. Home-page: https://github.com/Sonetel/sonetel-
-python Author: Aashish Author-email: dev.support@sonetel.com Project-URL: Bug
-Tracker, https://github.com/Sonetel/sonetel-python/issues Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: OS
-Independent Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Telecommunications
-Industry Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: sonetel Version: 0.2.0 Summary: A simple python
+wrapper for using Sonetel's REST APIs Home-page: https://github.com/Sonetel/
+sonetel-python Author: aashish Author-email: dev.support@sonetel.com License:
+MIT Project-URL: Bug Tracker, https://github.com/Sonetel/sonetel-python/issues
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Telecommunications Industry Classifier: Topic
+:: Communications Classifier: Topic :: Communications :: Telephony Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Classifier:
+License :: OSI Approved :: MIT License Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
-                     **** Sonetel API Python Wrapper ****
-       A simple Python wrapper for using Sonetel's REST API endpoints.
+                         **** Sonetel Python SDK ****
+            Python package for using Sonetel's REST API endpoints.
 
          Sonetel_Developer_Home . API_Documentation . Get_Free_Account
-## Introduction The Sonetel API is a REST based web-service that enables you to
-manage your Sonetel account from your own platform or service. You can manage
-your account, your phone numbers and make callback calls etc. This is a simple
-python wrapper to use Sonetel's communication APIs. For more information about
-the API, please see the [documentation](https://docs.sonetel.com/). ## Getting
-Started To use the module, you need a Sonetel account. If you don't already
-have one, get a free account from sonetel.com. ### Installation #### PIP Run
-the following command to install from pip. `pip install sonetel` #### Git To
-get the latest features, clone a specific [tag](https://github.com/Sonetel/
-sonetel-python/tags) and [follow these instructions](https://
-packaging.python.org/en/latest/tutorials/packaging-projects/) to build the
-module locally. ## Functions The following functions are support at the moment.
-More will be added in the future. - `get_balance()` - Get the prepaid balance
-of the account (e.g. '10'). Pass the argument `currency=True` to get the
-balance with the currency appended (e.g. '10 USD') - `get_token()` - Get the
-access token being used. - `get_accountid()` - Returns your Sonetel account ID.
-- `get_username()` - Returns the email address of the user that was used to
-create the token. - `get_voiceapps()` - get a list of all the voice apps in the
-account. - `get_refreshtoken()` - get the refresh token used to regenerate the
-access token when it expires. - `account_info()` - Fetch information about your
-account such as company name, balance, country, timezone, daily limit and so
-on. - `account_users()` - Details of all the users in your account. - `callback
-()` - Use our Callback API to make a callback call. - `create_token()` - Create
-a new access token. A new access token is automatically created when you call
-the Account resource the first time. - `subscription_buynum()` - Purchase a
-phone number. Requires a phone number to be passed. Use the `/
-availablephonenumber` API endpoint to see a list of phone numbers available for
-purchase from a country and area. - `subscription_listnums()` - See the details
-of all the phone numbers purchased by you. Pass the parameter `e164only=True`
-to only get a list of E.164 numbers without any metadata. ## Examples ### 1.
-Create an access token ```python import os from sonetel import api user =
-os.environ.get('sonetelUserName') pswd = os.environ.get('sonetelPassword') s =
-api.Account(username=user,password=pswd) print(s.get_token()) ``` ### 2. Print
-your Sonetel account ID and the current prepaid balance. ```python import os
-from sonetel import api user = os.environ.get('sonetelUserName') pswd =
-os.environ.get('sonetelPassword') s = api.Account(username=user,password=pswd)
-print(f"Your account ID is {s.get_accountid()} and your prepaid balance is
-{s.get_balance()}.") ``` ### 3. List the phone numbers available in your
-account ```python import os from sonetel import api user = os.environ.get
-('sonetelUserName') pswd = os.environ.get('sonetelPassword') s = api.Account
-(username=user,password=pswd) print(s.subscription_listnums(e164only=True)) ```
-### 4. Make a callback call When making a callback call, `num1` is the
-destination where you will first answer the call before we call `num2`. This
-can be your mobile number, a SIP address or your Sonetel email address. If you
-set `num1` as your Sonetel email address, then the call will be handled as per
-your incoming call settings. ```python import os from sonetel import api user =
-os.environ.get('sonetelUserName') pswd = os.environ.get('sonetelPassword') s =
-api.Account(username=user,password=pswd) result = s.callback
-( num1="YOUR_NUMBER_OR_ADDRESS", num2="NUMBER_TO_CALL", ) print(result) ``` ###
-5. Refresh access token When your access token has expired, you can use the
+## 1. Introduction The Sonetel API is a REST based web-service that enables you
+to manage your Sonetel account from your own platform or service. You can
+manage your account, your phone numbers and make callback calls etc. This
+Python package provides an easy-to-use interface to integrate Sonetel's APIs
+with your service. For more information about the API, please see the
+[documentation](https://docs.sonetel.com/). ## 2. Get Started To use the
+package, you need a Sonetel account. If you don't already have one, get a free
+account from sonetel.com. ### 2.1 Installation #### 2.1.1 PIP This is the
+recommended way to install the module. It installs the latest stable version
+from the Python Package Index. `pip install sonetel` #### 2.1.2 Git To get the
+latest features, clone [the repository](https://github.com/Sonetel/sonetel-
+python) and [follow these instructions](https://packaging.python.org/en/latest/
+tutorials/packaging-projects/) to build the SDK locally. ### 2.2 Usage To use
+the package, add the following line to the top of your Python program. `import
+sonetel` Here's a description of the various modules and the methods available
+with each. #### 2.2.1 Auth The Auth module is used to generate and manage
+access tokens. To instantiate it, you need to pass your Sonetel username and
+password to it. It supports the following methods: 1. `create_token()` - create
+a new access token. Called automatically when a new instance is created. 2.
+`get_access_token()` - fetch the current access token. 3. `get_refresh_token()`
+- get the refresh token, used to refresh the access token. 4.
+`get_decoded_token()` - return the decoded JWT value. Returns a dict. #####
+Generate an access token ```python import os import sonetel as sntl user =
+os.environ.get('sonetelUsername') pswd = os.environ.get('sonetelPassword') s =
+sntl.Auth(username=user, password=pswd) print(s.get_access_token()) ``` #####
+Refresh access token When your access token has expired, you can use the
 `create_token()` method to get a new `access_token` & `refresh_token`. This
 automatically updates the Account object to use the newly generated access and
-refresh tokens. ```python import os from sonetel import api user =
-os.environ.get('sonetelUserName') pswd = os.environ.get('sonetelPassword') s =
-api.Account(username=user,password=pswd) print(s.get_token()) # Generate the
-refresh token and update the Account object response = s.create_token
-(refresh="yes", grant_type="refresh_token") print(response) ``` ### 6. Get
-decoded JWT token Get the decoded JWT token. ```python import os from sonetel
-import api user = os.environ.get('sonetelUserName') pswd = os.environ.get
-('sonetelPassword') s = api.Account(username=user,password=pswd) print
-(s.get_decodedtoken()) ``` ## Storing your credentials Please keep your
-credentials safe to avoid any misuse of your account. Do not hard code them
-into scripts or save them in files that are saved in any form of version
-control. You can add them to your operating system's environment variables and
-use Python's `os` module to fetch them. Assuming the username and password are
-stored in environment variables named `sonetelUserName` and `sonetelPassword`
-respectively, here's how you can access them from a script: ```python import os
-from sonetel import api user = os.environ.get('sonetelUserName') pswd =
-os.environ.get('sonetelPassword') s = api.Account(username=user,password=pswd)
-print(s.get_accountid()) ``` ## Help For help with the Sonetel API, have a look
-at the API_documentation. If you have an issue with the module, please [report
-an issue](https://github.com/Sonetel/sonetel-python/issues/issues) on GitHub.
+refresh tokens. ```python import os import sonetel as sntl user =
+os.environ.get('sonetelUsername') pswd = os.environ.get('sonetelPassword') s =
+sntl.Auth(username=user, password=pswd) print(s.get_access_token()) # Generate
+the refresh token and update the Account object response = s.create_token
+(refresh="yes", grant_type="refresh_token") print(response) ``` ##### Get
+decoded JWT token Get the decoded JWT token. ```python import os import sonetel
+as sntl user = os.environ.get('sonetelUsername') pswd = os.environ.get
+('sonetelPassword') s = sntl.Auth(username=user, password=pswd) print
+(s.get_decoded_token()) ``` #### 2.2.2 Account The Account module provides you
+information about your Sonetel account. For example, the prepaid balance,
+address and so on. It supports the following methods: 1. `get()` - Get
+information about the account. Return a dict with an overview of the
+information such as account ID, currency, prepaid balance, country and so on.
+2. `update()` - Update basic information about your account. 3. `get_balance()`
+- Returns the prepaid balance. Pass the parameter `currency` = `True` to
+include the currency with the returned value. 4. `get_accountid()` - Fetch the
+account ID. ##### Print your Sonetel account ID and the current prepaid
+balance. ```python import os from sonetel import Auth from sonetel import
+Account user = os.environ.get('sonetelUsername') pswd = os.environ.get
+('sonetelPassword') s = Auth(username=user,password=pswd) a = Account
+(s.get_access_token()) print(f"Your account ID is {a.get_accountid()} and your
+prepaid balance is {a.get_balance()}.") ``` #### 2.2.3 Call Use this to make
+callback calls with your Sonetel account. It supports the `callback()` method
+which requires your mobile number and the number of the person you wish to
+speak to. In a callback call, our system will first call you and when you
+answer, call the other number you provided. When the second call has been
+answered successfully, the calls will be connected together. ##### Make a
+callback call When making a callback call, `num1` is the destination where you
+will first answer the call before we call `num2`. This can be your mobile
+number, a SIP address or your Sonetel email address. If you set `num1` as your
+Sonetel email address, then the call will be handled as per your incoming call
+settings. ```python import os import sonetel user = os.environ.get
+('sonetelUsername') pswd = os.environ.get('sonetelPassword') s = sonetel.Auth
+(username=user,password=pswd) c = sonetel.Call(s.get_access_token()) result =
+c.callback( num1="YOUR_NUMBER_OR_ADDRESS", num2="NUMBER_TO_CALL", ) print
+(result) ``` #### 2.2.4 Phone Number The `Phonenumber` module allows you to
+manage phone numbers in your Sonetel account. It supports the following
+methods: 1. `get()` - get a list of phone numbers in your account. By default
+only returns a list of the E164 numbers. Set the parameter `e164only` equal to
+`False` to get detailed information. 2. `add()` - buy a new phone number. 3.
+`update()` - update the call forwarding settings for a phone number. 4. `delete
+()` - remove a phone number from your Sonetel account. ##### List the phone
+numbers available in your account ```python import os import sonetel user =
+os.environ.get('sonetelUsername') pswd = os.environ.get('sonetelPassword') s =
+sonetel.Auth(username=user,password=pswd) ph = sonetel.PhoneNumber
+(s.get_access_token()) print(ph.get()) ``` ## Storing your credentials Please
+keep your Sonetel login credentials safe to avoid any misuse of your account.
+Do not hard code them into scripts or save them in files that are saved in any
+form of version control. You can add them to your operating system's
+environment variables and use Python's `os` module to fetch them. Assuming the
+username and password are stored in environment variables named
+`sonetelUsername` and `sonetelPassword` respectively, here's how you can access
+them from a script: ```python import os import sonetel user = os.environ.get
+('sonetelUsername') pswd = os.environ.get('sonetelPassword') s = sonetel.Auth
+(username=user,password=pswd) print(s.get_access_token()) ``` ## Help For help
+with the Sonetel API, have a look at the API_documentation. If you have an
+issue with the module, please [report an issue](https://github.com/Sonetel/
+sonetel-python/issues/issues) on GitHub.
```

### Comparing `sonetel-0.1.5/README.md` & `sonetel-0.2.0/sonetel.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,246 @@
+Metadata-Version: 2.1
+Name: sonetel
+Version: 0.2.0
+Summary: A simple python wrapper for using Sonetel's REST APIs
+Home-page: https://github.com/Sonetel/sonetel-python
+Author: aashish
+Author-email: dev.support@sonetel.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/Sonetel/sonetel-python/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Telephony
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <br />
 <div align="center">
   <a href="https://github.com/Sonetel/sonetel-python">
     <img src="https://dl.dropboxusercontent.com/s/hn4o0v378od1aoo/logo_white_background.png" alt="Logo" width="80" height="80">
   </a>
 
-<h3 align="center">Sonetel API Python Wrapper</h3>
+<h3 align="center">Sonetel Python SDK</h3>
 
 <p align="center">
-    A simple Python wrapper for using Sonetel's REST API endpoints.
+    Python package for using Sonetel's REST API endpoints.
     <br />
     <br />
     <a href="https://sonetel.com/en/developer/">Sonetel Developer Home</a>
     .
     <a href="https://sonetel.com/en/developer/api-documentation/">API Documentation</a>
     .
     <a href="https://app.sonetel.com/register?tag=api-developer&simple=true">Get Free Account</a>
   </p>
 </div>
 
-## Introduction
+## 1. Introduction
 The Sonetel API is a REST based web-service that enables you to manage your Sonetel account from your own platform or service. You can manage your account, your phone numbers and make callback calls etc.
 
-This is a simple python wrapper to use Sonetel's communication APIs. For more information about the API, please see the [documentation](https://docs.sonetel.com/).
+This Python package provides an easy-to-use interface to integrate Sonetel's APIs with your service. For more information about the API, please see the [documentation](https://docs.sonetel.com/).
+
+## 2. Get Started
 
-## Getting Started
+To use the package, you need a Sonetel account. If you don't already have one, get a free account from <a href="https://app.sonetel.com/register?tag=api-developer&simple=true">sonetel.com</a>.
 
-To use the module, you need a Sonetel account. If you don't already have one, get a free account from <a href="https://app.sonetel.com/register?tag=api-developer&simple=true">sonetel.com</a>.
+### 2.1 Installation
 
-### Installation
+#### 2.1.1 PIP
 
-#### PIP
-Run the following command to install from pip.
+This is the recommended way to install the module. It installs the latest stable version from the Python Package Index.
 
 `pip install sonetel`
 
-#### Git
-To get the latest features, clone a specific [tag](https://github.com/Sonetel/sonetel-python/tags) and [follow these instructions](https://packaging.python.org/en/latest/tutorials/packaging-projects/) to build the module locally.
+#### 2.1.2 Git
+
+To get the latest features, clone [the repository](https://github.com/Sonetel/sonetel-python) and [follow these instructions](https://packaging.python.org/en/latest/tutorials/packaging-projects/) to build the SDK locally.
+
+### 2.2 Usage
+
+To use the package, add the following line to the top of your Python program.
+
+`import sonetel`
 
-## Functions
+Here's a description of the various modules and the methods available with each.
+#### 2.2.1 Auth
 
-The following functions are support at the moment. More will be added in the future.
+The Auth module is used to generate and manage access tokens.
 
-- `get_balance()` - Get the prepaid balance of the account (e.g. '10'). Pass the argument `currency=True` to get the balance with the currency appended (e.g. '10 USD')
-- `get_token()` - Get the access token being used.
-- `get_accountid()` - Returns your Sonetel account ID.
-- `get_username()` - Returns the email address of the user that was used to create the token.
-- `get_voiceapps()` - get a list of all the voice apps in the account.
-- `get_refreshtoken()` - get the refresh token used to regenerate the access token when it expires.
-- `account_info()` - Fetch information about your account such as company name, balance, country, timezone, daily limit and so on.
-- `account_users()` - Details of all the users in your account.
-- `callback()` - Use our Callback API to make a callback call.
-- `create_token()` - Create a new access token. A new access token is automatically created when you call the Account resource the first time.
-- `subscription_buynum()` - Purchase a phone number. Requires a phone number to be passed. Use the `/availablephonenumber` API endpoint to see a list of phone numbers available for purchase from a country and area.
-- `subscription_listnums()` - See the details of all the phone numbers purchased by you. Pass the parameter `e164only=True` to only get a list of E.164 numbers without any metadata.
+To instantiate it, you need to pass your Sonetel username and password to it. It supports the following methods:
 
-## Examples
+1. `create_token()` - create a new access token. Called automatically when a new instance is created.
+2. `get_access_token()` - fetch the current access token.
+3. `get_refresh_token()` - get the refresh token, used to refresh the access token.
+4. `get_decoded_token()` - return the decoded JWT value. Returns a dict.
 
-### 1. Create an access token
+##### Generate an access token
 
 ```python
 import os
-from sonetel import api
+import sonetel as sntl
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sntl.Auth(username=user, password=pswd)
 
-print(s.get_token())
+print(s.get_access_token())
 ```
 
-### 2. Print your Sonetel account ID and the current prepaid balance. 
+#####  Refresh access token
+
+When your access token has expired, you can use the `create_token()` method to get a new `access_token` & `refresh_token`.
+
+This automatically updates the Account object to use the newly generated access and refresh tokens.
 
 ```python
 import os
-from sonetel import api
+import sonetel as sntl
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sntl.Auth(username=user, password=pswd)
+
+print(s.get_access_token())
 
-print(f"Your account ID is {s.get_accountid()} and your prepaid balance is {s.get_balance()}.")
+# Generate the refresh token and update the Account object
+response = s.create_token(refresh="yes", grant_type="refresh_token")
+
+print(response)
 ```
 
-### 3. List the phone numbers available in your account
+##### Get decoded JWT token
+
+Get the decoded JWT token.
 
 ```python
 import os
-from sonetel import api
+import sonetel as sntl
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sntl.Auth(username=user, password=pswd)
+
+print(s.get_decoded_token())
 
-print(s.subscription_listnums(e164only=True))
 ```
 
-### 4. Make a callback call
+#### 2.2.2 Account
 
-When making a callback call, `num1` is the destination where you will first answer the call before we call `num2`. This can be your mobile number, a SIP address or your Sonetel email address. 
+The Account module provides you information about your Sonetel account. For example, the prepaid balance, address and so on.
 
-If you set `num1` as your Sonetel email address, then the call will be handled as per your incoming call settings.
+It supports the following methods:
+
+1. `get()` - Get information about the account. Return a dict with an overview of the information such as account ID, currency, prepaid balance, country and so on.
+2. `update()` - Update basic information about your account.
+3. `get_balance()` - Returns the prepaid balance. Pass the parameter `currency` = `True` to include the currency with the returned value.
+4. `get_accountid()` - Fetch the account ID.
+
+##### Print your Sonetel account ID and the current prepaid balance. 
 
 ```python
 import os
-from sonetel import api
+from sonetel import Auth
+from sonetel import Account
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = Auth(username=user,password=pswd)
 
-result = s.callback(
-    num1="YOUR_NUMBER_OR_ADDRESS",
-    num2="NUMBER_TO_CALL",
-)
-print(result)
+a = Account(s.get_access_token())
+
+print(f"Your account ID is {a.get_accountid()} and your prepaid balance is {a.get_balance()}.")
 ```
 
-### 5. Refresh access token
+#### 2.2.3 Call
 
-When your access token has expired, you can use the `create_token()` method to get a new `access_token` & `refresh_token`.
+Use this to make callback calls with your Sonetel account.
 
-This automatically updates the Account object to use the newly generated access and refresh tokens.
+It supports the `callback()` method which requires your mobile number and the number of the person you wish to speak to. In a callback call, our system will first call you and when you answer, call the other number you provided. When the second call has been answered successfully, the calls will be connected together.
+
+##### Make a callback call
+
+When making a callback call, `num1` is the destination where you will first answer the call before we call `num2`. This can be your mobile number, a SIP address or your Sonetel email address. 
+
+If you set `num1` as your Sonetel email address, then the call will be handled as per your incoming call settings.
 
 ```python
 import os
-from sonetel import api
+import sonetel
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sonetel.Auth(username=user,password=pswd)
 
-print(s.get_token())
+c = sonetel.Call(s.get_access_token())
 
-# Generate the refresh token and update the Account object
-response = s.create_token(refresh="yes", grant_type="refresh_token")
-
-print(response)
+result = c.callback(
+    num1="YOUR_NUMBER_OR_ADDRESS",
+    num2="NUMBER_TO_CALL",
+)
+print(result)
 ```
 
-### 6. Get decoded JWT token
+#### 2.2.4 Phone Number
 
-Get the decoded JWT token.
+The `Phonenumber` module allows you to manage phone numbers in your Sonetel account.
+
+It supports the following methods:
+
+1. `get()` - get a list of phone numbers in your account. By default only returns a list of the E164 numbers. Set the parameter `e164only` equal to `False` to get detailed information.
+2. `add()` - buy a new phone number.
+3. `update()` - update the call forwarding settings for a phone number.
+4. `delete()` - remove a phone number from your Sonetel account.
+
+##### List the phone numbers available in your account
 
 ```python
 import os
-from sonetel import api
+import sonetel
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sonetel.Auth(username=user,password=pswd)
 
-print(s.get_decodedtoken())
+ph = sonetel.PhoneNumber(s.get_access_token())
+print(ph.get())
 
 ```
 
 ## Storing your credentials
 
-Please keep your credentials safe to avoid any misuse of your account. Do not hard code them into scripts or save them in files that are saved in any form of version control.
+Please keep your Sonetel login credentials safe to avoid any misuse of your account. Do not hard code them into scripts or save them in files that are saved in any form of version control.
 
 You can add them to your operating system's environment variables and use Python's `os` module to fetch them.
 
-Assuming the username and password are stored in environment variables named `sonetelUserName` and `sonetelPassword` respectively, here's how you can access them from a script:
+Assuming the username and password are stored in environment variables named `sonetelUsername` and `sonetelPassword` respectively, here's how you can access them from a script:
 
 ```python
 import os
-from sonetel import api
+import sonetel
 
-user = os.environ.get('sonetelUserName')
+user = os.environ.get('sonetelUsername')
 pswd = os.environ.get('sonetelPassword')
 
-s = api.Account(username=user,password=pswd)
+s = sonetel.Auth(username=user,password=pswd)
 
-print(s.get_accountid())
+print(s.get_access_token())
 ```
 
 ## Help
 
 For help with the Sonetel API, have a look at the <a href="https://docs.sonetel.com">API documentation</a>.
 
-If you have an issue with the module, please [report an issue](https://github.com/Sonetel/sonetel-python/issues/issues) on GitHub.
+If you have an issue with the module, please [report an issue](https://github.com/Sonetel/sonetel-python/issues/issues) on GitHub.
```

#### html2text {}

```diff
@@ -1,78 +1,103 @@
-
+Metadata-Version: 2.1 Name: sonetel Version: 0.2.0 Summary: A simple python
+wrapper for using Sonetel's REST APIs Home-page: https://github.com/Sonetel/
+sonetel-python Author: aashish Author-email: dev.support@sonetel.com License:
+MIT Project-URL: Bug Tracker, https://github.com/Sonetel/sonetel-python/issues
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Telecommunications Industry Classifier: Topic
+:: Communications Classifier: Topic :: Communications :: Telephony Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Classifier:
+License :: OSI Approved :: MIT License Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
-                     **** Sonetel API Python Wrapper ****
-       A simple Python wrapper for using Sonetel's REST API endpoints.
+                         **** Sonetel Python SDK ****
+            Python package for using Sonetel's REST API endpoints.
 
          Sonetel_Developer_Home . API_Documentation . Get_Free_Account
-## Introduction The Sonetel API is a REST based web-service that enables you to
-manage your Sonetel account from your own platform or service. You can manage
-your account, your phone numbers and make callback calls etc. This is a simple
-python wrapper to use Sonetel's communication APIs. For more information about
-the API, please see the [documentation](https://docs.sonetel.com/). ## Getting
-Started To use the module, you need a Sonetel account. If you don't already
-have one, get a free account from sonetel.com. ### Installation #### PIP Run
-the following command to install from pip. `pip install sonetel` #### Git To
-get the latest features, clone a specific [tag](https://github.com/Sonetel/
-sonetel-python/tags) and [follow these instructions](https://
-packaging.python.org/en/latest/tutorials/packaging-projects/) to build the
-module locally. ## Functions The following functions are support at the moment.
-More will be added in the future. - `get_balance()` - Get the prepaid balance
-of the account (e.g. '10'). Pass the argument `currency=True` to get the
-balance with the currency appended (e.g. '10 USD') - `get_token()` - Get the
-access token being used. - `get_accountid()` - Returns your Sonetel account ID.
-- `get_username()` - Returns the email address of the user that was used to
-create the token. - `get_voiceapps()` - get a list of all the voice apps in the
-account. - `get_refreshtoken()` - get the refresh token used to regenerate the
-access token when it expires. - `account_info()` - Fetch information about your
-account such as company name, balance, country, timezone, daily limit and so
-on. - `account_users()` - Details of all the users in your account. - `callback
-()` - Use our Callback API to make a callback call. - `create_token()` - Create
-a new access token. A new access token is automatically created when you call
-the Account resource the first time. - `subscription_buynum()` - Purchase a
-phone number. Requires a phone number to be passed. Use the `/
-availablephonenumber` API endpoint to see a list of phone numbers available for
-purchase from a country and area. - `subscription_listnums()` - See the details
-of all the phone numbers purchased by you. Pass the parameter `e164only=True`
-to only get a list of E.164 numbers without any metadata. ## Examples ### 1.
-Create an access token ```python import os from sonetel import api user =
-os.environ.get('sonetelUserName') pswd = os.environ.get('sonetelPassword') s =
-api.Account(username=user,password=pswd) print(s.get_token()) ``` ### 2. Print
-your Sonetel account ID and the current prepaid balance. ```python import os
-from sonetel import api user = os.environ.get('sonetelUserName') pswd =
-os.environ.get('sonetelPassword') s = api.Account(username=user,password=pswd)
-print(f"Your account ID is {s.get_accountid()} and your prepaid balance is
-{s.get_balance()}.") ``` ### 3. List the phone numbers available in your
-account ```python import os from sonetel import api user = os.environ.get
-('sonetelUserName') pswd = os.environ.get('sonetelPassword') s = api.Account
-(username=user,password=pswd) print(s.subscription_listnums(e164only=True)) ```
-### 4. Make a callback call When making a callback call, `num1` is the
-destination where you will first answer the call before we call `num2`. This
-can be your mobile number, a SIP address or your Sonetel email address. If you
-set `num1` as your Sonetel email address, then the call will be handled as per
-your incoming call settings. ```python import os from sonetel import api user =
-os.environ.get('sonetelUserName') pswd = os.environ.get('sonetelPassword') s =
-api.Account(username=user,password=pswd) result = s.callback
-( num1="YOUR_NUMBER_OR_ADDRESS", num2="NUMBER_TO_CALL", ) print(result) ``` ###
-5. Refresh access token When your access token has expired, you can use the
+## 1. Introduction The Sonetel API is a REST based web-service that enables you
+to manage your Sonetel account from your own platform or service. You can
+manage your account, your phone numbers and make callback calls etc. This
+Python package provides an easy-to-use interface to integrate Sonetel's APIs
+with your service. For more information about the API, please see the
+[documentation](https://docs.sonetel.com/). ## 2. Get Started To use the
+package, you need a Sonetel account. If you don't already have one, get a free
+account from sonetel.com. ### 2.1 Installation #### 2.1.1 PIP This is the
+recommended way to install the module. It installs the latest stable version
+from the Python Package Index. `pip install sonetel` #### 2.1.2 Git To get the
+latest features, clone [the repository](https://github.com/Sonetel/sonetel-
+python) and [follow these instructions](https://packaging.python.org/en/latest/
+tutorials/packaging-projects/) to build the SDK locally. ### 2.2 Usage To use
+the package, add the following line to the top of your Python program. `import
+sonetel` Here's a description of the various modules and the methods available
+with each. #### 2.2.1 Auth The Auth module is used to generate and manage
+access tokens. To instantiate it, you need to pass your Sonetel username and
+password to it. It supports the following methods: 1. `create_token()` - create
+a new access token. Called automatically when a new instance is created. 2.
+`get_access_token()` - fetch the current access token. 3. `get_refresh_token()`
+- get the refresh token, used to refresh the access token. 4.
+`get_decoded_token()` - return the decoded JWT value. Returns a dict. #####
+Generate an access token ```python import os import sonetel as sntl user =
+os.environ.get('sonetelUsername') pswd = os.environ.get('sonetelPassword') s =
+sntl.Auth(username=user, password=pswd) print(s.get_access_token()) ``` #####
+Refresh access token When your access token has expired, you can use the
 `create_token()` method to get a new `access_token` & `refresh_token`. This
 automatically updates the Account object to use the newly generated access and
-refresh tokens. ```python import os from sonetel import api user =
-os.environ.get('sonetelUserName') pswd = os.environ.get('sonetelPassword') s =
-api.Account(username=user,password=pswd) print(s.get_token()) # Generate the
-refresh token and update the Account object response = s.create_token
-(refresh="yes", grant_type="refresh_token") print(response) ``` ### 6. Get
-decoded JWT token Get the decoded JWT token. ```python import os from sonetel
-import api user = os.environ.get('sonetelUserName') pswd = os.environ.get
-('sonetelPassword') s = api.Account(username=user,password=pswd) print
-(s.get_decodedtoken()) ``` ## Storing your credentials Please keep your
-credentials safe to avoid any misuse of your account. Do not hard code them
-into scripts or save them in files that are saved in any form of version
-control. You can add them to your operating system's environment variables and
-use Python's `os` module to fetch them. Assuming the username and password are
-stored in environment variables named `sonetelUserName` and `sonetelPassword`
-respectively, here's how you can access them from a script: ```python import os
-from sonetel import api user = os.environ.get('sonetelUserName') pswd =
-os.environ.get('sonetelPassword') s = api.Account(username=user,password=pswd)
-print(s.get_accountid()) ``` ## Help For help with the Sonetel API, have a look
-at the API_documentation. If you have an issue with the module, please [report
-an issue](https://github.com/Sonetel/sonetel-python/issues/issues) on GitHub.
+refresh tokens. ```python import os import sonetel as sntl user =
+os.environ.get('sonetelUsername') pswd = os.environ.get('sonetelPassword') s =
+sntl.Auth(username=user, password=pswd) print(s.get_access_token()) # Generate
+the refresh token and update the Account object response = s.create_token
+(refresh="yes", grant_type="refresh_token") print(response) ``` ##### Get
+decoded JWT token Get the decoded JWT token. ```python import os import sonetel
+as sntl user = os.environ.get('sonetelUsername') pswd = os.environ.get
+('sonetelPassword') s = sntl.Auth(username=user, password=pswd) print
+(s.get_decoded_token()) ``` #### 2.2.2 Account The Account module provides you
+information about your Sonetel account. For example, the prepaid balance,
+address and so on. It supports the following methods: 1. `get()` - Get
+information about the account. Return a dict with an overview of the
+information such as account ID, currency, prepaid balance, country and so on.
+2. `update()` - Update basic information about your account. 3. `get_balance()`
+- Returns the prepaid balance. Pass the parameter `currency` = `True` to
+include the currency with the returned value. 4. `get_accountid()` - Fetch the
+account ID. ##### Print your Sonetel account ID and the current prepaid
+balance. ```python import os from sonetel import Auth from sonetel import
+Account user = os.environ.get('sonetelUsername') pswd = os.environ.get
+('sonetelPassword') s = Auth(username=user,password=pswd) a = Account
+(s.get_access_token()) print(f"Your account ID is {a.get_accountid()} and your
+prepaid balance is {a.get_balance()}.") ``` #### 2.2.3 Call Use this to make
+callback calls with your Sonetel account. It supports the `callback()` method
+which requires your mobile number and the number of the person you wish to
+speak to. In a callback call, our system will first call you and when you
+answer, call the other number you provided. When the second call has been
+answered successfully, the calls will be connected together. ##### Make a
+callback call When making a callback call, `num1` is the destination where you
+will first answer the call before we call `num2`. This can be your mobile
+number, a SIP address or your Sonetel email address. If you set `num1` as your
+Sonetel email address, then the call will be handled as per your incoming call
+settings. ```python import os import sonetel user = os.environ.get
+('sonetelUsername') pswd = os.environ.get('sonetelPassword') s = sonetel.Auth
+(username=user,password=pswd) c = sonetel.Call(s.get_access_token()) result =
+c.callback( num1="YOUR_NUMBER_OR_ADDRESS", num2="NUMBER_TO_CALL", ) print
+(result) ``` #### 2.2.4 Phone Number The `Phonenumber` module allows you to
+manage phone numbers in your Sonetel account. It supports the following
+methods: 1. `get()` - get a list of phone numbers in your account. By default
+only returns a list of the E164 numbers. Set the parameter `e164only` equal to
+`False` to get detailed information. 2. `add()` - buy a new phone number. 3.
+`update()` - update the call forwarding settings for a phone number. 4. `delete
+()` - remove a phone number from your Sonetel account. ##### List the phone
+numbers available in your account ```python import os import sonetel user =
+os.environ.get('sonetelUsername') pswd = os.environ.get('sonetelPassword') s =
+sonetel.Auth(username=user,password=pswd) ph = sonetel.PhoneNumber
+(s.get_access_token()) print(ph.get()) ``` ## Storing your credentials Please
+keep your Sonetel login credentials safe to avoid any misuse of your account.
+Do not hard code them into scripts or save them in files that are saved in any
+form of version control. You can add them to your operating system's
+environment variables and use Python's `os` module to fetch them. Assuming the
+username and password are stored in environment variables named
+`sonetelUsername` and `sonetelPassword` respectively, here's how you can access
+them from a script: ```python import os import sonetel user = os.environ.get
+('sonetelUsername') pswd = os.environ.get('sonetelPassword') s = sonetel.Auth
+(username=user,password=pswd) print(s.get_access_token()) ``` ## Help For help
+with the Sonetel API, have a look at the API_documentation. If you have an
+issue with the module, please [report an issue](https://github.com/Sonetel/
+sonetel-python/issues/issues) on GitHub.
```

