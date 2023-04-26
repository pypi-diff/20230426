# Comparing `tmp/django-better-image-0.0.2.tar.gz` & `tmp/django-better-image-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-better-image-0.0.2.tar", last modified: Fri Jul 19 13:39:37 2019, max compression
+gzip compressed data, was "dist/django-better-image-0.0.4.tar", last modified: Wed Apr 26 15:48:57 2023, max compression
```

## Comparing `django-better-image-0.0.2.tar` & `django-better-image-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2019-07-19 13:39:37.000000 django-better-image-0.0.2/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       38 2019-07-19 13:39:37.000000 django-better-image-0.0.2/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       94 2019-07-19 13:36:17.000000 django-better-image-0.0.2/README.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2068 2019-07-19 13:38:26.000000 django-better-image-0.0.2/setup.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      230 2019-07-19 13:38:59.000000 django-better-image-0.0.2/django_better_image/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1135 2019-07-19 13:39:37.000000 django-better-image-0.0.2/PKG-INFO
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2019-07-19 13:34:16.000000 django-better-image-0.0.2/django_better_image.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      307 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       20 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       57 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1135 2019-07-19 13:39:37.000000 django-better-image-0.0.2/django_better_image.egg-info/PKG-INFO
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-04-26 15:48:57.000000 django-better-image-0.0.4/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image/
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     2691 2019-08-25 09:30:23.000000 django-better-image-0.0.4/django_better_image/forms.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     1002 2019-08-25 09:30:23.000000 django-better-image-0.0.4/django_better_image/fields.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      230 2019-08-27 07:39:22.000000 django-better-image-0.0.4/django_better_image/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image/templatetags/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2019-08-27 07:39:22.000000 django-better-image-0.0.4/django_better_image/templatetags/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      454 2019-08-27 07:39:22.000000 django-better-image-0.0.4/django_better_image/templatetags/django_better_image.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)      526 2022-06-08 10:18:15.000000 django-better-image-0.0.4/django_better_image/urls.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     3890 2019-08-25 09:30:23.000000 django-better-image-0.0.4/django_better_image/formfields.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     6733 2019-10-03 16:09:45.000000 django-better-image-0.0.4/django_better_image/views.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     6506 2022-06-02 14:21:24.000000 django-better-image-0.0.4/django_better_image/widgets.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       38 2023-04-26 15:48:57.000000 django-better-image-0.0.4/setup.cfg
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image.egg-info/
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)        1 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image.egg-info/dependency_links.txt
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)        1 2019-08-25 12:54:09.000000 django-better-image-0.0.4/django_better_image.egg-info/not-zip-safe
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)       64 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image.egg-info/requires.txt
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)     1058 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image.egg-info/PKG-INFO
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)       20 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image.egg-info/top_level.txt
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)      597 2023-04-26 15:48:57.000000 django-better-image-0.0.4/django_better_image.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2022-06-02 14:19:11.000000 django-better-image-0.0.4/setup.py
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)    26526 2019-08-25 09:30:23.000000 django-better-image-0.0.4/LICENSE
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1058 2023-04-26 15:48:57.000000 django-better-image-0.0.4/PKG-INFO
+-rw-r--r--   0 elapouya  (1000) elapouya  (1000)       94 2019-08-25 09:30:23.000000 django-better-image-0.0.4/README.rst
```

### Comparing `django-better-image-0.0.2/setup.py` & `django-better-image-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup,find_packages
+from setuptools import setup, find_packages
 import os
 import re
 
 
 def read(*names):
     values = dict()
     for name in names:
@@ -55,15 +55,16 @@
           "Programming Language :: Python :: 3.6",
       ],
       keywords='ImageField',
       url='https://github.com/elapouya/django-better-image',
       author='Eric Lapouyade',
       author_email='elapouya@gmail.com',
       license='LGPL 2.1',
-      packages=find_packages(exclude=['tests.*','tests','docs.*','docs']),
-      package_data={'': ['*.png',],},
-      install_requires=['django>=2',],
+      packages=find_packages(exclude=['tests.*', 'tests', 'docs.*', 'docs']),
+      package_data={'': ['*.png', ], },
+      install_requires=['django>=3',
+                        'pillow', ],
       extras_require={
         'tests' : [],
         'docs': ['Sphinx', 'sphinxcontrib-napoleon'],
       },
       zip_safe=False)
```

### Comparing `django-better-image-0.0.2/PKG-INFO` & `django-better-image-0.0.4/django_better_image.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 Metadata-Version: 2.1
 Name: django-better-image
-Version: 0.0.2
+Version: 0.0.4
 Summary: Better Django ImageField
 Home-page: https://github.com/elapouya/django-better-image
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: LGPL 2.1
-Description: 
-        ===================
-        django-better-image
-        ===================
-        
-        Django app for better ImageField
-        
-        
-        News
-        ====
-        
-        
 Keywords: ImageField
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
@@ -29,9 +17,24 @@
 Classifier: Framework :: Django :: 2.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
+
+===================
+django-better-image
+===================
+
+Django app for better ImageField
+
+
+News
+====
+
+
+
```

### Comparing `django-better-image-0.0.2/django_better_image.egg-info/PKG-INFO` & `django-better-image-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 Metadata-Version: 2.1
 Name: django-better-image
-Version: 0.0.2
+Version: 0.0.4
 Summary: Better Django ImageField
 Home-page: https://github.com/elapouya/django-better-image
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: LGPL 2.1
-Description: 
-        ===================
-        django-better-image
-        ===================
-        
-        Django app for better ImageField
-        
-        
-        News
-        ====
-        
-        
 Keywords: ImageField
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
@@ -29,9 +17,24 @@
 Classifier: Framework :: Django :: 2.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
+
+===================
+django-better-image
+===================
+
+Django app for better ImageField
+
+
+News
+====
+
+
+
```

