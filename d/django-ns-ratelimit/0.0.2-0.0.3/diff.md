# Comparing `tmp/django-ns-ratelimit-0.0.2.tar.gz` & `tmp/django-ns-ratelimit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ns-ratelimit-0.0.2.tar", last modified: Wed Apr 26 10:51:29 2023, max compression
+gzip compressed data, was "django-ns-ratelimit-0.0.3.tar", last modified: Wed Apr 26 10:57:41 2023, max compression
```

## Comparing `django-ns-ratelimit-0.0.2.tar` & `django-ns-ratelimit-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 nonstopio  (1000) nonstopio  (1000)        0 2023-04-26 10:51:29.021216 django-ns-ratelimit-0.0.2/
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     3189 2023-04-26 10:51:29.021216 django-ns-ratelimit-0.0.2/PKG-INFO
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     1624 2023-04-26 10:50:40.000000 django-ns-ratelimit-0.0.2/README.rst
-drwxrwxr-x   0 nonstopio  (1000) nonstopio  (1000)        0 2023-04-26 10:51:29.021216 django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     3189 2023-04-26 10:51:28.000000 django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/PKG-INFO
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)      328 2023-04-26 10:51:29.000000 django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/SOURCES.txt
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)        1 2023-04-26 10:51:28.000000 django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/dependency_links.txt
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       15 2023-04-26 10:51:28.000000 django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/requires.txt
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       10 2023-04-26 10:51:28.000000 django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/top_level.txt
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       89 2023-04-24 18:52:48.000000 django-ns-ratelimit-0.0.2/pyproject.toml
-drwxrwxr-x   0 nonstopio  (1000) nonstopio  (1000)        0 2023-04-26 10:51:29.021216 django-ns-ratelimit-0.0.2/ratelimit/
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     2551 2023-04-26 10:29:07.000000 django-ns-ratelimit-0.0.2/ratelimit/__init__.py
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     2173 2023-04-24 21:19:16.000000 django-ns-ratelimit-0.0.2/ratelimit/decorators.py
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     1494 2023-04-25 10:25:12.000000 django-ns-ratelimit-0.0.2/ratelimit/middleware.py
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)      843 2023-04-26 10:51:29.021216 django-ns-ratelimit-0.0.2/setup.cfg
--rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       83 2023-04-24 21:37:20.000000 django-ns-ratelimit-0.0.2/setup.py
+drwxrwxr-x   0 nonstopio  (1000) nonstopio  (1000)        0 2023-04-26 10:57:41.009230 django-ns-ratelimit-0.0.3/
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     3084 2023-04-26 10:57:41.009230 django-ns-ratelimit-0.0.3/PKG-INFO
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     1527 2023-04-26 10:54:10.000000 django-ns-ratelimit-0.0.3/README.rst
+drwxrwxr-x   0 nonstopio  (1000) nonstopio  (1000)        0 2023-04-26 10:57:41.009230 django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     3084 2023-04-26 10:57:40.000000 django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/PKG-INFO
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)      328 2023-04-26 10:57:40.000000 django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)        1 2023-04-26 10:57:40.000000 django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       15 2023-04-26 10:57:40.000000 django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/requires.txt
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       10 2023-04-26 10:57:40.000000 django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/top_level.txt
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       89 2023-04-24 18:52:48.000000 django-ns-ratelimit-0.0.3/pyproject.toml
+drwxrwxr-x   0 nonstopio  (1000) nonstopio  (1000)        0 2023-04-26 10:57:41.009230 django-ns-ratelimit-0.0.3/ratelimit/
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     2551 2023-04-26 10:29:07.000000 django-ns-ratelimit-0.0.3/ratelimit/__init__.py
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     2173 2023-04-24 21:19:16.000000 django-ns-ratelimit-0.0.3/ratelimit/decorators.py
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)     1494 2023-04-25 10:25:12.000000 django-ns-ratelimit-0.0.3/ratelimit/middleware.py
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)      905 2023-04-26 10:57:41.009230 django-ns-ratelimit-0.0.3/setup.cfg
+-rw-rw-r--   0 nonstopio  (1000) nonstopio  (1000)       83 2023-04-24 21:37:20.000000 django-ns-ratelimit-0.0.3/setup.py
```

### Comparing `django-ns-ratelimit-0.0.2/PKG-INFO` & `django-ns-ratelimit-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 Metadata-Version: 2.1
 Name: django-ns-ratelimit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django app for limit authorized and anonymous users.
-Home-page: UNKNOWN
+Home-page: https://github.com/shaileshkumar123/django-ns-ratelimit
 Author: shailesh jadhav
 License: UNKNOWN
 Description: # DJANGO-NS-RATELIMIT
         
         ## Project description
         django-ns-ratelimit is django app for limit requests using rate limit class, decorators and middleware.
         
-        ## Installation
-        
-        ```
-        pip install -i https://test.pypi.org/simple/ django-ns-ratelimit==1.0
-        ```
-        
-        
         ## Usage
         
         # Periods in format:
         ```
             S: For seconds
             M: For minutes
             H: For hour
```

### Comparing `django-ns-ratelimit-0.0.2/README.rst` & `django-ns-ratelimit-0.0.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 # DJANGO-NS-RATELIMIT
 
 ## Project description
 django-ns-ratelimit is django app for limit requests using rate limit class, decorators and middleware.
 
-## Installation
-
-```
-pip install -i https://test.pypi.org/simple/ django-ns-ratelimit==1.0
-```
-
-
 ## Usage
 
 # Periods in format:
 ```
     S: For seconds
     M: For minutes
     H: For hour
```

### Comparing `django-ns-ratelimit-0.0.2/django_ns_ratelimit.egg-info/PKG-INFO` & `django-ns-ratelimit-0.0.3/django_ns_ratelimit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 Metadata-Version: 2.1
 Name: django-ns-ratelimit
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django app for limit authorized and anonymous users.
-Home-page: UNKNOWN
+Home-page: https://github.com/shaileshkumar123/django-ns-ratelimit
 Author: shailesh jadhav
 License: UNKNOWN
 Description: # DJANGO-NS-RATELIMIT
         
         ## Project description
         django-ns-ratelimit is django app for limit requests using rate limit class, decorators and middleware.
         
-        ## Installation
-        
-        ```
-        pip install -i https://test.pypi.org/simple/ django-ns-ratelimit==1.0
-        ```
-        
-        
         ## Usage
         
         # Periods in format:
         ```
             S: For seconds
             M: For minutes
             H: For hour
```

### Comparing `django-ns-ratelimit-0.0.2/ratelimit/__init__.py` & `django-ns-ratelimit-0.0.3/ratelimit/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ns-ratelimit-0.0.2/ratelimit/decorators.py` & `django-ns-ratelimit-0.0.3/ratelimit/decorators.py`

 * *Files identical despite different names*

### Comparing `django-ns-ratelimit-0.0.2/ratelimit/middleware.py` & `django-ns-ratelimit-0.0.3/ratelimit/middleware.py`

 * *Files identical despite different names*

### Comparing `django-ns-ratelimit-0.0.2/setup.cfg` & `django-ns-ratelimit-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [metadata]
 name = django-ns-ratelimit
-version = v0.0.2
+version = v0.0.3
 description = A Django app for limit authorized and anonymous users.
 long_description = file: README.rst
 author = shailesh jadhav
+url = https://github.com/shaileshkumar123/django-ns-ratelimit
 github = https://github.com/shaileshkumar123/django-ns-ratelimit
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Intended Audience :: Developers
 	Operating System :: OS Independent
```

