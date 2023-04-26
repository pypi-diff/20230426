# Comparing `tmp/logsnag-0.1.4.tar.gz` & `tmp/logsnag-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logsnag-0.1.4.tar", last modified: Wed Jan 25 14:29:00 2023, max compression
+gzip compressed data, was "logsnag-1.0.0b2.tar", last modified: Tue Apr 25 18:55:47 2023, max compression
```

## Comparing `logsnag-0.1.4.tar` & `logsnag-1.0.0b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shayan     (501) staff       (20)        0 2023-01-25 14:29:00.419948 logsnag-0.1.4/
--rw-r--r--   0 shayan     (501) staff       (20)     1063 2022-08-09 03:09:36.000000 logsnag-0.1.4/LICENSE
--rw-r--r--   0 shayan     (501) staff       (20)     1806 2023-01-25 14:29:00.419818 logsnag-0.1.4/PKG-INFO
--rw-r--r--   0 shayan     (501) staff       (20)     1051 2022-10-21 18:24:34.000000 logsnag-0.1.4/README.md
-drwxr-xr-x   0 shayan     (501) staff       (20)        0 2023-01-25 14:29:00.418837 logsnag-0.1.4/logsnag/
--rw-r--r--   0 shayan     (501) staff       (20)      116 2022-08-09 03:09:36.000000 logsnag-0.1.4/logsnag/__init__.py
--rw-r--r--   0 shayan     (501) staff       (20)      213 2022-10-21 18:24:34.000000 logsnag-0.1.4/logsnag/constants.py
--rw-r--r--   0 shayan     (501) staff       (20)       91 2022-08-09 03:09:36.000000 logsnag-0.1.4/logsnag/exceptions.py
--rw-r--r--   0 shayan     (501) staff       (20)     3391 2023-01-25 14:28:51.000000 logsnag-0.1.4/logsnag/logsnag.py
--rw-r--r--   0 shayan     (501) staff       (20)      249 2022-08-09 03:09:36.000000 logsnag-0.1.4/logsnag/utils.py
--rw-r--r--   0 shayan     (501) staff       (20)       45 2023-01-25 14:28:45.000000 logsnag-0.1.4/logsnag/version.py
-drwxr-xr-x   0 shayan     (501) staff       (20)        0 2023-01-25 14:29:00.419556 logsnag-0.1.4/logsnag.egg-info/
--rw-r--r--   0 shayan     (501) staff       (20)     1806 2023-01-25 14:29:00.000000 logsnag-0.1.4/logsnag.egg-info/PKG-INFO
--rw-r--r--   0 shayan     (501) staff       (20)      298 2023-01-25 14:29:00.000000 logsnag-0.1.4/logsnag.egg-info/SOURCES.txt
--rw-r--r--   0 shayan     (501) staff       (20)        1 2023-01-25 14:29:00.000000 logsnag-0.1.4/logsnag.egg-info/dependency_links.txt
--rw-r--r--   0 shayan     (501) staff       (20)        9 2023-01-25 14:29:00.000000 logsnag-0.1.4/logsnag.egg-info/requires.txt
--rw-r--r--   0 shayan     (501) staff       (20)        8 2023-01-25 14:29:00.000000 logsnag-0.1.4/logsnag.egg-info/top_level.txt
--rw-r--r--   0 shayan     (501) staff       (20)       38 2023-01-25 14:29:00.420091 logsnag-0.1.4/setup.cfg
--rw-r--r--   0 shayan     (501) staff       (20)     1046 2023-01-25 14:28:27.000000 logsnag-0.1.4/setup.py
+drwxr-xr-x   0 shayan     (501) staff       (20)        0 2023-04-25 18:55:47.691112 logsnag-1.0.0b2/
+-rw-r--r--   0 shayan     (501) staff       (20)     1063 2022-08-09 03:09:36.000000 logsnag-1.0.0b2/LICENSE
+-rw-r--r--   0 shayan     (501) staff       (20)     2112 2023-04-25 18:55:47.690976 logsnag-1.0.0b2/PKG-INFO
+-rw-r--r--   0 shayan     (501) staff       (20)     1355 2023-04-25 18:48:51.000000 logsnag-1.0.0b2/README.md
+drwxr-xr-x   0 shayan     (501) staff       (20)        0 2023-04-25 18:55:47.690086 logsnag-1.0.0b2/logsnag/
+-rw-r--r--   0 shayan     (501) staff       (20)      116 2022-08-09 03:09:36.000000 logsnag-1.0.0b2/logsnag/__init__.py
+-rw-r--r--   0 shayan     (501) staff       (20)      267 2023-04-25 18:48:51.000000 logsnag-1.0.0b2/logsnag/constants.py
+-rw-r--r--   0 shayan     (501) staff       (20)       91 2022-08-09 03:09:36.000000 logsnag-1.0.0b2/logsnag/exceptions.py
+-rw-r--r--   0 shayan     (501) staff       (20)     6145 2023-04-25 18:48:51.000000 logsnag-1.0.0b2/logsnag/logsnag.py
+-rw-r--r--   0 shayan     (501) staff       (20)      249 2022-08-09 03:09:36.000000 logsnag-1.0.0b2/logsnag/utils.py
+-rw-r--r--   0 shayan     (501) staff       (20)       47 2023-04-25 18:55:44.000000 logsnag-1.0.0b2/logsnag/version.py
+drwxr-xr-x   0 shayan     (501) staff       (20)        0 2023-04-25 18:55:47.690772 logsnag-1.0.0b2/logsnag.egg-info/
+-rw-r--r--   0 shayan     (501) staff       (20)     2112 2023-04-25 18:55:47.000000 logsnag-1.0.0b2/logsnag.egg-info/PKG-INFO
+-rw-r--r--   0 shayan     (501) staff       (20)      298 2023-04-25 18:55:47.000000 logsnag-1.0.0b2/logsnag.egg-info/SOURCES.txt
+-rw-r--r--   0 shayan     (501) staff       (20)        1 2023-04-25 18:55:47.000000 logsnag-1.0.0b2/logsnag.egg-info/dependency_links.txt
+-rw-r--r--   0 shayan     (501) staff       (20)        9 2023-04-25 18:55:47.000000 logsnag-1.0.0b2/logsnag.egg-info/requires.txt
+-rw-r--r--   0 shayan     (501) staff       (20)        8 2023-04-25 18:55:47.000000 logsnag-1.0.0b2/logsnag.egg-info/top_level.txt
+-rw-r--r--   0 shayan     (501) staff       (20)       38 2023-04-25 18:55:47.691158 logsnag-1.0.0b2/setup.cfg
+-rw-r--r--   0 shayan     (501) staff       (20)     1048 2023-04-25 18:55:44.000000 logsnag-1.0.0b2/setup.py
```

### Comparing `logsnag-0.1.4/LICENSE` & `logsnag-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `logsnag-0.1.4/PKG-INFO` & `logsnag-1.0.0b2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logsnag
-Version: 0.1.4
+Version: 1.0.0b2
 Summary: LogSnag API Wrapper
 Home-page: https://github.com/logsnag/logsnag.py
 Author: Shayan Taslim
 Author-email: shayan@logsnag.com
 License: MIT
 Project-URL: Homepage, https://logsnag.com
 Project-URL: Documentation, https://docs.logsnag.com
@@ -51,31 +51,54 @@
 ```python
 logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
 ```
 
 ### Publish Event
 
 ```python
-logsnag.publish(
+logsnag.track(
     channel="waitlist",
     event="User Joined",
+    user_id="user_123",
     description="Email: john@doe.com",
     icon="🎉",
     tags={
-      "email": "john@doe.com",
-      "user-id": "uid-12"  
+      "source": "google",
     },
     notify=True
 )
 ```
 
+### User Properties
+
+```python
+logsnag.identify(
+    user_id="user_123",
+    properties={
+        "name": "John Doe",
+        "email": "john@doe.com",
+        "plan": "free",
+    }
+)
+```
+
 ### Publish Insight
 
 ```python
-logsnag.insight(
+logsnag.insight.track(
     title='User Count',
     value=100,
     icon='👨',
 )
 ```
 
+### Increment Insight
+
+```python
+logsnag.insight.increment(
+    title='User Count',
+    value=1,
+    icon='👨',
+)
+```
+
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: logsnag Version: 0.1.4 Summary: LogSnag API Wrapper
-Home-page: https://github.com/logsnag/logsnag.py Author: Shayan Taslim Author-
-email: shayan@logsnag.com License: MIT Project-URL: Homepage, https://
+Metadata-Version: 2.1 Name: logsnag Version: 1.0.0b2 Summary: LogSnag API
+Wrapper Home-page: https://github.com/logsnag/logsnag.py Author: Shayan Taslim
+Author-email: shayan@logsnag.com License: MIT Project-URL: Homepage, https://
 logsnag.com Project-URL: Documentation, https://docs.logsnag.com Project-URL:
 Playground, https://logsnag.com/playground Project-URL: Github, https://
 github.com/LogSnag/logsnag.py Platform: UNKNOWN Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
@@ -12,12 +12,15 @@
                              ****** LogSnag ******
                Get notifications and track your project events.
                           [Discord] [Documentation]
 
 ## Installation ```sh pip3 install logsnag ``` ## Usage ### Import Library
 ```python from logsnag import LogSnag ``` ### Initialize Client ```python
 logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
-``` ### Publish Event ```python logsnag.publish( channel="waitlist",
-event="User Joined", description="Email: john@doe.com", icon="ð", tags=
-{ "email": "john@doe.com", "user-id": "uid-12" }, notify=True ) ``` ### Publish
-Insight ```python logsnag.insight( title='User Count', value=100, icon='ð¨',
-) ```
+``` ### Publish Event ```python logsnag.track( channel="waitlist", event="User
+Joined", user_id="user_123", description="Email: john@doe.com", icon="ð",
+tags={ "source": "google", }, notify=True ) ``` ### User Properties ```python
+logsnag.identify( user_id="user_123", properties={ "name": "John Doe", "email":
+"john@doe.com", "plan": "free", } ) ``` ### Publish Insight ```python
+logsnag.insight.track( title='User Count', value=100, icon='ð¨', ) ``` ###
+Increment Insight ```python logsnag.insight.increment( title='User Count',
+value=1, icon='ð¨', ) ```
```

### Comparing `logsnag-0.1.4/README.md` & `logsnag-1.0.0b2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -29,29 +29,52 @@
 ```python
 logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
 ```
 
 ### Publish Event
 
 ```python
-logsnag.publish(
+logsnag.track(
     channel="waitlist",
     event="User Joined",
+    user_id="user_123",
     description="Email: john@doe.com",
     icon="🎉",
     tags={
-      "email": "john@doe.com",
-      "user-id": "uid-12"  
+      "source": "google",
     },
     notify=True
 )
 ```
 
+### User Properties
+
+```python
+logsnag.identify(
+    user_id="user_123",
+    properties={
+        "name": "John Doe",
+        "email": "john@doe.com",
+        "plan": "free",
+    }
+)
+```
+
 ### Publish Insight
 
 ```python
-logsnag.insight(
+logsnag.insight.track(
     title='User Count',
     value=100,
     icon='👨',
 )
 ```
+
+### Increment Insight
+
+```python
+logsnag.insight.increment(
+    title='User Count',
+    value=1,
+    icon='👨',
+)
+```
```

#### html2text {}

```diff
@@ -2,12 +2,15 @@
                              ****** LogSnag ******
                Get notifications and track your project events.
                           [Discord] [Documentation]
 
 ## Installation ```sh pip3 install logsnag ``` ## Usage ### Import Library
 ```python from logsnag import LogSnag ``` ### Initialize Client ```python
 logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
-``` ### Publish Event ```python logsnag.publish( channel="waitlist",
-event="User Joined", description="Email: john@doe.com", icon="ð", tags=
-{ "email": "john@doe.com", "user-id": "uid-12" }, notify=True ) ``` ### Publish
-Insight ```python logsnag.insight( title='User Count', value=100, icon='ð¨',
-) ```
+``` ### Publish Event ```python logsnag.track( channel="waitlist", event="User
+Joined", user_id="user_123", description="Email: john@doe.com", icon="ð",
+tags={ "source": "google", }, notify=True ) ``` ### User Properties ```python
+logsnag.identify( user_id="user_123", properties={ "name": "John Doe", "email":
+"john@doe.com", "plan": "free", } ) ``` ### Publish Insight ```python
+logsnag.insight.track( title='User Count', value=100, icon='ð¨', ) ``` ###
+Increment Insight ```python logsnag.insight.increment( title='User Count',
+value=1, icon='ð¨', ) ```
```

### Comparing `logsnag-0.1.4/logsnag.egg-info/PKG-INFO` & `logsnag-1.0.0b2/logsnag.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logsnag
-Version: 0.1.4
+Version: 1.0.0b2
 Summary: LogSnag API Wrapper
 Home-page: https://github.com/logsnag/logsnag.py
 Author: Shayan Taslim
 Author-email: shayan@logsnag.com
 License: MIT
 Project-URL: Homepage, https://logsnag.com
 Project-URL: Documentation, https://docs.logsnag.com
@@ -51,31 +51,54 @@
 ```python
 logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
 ```
 
 ### Publish Event
 
 ```python
-logsnag.publish(
+logsnag.track(
     channel="waitlist",
     event="User Joined",
+    user_id="user_123",
     description="Email: john@doe.com",
     icon="🎉",
     tags={
-      "email": "john@doe.com",
-      "user-id": "uid-12"  
+      "source": "google",
     },
     notify=True
 )
 ```
 
+### User Properties
+
+```python
+logsnag.identify(
+    user_id="user_123",
+    properties={
+        "name": "John Doe",
+        "email": "john@doe.com",
+        "plan": "free",
+    }
+)
+```
+
 ### Publish Insight
 
 ```python
-logsnag.insight(
+logsnag.insight.track(
     title='User Count',
     value=100,
     icon='👨',
 )
 ```
 
+### Increment Insight
+
+```python
+logsnag.insight.increment(
+    title='User Count',
+    value=1,
+    icon='👨',
+)
+```
+
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: logsnag Version: 0.1.4 Summary: LogSnag API Wrapper
-Home-page: https://github.com/logsnag/logsnag.py Author: Shayan Taslim Author-
-email: shayan@logsnag.com License: MIT Project-URL: Homepage, https://
+Metadata-Version: 2.1 Name: logsnag Version: 1.0.0b2 Summary: LogSnag API
+Wrapper Home-page: https://github.com/logsnag/logsnag.py Author: Shayan Taslim
+Author-email: shayan@logsnag.com License: MIT Project-URL: Homepage, https://
 logsnag.com Project-URL: Documentation, https://docs.logsnag.com Project-URL:
 Playground, https://logsnag.com/playground Project-URL: Github, https://
 github.com/LogSnag/logsnag.py Platform: UNKNOWN Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
@@ -12,12 +12,15 @@
                              ****** LogSnag ******
                Get notifications and track your project events.
                           [Discord] [Documentation]
 
 ## Installation ```sh pip3 install logsnag ``` ## Usage ### Import Library
 ```python from logsnag import LogSnag ``` ### Initialize Client ```python
 logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
-``` ### Publish Event ```python logsnag.publish( channel="waitlist",
-event="User Joined", description="Email: john@doe.com", icon="ð", tags=
-{ "email": "john@doe.com", "user-id": "uid-12" }, notify=True ) ``` ### Publish
-Insight ```python logsnag.insight( title='User Count', value=100, icon='ð¨',
-) ```
+``` ### Publish Event ```python logsnag.track( channel="waitlist", event="User
+Joined", user_id="user_123", description="Email: john@doe.com", icon="ð",
+tags={ "source": "google", }, notify=True ) ``` ### User Properties ```python
+logsnag.identify( user_id="user_123", properties={ "name": "John Doe", "email":
+"john@doe.com", "plan": "free", } ) ``` ### Publish Insight ```python
+logsnag.insight.track( title='User Count', value=100, icon='ð¨', ) ``` ###
+Increment Insight ```python logsnag.insight.increment( title='User Count',
+value=1, icon='ð¨', ) ```
```

### Comparing `logsnag-0.1.4/setup.py` & `logsnag-1.0.0b2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="logsnag",
-    version='0.1.4',
+    version='1.0.0b2',
     description="LogSnag API Wrapper",
     long_description=README,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://logsnag.com',
         'Documentation': 'https://docs.logsnag.com',
         'Playground': 'https://logsnag.com/playground',
```

