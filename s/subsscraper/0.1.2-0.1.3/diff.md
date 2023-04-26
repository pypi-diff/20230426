# Comparing `tmp/subsscraper-0.1.2.tar.gz` & `tmp/subsscraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsscraper-0.1.2.tar", max compression
+gzip compressed data, was "subsscraper-0.1.3.tar", max compression
```

## Comparing `subsscraper-0.1.2.tar` & `subsscraper-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      405 2023-04-25 16:49:15.746913 subsscraper-0.1.2/README.md
--rw-r--r--   0        0        0      473 2023-04-25 16:50:01.270247 subsscraper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 16:15:03.420177 subsscraper-0.1.2/src/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 16:29:46.093540 subsscraper-0.1.2/src/conf/__init__.py
--rw-r--r--   0        0        0      349 2023-04-25 16:15:03.420177 subsscraper-0.1.2/src/conf/config.yaml
--rw-r--r--   0        0        0     1436 2023-04-25 16:15:03.420177 subsscraper-0.1.2/src/search.py
--rw-r--r--   0        0        0     2872 2023-04-25 16:40:48.026895 subsscraper-0.1.2/src/subscraper.py
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 subsscraper-0.1.2/setup.py
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 subsscraper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-04-25 17:00:16.740268 subsscraper-0.1.3/README.md
+-rw-r--r--   0        0        0      473 2023-04-25 17:00:27.936935 subsscraper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 16:15:03.420177 subsscraper-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:29:46.093540 subsscraper-0.1.3/src/conf/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-25 16:15:03.420177 subsscraper-0.1.3/src/conf/config.yaml
+-rw-r--r--   0        0        0     1436 2023-04-25 16:15:03.420177 subsscraper-0.1.3/src/search.py
+-rw-r--r--   0        0        0     2872 2023-04-25 16:40:48.026895 subsscraper-0.1.3/src/subscraper.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 subsscraper-0.1.3/setup.py
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 subsscraper-0.1.3/PKG-INFO
```

### Comparing `subsscraper-0.1.2/src/search.py` & `subsscraper-0.1.3/src/search.py`

 * *Files identical despite different names*

### Comparing `subsscraper-0.1.2/src/subscraper.py` & `subsscraper-0.1.3/src/subscraper.py`

 * *Files identical despite different names*

### Comparing `subsscraper-0.1.2/setup.py` & `subsscraper-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['search = src.search:main',
                      'subscrape = src.subscraper:main']}
 
 setup_kwargs = {
     'name': 'subsscraper',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
-    'long_description': 'SubScraper\n---------\n\nRun command for generate urls\n```commandline\nsearch\nsearch search.cnt=2 # for 2 urls\n```\n\nRun command for subscrape urls\n```commandline\nsubscrape\n```\n\nDefault configs\n```commandline\nsearch:\n  output_folder: data\n  result_file: urls.txt\n  cnt: 10\n  query: машинное обучение лекции таймкоды\n\nscraper:\n  output_folder: ${search.output_folder}/dataset\n```\n\n',
+    'long_description': 'SubScraper\n---------\n\nRun command for generate urls\n```commandline\nsearch\nsearch search.cnt=2 # for 2 urls\nsearch \'search.query="лекции таймкоды"\' search.cnt=2 # override cyrillic (more quotes)\n```\n\nRun command for subscrape urls\n```commandline\nsubscrape\n```\n\nDefault configs\n```commandline\nsearch:\n  output_folder: data\n  result_file: urls.txt\n  cnt: 10\n  query: машинное обучение лекции таймкоды\n\nscraper:\n  output_folder: ${search.output_folder}/dataset\n```\n\n',
     'author': 'tupiznak',
     'author_email': 'akej-vonavi@mail.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

