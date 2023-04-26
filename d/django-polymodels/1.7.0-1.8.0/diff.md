# Comparing `tmp/django-polymodels-1.7.0.tar.gz` & `tmp/django-polymodels-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-polymodels-1.7.0.tar", last modified: Sat Mar 20 06:21:10 2021, max compression
+gzip compressed data, was "dist/django-polymodels-1.8.0.tar", last modified: Tue Apr 25 15:00:12 2023, max compression
```

## Comparing `django-polymodels-1.7.0.tar` & `django-polymodels-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 06:21:10.000000 django-polymodels-1.7.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1424 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-03-20 06:21:10.000000 django-polymodels-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 06:21:10.000000 django-polymodels-1.7.0/django_polymodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-20 06:21:09.000000 django-polymodels-1.7.0/django_polymodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-03-20 06:21:10.000000 django-polymodels-1.7.0/django_polymodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7343 2021-03-20 06:21:09.000000 django-polymodels-1.7.0/django_polymodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-20 06:21:09.000000 django-polymodels-1.7.0/django_polymodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-20 06:21:09.000000 django-polymodels-1.7.0/django_polymodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 06:21:10.000000 django-polymodels-1.7.0/polymodels/
--rw-r--r--   0 runner    (1001) docker     (121)     7475 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/polymodels/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/polymodels/managers.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/polymodels/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/polymodels/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/polymodels/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/polymodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7343 2021-03-20 06:21:10.000000 django-polymodels-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-03-20 06:20:55.000000 django-polymodels-1.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/django_polymodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/django_polymodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/django_polymodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/django_polymodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/django_polymodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/django_polymodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/polymodels/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/polymodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/polymodels/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/polymodels/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/polymodels/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/polymodels/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/polymodels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1425 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:00:12.000000 django-polymodels-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 14:59:59.000000 django-polymodels-1.8.0/tests/test_related.py
```

### Comparing `django-polymodels-1.7.0/setup.py` & `django-polymodels-1.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,31 @@
     description='Polymorphic models implementation for django',
     long_description=long_desc,
     long_description_content_type='text/x-rst',
     url=github_url,
     author='Simon Charette',
     author_email='charette.s@gmail.com',
     install_requires=(
-        'Django>=2.2',
+        'Django>=3.2',
     ),
     packages=find_packages(exclude=['tests', 'tests.*']),
     include_package_data=True,
     license='MIT License',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
 )
```

### Comparing `django-polymodels-1.7.0/django_polymodels.egg-info/PKG-INFO` & `django-polymodels-1.8.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,190 +1,190 @@
 Metadata-Version: 2.1
 Name: django-polymodels
-Version: 1.7.0
+Version: 1.8.0
 Summary: Polymorphic models implementation for django
 Home-page: https://github.com/charettes/django-polymodels
 Author: Simon Charette
 Author-email: charette.s@gmail.com
 License: MIT License
-Description: #################
-        django-polymodels
-        #################
-        
-        A django application that provides a simple way to retrieve models type casted
-        to their original ``ContentType``.
-        
-        .. image:: https://travis-ci.org/charettes/django-polymodels.svg?branch=master
-            :target: https://travis-ci.org/charettes/django-polymodels
-        
-        .. image:: https://coveralls.io/repos/charettes/django-polymodels/badge.svg?branch=master&service=github
-            :target: https://coveralls.io/github/charettes/django-polymodels?branch=master
-        
-        ************
-        Installation
-        ************
-        
-        >>> pip install django-polymodels
-        
-        Make sure ``'django.contrib.contenttypes'`` and ``'polymodels'`` are in
-        your `INSTALLED_APPS`
-        
-        ::
-        
-            INSTALLED_APPS += ('django.contrib.contenttypes', 'polymodels')
-        
-        *****
-        Usage
-        *****
-        
-        Subclass ``PolymorphicModel``, an abstract model class.
-        
-        ::
-        
-            from django.db import models
-            from polymodels.models import PolymorphicModel
-        
-            class Animal(PolymorphicModel):
-                name = models.CharField(max_length=255)
-        
-                def __str__(self):
-                    return self.name
-        
-            class Mammal(Animal):
-                pass
-        
-            class Dog(Mammal):
-                pass
-        
-            class Reptile(Animal):
-                pass
-        
-            class Snake(Reptile):
-                class Meta:
-                    proxy = True
-        
-        Objects are created the same way as usual and their associated ``ContentType``
-        is saved automatically:
-        
-        >>> animal = Animal.objects.create(name='animal')
-        >>> mammal = Mammal.objects.create(name='mammal')
-        >>> reptile = Reptile.objects.create(name='reptile')
-        >>> snake = Snake.objects.create(name='snake')
-        
-        To retreive *type casted* instances from the ``Animal.objects`` manager you just
-        have to use the ``select_subclasses`` method.
-        
-        >>> Animal.objects.select_subclasses()
-        [<Animal: animal>, <Mammal: mammal>, <Reptile: reptile>, <Snake: snake>]
-        
-        You can also retreive a subset of the subclasses by passing them as arguments to
-        ``select_subclass``.
-        
-        >>> Animal.objects.select_subclasses(Reptile)
-        [<Reptile: reptile>, <Snake: snake>]
-        
-        Or directly from subclasses managers.
-        
-        >>> Reptile.objects.select_subclasses(Snake)
-        [<Snake: snake>]
-        
-        Note that you can also retrieve original results by avoiding the
-        ``select_subclasses`` call.
-        
-        >>> Animal.objects.all()
-        [<Animal: animal>, <Animal: mammal>, <Animal: reptile>, <Animal: snake>]
-        
-        It's also possible to select only instances of the model to which the
-        manager is attached by using the ``exclude_subclasses`` method.
-        
-        >>> Mammal.objects.all()
-        [<Mammal: mammal>]
-        
-        Each instance of ``PolymorphicModel`` has a ``type_cast`` method that knows how
-        to convert itself to the correct ``ContentType``.
-        
-        >>> animal_snake = Animal.objects.get(pk=snake.pk)
-        <Animal: snake>
-        >>> animal_snake.type_cast()
-        <Snake: snake>
-        >>> animal_snake.type_cast(Reptile)
-        <Reptile: snake>
-        
-        If the ``PolymorphicModel.content_type`` fields conflicts with one of your
-        existing fields you just have to subclass
-        ``polymodels.models.BasePolymorphicModel`` and specify which field *polymodels*
-        should use instead by defining a ``CONTENT_TYPE_FIELD`` attribute on your model.
-        This field must be a ``ForeignKey`` to ``ContentType``.
-        
-        ::
-        
-            from django.contrib.contenttypes.models import ContentType
-            from django.db import models
-            from polymodels.models import BasePolymorphicModel
-        
-            class MyModel(BasePolymorphicModel):
-                CONTENT_TYPE_FIELD = 'polymorphic_ct'
-                polymorphic_ct = models.ForeignKey(ContentType)
-        
-        ************
-        How it works
-        ************
-        
-        Under the hood ``select_subclasses`` calls ``seleted_related`` to avoid
-        unnecessary queries and ``filter`` if you pass some classes to it. On queryset
-        iteration, the fetched instanced are converted to their correct type by calling
-        ``BasePolymorphicModel.type_cast``. Note that those lookups are cached on class
-        creation to avoid computing them on every single query.
-        
-        
-        ******************
-        Note of the author
-        ******************
-        
-        I'm aware there's already plenty of existing projects tackling the whole
-        **model-inheritance-type-casting-thing** such as `django-polymorphic`_. However
-        I wanted to implement this feature in a lightweight way: no
-        ``__metaclass__`` or ``__init__`` overrides while using django's public API as
-        much as possible. In the end, this was really just an extraction of
-        `django-mutant`_'s own mecanism of handling this since I needed it as a
-        standalone app for another project.
-        
-        .. _django-polymorphic: https://github.com/chrisglass/django_polymorphic
-        .. _django-mutant: https://github.com/charettes/django-mutant
-        
-        
-        **********
-        Contribute
-        **********
-        
-        If you happen to encounter a bug or would like to suggest a feature addition
-        please `file an issue`_ or `create a pull request`_ containing **tests**.
-        
-        .. _file an issue: https://github.com/charettes/django-polymodels/issues
-        .. _create a pull request: https://github.com/charettes/django-polymodels/pulls
-        
-        *******
-        Credits
-        *******
-        
-        * Inspired by a `post of Jeff Elmores`_.
-        
-        .. _post of Jeff Elmores: http://jeffelmore.org/2010/11/11/automatic-downcasting-of-inherited-models-in-django/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+#################
+django-polymodels
+#################
+
+A django application that provides a simple way to retrieve models type casted
+to their original ``ContentType``.
+
+.. image:: https://travis-ci.org/charettes/django-polymodels.svg?branch=master
+    :target: https://travis-ci.org/charettes/django-polymodels
+
+.. image:: https://coveralls.io/repos/charettes/django-polymodels/badge.svg?branch=master&service=github
+    :target: https://coveralls.io/github/charettes/django-polymodels?branch=master
+
+************
+Installation
+************
+
+>>> pip install django-polymodels
+
+Make sure ``'django.contrib.contenttypes'`` and ``'polymodels'`` are in
+your `INSTALLED_APPS`
+
+::
+
+    INSTALLED_APPS += ('django.contrib.contenttypes', 'polymodels')
+
+*****
+Usage
+*****
+
+Subclass ``PolymorphicModel``, an abstract model class.
+
+::
+
+    from django.db import models
+    from polymodels.models import PolymorphicModel
+
+    class Animal(PolymorphicModel):
+        name = models.CharField(max_length=255)
+
+        def __str__(self):
+            return self.name
+
+    class Mammal(Animal):
+        pass
+
+    class Dog(Mammal):
+        pass
+
+    class Reptile(Animal):
+        pass
+
+    class Snake(Reptile):
+        class Meta:
+            proxy = True
+
+Objects are created the same way as usual and their associated ``ContentType``
+is saved automatically:
+
+>>> animal = Animal.objects.create(name='animal')
+>>> mammal = Mammal.objects.create(name='mammal')
+>>> reptile = Reptile.objects.create(name='reptile')
+>>> snake = Snake.objects.create(name='snake')
+
+To retreive *type casted* instances from the ``Animal.objects`` manager you just
+have to use the ``select_subclasses`` method.
+
+>>> Animal.objects.select_subclasses()
+[<Animal: animal>, <Mammal: mammal>, <Reptile: reptile>, <Snake: snake>]
+
+You can also retreive a subset of the subclasses by passing them as arguments to
+``select_subclass``.
+
+>>> Animal.objects.select_subclasses(Reptile)
+[<Reptile: reptile>, <Snake: snake>]
+
+Or directly from subclasses managers.
+
+>>> Reptile.objects.select_subclasses(Snake)
+[<Snake: snake>]
+
+Note that you can also retrieve original results by avoiding the
+``select_subclasses`` call.
+
+>>> Animal.objects.all()
+[<Animal: animal>, <Animal: mammal>, <Animal: reptile>, <Animal: snake>]
+
+It's also possible to select only instances of the model to which the
+manager is attached by using the ``exclude_subclasses`` method.
+
+>>> Mammal.objects.all()
+[<Mammal: mammal>]
+
+Each instance of ``PolymorphicModel`` has a ``type_cast`` method that knows how
+to convert itself to the correct ``ContentType``.
+
+>>> animal_snake = Animal.objects.get(pk=snake.pk)
+<Animal: snake>
+>>> animal_snake.type_cast()
+<Snake: snake>
+>>> animal_snake.type_cast(Reptile)
+<Reptile: snake>
+
+If the ``PolymorphicModel.content_type`` fields conflicts with one of your
+existing fields you just have to subclass
+``polymodels.models.BasePolymorphicModel`` and specify which field *polymodels*
+should use instead by defining a ``CONTENT_TYPE_FIELD`` attribute on your model.
+This field must be a ``ForeignKey`` to ``ContentType``.
+
+::
+
+    from django.contrib.contenttypes.models import ContentType
+    from django.db import models
+    from polymodels.models import BasePolymorphicModel
+
+    class MyModel(BasePolymorphicModel):
+        CONTENT_TYPE_FIELD = 'polymorphic_ct'
+        polymorphic_ct = models.ForeignKey(ContentType)
+
+************
+How it works
+************
+
+Under the hood ``select_subclasses`` calls ``seleted_related`` to avoid
+unnecessary queries and ``filter`` if you pass some classes to it. On queryset
+iteration, the fetched instanced are converted to their correct type by calling
+``BasePolymorphicModel.type_cast``. Note that those lookups are cached on class
+creation to avoid computing them on every single query.
+
+
+******************
+Note of the author
+******************
+
+I'm aware there's already plenty of existing projects tackling the whole
+**model-inheritance-type-casting-thing** such as `django-polymorphic`_. However
+I wanted to implement this feature in a lightweight way: no
+``__metaclass__`` or ``__init__`` overrides while using django's public API as
+much as possible. In the end, this was really just an extraction of
+`django-mutant`_'s own mecanism of handling this since I needed it as a
+standalone app for another project.
+
+.. _django-polymorphic: https://github.com/chrisglass/django_polymorphic
+.. _django-mutant: https://github.com/charettes/django-mutant
+
+
+**********
+Contribute
+**********
+
+If you happen to encounter a bug or would like to suggest a feature addition
+please `file an issue`_ or `create a pull request`_ containing **tests**.
+
+.. _file an issue: https://github.com/charettes/django-polymodels/issues
+.. _create a pull request: https://github.com/charettes/django-polymodels/pulls
+
+*******
+Credits
+*******
+
+* Inspired by a `post of Jeff Elmores`_.
+
+.. _post of Jeff Elmores: http://jeffelmore.org/2010/11/11/automatic-downcasting-of-inherited-models-in-django/
```

### Comparing `django-polymodels-1.7.0/polymodels/models.py` & `django-polymodels-1.8.0/polymodels/models.py`

 * *Files identical despite different names*

### Comparing `django-polymodels-1.7.0/polymodels/managers.py` & `django-polymodels-1.8.0/polymodels/managers.py`

 * *Files identical despite different names*

### Comparing `django-polymodels-1.7.0/polymodels/utils.py` & `django-polymodels-1.8.0/polymodels/utils.py`

 * *Files identical despite different names*

### Comparing `django-polymodels-1.7.0/polymodels/forms.py` & `django-polymodels-1.8.0/polymodels/forms.py`

 * *Files identical despite different names*

### Comparing `django-polymodels-1.7.0/polymodels/fields.py` & `django-polymodels-1.8.0/polymodels/fields.py`

 * *Files identical despite different names*

### Comparing `django-polymodels-1.7.0/README.rst` & `django-polymodels-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-polymodels-1.7.0/PKG-INFO` & `django-polymodels-1.8.0/django_polymodels.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,190 +1,190 @@
 Metadata-Version: 2.1
 Name: django-polymodels
-Version: 1.7.0
+Version: 1.8.0
 Summary: Polymorphic models implementation for django
 Home-page: https://github.com/charettes/django-polymodels
 Author: Simon Charette
 Author-email: charette.s@gmail.com
 License: MIT License
-Description: #################
-        django-polymodels
-        #################
-        
-        A django application that provides a simple way to retrieve models type casted
-        to their original ``ContentType``.
-        
-        .. image:: https://travis-ci.org/charettes/django-polymodels.svg?branch=master
-            :target: https://travis-ci.org/charettes/django-polymodels
-        
-        .. image:: https://coveralls.io/repos/charettes/django-polymodels/badge.svg?branch=master&service=github
-            :target: https://coveralls.io/github/charettes/django-polymodels?branch=master
-        
-        ************
-        Installation
-        ************
-        
-        >>> pip install django-polymodels
-        
-        Make sure ``'django.contrib.contenttypes'`` and ``'polymodels'`` are in
-        your `INSTALLED_APPS`
-        
-        ::
-        
-            INSTALLED_APPS += ('django.contrib.contenttypes', 'polymodels')
-        
-        *****
-        Usage
-        *****
-        
-        Subclass ``PolymorphicModel``, an abstract model class.
-        
-        ::
-        
-            from django.db import models
-            from polymodels.models import PolymorphicModel
-        
-            class Animal(PolymorphicModel):
-                name = models.CharField(max_length=255)
-        
-                def __str__(self):
-                    return self.name
-        
-            class Mammal(Animal):
-                pass
-        
-            class Dog(Mammal):
-                pass
-        
-            class Reptile(Animal):
-                pass
-        
-            class Snake(Reptile):
-                class Meta:
-                    proxy = True
-        
-        Objects are created the same way as usual and their associated ``ContentType``
-        is saved automatically:
-        
-        >>> animal = Animal.objects.create(name='animal')
-        >>> mammal = Mammal.objects.create(name='mammal')
-        >>> reptile = Reptile.objects.create(name='reptile')
-        >>> snake = Snake.objects.create(name='snake')
-        
-        To retreive *type casted* instances from the ``Animal.objects`` manager you just
-        have to use the ``select_subclasses`` method.
-        
-        >>> Animal.objects.select_subclasses()
-        [<Animal: animal>, <Mammal: mammal>, <Reptile: reptile>, <Snake: snake>]
-        
-        You can also retreive a subset of the subclasses by passing them as arguments to
-        ``select_subclass``.
-        
-        >>> Animal.objects.select_subclasses(Reptile)
-        [<Reptile: reptile>, <Snake: snake>]
-        
-        Or directly from subclasses managers.
-        
-        >>> Reptile.objects.select_subclasses(Snake)
-        [<Snake: snake>]
-        
-        Note that you can also retrieve original results by avoiding the
-        ``select_subclasses`` call.
-        
-        >>> Animal.objects.all()
-        [<Animal: animal>, <Animal: mammal>, <Animal: reptile>, <Animal: snake>]
-        
-        It's also possible to select only instances of the model to which the
-        manager is attached by using the ``exclude_subclasses`` method.
-        
-        >>> Mammal.objects.all()
-        [<Mammal: mammal>]
-        
-        Each instance of ``PolymorphicModel`` has a ``type_cast`` method that knows how
-        to convert itself to the correct ``ContentType``.
-        
-        >>> animal_snake = Animal.objects.get(pk=snake.pk)
-        <Animal: snake>
-        >>> animal_snake.type_cast()
-        <Snake: snake>
-        >>> animal_snake.type_cast(Reptile)
-        <Reptile: snake>
-        
-        If the ``PolymorphicModel.content_type`` fields conflicts with one of your
-        existing fields you just have to subclass
-        ``polymodels.models.BasePolymorphicModel`` and specify which field *polymodels*
-        should use instead by defining a ``CONTENT_TYPE_FIELD`` attribute on your model.
-        This field must be a ``ForeignKey`` to ``ContentType``.
-        
-        ::
-        
-            from django.contrib.contenttypes.models import ContentType
-            from django.db import models
-            from polymodels.models import BasePolymorphicModel
-        
-            class MyModel(BasePolymorphicModel):
-                CONTENT_TYPE_FIELD = 'polymorphic_ct'
-                polymorphic_ct = models.ForeignKey(ContentType)
-        
-        ************
-        How it works
-        ************
-        
-        Under the hood ``select_subclasses`` calls ``seleted_related`` to avoid
-        unnecessary queries and ``filter`` if you pass some classes to it. On queryset
-        iteration, the fetched instanced are converted to their correct type by calling
-        ``BasePolymorphicModel.type_cast``. Note that those lookups are cached on class
-        creation to avoid computing them on every single query.
-        
-        
-        ******************
-        Note of the author
-        ******************
-        
-        I'm aware there's already plenty of existing projects tackling the whole
-        **model-inheritance-type-casting-thing** such as `django-polymorphic`_. However
-        I wanted to implement this feature in a lightweight way: no
-        ``__metaclass__`` or ``__init__`` overrides while using django's public API as
-        much as possible. In the end, this was really just an extraction of
-        `django-mutant`_'s own mecanism of handling this since I needed it as a
-        standalone app for another project.
-        
-        .. _django-polymorphic: https://github.com/chrisglass/django_polymorphic
-        .. _django-mutant: https://github.com/charettes/django-mutant
-        
-        
-        **********
-        Contribute
-        **********
-        
-        If you happen to encounter a bug or would like to suggest a feature addition
-        please `file an issue`_ or `create a pull request`_ containing **tests**.
-        
-        .. _file an issue: https://github.com/charettes/django-polymodels/issues
-        .. _create a pull request: https://github.com/charettes/django-polymodels/pulls
-        
-        *******
-        Credits
-        *******
-        
-        * Inspired by a `post of Jeff Elmores`_.
-        
-        .. _post of Jeff Elmores: http://jeffelmore.org/2010/11/11/automatic-downcasting-of-inherited-models-in-django/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+#################
+django-polymodels
+#################
+
+A django application that provides a simple way to retrieve models type casted
+to their original ``ContentType``.
+
+.. image:: https://travis-ci.org/charettes/django-polymodels.svg?branch=master
+    :target: https://travis-ci.org/charettes/django-polymodels
+
+.. image:: https://coveralls.io/repos/charettes/django-polymodels/badge.svg?branch=master&service=github
+    :target: https://coveralls.io/github/charettes/django-polymodels?branch=master
+
+************
+Installation
+************
+
+>>> pip install django-polymodels
+
+Make sure ``'django.contrib.contenttypes'`` and ``'polymodels'`` are in
+your `INSTALLED_APPS`
+
+::
+
+    INSTALLED_APPS += ('django.contrib.contenttypes', 'polymodels')
+
+*****
+Usage
+*****
+
+Subclass ``PolymorphicModel``, an abstract model class.
+
+::
+
+    from django.db import models
+    from polymodels.models import PolymorphicModel
+
+    class Animal(PolymorphicModel):
+        name = models.CharField(max_length=255)
+
+        def __str__(self):
+            return self.name
+
+    class Mammal(Animal):
+        pass
+
+    class Dog(Mammal):
+        pass
+
+    class Reptile(Animal):
+        pass
+
+    class Snake(Reptile):
+        class Meta:
+            proxy = True
+
+Objects are created the same way as usual and their associated ``ContentType``
+is saved automatically:
+
+>>> animal = Animal.objects.create(name='animal')
+>>> mammal = Mammal.objects.create(name='mammal')
+>>> reptile = Reptile.objects.create(name='reptile')
+>>> snake = Snake.objects.create(name='snake')
+
+To retreive *type casted* instances from the ``Animal.objects`` manager you just
+have to use the ``select_subclasses`` method.
+
+>>> Animal.objects.select_subclasses()
+[<Animal: animal>, <Mammal: mammal>, <Reptile: reptile>, <Snake: snake>]
+
+You can also retreive a subset of the subclasses by passing them as arguments to
+``select_subclass``.
+
+>>> Animal.objects.select_subclasses(Reptile)
+[<Reptile: reptile>, <Snake: snake>]
+
+Or directly from subclasses managers.
+
+>>> Reptile.objects.select_subclasses(Snake)
+[<Snake: snake>]
+
+Note that you can also retrieve original results by avoiding the
+``select_subclasses`` call.
+
+>>> Animal.objects.all()
+[<Animal: animal>, <Animal: mammal>, <Animal: reptile>, <Animal: snake>]
+
+It's also possible to select only instances of the model to which the
+manager is attached by using the ``exclude_subclasses`` method.
+
+>>> Mammal.objects.all()
+[<Mammal: mammal>]
+
+Each instance of ``PolymorphicModel`` has a ``type_cast`` method that knows how
+to convert itself to the correct ``ContentType``.
+
+>>> animal_snake = Animal.objects.get(pk=snake.pk)
+<Animal: snake>
+>>> animal_snake.type_cast()
+<Snake: snake>
+>>> animal_snake.type_cast(Reptile)
+<Reptile: snake>
+
+If the ``PolymorphicModel.content_type`` fields conflicts with one of your
+existing fields you just have to subclass
+``polymodels.models.BasePolymorphicModel`` and specify which field *polymodels*
+should use instead by defining a ``CONTENT_TYPE_FIELD`` attribute on your model.
+This field must be a ``ForeignKey`` to ``ContentType``.
+
+::
+
+    from django.contrib.contenttypes.models import ContentType
+    from django.db import models
+    from polymodels.models import BasePolymorphicModel
+
+    class MyModel(BasePolymorphicModel):
+        CONTENT_TYPE_FIELD = 'polymorphic_ct'
+        polymorphic_ct = models.ForeignKey(ContentType)
+
+************
+How it works
+************
+
+Under the hood ``select_subclasses`` calls ``seleted_related`` to avoid
+unnecessary queries and ``filter`` if you pass some classes to it. On queryset
+iteration, the fetched instanced are converted to their correct type by calling
+``BasePolymorphicModel.type_cast``. Note that those lookups are cached on class
+creation to avoid computing them on every single query.
+
+
+******************
+Note of the author
+******************
+
+I'm aware there's already plenty of existing projects tackling the whole
+**model-inheritance-type-casting-thing** such as `django-polymorphic`_. However
+I wanted to implement this feature in a lightweight way: no
+``__metaclass__`` or ``__init__`` overrides while using django's public API as
+much as possible. In the end, this was really just an extraction of
+`django-mutant`_'s own mecanism of handling this since I needed it as a
+standalone app for another project.
+
+.. _django-polymorphic: https://github.com/chrisglass/django_polymorphic
+.. _django-mutant: https://github.com/charettes/django-mutant
+
+
+**********
+Contribute
+**********
+
+If you happen to encounter a bug or would like to suggest a feature addition
+please `file an issue`_ or `create a pull request`_ containing **tests**.
+
+.. _file an issue: https://github.com/charettes/django-polymodels/issues
+.. _create a pull request: https://github.com/charettes/django-polymodels/pulls
+
+*******
+Credits
+*******
+
+* Inspired by a `post of Jeff Elmores`_.
+
+.. _post of Jeff Elmores: http://jeffelmore.org/2010/11/11/automatic-downcasting-of-inherited-models-in-django/
```

### Comparing `django-polymodels-1.7.0/LICENSE` & `django-polymodels-1.8.0/LICENSE`

 * *Files identical despite different names*

