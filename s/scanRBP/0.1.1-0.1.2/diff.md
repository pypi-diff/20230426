# Comparing `tmp/scanRBP-0.1.1.tar.gz` & `tmp/scanRBP-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanRBP-0.1.1.tar", last modified: Wed Apr 26 10:58:40 2023, max compression
+gzip compressed data, was "scanRBP-0.1.2.tar", last modified: Wed Apr 26 11:01:37 2023, max compression
```

## Comparing `scanRBP-0.1.1.tar` & `scanRBP-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 10:58:40.572126 scanRBP-0.1.1/
--rw-rw-r--   0 rotg     (2023757) games       (20)     3972 2023-04-26 10:58:40.571788 scanRBP-0.1.1/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     3640 2023-04-21 15:01:09.000000 scanRBP-0.1.1/README.md
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 10:58:40.565398 scanRBP-0.1.1/scanRBP/
--rw-rw-r--   0 rotg     (2023757) games       (20)      445 2023-04-26 10:50:15.000000 scanRBP-0.1.1/scanRBP/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 10:58:40.570483 scanRBP-0.1.1/scanRBP/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2072 2023-04-26 10:07:04.000000 scanRBP-0.1.1/scanRBP/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 10:58:40.571115 scanRBP-0.1.1/scanRBP/pwm/
--rw-rw-r--   0 rotg     (2023757) games       (20)     1732 2023-04-26 10:56:17.000000 scanRBP-0.1.1/scanRBP/pwm/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     7703 2023-04-26 10:51:01.000000 scanRBP-0.1.1/scanRBP/scanRBP
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 10:58:34.000000 scanRBP-0.1.1/scanRBP/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 10:58:40.569646 scanRBP-0.1.1/scanRBP.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)     3972 2023-04-26 10:58:40.566357 scanRBP-0.1.1/scanRBP.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      305 2023-04-26 10:58:40.567030 scanRBP-0.1.1/scanRBP.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 10:58:40.567723 scanRBP-0.1.1/scanRBP.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 10:02:27.000000 scanRBP-0.1.1/scanRBP.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       41 2023-04-26 10:58:40.569213 scanRBP-0.1.1/scanRBP.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        8 2023-04-26 10:58:40.569835 scanRBP-0.1.1/scanRBP.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-26 10:58:40.572236 scanRBP-0.1.1/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1015 2023-04-26 10:46:46.000000 scanRBP-0.1.1/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.670941 scanRBP-0.1.2/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3972 2023-04-26 11:01:37.670398 scanRBP-0.1.2/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3640 2023-04-21 15:01:09.000000 scanRBP-0.1.2/README.md
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.665728 scanRBP-0.1.2/scanRBP/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      445 2023-04-26 10:50:15.000000 scanRBP-0.1.2/scanRBP/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.669051 scanRBP-0.1.2/scanRBP/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2072 2023-04-26 10:07:04.000000 scanRBP-0.1.2/scanRBP/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.669499 scanRBP-0.1.2/scanRBP/pwm/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1732 2023-04-26 10:56:17.000000 scanRBP-0.1.2/scanRBP/pwm/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     7703 2023-04-26 10:51:01.000000 scanRBP-0.1.2/scanRBP/scanRBP
+-rw-rw-r--   0 rotg     (2023757) games       (20)      104 2023-04-26 08:34:41.000000 scanRBP-0.1.2/scanRBP/scanRBP.config.example
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 11:01:30.000000 scanRBP-0.1.2/scanRBP/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.668515 scanRBP-0.1.2/scanRBP.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3972 2023-04-26 11:01:37.666288 scanRBP-0.1.2/scanRBP.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      336 2023-04-26 11:01:37.666775 scanRBP-0.1.2/scanRBP.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 11:01:37.667185 scanRBP-0.1.2/scanRBP.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 10:02:27.000000 scanRBP-0.1.2/scanRBP.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       41 2023-04-26 11:01:37.668258 scanRBP-0.1.2/scanRBP.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        8 2023-04-26 11:01:37.668621 scanRBP-0.1.2/scanRBP.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-26 11:01:37.671078 scanRBP-0.1.2/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1041 2023-04-26 11:01:07.000000 scanRBP-0.1.2/setup.py
```

### Comparing `scanRBP-0.1.1/PKG-INFO` & `scanRBP-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.1
+Version: 0.1.2
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `scanRBP-0.1.1/README.md` & `scanRBP-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.1/scanRBP/config/__init__.py` & `scanRBP-0.1.2/scanRBP/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.1/scanRBP/pwm/__init__.py` & `scanRBP-0.1.2/scanRBP/pwm/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.1/scanRBP/scanRBP` & `scanRBP-0.1.2/scanRBP/scanRBP`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.1/scanRBP.egg-info/PKG-INFO` & `scanRBP-0.1.2/scanRBP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.1
+Version: 0.1.2
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `scanRBP-0.1.1/setup.py` & `scanRBP-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     author='Gregor Rot',
     scripts=["scanRBP/scanRBP"],
     author_email='gregor.rot@gmail.com',
     url='https://github.com/grexor/scanRBP',
     keywords=['scanRBP', 'bioinformatics', 'RBP', 'RNA-protein binding', 'toolkit'],
     include_package_data=True,
     package_data={
-        'scanRBP': ['version'],
+        'scanRBP': ['version', 'scanRBP.config.example'],
     },
     install_requires=["scipy", "biopython", "seaborn", "matplotlib", "pybio"],
 )
```

