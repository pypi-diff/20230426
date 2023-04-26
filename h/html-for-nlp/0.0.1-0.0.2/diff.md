# Comparing `tmp/html_for_nlp-0.0.1.tar.gz` & `tmp/html_for_nlp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_for_nlp-0.0.1.tar", last modified: Tue Apr  4 14:11:20 2023, max compression
+gzip compressed data, was "html_for_nlp-0.0.2.tar", last modified: Wed Apr 26 10:40:49 2023, max compression
```

## Comparing `html_for_nlp-0.0.1.tar` & `html_for_nlp-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 14:11:20.208834 html_for_nlp-0.0.1/
--rw-rw-rw-   0        0        0     1052 2023-04-04 14:11:20.208834 html_for_nlp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-04-04 13:55:18.000000 html_for_nlp-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 14:11:20.188657 html_for_nlp-0.0.1/html_for_nlp/
--rw-rw-rw-   0        0        0     4559 2023-04-04 13:38:01.000000 html_for_nlp-0.0.1/html_for_nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 14:11:20.208834 html_for_nlp-0.0.1/html_for_nlp.egg-info/
--rw-rw-rw-   0        0        0     1052 2023-04-04 14:11:20.000000 html_for_nlp-0.0.1/html_for_nlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-04 14:11:20.000000 html_for_nlp-0.0.1/html_for_nlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 14:11:20.000000 html_for_nlp-0.0.1/html_for_nlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-04 14:11:20.000000 html_for_nlp-0.0.1/html_for_nlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-04 14:11:20.000000 html_for_nlp-0.0.1/html_for_nlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 14:11:20.208834 html_for_nlp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-04-04 13:46:28.000000 html_for_nlp-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:40:49.316704 html_for_nlp-0.0.2/
+-rw-rw-rw-   0        0        0     1052 2023-04-26 10:40:49.315597 html_for_nlp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-04-04 13:55:18.000000 html_for_nlp-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 10:40:49.306470 html_for_nlp-0.0.2/html_for_nlp/
+-rw-rw-rw-   0        0        0     7731 2023-04-26 10:25:14.000000 html_for_nlp-0.0.2/html_for_nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:40:49.314591 html_for_nlp-0.0.2/html_for_nlp.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-04-26 10:40:49.000000 html_for_nlp-0.0.2/html_for_nlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-26 10:40:49.000000 html_for_nlp-0.0.2/html_for_nlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 10:40:49.000000 html_for_nlp-0.0.2/html_for_nlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-26 10:40:49.000000 html_for_nlp-0.0.2/html_for_nlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-26 10:40:49.000000 html_for_nlp-0.0.2/html_for_nlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 10:40:49.316704 html_for_nlp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-04-26 10:37:06.000000 html_for_nlp-0.0.2/setup.py
```

### Comparing `html_for_nlp-0.0.1/PKG-INFO` & `html_for_nlp-0.0.2/html_for_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: html_for_nlp
-Version: 0.0.1
+Name: html-for-nlp
+Version: 0.0.2
 Summary: HTML for NLP
 Home-page: https://github.com/druskacik/html_for_nlp
 Author: Róbert Druska
 Author-email: robert.druska@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `html_for_nlp-0.0.1/README.md` & `html_for_nlp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `html_for_nlp-0.0.1/html_for_nlp.egg-info/PKG-INFO` & `html_for_nlp-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: html-for-nlp
-Version: 0.0.1
+Name: html_for_nlp
+Version: 0.0.2
 Summary: HTML for NLP
 Home-page: https://github.com/druskacik/html_for_nlp
 Author: Róbert Druska
 Author-email: robert.druska@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

