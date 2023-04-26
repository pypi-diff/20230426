# Comparing `tmp/datatable-faker-0.1.2.tar.gz` & `tmp/datatable-faker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-faker-0.1.2.tar", last modified: Tue Apr 25 14:14:57 2023, max compression
+gzip compressed data, was "datatable-faker-0.1.3.tar", last modified: Wed Apr 26 05:09:09 2023, max compression
```

## Comparing `datatable-faker-0.1.2.tar` & `datatable-faker-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:14:57.350004 datatable-faker-0.1.2/
--rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-25 14:14:57.350004 datatable-faker-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1752 2023-04-25 14:09:34.000000 datatable-faker-0.1.2/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 14:14:57.350004 datatable-faker-0.1.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      982 2023-04-25 14:10:39.000000 datatable-faker-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:14:57.350004 datatable-faker-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:14:57.350004 datatable-faker-0.1.2/src/datatable_faker/
--rw-rw-r--   0 root         (0) root         (0)     1928 2023-04-25 13:23:34.000000 datatable-faker-0.1.2/src/datatable_faker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:14:57.350004 datatable-faker-0.1.2/src/datatable_faker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-25 14:14:57.000000 datatable-faker-0.1.2/src/datatable_faker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-25 14:14:57.000000 datatable-faker-0.1.2/src/datatable_faker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 14:14:57.000000 datatable-faker-0.1.2/src/datatable_faker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-25 14:14:57.000000 datatable-faker-0.1.2/src/datatable_faker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-25 14:14:57.000000 datatable-faker-0.1.2/src/datatable_faker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/
+-rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1751 2023-04-26 05:06:25.000000 datatable-faker-0.1.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      982 2023-04-26 05:07:45.000000 datatable-faker-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/src/datatable_faker/
+-rw-rw-r--   0 root         (0) root         (0)     1819 2023-04-26 05:06:16.000000 datatable-faker-0.1.3/src/datatable_faker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-04-26 05:03:55.000000 datatable-faker-0.1.3/src/datatable_faker/check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/src/datatable_faker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      302 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/top_level.txt
```

### Comparing `datatable-faker-0.1.2/LICENSE` & `datatable-faker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.2/PKG-INFO` & `datatable-faker-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 License-File: LICENSE
 
 datatable-faker
 ================
 
-Library to generate fake datatable for unittest 
+Library to generate fake datatable for unittest
 
 .. image:: https://img.shields.io/pypi/v/datatable-faker
    :target: https://pypi.python.org/pypi/datatable-faker/
 
 .. image:: https://github.com/Agent-Hellboy/datatable-faker/actions/workflows/python-publish.yml/badge.svg
     :target: https://github.com/Agent-Hellboy/datatable-faker/
```

### Comparing `datatable-faker-0.1.2/README.rst` & `datatable-faker-0.1.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 datatable-faker
 ================
 
-Library to generate fake datatable for unittest 
+Library to generate fake datatable for unittest
 
 .. image:: https://img.shields.io/pypi/v/datatable-faker
    :target: https://pypi.python.org/pypi/datatable-faker/
 
 .. image:: https://github.com/Agent-Hellboy/datatable-faker/actions/workflows/python-publish.yml/badge.svg
     :target: https://github.com/Agent-Hellboy/datatable-faker/
```

### Comparing `datatable-faker-0.1.2/setup.py` & `datatable-faker-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="datatable-faker",
     author="Prince Roshan",
-    version='0.1.2',
+    version='0.1.3',
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/Agent-Hellboy/datatable-faker",
     description="Library to generate fake datatable for unittest ",
     long_description=read("README.rst"),
     license="MIT",
     package_dir={'': 'src'},
     packages=['datatable_faker'],
```

### Comparing `datatable-faker-0.1.2/src/datatable_faker/__init__.py` & `datatable-faker-0.1.3/src/datatable_faker/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import get_type_hints, List, Dict
 from faker import Faker
 
-fake = Faker()
+import dataclasses
 
-class BaseModel:
-    def __init__(self, **kwargs):
-        for key, value in kwargs.items():
-            setattr(self, key, value)
+fake = Faker()
 
 def generate_fake_data(cls):
     fake_data = {}
     type_hints = get_type_hints(cls)
     for attribute_name in type_hints:
         attribute_type = type_hints[attribute_name]
         if attribute_type == str:
@@ -33,10 +30,10 @@
             fake_data[attribute_name] = {fake.word(): fake.word() for _ in range(3)}
         elif attribute_type == Dict[str, int]:
             fake_data[attribute_name] = {fake.word(): fake.random_int() for _ in range(3)}
         elif attribute_type == Dict[str, float]:
             fake_data[attribute_name] = {fake.word(): fake.pyfloat() for _ in range(3)}
         elif attribute_type == Dict[str, bool]:
             fake_data[attribute_name] = {fake.word(): fake.boolean() for _ in range(3)}
-        elif issubclass(attribute_type, BaseModel):
+        elif dataclasses.is_dataclass(attribute_type):
             fake_data[attribute_name] = generate_fake_data(attribute_type)
     return cls(**fake_data)
```

### Comparing `datatable-faker-0.1.2/src/datatable_faker.egg-info/PKG-INFO` & `datatable-faker-0.1.3/src/datatable_faker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 License-File: LICENSE
 
 datatable-faker
 ================
 
-Library to generate fake datatable for unittest 
+Library to generate fake datatable for unittest
 
 .. image:: https://img.shields.io/pypi/v/datatable-faker
    :target: https://pypi.python.org/pypi/datatable-faker/
 
 .. image:: https://github.com/Agent-Hellboy/datatable-faker/actions/workflows/python-publish.yml/badge.svg
     :target: https://github.com/Agent-Hellboy/datatable-faker/
```

