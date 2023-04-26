# Comparing `tmp/uib_experiments-1.6.0.tar.gz` & `tmp/uib_experiments-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\miquel\Development\09 - Libs\uib_experiments\dist\.tmp-0gstsjv8\uib_experiments-1.6.0.tar", last modified: Wed Apr 26 13:20:44 2023, max compression
+gzip compressed data, was "C:\Users\miquel\Development\09 - Libs\uib_experiments\dist\.tmp-gt3567hi\uib_experiments-1.6.1.tar", last modified: Wed Apr 26 13:42:17 2023, max compression
```

## Comparing `uib_experiments-1.6.0.tar` & `uib_experiments-1.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/
--rw-rw-rw-   0        0        0     1092 2021-07-02 09:15:14.000000 uib_experiments-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      430 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      210 2021-07-02 09:15:14.000000 uib_experiments-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-04-26 13:19:39.000000 uib_experiments-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments/
--rw-rw-rw-   0        0        0      217 2021-10-15 08:43:53.000000 uib_experiments-1.6.0/uib_experiments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments/data/
--rw-rw-rw-   0        0        0       37 2021-07-02 09:15:14.000000 uib_experiments-1.6.0/uib_experiments/data/__init__.py
--rw-rw-rw-   0        0        0     4532 2021-07-02 09:15:14.000000 uib_experiments-1.6.0/uib_experiments/data/dades.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments/database_model/
--rw-rw-rw-   0        0        0        0 2021-10-14 12:15:26.000000 uib_experiments-1.6.0/uib_experiments/database_model/__init__.py
--rw-rw-rw-   0        0        0     5249 2021-11-08 14:34:27.000000 uib_experiments-1.6.0/uib_experiments/database_model/database.py
--rw-rw-rw-   0        0        0     1985 2021-11-08 08:52:24.000000 uib_experiments-1.6.0/uib_experiments/decorator.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments/experiment/
--rw-rw-rw-   0        0        0       48 2021-07-02 09:15:14.000000 uib_experiments-1.6.0/uib_experiments/experiment/__init__.py
--rw-rw-rw-   0        0        0    17124 2023-04-26 09:23:50.000000 uib_experiments-1.6.0/uib_experiments/experiment/experiment.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments/keras/
--rw-rw-rw-   0        0        0       46 2021-07-02 09:15:14.000000 uib_experiments-1.6.0/uib_experiments/keras/__init__.py
--rw-rw-rw-   0        0        0     2925 2021-07-02 09:24:51.000000 uib_experiments-1.6.0/uib_experiments/keras/telegramCallback.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments.egg-info/
--rw-rw-rw-   0        0        0      430 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-07-02 11:30:14.000000 uib_experiments-1.6.0/uib_experiments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       58 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-26 13:20:44.000000 uib_experiments-1.6.0/uib_experiments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/
+-rw-rw-rw-   0        0        0     1092 2021-07-02 09:15:14.000000 uib_experiments-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0      430 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2021-07-02 09:15:14.000000 uib_experiments-1.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-04-26 13:42:03.000000 uib_experiments-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments/
+-rw-rw-rw-   0        0        0      217 2021-10-15 08:43:53.000000 uib_experiments-1.6.1/uib_experiments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments/data/
+-rw-rw-rw-   0        0        0       37 2021-07-02 09:15:14.000000 uib_experiments-1.6.1/uib_experiments/data/__init__.py
+-rw-rw-rw-   0        0        0     4532 2021-07-02 09:15:14.000000 uib_experiments-1.6.1/uib_experiments/data/dades.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments/database_model/
+-rw-rw-rw-   0        0        0        0 2021-10-14 12:15:26.000000 uib_experiments-1.6.1/uib_experiments/database_model/__init__.py
+-rw-rw-rw-   0        0        0     5249 2021-11-08 14:34:27.000000 uib_experiments-1.6.1/uib_experiments/database_model/database.py
+-rw-rw-rw-   0        0        0     1985 2021-11-08 08:52:24.000000 uib_experiments-1.6.1/uib_experiments/decorator.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments/experiment/
+-rw-rw-rw-   0        0        0       48 2021-07-02 09:15:14.000000 uib_experiments-1.6.1/uib_experiments/experiment/__init__.py
+-rw-rw-rw-   0        0        0    17128 2023-04-26 13:41:59.000000 uib_experiments-1.6.1/uib_experiments/experiment/experiment.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments/keras/
+-rw-rw-rw-   0        0        0       46 2021-07-02 09:15:14.000000 uib_experiments-1.6.1/uib_experiments/keras/__init__.py
+-rw-rw-rw-   0        0        0     2925 2021-07-02 09:24:51.000000 uib_experiments-1.6.1/uib_experiments/keras/telegramCallback.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments.egg-info/
+-rw-rw-rw-   0        0        0      430 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-07-02 11:30:14.000000 uib_experiments-1.6.1/uib_experiments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-26 13:42:17.000000 uib_experiments-1.6.1/uib_experiments.egg-info/top_level.txt
```

### Comparing `uib_experiments-1.6.0/LICENSE` & `uib_experiments-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uib_experiments-1.6.0/setup.py` & `uib_experiments-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = "Package to handle scientific experiments easily"
 
 setup(name='uib_experiments',
-      version='1.6.0',
+      version='1.6.1',
       description='Handle the experiments.',
       long_description=LONG_DESCRIPTION,
       url='https://github.com/miquelmn/uib_experiments',
       author='Miquel Miró Nicolau, Dr. Gabriel Moyà Alcover',
       author_email='miquel.miro@uib.cat, gabriel_moya@uib.es',
       download_url="https://github.com/miquelmn/uib_experiments/archive/refs/tags/v0.9.2.tar.gz",
       packages=find_packages(),
```

### Comparing `uib_experiments-1.6.0/uib_experiments/data/dades.py` & `uib_experiments-1.6.1/uib_experiments/data/dades.py`

 * *Files identical despite different names*

### Comparing `uib_experiments-1.6.0/uib_experiments/database_model/database.py` & `uib_experiments-1.6.1/uib_experiments/database_model/database.py`

 * *Files identical despite different names*

### Comparing `uib_experiments-1.6.0/uib_experiments/decorator.py` & `uib_experiments-1.6.1/uib_experiments/decorator.py`

 * *Files identical despite different names*

### Comparing `uib_experiments-1.6.0/uib_experiments/experiment/experiment.py` & `uib_experiments-1.6.1/uib_experiments/experiment/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         Constructs an string with information about the experiment.
 
         """
         resum = "%s \tExperiment %s started" % (
             datetime.datetime.fromtimestamp(self._start_time).strftime("%d/%m/%Y %H:%M:%S"),
             str(self._num_exp))
 
-        resum += self.__get_resume()
+        resum += self.__get_extra_info()
 
         resum += f"\n\t\t\tElapsed time {self.time} minutes"
 
         date_str = datetime.datetime.fromtimestamp(self._end_time).strftime("%d/%m/%Y %H:%M:%S")
 
         resum += f"\n{date_str} \tExperiment {self._num_exp} finished"
```

### Comparing `uib_experiments-1.6.0/uib_experiments/keras/telegramCallback.py` & `uib_experiments-1.6.1/uib_experiments/keras/telegramCallback.py`

 * *Files identical despite different names*

### Comparing `uib_experiments-1.6.0/uib_experiments.egg-info/SOURCES.txt` & `uib_experiments-1.6.1/uib_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

