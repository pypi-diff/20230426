# Comparing `tmp/django-seal-1.5.0.tar.gz` & `tmp/django-seal-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-seal-1.5.0.tar", last modified: Mon Feb 20 05:08:06 2023, max compression
+gzip compressed data, was "dist/django-seal-1.5.1.tar", last modified: Wed Apr 26 14:11:55 2023, max compression
```

## Comparing `django-seal-1.5.0.tar` & `django-seal-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:08:06.000000 django-seal-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-20 05:07:56.000000 django-seal-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-02-20 05:08:06.000000 django-seal-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-02-20 05:07:56.000000 django-seal-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:08:06.000000 django-seal-1.5.0/django_seal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-02-20 05:08:06.000000 django-seal-1.5.0/django_seal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-20 05:08:06.000000 django-seal-1.5.0/django_seal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 05:08:06.000000 django-seal-1.5.0/django_seal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-20 05:08:06.000000 django-seal-1.5.0/django_seal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 05:08:06.000000 django-seal-1.5.0/django_seal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:08:06.000000 django-seal-1.5.0/seal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 05:07:56.000000 django-seal-1.5.0/seal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-02-20 05:07:56.000000 django-seal-1.5.0/seal/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-20 05:07:56.000000 django-seal-1.5.0/seal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-02-20 05:07:56.000000 django-seal-1.5.0/seal/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-20 05:07:56.000000 django-seal-1.5.0/seal/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-20 05:08:06.000000 django-seal-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-02-20 05:07:56.000000 django-seal-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:08:06.000000 django-seal-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-02-20 05:07:56.000000 django-seal-1.5.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    26069 2023-02-20 05:07:56.000000 django-seal-1.5.0/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:11:55.000000 django-seal-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 14:11:39.000000 django-seal-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-26 14:11:55.000000 django-seal-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-26 14:11:39.000000 django-seal-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:11:55.000000 django-seal-1.5.1/django_seal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-26 14:11:55.000000 django-seal-1.5.1/django_seal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 14:11:55.000000 django-seal-1.5.1/django_seal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:11:55.000000 django-seal-1.5.1/django_seal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 14:11:55.000000 django-seal-1.5.1/django_seal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 14:11:55.000000 django-seal-1.5.1/django_seal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:11:55.000000 django-seal-1.5.1/seal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:11:39.000000 django-seal-1.5.1/seal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-04-26 14:11:39.000000 django-seal-1.5.1/seal/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 14:11:39.000000 django-seal-1.5.1/seal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-26 14:11:39.000000 django-seal-1.5.1/seal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-26 14:11:39.000000 django-seal-1.5.1/seal/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-26 14:11:55.000000 django-seal-1.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2023-04-26 14:11:39.000000 django-seal-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:11:55.000000 django-seal-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-04-26 14:11:39.000000 django-seal-1.5.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26421 2023-04-26 14:11:39.000000 django-seal-1.5.1/tests/test_query.py
```

### Comparing `django-seal-1.5.0/LICENSE` & `django-seal-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-seal-1.5.0/PKG-INFO` & `django-seal-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-seal
-Version: 1.5.0
+Version: 1.5.1
 Summary: Allows ORM constructs to be sealed to prevent them from executing queries on attribute accesses.
 Home-page: https://github.com/charettes/django-seal
 Author: Simon Charette
 Author-email: simon.charette@zapier.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-seal-1.5.0/README.rst` & `django-seal-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-seal-1.5.0/django_seal.egg-info/PKG-INFO` & `django-seal-1.5.1/django_seal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-seal
-Version: 1.5.0
+Version: 1.5.1
 Summary: Allows ORM constructs to be sealed to prevent them from executing queries on attribute accesses.
 Home-page: https://github.com/charettes/django-seal
 Author: Simon Charette
 Author-email: simon.charette@zapier.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-seal-1.5.0/seal/descriptors.py` & `django-seal-1.5.1/seal/descriptors.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,21 @@
     def _fetch_all(self):
         if self._result_cache is None:
             warnings.warn(
                 self._sealed_warning, category=UnsealedAttributeAccess, stacklevel=3
             )
         super()._fetch_all()
 
+    def __reduce__(self):
+        return (
+            _unpickle_sealed_related_queryset,
+            (self._unsealed_class,),
+            self.__getstate__(),
+        )
+
 
 class SealedPrefetchMixin(object):
     def _get_default_prefetch_queryset(self):
         return self.get_queryset()
 
     def get_prefetch_queryset(self, instances, queryset=None):
         if queryset is None:
@@ -76,14 +83,19 @@
         (_SealedRelatedQuerySet, queryset_cls),
         {
             "_unsealed_class": queryset_cls,
         },
     )
 
 
+def _unpickle_sealed_related_queryset(queryset_cls):
+    cls = _sealed_related_queryset_type_factory(queryset_cls)
+    return cls.__new__(cls)
+
+
 def seal_related_queryset(queryset, warning):
     """
     Seal a related queryset to prevent it from being fetched directly.
     """
     queryset.__class__ = _sealed_related_queryset_type_factory(queryset.__class__)
     queryset._sealed_warning = warning
     return queryset
```

### Comparing `django-seal-1.5.0/seal/models.py` & `django-seal-1.5.1/seal/models.py`

 * *Files identical despite different names*

### Comparing `django-seal-1.5.0/seal/query.py` & `django-seal-1.5.1/seal/query.py`

 * *Files identical despite different names*

### Comparing `django-seal-1.5.0/setup.py` & `django-seal-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open('README.rst') as file_:
     long_description = file_.read()
 
 setup(
     name='django-seal',
-    version='1.5.0',
+    version='1.5.1',
     description=(
         'Allows ORM constructs to be sealed to prevent them from executing '
         'queries on attribute accesses.'
     ),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://github.com/charettes/django-seal',
@@ -24,14 +24,15 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `django-seal-1.5.0/tests/test_models.py` & `django-seal-1.5.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-seal-1.5.0/tests/test_query.py` & `django-seal-1.5.1/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pickle
 import warnings
 
 from django.apps import apps
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.db.models import Prefetch
 from django.db.models.query import ModelIterable
@@ -500,14 +501,21 @@
                 SeaGull.objects.seal().prefetch_related("nicknames").order_by("pk")
             )
         self.assertEqual(results, [self.gull, other_gull])
         with self.assertNumQueries(0):
             self.assertEqual(list(results[0].nicknames.all()), [self.nickname])
             self.assertEqual(list(results[1].nicknames.all()), [other_nickname])
 
+    def test_related_sealed_pickleability(self):
+        location = Location.objects.prefetch_related("climates").seal().get()
+        climates_dump = pickle.dumps(location.climates.all())
+        climates = pickle.loads(climates_dump)
+        with self.assertNumQueries(0):
+            self.assertEqual(list(climates)[0], self.climate)
+
 
 class SealableQuerySetInteractionTests(SimpleTestCase):
     def test_values_seal_disallowed(self):
         with self.assertRaisesMessage(
             TypeError, "Cannot call seal() after .values() or .values_list()"
         ):
             SeaGull.objects.values("id").seal()
```

