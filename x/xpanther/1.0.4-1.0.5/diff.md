# Comparing `tmp/xpanther-1.0.4.tar.gz` & `tmp/xpanther-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.0.4.tar", last modified: Sun Feb 19 14:08:46 2023, max compression
+gzip compressed data, was "xpanther-1.0.5.tar", last modified: Wed Apr 26 14:43:47 2023, max compression
```

## Comparing `xpanther-1.0.4.tar` & `xpanther-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 14:08:46.631243 xpanther-1.0.4/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     5863 2023-02-19 14:08:46.631243 xpanther-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5386 2023-02-19 14:07:14.000000 xpanther-1.0.4/README.md
--rw-rw-rw-   0        0        0      565 2023-02-19 14:05:11.000000 xpanther-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-19 14:08:46.633260 xpanther-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-19 14:08:46.593178 xpanther-1.0.4/xpanther/
--rw-rw-rw-   0        0        0       61 2023-02-16 15:26:13.000000 xpanther-1.0.4/xpanther/__init__.py
--rw-rw-rw-   0        0        0    20070 2023-02-19 14:05:11.000000 xpanther-1.0.4/xpanther/main.py
--rw-rw-rw-   0        0        0     2467 2023-02-19 14:05:11.000000 xpanther-1.0.4/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-02-19 14:08:46.625969 xpanther-1.0.4/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5863 2023-02-19 14:08:46.000000 xpanther-1.0.4/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-02-19 14:08:46.000000 xpanther-1.0.4/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 14:08:46.000000 xpanther-1.0.4/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-19 14:08:46.000000 xpanther-1.0.4/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 14:43:47.593200 xpanther-1.0.5/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5863 2023-04-26 14:43:47.593200 xpanther-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5386 2023-02-19 14:07:14.000000 xpanther-1.0.5/README.md
+-rw-rw-rw-   0        0        0      633 2023-04-26 14:42:52.000000 xpanther-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:43:47.593200 xpanther-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 14:43:47.538584 xpanther-1.0.5/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-04-26 14:42:52.000000 xpanther-1.0.5/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    20075 2023-04-26 14:42:52.000000 xpanther-1.0.5/xpanther/main.py
+-rw-rw-rw-   0        0        0     2467 2023-02-19 14:05:11.000000 xpanther-1.0.5/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:43:47.593200 xpanther-1.0.5/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5863 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.0.4/LICENSE` & `xpanther-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.4/PKG-INFO` & `xpanther-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.4
+Version: 1.0.5
 Summary: Find unique relative xpath of any html/xml element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `xpanther-1.0.4/README.md` & `xpanther-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.4/pyproject.toml` & `xpanther-1.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpanther"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Find unique relative xpath of any html/xml element"
 readme = "README.md"
 requires-python = ">=3.7"
+dependencies = [
+    "bs4 >= 0.0.1",
+    "selenium >= 4.9.0",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `xpanther-1.0.4/xpanther/main.py` & `xpanther-1.0.5/xpanther/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     def __select_attribute_pool_size(self, elements):
         if self.__speed == 'normal':
             speed = 25
         elif self.__speed == 'slow':
             speed = 35
         elif self.__speed == 'fast':
             speed = 15
-        elif type(self.__speed) == int and self.__speed <= 50:
+        elif type(self.__speed) == int and int(self.__speed) <= 50:
             speed = self.__speed
         else:
             speed = 25
         return [elements[0][:speed], elements[1], elements[2]]
 
     def __format_XPATH(self, unique_elements, all_elements):
         combination = False
```

### Comparing `xpanther-1.0.4/xpanther/main_ide.py` & `xpanther-1.0.5/xpanther/main_ide.py`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.4/xpanther.egg-info/PKG-INFO` & `xpanther-1.0.5/xpanther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.4
+Version: 1.0.5
 Summary: Find unique relative xpath of any html/xml element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

