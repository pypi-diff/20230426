# Comparing `tmp/drf-social-oauth2-2.1.0.tar.gz` & `tmp/drf-social-oauth2-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-social-oauth2-2.1.0.tar", last modified: Mon Apr 24 13:22:46 2023, max compression
+gzip compressed data, was "drf-social-oauth2-2.1.1.tar", last modified: Wed Apr 26 12:03:38 2023, max compression
```

## Comparing `drf-social-oauth2-2.1.0.tar` & `drf-social-oauth2-2.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.647394 drf-social-oauth2-2.1.0/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     6286 2023-04-24 13:22:06.000000 drf-social-oauth2-2.1.0/CHANGELOG.rst
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.0/LICENSE.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.0/MANIFEST.in
--rw-r--r--   0 wagner.delima   (502) staff       (20)    20761 2023-04-24 13:22:46.647057 drf-social-oauth2-2.1.0/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)    19961 2023-04-24 12:27:32.000000 drf-social-oauth2-2.1.0/README.rst
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.639953 drf-social-oauth2-2.1.0/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-24 12:27:32.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-16 14:33:15.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_grants.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      945 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/serializers.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2036 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/test_settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2288 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/urls.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     9065 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/views.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.643203 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/
--rw-r--r--   0 wagner.delima   (502) staff       (20)    20761 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/requires.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/top_level.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.0/pyproject.toml
--rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-24 13:22:46.647489 drf-social-oauth2-2.1.0/setup.cfg
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.1.0/setup.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.643553 drf-social-oauth2-2.1.0/tests/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.0/tests/__init__.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.646287 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/drf_fixtures.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4268 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     7034 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.893978 drf-social-oauth2-2.1.1/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     6286 2023-04-24 13:22:06.000000 drf-social-oauth2-2.1.1/CHANGELOG.rst
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.1/LICENSE.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.1/MANIFEST.in
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-26 12:03:38.893609 drf-social-oauth2-2.1.1/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      933 2023-04-25 12:21:07.000000 drf-social-oauth2-2.1.1/README.rst
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.884583 drf-social-oauth2-2.1.1/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-26 11:59:21.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-16 14:33:15.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_grants.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      945 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/serializers.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2036 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/test_settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2288 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/urls.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     8784 2023-04-26 11:59:21.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.888647 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/requires.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.1/pyproject.toml
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-26 12:03:38.894089 drf-social-oauth2-2.1.1/setup.cfg
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.1.1/setup.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.889415 drf-social-oauth2-2.1.1/tests/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.1/tests/__init__.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.892630 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/drf_fixtures.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4268 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7034 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_views.py
```

### Comparing `drf-social-oauth2-2.1.0/CHANGELOG.rst` & `drf-social-oauth2-2.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/LICENSE.txt` & `drf-social-oauth2-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/__init__.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 drf-social-oauth2 offers support to oauth2 authentication and authorization.
 It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application.
 By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter
 and a ton more!
 """
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 try:
     from secrets import SystemRandom
 except ImportError:
     from random import SystemRandom
```

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/authentication.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/backends.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_backends.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_endpoints.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_grants.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_grants.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/serializers.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/settings.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/test_settings.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/test_settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/urls.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/urls.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2/views.py` & `drf-social-oauth2-2.1.1/drf_social_oauth2/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,18 +76,15 @@
             return Response(
                 data={
                     'invalid_grant': 'The access token of your Refresh Token does not exist.'
                 },
                 status=HTTP_400_BAD_REQUEST,
             )
 
-        response = Response(data=json_loads(body), status=status)
-        for k, v in headers.items():
-            response[k] = v
-        return response
+        return Response(data=json_loads(body), status=status)
 
 
 class ConvertTokenView(CsrfExemptMixin, OAuthLibMixin, APIView):
     """
     Implements an endpoint to convert a provider token to an access token
 
     The endpoint is used in the following flows:
@@ -133,19 +130,15 @@
             )
         except AccessDeniedError:
             return Response(
                 {'access_denied': f'The token you provided is invalid or expired.'},
                 status=HTTP_400_BAD_REQUEST,
             )
 
-        response = Response(data=json_loads(body), status=status)
-
-        for k, v in headers.items():
-            response[k] = v
-        return response
+        return Response(data=json_loads(body), status=status)
 
 
 class RevokeTokenView(CsrfExemptMixin, OAuthLibMixin, APIView):
     """
     Implements an endpoint to revoke access or refresh tokens
     """
 
@@ -159,22 +152,18 @@
         serializer.is_valid(raise_exception=True)
         # Use the rest framework `.data` to fake the post body of the django request.
         request._request.POST = request._request.POST.copy()
         for key, value in serializer.validated_data.items():
             request._request.POST[key] = value
 
         url, headers, body, status = self.create_revocation_response(request._request)
-        response = Response(
+        return Response(
             data=json_loads(body) if body else '', status=status if body else 204
         )
 
-        for k, v in headers.items():
-            response[k] = v
-        return response
-
 
 class InvalidateSessions(APIView):
     """
     Delete all access tokens associated with a client id.
     """
 
     permission_classes = (IsAuthenticated,)
```

### Comparing `drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/SOURCES.txt` & `drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/setup.py` & `drf-social-oauth2-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/tests/drf_social_oauth2/drf_fixtures.py` & `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/drf_fixtures.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_authentication.py` & `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_oauth2_endpoints.py` & `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_views.py` & `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_views.py`

 * *Files identical despite different names*

