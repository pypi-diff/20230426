# Comparing `tmp/pts_tdk_lambda_psu-0.0.8.tar.gz` & `tmp/pts_tdk_lambda_psu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pts_tdk_lambda_psu-0.0.8.tar", last modified: Tue Aug  2 10:02:18 2022, max compression
+gzip compressed data, was "dist/pts_tdk_lambda_psu-0.0.9.tar", last modified: Thu Jan 26 15:10:27 2023, max compression
```

## Comparing `pts_tdk_lambda_psu-0.0.8.tar` & `pts_tdk_lambda_psu-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shuparnadeb   (501) staff       (20)        0 2022-08-02 10:02:18.495164 pts_tdk_lambda_psu-0.0.8/
--rw-r--r--   0 shuparnadeb   (501) staff       (20)     1069 2022-07-07 12:33:54.000000 pts_tdk_lambda_psu-0.0.8/LICENSE.txt
--rw-r--r--   0 shuparnadeb   (501) staff       (20)     3111 2022-08-02 10:02:18.494955 pts_tdk_lambda_psu-0.0.8/PKG-INFO
--rw-r--r--   0 shuparnadeb   (501) staff       (20)     2624 2022-07-14 15:06:41.000000 pts_tdk_lambda_psu-0.0.8/README.md
-drwxr-xr-x   0 shuparnadeb   (501) staff       (20)        0 2022-08-02 10:02:18.494129 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu/
--rw-r--r--   0 shuparnadeb   (501) staff       (20)       40 2022-07-07 12:43:35.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu/__init__.py
--rw-r--r--   0 shuparnadeb   (501) staff       (20)    14551 2022-08-02 09:45:57.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu/tdklambda_psu.py
-drwxr-xr-x   0 shuparnadeb   (501) staff       (20)        0 2022-08-02 10:02:18.494776 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/
--rw-r--r--   0 shuparnadeb   (501) staff       (20)     3111 2022-08-02 10:02:18.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/PKG-INFO
--rw-r--r--   0 shuparnadeb   (501) staff       (20)      306 2022-08-02 10:02:18.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/SOURCES.txt
--rw-r--r--   0 shuparnadeb   (501) staff       (20)        1 2022-08-02 10:02:18.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/dependency_links.txt
--rw-r--r--   0 shuparnadeb   (501) staff       (20)       72 2022-08-02 10:02:18.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/requires.txt
--rw-r--r--   0 shuparnadeb   (501) staff       (20)       19 2022-08-02 10:02:18.000000 pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/top_level.txt
--rw-r--r--   0 shuparnadeb   (501) staff       (20)       38 2022-08-02 10:02:18.495235 pts_tdk_lambda_psu-0.0.8/setup.cfg
--rw-r--r--   0 shuparnadeb   (501) staff       (20)      910 2022-08-02 09:56:33.000000 pts_tdk_lambda_psu-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-01-26 15:10:17.000000 pts_tdk_lambda_psu-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu/
+-rw-rw-rw-   0 root         (0) root         (0)    14551 2023-01-26 15:10:17.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu/tdklambda_psu.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-01-26 15:10:17.000000 pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-01-26 15:10:17.000000 pts_tdk_lambda_psu-0.0.9/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-01-26 15:10:17.000000 pts_tdk_lambda_psu-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:10:27.000000 pts_tdk_lambda_psu-0.0.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pts_tdk_lambda_psu-0.0.8/LICENSE.txt` & `pts_tdk_lambda_psu-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_tdk_lambda_psu-0.0.8/PKG-INFO` & `pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: pts_tdk_lambda_psu
-Version: 0.0.8
+Name: pts-tdk-lambda-psu
+Version: 0.0.9
 Summary: TDK Lambda PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/tdklambda_psu_interface
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # TDKLambda_PSU_Interface
@@ -89,7 +90,8 @@
 Your pipenv environment will be in the ~./virtualenvs folder.
 Make sure to add the interpreter on your IDE if not automatically added by navigating to the virtualenv folder for your repo and selecting the correct python3 file from /bin/.
 
 ***
 
 ## Maintainers
 Maintainers: @julianpass and @shuparnadeb_pts
+
```

### Comparing `pts_tdk_lambda_psu-0.0.8/README.md` & `pts_tdk_lambda_psu-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu/tdklambda_psu.py` & `pts_tdk_lambda_psu-0.0.9/pts_tdk_lambda_psu/tdklambda_psu.py`

 * *Files identical despite different names*

### Comparing `pts_tdk_lambda_psu-0.0.8/pts_tdk_lambda_psu.egg-info/PKG-INFO` & `pts_tdk_lambda_psu-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: pts-tdk-lambda-psu
-Version: 0.0.8
+Name: pts_tdk_lambda_psu
+Version: 0.0.9
 Summary: TDK Lambda PSU Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/tdklambda_psu_interface
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # TDKLambda_PSU_Interface
@@ -89,7 +90,8 @@
 Your pipenv environment will be in the ~./virtualenvs folder.
 Make sure to add the interpreter on your IDE if not automatically added by navigating to the virtualenv folder for your repo and selecting the correct python3 file from /bin/.
 
 ***
 
 ## Maintainers
 Maintainers: @julianpass and @shuparnadeb_pts
+
```

### Comparing `pts_tdk_lambda_psu-0.0.8/setup.py` & `pts_tdk_lambda_psu-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_tdk_lambda_psu",
-    version="0.0.8",
+    version="0.0.9",
     author="Pass testing Solutions GmbH",
     description="TDK Lambda PSU Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/tdklambda_psu_interface",
     license="MIT",
```

