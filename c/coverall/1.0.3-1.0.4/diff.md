# Comparing `tmp/coverall-1.0.3.tar.gz` & `tmp/coverall-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverall-1.0.3.tar", last modified: Tue Apr 25 18:34:06 2023, max compression
+gzip compressed data, was "coverall-1.0.4.tar", last modified: Tue Apr 25 18:42:10 2023, max compression
```

## Comparing `coverall-1.0.3.tar` & `coverall-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:34:06.559395 coverall-1.0.3/
--rw-rw-rw-   0        0        0      162 2023-04-19 03:06:01.000000 coverall-1.0.3/HISTORY.md
--rw-rw-rw-   0        0        0     1068 2023-04-19 03:10:04.000000 coverall-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-04-25 18:22:11.000000 coverall-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      542 2023-04-25 18:34:06.558393 coverall-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-19 03:04:05.000000 coverall-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 18:34:06.546380 coverall-1.0.3/coverall/
--rw-rw-rw-   0        0        0       50 2023-04-25 18:04:37.000000 coverall-1.0.3/coverall/__init__.py
--rw-rw-rw-   0        0        0     6340 2023-04-25 18:25:35.000000 coverall-1.0.3/coverall/cover.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:34:06.558393 coverall-1.0.3/coverall.egg-info/
--rw-rw-rw-   0        0        0      542 2023-04-25 18:34:06.000000 coverall-1.0.3/coverall.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-25 18:34:06.000000 coverall-1.0.3/coverall.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:34:06.000000 coverall-1.0.3/coverall.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 18:34:06.000000 coverall-1.0.3/coverall.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 18:34:06.000000 coverall-1.0.3/coverall.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 18:34:06.559395 coverall-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-04-25 18:22:49.000000 coverall-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:42:10.648364 coverall-1.0.4/
+-rw-rw-rw-   0        0        0      162 2023-04-19 03:06:01.000000 coverall-1.0.4/HISTORY.md
+-rw-rw-rw-   0        0        0     1068 2023-04-19 03:10:04.000000 coverall-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-04-25 18:22:11.000000 coverall-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      542 2023-04-25 18:42:10.647372 coverall-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-19 03:04:05.000000 coverall-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 18:42:10.637322 coverall-1.0.4/coverall/
+-rw-rw-rw-   0        0        0      207 2023-04-25 18:41:23.000000 coverall-1.0.4/coverall/__init__.py
+-rw-rw-rw-   0        0        0     6340 2023-04-25 18:41:49.000000 coverall-1.0.4/coverall/cover.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:42:10.646372 coverall-1.0.4/coverall.egg-info/
+-rw-rw-rw-   0        0        0      542 2023-04-25 18:42:10.000000 coverall-1.0.4/coverall.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-25 18:42:10.000000 coverall-1.0.4/coverall.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 18:42:10.000000 coverall-1.0.4/coverall.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 18:42:10.000000 coverall-1.0.4/coverall.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 18:42:10.000000 coverall-1.0.4/coverall.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 18:42:10.648364 coverall-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-04-25 18:41:31.000000 coverall-1.0.4/setup.py
```

### Comparing `coverall-1.0.3/LICENSE.txt` & `coverall-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverall-1.0.3/PKG-INFO` & `coverall-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverall
-Version: 1.0.3
+Version: 1.0.4
 Summary: Useful tools to work through Exact Cover, Set Cover, and Max Cover Problems
 Download-URL: https://pypi.org/project/coverall/
 Author: Brancen Clement
 Author-email: Brancenc@gmail.com
 License: MIT
 Keywords: MaxCover,SetCover,ExactCover
 Description-Content-Type: text/markdown
```

### Comparing `coverall-1.0.3/coverall/cover.py` & `coverall-1.0.4/coverall/cover.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         active_columns.setall(1)
         active_rows.setall(1)
         
         return [set_rows, active_columns, active_rows]
     
 
 def exactCover(universe, sets):
-    #stuff will go here
+    #notes will go here
     matrix_set = createMatrix(universe, sets, 'c')
     default_columns = matrix_set[1]
     default_rows = matrix_set[2]
     exactCover.matrix = matrix_set[0]
     
     
     def exactCoverHelper(columns, rows):
```

### Comparing `coverall-1.0.3/coverall.egg-info/PKG-INFO` & `coverall-1.0.4/coverall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverall
-Version: 1.0.3
+Version: 1.0.4
 Summary: Useful tools to work through Exact Cover, Set Cover, and Max Cover Problems
 Download-URL: https://pypi.org/project/coverall/
 Author: Brancen Clement
 Author-email: Brancenc@gmail.com
 License: MIT
 Keywords: MaxCover,SetCover,ExactCover
 Description-Content-Type: text/markdown
```

### Comparing `coverall-1.0.3/setup.py` & `coverall-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='coverall',
-    version='1.0.3',
+    version='1.0.4',
     description='Useful tools to work through Exact Cover, Set Cover, and Max Cover Problems',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Brancen Clement',
     author_email='Brancenc@gmail.com',
```

