# Comparing `tmp/adminfinder-1.0.2.tar.gz` & `tmp/adminfinder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adminfinder-1.0.2.tar", last modified: Wed Apr 26 09:30:58 2023, max compression
+gzip compressed data, was "adminfinder-1.0.3.tar", last modified: Wed Apr 26 09:44:12 2023, max compression
```

## Comparing `adminfinder-1.0.2.tar` & `adminfinder-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:30:58.913368 adminfinder-1.0.2/
--rw-rw-rw-   0        0        0     1092 2023-04-25 10:57:31.000000 adminfinder-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1092 2023-04-25 10:57:31.000000 adminfinder-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      890 2023-04-26 09:30:58.913368 adminfinder-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1433 2023-04-25 11:43:46.000000 adminfinder-1.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 09:30:58.905028 adminfinder-1.0.2/adminfinder/
--rw-rw-rw-   0        0        0       36 2023-04-26 09:27:30.000000 adminfinder-1.0.2/adminfinder/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-04-25 14:07:56.000000 adminfinder-1.0.2/adminfinder/app.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:30:58.913368 adminfinder-1.0.2/adminfinder.egg-info/
--rw-rw-rw-   0        0        0      890 2023-04-26 09:30:58.000000 adminfinder-1.0.2/adminfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-04-26 09:30:58.000000 adminfinder-1.0.2/adminfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:30:58.000000 adminfinder-1.0.2/adminfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-26 09:30:58.000000 adminfinder-1.0.2/adminfinder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 09:30:58.000000 adminfinder-1.0.2/adminfinder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-26 09:30:58.000000 adminfinder-1.0.2/adminfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 09:30:58.913368 adminfinder-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-04-26 09:29:18.000000 adminfinder-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:44:12.555379 adminfinder-1.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-25 10:57:31.000000 adminfinder-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1092 2023-04-25 10:57:31.000000 adminfinder-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      890 2023-04-26 09:44:12.555379 adminfinder-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1433 2023-04-25 11:43:46.000000 adminfinder-1.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:44:12.555379 adminfinder-1.0.3/adminfinder/
+-rw-rw-rw-   0        0        0      770 2023-04-26 09:43:04.000000 adminfinder-1.0.3/adminfinder/__init__.py
+-rw-rw-rw-   0        0        0     2709 2023-04-26 09:42:51.000000 adminfinder-1.0.3/adminfinder/app.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:44:12.555379 adminfinder-1.0.3/adminfinder.egg-info/
+-rw-rw-rw-   0        0        0      890 2023-04-26 09:44:12.000000 adminfinder-1.0.3/adminfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-04-26 09:44:12.000000 adminfinder-1.0.3/adminfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:44:12.000000 adminfinder-1.0.3/adminfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-26 09:44:12.000000 adminfinder-1.0.3/adminfinder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 09:44:12.000000 adminfinder-1.0.3/adminfinder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 09:44:12.000000 adminfinder-1.0.3/adminfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:44:12.571005 adminfinder-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-04-26 09:38:52.000000 adminfinder-1.0.3/setup.py
```

### Comparing `adminfinder-1.0.2/LICENSE` & `adminfinder-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adminfinder-1.0.2/LICENSE.txt` & `adminfinder-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adminfinder-1.0.2/PKG-INFO` & `adminfinder-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adminfinder
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for finding admin panels and login pages
 Home-page: https://github.com/username/adminfinder-alpha
 Author: Keyvan Hardani
 Author-email: dev@keyvvan.com
 License: MIT
 Keywords: admin panel login page finder
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `adminfinder-1.0.2/README.txt` & `adminfinder-1.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `adminfinder-1.0.2/adminfinder/app.py` & `adminfinder-1.0.3/adminfinder/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,16 @@
 import requests
 import argparse
 import logging
 from cloudscraper import create_scraper
 from termcolor import colored
 
-banner_top = """ 
+version = colored("Version 1.0.3 by Keyvan Hardani (dev@keyvvan.com)", "red")
 
-                ,%%%%%%,
-               ,%%/\%%%%/\%%
-              ,%%%\c "" J/%%%
-  %.       %%%%/ o  o \%%%%%
-  `%%.     %%%%    _  |%%%%
-   `%%     `%%%%(__Y__)%%'      AdminFinder Alpha
-   //       ;%%%%`\-/%%%%'
-  ((       /  O \%%%%^^^
-   \\     ,'     `--' |//
-    \\   /           // 
-     `"`'           ((
-
-
-            """
-
-banner_bottom = """
-            """
-
-version = colored("Version 1.0.1 by Keyvan Hardani (keyvan@hardani.de)", "red")
-
-BANNER = banner_top + version + banner_bottom
 # Set up command-line arguments
-print(BANNER)
 parser = argparse.ArgumentParser(description="Search for an admin panel on a website.")
 parser.add_argument("-u", "--url", required=True, help="The URL of the website to search.")
 parser.add_argument("-b", "--bypass", action="store_true", help="Bypass Cloudflare protection.")
 parser.add_argument("-f", "--file", required=True, help="The path of the file containing admin paths.")
 
 # Set up logger
 logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
@@ -71,14 +49,38 @@
             print(colored(f"Found admin panel at {admin_url}", "green"))
             break
 
     if not found:
         logger.info("Admin panel not found")
         print(colored("Admin panel not found", "red"))
 
-# Parse command-line arguments and call search_admin_panel function
 if __name__ == "__main__":
+    banner_top = """ 
+
+                ,%%%%%%,
+               ,%%/\%%%%/\%%
+              ,%%%\c "" J/%%%
+  %.       %%%%/ o  o \%%%%%
+  `%%.     %%%%    _  |%%%%
+   `%%     `%%%%(__Y__)%%'      AdminFinder Alpha
+   //       ;%%%%`\-/%%%%'
+  ((       /  O \%%%%^^^
+   \\     ,'     `--' |//
+    \\   /           // 
+     `"`'           ((
+
+
+            """
+
+    banner_bottom = """
+            """
+
+    BANNER = banner_top + version + banner_bottom
+
+    print(BANNER)
+    print('python app.py -u https://google.com -f paths.txt // Path file included, you can use it.')
+
     args = parser.parse_args()
     url = add_trailing_slash(args.url)
     bypass = args.bypass
     admin_paths_file = args.file
     search_admin_panel(url, bypass, admin_paths_file)
```

### Comparing `adminfinder-1.0.2/adminfinder.egg-info/PKG-INFO` & `adminfinder-1.0.3/adminfinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adminfinder
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for finding admin panels and login pages
 Home-page: https://github.com/username/adminfinder-alpha
 Author: Keyvan Hardani
 Author-email: dev@keyvvan.com
 License: MIT
 Keywords: admin panel login page finder
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `adminfinder-1.0.2/setup.py` & `adminfinder-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='adminfinder',
-    version='1.0.2',
+    version='1.0.3',
     description='A tool for finding admin panels and login pages',
     long_description='A tool for finding admin panels and login pages. It uses a list of paths and a list of common admin panels and login pages to perform the search.',
     url='https://github.com/username/adminfinder-alpha',
     author='Keyvan Hardani',
     author_email='dev@keyvvan.com',
     license='MIT',
     classifiers=[
```

