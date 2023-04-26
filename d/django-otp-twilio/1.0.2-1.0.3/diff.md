# Comparing `tmp/django-otp-twilio-1.0.2.tar.gz` & `tmp/django-otp-twilio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-otp-twilio-1.0.2.tar", last modified: Tue Apr 11 17:57:02 2023, max compression
+gzip compressed data, was "dist/django-otp-twilio-1.0.3.tar", last modified: Tue Apr 25 17:51:13 2023, max compression
```

## Comparing `django-otp-twilio-1.0.2.tar` & `django-otp-twilio-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     4623 2023-04-11 17:56:33.000000 django-otp-twilio-1.0.2/CHANGES.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1297 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/LICENSE
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      100 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/MANIFEST.in
--rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/PKG-INFO
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      710 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/README.rst
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/docs/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     5709 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/docs/Makefile
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/docs/ext/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      217 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/docs/ext/otpdocs.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/docs/source/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)       54 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/docs/source/changes.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     8876 2023-04-11 17:56:33.000000 django-otp-twilio-1.0.2/docs/source/conf.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     3029 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.2/docs/source/index.rst
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      147 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/setup.cfg
--rwxrwxr-x   0 psagers   (1000) psagers   (1000)     1087 2023-04-11 17:56:33.000000 django-otp-twilio-1.0.2/setup.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/
--rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/PKG-INFO
--rw-r--r--   0 psagers   (1000) psagers   (1000)      752 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/SOURCES.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)        1 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/dependency_links.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)       27 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/requires.txt
--rw-r--r--   0 psagers   (1000) psagers   (1000)       11 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/top_level.txt
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/otp_twilio/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/__init__.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      667 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/admin.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      146 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/apps.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     1053 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.2/src/otp_twilio/conf.py
-drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-11 17:57:02.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1411 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0001_initial.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      540 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0002_last_t.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)      463 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0003_longer_number.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     1465 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/0004_sidechanneldevice.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/migrations/__init__.py
--rw-r--r--   0 psagers   (1000) psagers   (1000)     4072 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.2/src/otp_twilio/models.py
--rw-rw-r--   0 psagers   (1000) psagers   (1000)     3209 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.2/src/otp_twilio/tests.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     4888 2023-04-25 17:50:32.000000 django-otp-twilio-1.0.3/CHANGES.rst
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     1297 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/LICENSE
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      100 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/MANIFEST.in
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/PKG-INFO
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      710 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/README.rst
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/docs/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     5709 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/docs/Makefile
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/docs/ext/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      217 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/docs/ext/otpdocs.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/docs/source/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)       54 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/docs/source/changes.rst
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     8876 2023-04-25 17:50:32.000000 django-otp-twilio-1.0.3/docs/source/conf.py
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     3029 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.3/docs/source/index.rst
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      147 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/setup.cfg
+-rwxrwxr-x   0 psagers   (1000) psagers   (1000)     1087 2023-04-25 17:50:32.000000 django-otp-twilio-1.0.3/setup.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     1549 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/PKG-INFO
+-rw-r--r--   0 psagers   (1000) psagers   (1000)      752 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 psagers   (1000) psagers   (1000)        1 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 psagers   (1000) psagers   (1000)       27 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/requires.txt
+-rw-r--r--   0 psagers   (1000) psagers   (1000)       11 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/top_level.txt
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/otp_twilio/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/__init__.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      667 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/admin.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      146 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/apps.py
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     1053 2023-04-11 17:51:34.000000 django-otp-twilio-1.0.3/src/otp_twilio/conf.py
+drwxr-xr-x   0 psagers   (1000) psagers   (1000)        0 2023-04-25 17:51:13.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     1411 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0001_initial.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      540 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0002_last_t.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)      463 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0003_longer_number.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     1465 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/0004_sidechanneldevice.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)        0 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/migrations/__init__.py
+-rw-r--r--   0 psagers   (1000) psagers   (1000)     4080 2023-04-25 17:47:23.000000 django-otp-twilio-1.0.3/src/otp_twilio/models.py
+-rw-rw-r--   0 psagers   (1000) psagers   (1000)     3209 2022-01-13 18:26:54.000000 django-otp-twilio-1.0.3/src/otp_twilio/tests.py
```

### Comparing `django-otp-twilio-1.0.2/CHANGES.rst` & `django-otp-twilio-1.0.3/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+v1.0.3 - April 25, 2023 - Fix API key handling
+--------------------------------------------------------------------------------
+
+Fix `#6`_: Code uses "TWILIO_API_KEY" instead of "OTP_TWILIO_API_KEY"
+
+.. _#6: https://github.com/django-otp/django-otp-twilio/pull/6
+
+
 v1.0.2 - April 11, 2023 - New configuration options
 --------------------------------------------------------------------------------
 
 - Allow configuration of API URL and API key.
 
 
 v1.0.1 - November 29, 2021 - Forward compatibility
```

### Comparing `django-otp-twilio-1.0.2/LICENSE` & `django-otp-twilio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/PKG-INFO` & `django-otp-twilio-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp-twilio
-Version: 1.0.2
+Version: 1.0.3
 Summary: A django-otp plugin that delivers tokens via Twilio's SMS service.
 Home-page: https://github.com/django-otp/django-otp-twilio
 Author: Peter Sagerson
 Author-email: psagers@ignorare.net
 License: BSD
 Project-URL: Documentation, https://django-otp-twilio.readthedocs.io/
 Project-URL: Source, https://github.com/django-otp/django-otp-twilio
```

### Comparing `django-otp-twilio-1.0.2/README.rst` & `django-otp-twilio-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/docs/Makefile` & `django-otp-twilio-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/docs/source/conf.py` & `django-otp-twilio-1.0.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 copyright = u'2012, Peter Sagerson'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.0.2'
+release = '1.0.3'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `django-otp-twilio-1.0.2/docs/source/index.rst` & `django-otp-twilio-1.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/setup.py` & `django-otp-twilio-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='django-otp-twilio',
-    version='1.0.2',
+    version='1.0.3',
     description="A django-otp plugin that delivers tokens via Twilio's SMS service.",
     author="Peter Sagerson",
     author_email='psagers@ignorare.net',
     url='https://github.com/django-otp/django-otp-twilio',
     project_urls={
         "Documentation": 'https://django-otp-twilio.readthedocs.io/',
         "Source": 'https://github.com/django-otp/django-otp-twilio',
```

### Comparing `django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/PKG-INFO` & `django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp-twilio
-Version: 1.0.2
+Version: 1.0.3
 Summary: A django-otp plugin that delivers tokens via Twilio's SMS service.
 Home-page: https://github.com/django-otp/django-otp-twilio
 Author: Peter Sagerson
 Author-email: psagers@ignorare.net
 License: BSD
 Project-URL: Documentation, https://django-otp-twilio.readthedocs.io/
 Project-URL: Source, https://github.com/django-otp/django-otp-twilio
```

### Comparing `django-otp-twilio-1.0.2/src/django_otp_twilio.egg-info/SOURCES.txt` & `django-otp-twilio-1.0.3/src/django_otp_twilio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/admin.py` & `django-otp-twilio-1.0.3/src/otp_twilio/admin.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/conf.py` & `django-otp-twilio-1.0.3/src/otp_twilio/conf.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/migrations/0001_initial.py` & `django-otp-twilio-1.0.3/src/otp_twilio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/migrations/0002_last_t.py` & `django-otp-twilio-1.0.3/src/otp_twilio/migrations/0002_last_t.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/migrations/0004_sidechanneldevice.py` & `django-otp-twilio-1.0.3/src/otp_twilio/migrations/0004_sidechanneldevice.py`

 * *Files identical despite different names*

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/models.py` & `django-otp-twilio-1.0.3/src/otp_twilio/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             'From': settings.OTP_TWILIO_FROM,
             'To': self.number,
             'Body': str(token),
         }
 
         response = requests.post(
             url, data=data,
-            auth=(settings.TWILIO_API_KEY if settings.TWILIO_API_KEY else settings.OTP_TWILIO_ACCOUNT, settings.OTP_TWILIO_AUTH)
+            auth=(settings.OTP_TWILIO_API_KEY if settings.OTP_TWILIO_API_KEY else settings.OTP_TWILIO_ACCOUNT, settings.OTP_TWILIO_AUTH)
         )
 
         try:
             response.raise_for_status()
         except Exception as e:
             logger.exception('Error sending token by Twilio SMS: {0}'.format(e))
             raise
```

### Comparing `django-otp-twilio-1.0.2/src/otp_twilio/tests.py` & `django-otp-twilio-1.0.3/src/otp_twilio/tests.py`

 * *Files identical despite different names*

