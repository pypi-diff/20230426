# Comparing `tmp/base_class_autotests-1.0.0.tar.gz` & `tmp/base_class_autotests-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_class_autotests-1.0.0.tar", last modified: Sat Apr 22 19:04:54 2023, max compression
+gzip compressed data, was "base_class_autotests-2.0.0.tar", last modified: Tue Apr 25 16:33:33 2023, max compression
```

## Comparing `base_class_autotests-1.0.0.tar` & `base_class_autotests-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 19:04:54.737233 base_class_autotests-1.0.0/
--rw-rw-rw-   0        0        0      532 2023-04-22 19:04:54.737233 base_class_autotests-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-04-22 19:04:18.000000 base_class_autotests-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 19:04:54.721610 base_class_autotests-1.0.0/base_class_autotests/
--rw-rw-rw-   0        0        0        0 2023-04-22 18:39:43.000000 base_class_autotests-1.0.0/base_class_autotests/__init__.py
--rw-rw-rw-   0        0        0    11600 2023-04-22 18:47:32.000000 base_class_autotests-1.0.0/base_class_autotests/base_class_autotests.py
-drwxrwxrwx   0        0        0        0 2023-04-22 19:04:54.721610 base_class_autotests-1.0.0/base_class_autotests.egg-info/
--rw-rw-rw-   0        0        0      532 2023-04-22 19:04:54.000000 base_class_autotests-1.0.0/base_class_autotests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-22 19:04:54.000000 base_class_autotests-1.0.0/base_class_autotests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 19:04:54.000000 base_class_autotests-1.0.0/base_class_autotests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-22 19:04:54.000000 base_class_autotests-1.0.0/base_class_autotests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-22 19:04:54.000000 base_class_autotests-1.0.0/base_class_autotests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 19:04:54.737233 base_class_autotests-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-04-22 18:56:57.000000 base_class_autotests-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:33:33.291437 base_class_autotests-2.0.0/
+-rw-rw-rw-   0        0        0    35746 2023-04-25 15:12:23.000000 base_class_autotests-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      556 2023-04-25 16:33:33.289452 base_class_autotests-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-04-22 19:04:18.000000 base_class_autotests-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 16:33:33.272437 base_class_autotests-2.0.0/base_class_autotests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 18:39:43.000000 base_class_autotests-2.0.0/base_class_autotests/__init__.py
+-rw-rw-rw-   0        0        0    11621 2023-04-25 15:07:26.000000 base_class_autotests-2.0.0/base_class_autotests/base_class_autotests.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:33:33.285436 base_class_autotests-2.0.0/base_class_autotests.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-04-25 16:33:33.000000 base_class_autotests-2.0.0/base_class_autotests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-25 16:33:33.000000 base_class_autotests-2.0.0/base_class_autotests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 16:33:33.000000 base_class_autotests-2.0.0/base_class_autotests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-25 16:33:33.000000 base_class_autotests-2.0.0/base_class_autotests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-25 16:33:33.000000 base_class_autotests-2.0.0/base_class_autotests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 16:33:33.291437 base_class_autotests-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-04-25 16:29:41.000000 base_class_autotests-2.0.0/setup.py
```

### Comparing `base_class_autotests-1.0.0/PKG-INFO` & `base_class_autotests-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: base_class_autotests
-Version: 1.0.0
+Version: 2.0.0
 Summary: Base class with basic checks of the elements
-Home-page: https://github.com/daoxwang-team/base_class_autotests
+Home-page: https://coderepo.corp.tander.ru/mishin_va/basic_checks
 Author: Kostuchenko_VA, Mishin_VA
 Author-email: kostuchenko_va@magnit.ru, mishin_va@magnit.ru
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # base_class_autotests
 Base class containing basic checks of the elements
```

### Comparing `base_class_autotests-1.0.0/base_class_autotests/base_class_autotests.py` & `base_class_autotests-2.0.0/base_class_autotests/base_class_autotests.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """Класс базовых действий: подключение к БД, проверка наличия элемента """
 
     def __init__(self, browser, cursor, timeout=1):
         self.browser = browser
         self.cursor = cursor
         self.browser.implicitly_wait(timeout)
         self.logger = logging.getLogger(type(self).__name__)
-        file_handler = logging.FileHandler("example_1.log")
+        file_handler = logging.FileHandler(f"logs/{self.browser.test_name}.log")
         file_handler.setFormatter(logging.Formatter("[%(asctime)s: %(levelname)s] %(message)s"))
         self.logger.addHandler(file_handler)
         self.logger.setLevel(logging.DEBUG)
 
     @allure.step("Open url: {url}")
     def open_page(self, url):
         """Открытие веб-страницы
```

### Comparing `base_class_autotests-1.0.0/base_class_autotests.egg-info/PKG-INFO` & `base_class_autotests-2.0.0/base_class_autotests.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: base-class-autotests
-Version: 1.0.0
+Version: 2.0.0
 Summary: Base class with basic checks of the elements
-Home-page: https://github.com/daoxwang-team/base_class_autotests
+Home-page: https://coderepo.corp.tander.ru/mishin_va/basic_checks
 Author: Kostuchenko_VA, Mishin_VA
 Author-email: kostuchenko_va@magnit.ru, mishin_va@magnit.ru
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # base_class_autotests
 Base class containing basic checks of the elements
```

### Comparing `base_class_autotests-1.0.0/setup.py` & `base_class_autotests-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = [
-    "selenium==4.5.0",
+    "selenium==4.9.0",
     "allure-pytest==2.13.1"
 ]
 
 setup(
     name="base_class_autotests",
-    version="1.0.0",
+    version="2.0.0",
     author="Kostuchenko_VA, Mishin_VA",
     author_email="kostuchenko_va@magnit.ru, mishin_va@magnit.ru",
     description="Base class with basic checks of the elements",
     long_description=readme,
     long_description_content_type="text/markdown",
-    url="https://github.com/daoxwang-team/base_class_autotests",
+    url="https://coderepo.corp.tander.ru/mishin_va/basic_checks",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

