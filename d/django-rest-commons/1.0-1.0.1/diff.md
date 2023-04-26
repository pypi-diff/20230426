# Comparing `tmp/django_rest_commons-1.0.tar.gz` & `tmp/django_rest_commons-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rest_commons-1.0.tar", last modified: Tue Apr 25 22:43:23 2023, max compression
+gzip compressed data, was "django_rest_commons-1.0.1.tar", last modified: Wed Apr 26 03:09:07 2023, max compression
```

## Comparing `django_rest_commons-1.0.tar` & `django_rest_commons-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,16 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-04-25 22:43:23.193032 django_rest_commons-1.0/
--rw-r--r--   0 leondaz    (501) staff       (20)      273 2023-04-25 22:43:23.193077 django_rest_commons-1.0/PKG-INFO
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-04-25 22:43:23.193007 django_rest_commons-1.0/django_rest_commons/
--rw-r--r--   0 leondaz    (501) staff       (20)      144 2023-04-25 21:24:24.467213 django_rest_commons-1.0/django_rest_commons/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2471 2023-04-25 22:01:39.479409 django_rest_commons-1.0/django_rest_commons/mixins.py
--rw-r--r--   0 leondaz    (501) staff       (20)     3261 2023-04-25 21:21:45.545122 django_rest_commons-1.0/django_rest_commons/serializers.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2208 2023-04-25 22:11:45.770300 django_rest_commons-1.0/django_rest_commons/viewsets.py
--rw-r--r--   0 leondaz    (501) staff       (20)      309 2023-04-25 22:42:40.615373 django_rest_commons-1.0/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-04-26 03:09:07.520226 django_rest_commons-1.0.1/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1062 2023-04-25 22:48:42.000000 django_rest_commons-1.0.1/LICENSE.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)      245 2023-04-26 03:09:07.520099 django_rest_commons-1.0.1/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     1737 2023-04-25 22:51:44.000000 django_rest_commons-1.0.1/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-04-26 03:09:07.519537 django_rest_commons-1.0.1/django_rest_commons/
+-rw-r--r--   0 leondaz    (501) staff       (20)      144 2023-04-25 21:24:24.000000 django_rest_commons-1.0.1/django_rest_commons/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2697 2023-04-26 03:06:40.000000 django_rest_commons-1.0.1/django_rest_commons/mixins.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     3273 2023-04-26 03:06:44.000000 django_rest_commons-1.0.1/django_rest_commons/serializers.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2208 2023-04-25 22:11:45.000000 django_rest_commons-1.0.1/django_rest_commons/viewsets.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-04-26 03:09:07.519952 django_rest_commons-1.0.1/django_rest_commons.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      245 2023-04-26 03:09:07.000000 django_rest_commons-1.0.1/django_rest_commons.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      331 2023-04-26 03:09:07.000000 django_rest_commons-1.0.1/django_rest_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-04-26 03:09:07.000000 django_rest_commons-1.0.1/django_rest_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       20 2023-04-26 03:09:07.000000 django_rest_commons-1.0.1/django_rest_commons.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-04-26 03:09:07.520259 django_rest_commons-1.0.1/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      312 2023-04-26 03:09:01.000000 django_rest_commons-1.0.1/setup.py
```

### Comparing `django_rest_commons-1.0/django_rest_commons/mixins.py` & `django_rest_commons-1.0.1/django_rest_commons/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from rest_framework import status
 from rest_framework.mixins import CreateModelMixin as BaseCreateModelMixin
 from rest_framework.mixins import UpdateModelMixin as BaseUpdateModelMixin
 from rest_framework.response import Response
 
 
 class CommonCreateModelMixin(BaseCreateModelMixin):
-    """Allows create to use get_input_serializer & get_output_serializer"""
+    """Allows the create action to use get_input_serializer & get_output_serializer"""
 
     def create(self, request, *args, **kwargs):
         input_serializer = self.get_input_serializer(data=request.data)
         input_serializer.is_valid(raise_exception=True)
 
         instance = self.perform_create(input_serializer)
         output_serializer = self.get_output_serializer(instance)
@@ -51,19 +51,25 @@
     """Can take in input_serializer & output_serializer in update or create. So the request body doesn't have to match
     the response body.
     """
 
     input_serializer_class = None
     output_serializer_class = None
 
-    def get_output_serializer(self):
+    def get_output_serializer(self, *args, **kwargs):
         """
         Returns the output serializer
         :return:
         """
-        return self.output_serializer_class or self.serializer_class
+        if self.output_serializer_class:
+            return self.output_serializer_class(*args, **kwargs)
 
-    def get_input_serializer(self):
+        return self.get_serializer(*args, **kwargs)
+
+    def get_input_serializer(self, *args, **kwargs):
         """
         Returns the input serializer
         """
-        return self.input_serializer_class or self.serializer_class
+        if self.input_serializer_class:
+            return self.input_serializer_class(*args, **kwargs)
+
+        return self.serializer_class(*args, **kwargs)
```

### Comparing `django_rest_commons-1.0/django_rest_commons/serializers.py` & `django_rest_commons-1.0.1/django_rest_commons/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return self.parent.__class__(value).data
 
 
 class EnumSerializer(serializers.BaseSerializer):
     """A serializer for enums
 
     :param enum: The enum to serialize
-    :type enum: enum.Enum
+    :type enum: instance of enum.Enum
 
     .. code-block:: python
         :caption: models.py
 
         class Human(models.Model):
             class Level(models.IntegerChoices):
                 BEGINNER = 0
```

### Comparing `django_rest_commons-1.0/django_rest_commons/viewsets.py` & `django_rest_commons-1.0.1/django_rest_commons/viewsets.py`

 * *Files identical despite different names*

