# Comparing `tmp/django_ses-3.4.0.tar.gz` & `tmp/django_ses-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ses-3.4.0.tar", max compression
+gzip compressed data, was "django_ses-3.4.1.tar", max compression
```

## Comparing `django_ses-3.4.0.tar` & `django_ses-3.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1057 2023-04-24 16:20:44.326568 django_ses-3.4.0/LICENSE
--rw-r--r--   0        0        0    22379 2023-04-24 16:20:44.326568 django_ses-3.4.0/README.rst
--rw-r--r--   0        0        0    13974 2023-04-24 16:20:44.326568 django_ses-3.4.0/django_ses/__init__.py
--rw-r--r--   0        0        0      232 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/admin.py
--rw-r--r--   0        0        0      181 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/apps.py
--rw-r--r--   0        0        0       65 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/deprecation.py
--rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/commands/__init__.py
--rw-r--r--   0        0        0     2328 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/commands/get_ses_statistics.py
--rw-r--r--   0        0        0     2700 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/management/commands/ses_email_address.py
--rw-r--r--   0        0        0      897 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/migrations/__init__.py
--rw-r--r--   0        0        0      455 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/models.py
--rw-r--r--   0        0        0     2677 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/settings.py
--rw-r--r--   0        0        0      290 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/signals.py
--rw-r--r--   0        0        0     4894 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/templates/django_ses/send_stats.html
--rw-r--r--   0        0        0      157 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/urls.py
--rw-r--r--   0        0        0     9218 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/utils.py
--rw-r--r--   0        0        0    20602 2023-04-24 16:20:44.330568 django_ses-3.4.0/django_ses/views.py
--rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/__init__.py
--rw-r--r--   0        0        0       90 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/local_settings.template.py
--rw-r--r--   0        0        0      215 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/middleware.py
--rw-r--r--   0        0        0     2173 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/settings.py
--rw-r--r--   0        0        0      295 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/templates/base.html
--rw-r--r--   0        0        0      220 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/templates/index.html
--rw-r--r--   0        0        0      756 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/templates/send-email.html
--rw-r--r--   0        0        0      818 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/urls.py
--rw-r--r--   0        0        0      885 2023-04-24 16:20:44.330568 django_ses-3.4.0/example/views.py
--rw-r--r--   0        0        0     1560 2023-04-24 16:20:44.330568 django_ses-3.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/__init__.py
--rw-r--r--   0        0        0    15650 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_backend.py
--rw-r--r--   0        0        0     2481 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_commands.py
--rw-r--r--   0        0        0     2609 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_settings.py
--rw-r--r--   0        0        0     5200 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_stats.py
--rw-r--r--   0        0        0      366 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_urls.py
--rw-r--r--   0        0        0    12140 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_verifier.py
--rw-r--r--   0        0        0    13333 2023-04-24 16:20:44.330568 django_ses-3.4.0/tests/test_views.py
--rw-r--r--   0        0        0      115 2023-04-24 16:20:44.334568 django_ses-3.4.0/tests/utils.py
--rw-r--r--   0        0        0    24096 1970-01-01 00:00:00.000000 django_ses-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-25 21:41:20.616224 django_ses-3.4.1/LICENSE
+-rw-r--r--   0        0        0    22619 2023-04-25 21:41:20.616224 django_ses-3.4.1/README.rst
+-rw-r--r--   0        0        0    14037 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/__init__.py
+-rw-r--r--   0        0        0      232 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/admin.py
+-rw-r--r--   0        0        0      181 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/apps.py
+-rw-r--r--   0        0        0       65 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/deprecation.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/commands/get_ses_statistics.py
+-rw-r--r--   0        0        0     2700 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/commands/ses_email_address.py
+-rw-r--r--   0        0        0      897 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/models.py
+-rw-r--r--   0        0        0     2677 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/settings.py
+-rw-r--r--   0        0        0      290 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/signals.py
+-rw-r--r--   0        0        0     4894 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/templates/django_ses/send_stats.html
+-rw-r--r--   0        0        0      157 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/urls.py
+-rw-r--r--   0        0        0     9218 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/utils.py
+-rw-r--r--   0        0        0    20602 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/views.py
+-rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/local_settings.template.py
+-rw-r--r--   0        0        0      215 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/middleware.py
+-rw-r--r--   0        0        0     2173 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/settings.py
+-rw-r--r--   0        0        0      295 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/templates/base.html
+-rw-r--r--   0        0        0      220 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/templates/index.html
+-rw-r--r--   0        0        0      756 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/templates/send-email.html
+-rw-r--r--   0        0        0      818 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/urls.py
+-rw-r--r--   0        0        0      885 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/views.py
+-rw-r--r--   0        0        0     1560 2023-04-25 21:41:20.616224 django_ses-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/__init__.py
+-rw-r--r--   0        0        0    15650 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_backend.py
+-rw-r--r--   0        0        0     2481 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_commands.py
+-rw-r--r--   0        0        0     2609 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_settings.py
+-rw-r--r--   0        0        0     5200 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_stats.py
+-rw-r--r--   0        0        0      366 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_urls.py
+-rw-r--r--   0        0        0    12140 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_verifier.py
+-rw-r--r--   0        0        0    13333 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_views.py
+-rw-r--r--   0        0        0      115 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/utils.py
+-rw-r--r--   0        0        0    24336 1970-01-01 00:00:00.000000 django_ses-3.4.1/PKG-INFO
```

### Comparing `django_ses-3.4.0/LICENSE` & `django_ses-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/README.rst` & `django_ses-3.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -475,23 +475,28 @@
 ``AWS_SES_REGION_NAME``, ``AWS_SES_REGION_ENDPOINT``
   Optionally specify what region your SES service is using. Note that this is
   required if your SES service is not using us-east-1, as omitting these settings
   implies this region. Details:
   http://readthedocs.org/docs/boto/en/latest/ref/ses.html#boto.ses.regions
   http://docs.aws.amazon.com/general/latest/gr/rande.html
 
+``USE_SES_V2``
+  Optional. If you want to use client v2, you'll need to add `USE_SES_V2=True`. 
+  Some settings will need this flag enabled.
+  See https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#id87
+
 ``AWS_SES_FROM_EMAIL``
   Optional. The email address to be used as the "From" address for the email. The address that you specify has to be verified.  
   For more information please refer to https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#SESV2.Client.send_email
+
 ``AWS_SES_RETURN_PATH``
   Optional. Use `AWS_SES_RETURN_PATH` to receive complaint notifications
   You must use the v2 client by setting `USE_SES_V2=True` for this setting to work, otherwise it is ignored.
   https://docs.aws.amazon.com/ses/latest/APIReference-V2/API_SendEmail.html#API_SendEmail_RequestSyntax
 
-
 ``AWS_SES_CONFIGURATION_SET``
   Optional. Use this to mark your e-mails as from being from a particular SES
   Configuration Set. Set this to a string if you want all messages to have the
   same configuration set.  Set this to a callable if you want to set
   configuration set on a per message basis.
 
 ``TIME_ZONE``
```

### Comparing `django_ses-3.4.0/django_ses/__init__.py` & `django_ses-3.4.1/django_ses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,14 @@
 
     def _get_v2_parameters(self, message, source, email_feedback):
         """V2-Style raw payload for `send_email`.
 
         https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#SESV2.Client.send_email
         """
         params = dict(
-            FeedbackForwardingEmailAddress=email_feedback,
             FromEmailAddress=source or message.from_email,
             Destination={
                 'ToAddresses': message.recipients()
             },
             Content={
                 'Raw': {
                     'Data': dkim_sign(message.message().as_string(),
@@ -263,14 +262,17 @@
                                       dkim_selector=self.dkim_selector,
                                       dkim_headers=self.dkim_headers)
                 }
             }
         )
         if self.ses_from_arn or self.ses_source_arn:
             params['FromEmailAddressIdentityArn'] = self.ses_from_arn or self.ses_source_arn
+        if email_feedback is not None:
+            params['FeedbackForwardingEmailAddress'] = email_feedback
+            
         return params
 
     def _get_v1_parameters(self, message, source):
         """V1-Style raw payload for `send_raw_email`
 
         https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/ses.html#SES.Client.send_raw_email
         """
```

### Comparing `django_ses-3.4.0/django_ses/management/commands/get_ses_statistics.py` & `django_ses-3.4.1/django_ses/management/commands/get_ses_statistics.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/django_ses/management/commands/ses_email_address.py` & `django_ses-3.4.1/django_ses/management/commands/ses_email_address.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/django_ses/migrations/0001_initial.py` & `django_ses-3.4.1/django_ses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/django_ses/settings.py` & `django_ses-3.4.1/django_ses/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/django_ses/templates/django_ses/send_stats.html` & `django_ses-3.4.1/django_ses/templates/django_ses/send_stats.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/django_ses/utils.py` & `django_ses-3.4.1/django_ses/utils.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/django_ses/views.py` & `django_ses-3.4.1/django_ses/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/example/settings.py` & `django_ses-3.4.1/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/example/templates/send-email.html` & `django_ses-3.4.1/example/templates/send-email.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/example/urls.py` & `django_ses-3.4.1/example/urls.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/example/views.py` & `django_ses-3.4.1/example/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/pyproject.toml` & `django_ses-3.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ses"
-version = "3.4.0"
+version = "3.4.1"
 description = "A Django email backend for Amazon's Simple Email Service"
 authors = [
     "Harry Marr <harry@hmarr.com>",
     "Wes Winham <winhamwr@gmail.com>",
     "Ross Lawley <ross.lawley@gmail.com>",
     "Paul Craciunoiu <paul@craciunoiu.net>",
 ]
```

### Comparing `django_ses-3.4.0/tests/test_backend.py` & `django_ses-3.4.1/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/tests/test_commands.py` & `django_ses-3.4.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/tests/test_settings.py` & `django_ses-3.4.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/tests/test_stats.py` & `django_ses-3.4.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/tests/test_verifier.py` & `django_ses-3.4.1/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/tests/test_views.py` & `django_ses-3.4.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.0/PKG-INFO` & `django_ses-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ses
-Version: 3.4.0
+Version: 3.4.1
 Summary: A Django email backend for Amazon's Simple Email Service
 Home-page: https://github.com/django-ses/django-ses
 License: MIT
 Author: Harry Marr
 Author-email: harry@hmarr.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -516,23 +516,28 @@
 ``AWS_SES_REGION_NAME``, ``AWS_SES_REGION_ENDPOINT``
   Optionally specify what region your SES service is using. Note that this is
   required if your SES service is not using us-east-1, as omitting these settings
   implies this region. Details:
   http://readthedocs.org/docs/boto/en/latest/ref/ses.html#boto.ses.regions
   http://docs.aws.amazon.com/general/latest/gr/rande.html
 
+``USE_SES_V2``
+  Optional. If you want to use client v2, you'll need to add `USE_SES_V2=True`. 
+  Some settings will need this flag enabled.
+  See https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#id87
+
 ``AWS_SES_FROM_EMAIL``
   Optional. The email address to be used as the "From" address for the email. The address that you specify has to be verified.  
   For more information please refer to https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/sesv2.html#SESV2.Client.send_email
+
 ``AWS_SES_RETURN_PATH``
   Optional. Use `AWS_SES_RETURN_PATH` to receive complaint notifications
   You must use the v2 client by setting `USE_SES_V2=True` for this setting to work, otherwise it is ignored.
   https://docs.aws.amazon.com/ses/latest/APIReference-V2/API_SendEmail.html#API_SendEmail_RequestSyntax
 
-
 ``AWS_SES_CONFIGURATION_SET``
   Optional. Use this to mark your e-mails as from being from a particular SES
   Configuration Set. Set this to a string if you want all messages to have the
   same configuration set.  Set this to a callable if you want to set
   configuration set on a per message basis.
 
 ``TIME_ZONE``
```

