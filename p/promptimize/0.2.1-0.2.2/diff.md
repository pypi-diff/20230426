# Comparing `tmp/promptimize-0.2.1.tar.gz` & `tmp/promptimize-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptimize-0.2.1.tar", last modified: Tue Apr 25 16:51:14 2023, max compression
+gzip compressed data, was "promptimize-0.2.2.tar", last modified: Tue Apr 25 16:55:17 2023, max compression
```

## Comparing `promptimize-0.2.1.tar` & `promptimize-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.477422 promptimize-0.2.1/
--rw-r--r--   0 max        (501) staff       (20)       56 2023-04-07 20:39:22.000000 promptimize-0.2.1/.gitignore
--rw-r--r--   0 max        (501) staff       (20)       57 2023-04-08 19:15:24.000000 promptimize-0.2.1/.mypy.ini
--rw-r--r--   0 max        (501) staff       (20)     2058 2023-04-25 01:37:21.000000 promptimize-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 max        (501) staff       (20)    11358 2023-04-08 19:28:50.000000 promptimize-0.2.1/LICENSE
--rw-r--r--   0 max        (501) staff       (20)    13032 2023-04-25 16:51:14.477026 promptimize-0.2.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)    10570 2023-04-25 16:43:35.000000 promptimize-0.2.1/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.457610 promptimize-0.2.1/docs/
--rw-r--r--   0 max        (501) staff       (20)      685 2023-04-08 20:12:24.000000 promptimize-0.2.1/docs/Makefile
--rwxr-xr-x   0 max        (501) staff       (20)      565 2023-04-25 01:09:25.000000 promptimize-0.2.1/docs/publish.sh
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.460566 promptimize-0.2.1/docs/source/
--rw-r--r--   0 max        (501) staff       (20)     8144 2023-04-20 19:39:26.000000 promptimize-0.2.1/docs/source/README.md
--rw-r--r--   0 max        (501) staff       (20)     1268 2023-04-20 01:56:57.000000 promptimize-0.2.1/docs/source/conf.py
--rw-r--r--   0 max        (501) staff       (20)      111 2023-04-20 02:07:39.000000 promptimize-0.2.1/docs/source/index.rst
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.463609 promptimize-0.2.1/examples/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.465810 promptimize-0.2.1/examples/__pycache__/
--rw-r--r--   0 max        (501) staff       (20)     2557 2023-04-05 07:54:58.000000 promptimize-0.2.1/examples/__pycache__/use_cases.cpython-38.pyc
--rw-r--r--   0 max        (501) staff       (20)     2937 2023-04-25 00:36:26.000000 promptimize-0.2.1/examples/readme_examples.py
--rw-r--r--   0 max        (501) staff       (20)      892 2023-04-20 19:54:23.000000 promptimize-0.2.1/examples/readme_hello_world.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.473654 promptimize-0.2.1/promptimize/
--rw-r--r--   0 max        (501) staff       (20)       40 2023-04-25 01:13:35.000000 promptimize-0.2.1/promptimize/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     3556 2023-04-25 01:15:16.000000 promptimize-0.2.1/promptimize/cli.py
--rw-r--r--   0 max        (501) staff       (20)     1843 2023-04-25 01:16:34.000000 promptimize-0.2.1/promptimize/crawler.py
--rw-r--r--   0 max        (501) staff       (20)     4192 2023-04-25 01:20:03.000000 promptimize-0.2.1/promptimize/evals.py
--rw-r--r--   0 max        (501) staff       (20)     7673 2023-04-25 16:45:38.000000 promptimize-0.2.1/promptimize/prompt_cases.py
--rw-r--r--   0 max        (501) staff       (20)     3181 2023-04-25 16:49:57.000000 promptimize-0.2.1/promptimize/reports.py
--rw-r--r--   0 max        (501) staff       (20)      200 2023-04-05 07:16:13.000000 promptimize-0.2.1/promptimize/simple_jinja.py
--rw-r--r--   0 max        (501) staff       (20)     5910 2023-04-25 01:25:06.000000 promptimize-0.2.1/promptimize/suite.py
--rw-r--r--   0 max        (501) staff       (20)     9068 2023-04-25 01:25:49.000000 promptimize-0.2.1/promptimize/utils.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:51:14.476341 promptimize-0.2.1/promptimize.egg-info/
--rw-r--r--   0 max        (501) staff       (20)    13032 2023-04-25 16:51:14.000000 promptimize-0.2.1/promptimize.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      743 2023-04-25 16:51:14.000000 promptimize-0.2.1/promptimize.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-25 16:51:14.000000 promptimize-0.2.1/promptimize.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       71 2023-04-25 16:51:14.000000 promptimize-0.2.1/promptimize.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)       65 2023-04-25 16:51:14.000000 promptimize-0.2.1/promptimize.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       12 2023-04-25 16:51:14.000000 promptimize-0.2.1/promptimize.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)       31 2023-04-25 01:19:56.000000 promptimize-0.2.1/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       97 2023-04-25 01:11:21.000000 promptimize-0.2.1/requirements-dev.txt
--rw-r--r--   0 max        (501) staff       (20)       65 2023-04-19 00:07:38.000000 promptimize-0.2.1/requirements.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2023-04-25 16:51:14.477539 promptimize-0.2.1/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      899 2023-04-25 16:50:40.000000 promptimize-0.2.1/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.940752 promptimize-0.2.2/
+-rw-r--r--   0 max        (501) staff       (20)       56 2023-04-07 20:39:22.000000 promptimize-0.2.2/.gitignore
+-rw-r--r--   0 max        (501) staff       (20)       57 2023-04-08 19:15:24.000000 promptimize-0.2.2/.mypy.ini
+-rw-r--r--   0 max        (501) staff       (20)     2058 2023-04-25 01:37:21.000000 promptimize-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 max        (501) staff       (20)    11358 2023-04-08 19:28:50.000000 promptimize-0.2.2/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)    13056 2023-04-25 16:55:17.940003 promptimize-0.2.2/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)    10594 2023-04-25 16:53:54.000000 promptimize-0.2.2/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.927226 promptimize-0.2.2/docs/
+-rw-r--r--   0 max        (501) staff       (20)      685 2023-04-08 20:12:24.000000 promptimize-0.2.2/docs/Makefile
+-rwxr-xr-x   0 max        (501) staff       (20)      565 2023-04-25 01:09:25.000000 promptimize-0.2.2/docs/publish.sh
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.929436 promptimize-0.2.2/docs/source/
+-rw-r--r--   0 max        (501) staff       (20)     8144 2023-04-20 19:39:26.000000 promptimize-0.2.2/docs/source/README.md
+-rw-r--r--   0 max        (501) staff       (20)     1268 2023-04-20 01:56:57.000000 promptimize-0.2.2/docs/source/conf.py
+-rw-r--r--   0 max        (501) staff       (20)      111 2023-04-20 02:07:39.000000 promptimize-0.2.2/docs/source/index.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.930704 promptimize-0.2.2/examples/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.931418 promptimize-0.2.2/examples/__pycache__/
+-rw-r--r--   0 max        (501) staff       (20)     2557 2023-04-05 07:54:58.000000 promptimize-0.2.2/examples/__pycache__/use_cases.cpython-38.pyc
+-rw-r--r--   0 max        (501) staff       (20)     2937 2023-04-25 00:36:26.000000 promptimize-0.2.2/examples/readme_examples.py
+-rw-r--r--   0 max        (501) staff       (20)      892 2023-04-20 19:54:23.000000 promptimize-0.2.2/examples/readme_hello_world.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.936206 promptimize-0.2.2/promptimize/
+-rw-r--r--   0 max        (501) staff       (20)       40 2023-04-25 01:13:35.000000 promptimize-0.2.2/promptimize/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     3556 2023-04-25 01:15:16.000000 promptimize-0.2.2/promptimize/cli.py
+-rw-r--r--   0 max        (501) staff       (20)     1843 2023-04-25 01:16:34.000000 promptimize-0.2.2/promptimize/crawler.py
+-rw-r--r--   0 max        (501) staff       (20)     4192 2023-04-25 01:20:03.000000 promptimize-0.2.2/promptimize/evals.py
+-rw-r--r--   0 max        (501) staff       (20)     7673 2023-04-25 16:45:38.000000 promptimize-0.2.2/promptimize/prompt_cases.py
+-rw-r--r--   0 max        (501) staff       (20)     3181 2023-04-25 16:49:57.000000 promptimize-0.2.2/promptimize/reports.py
+-rw-r--r--   0 max        (501) staff       (20)      200 2023-04-05 07:16:13.000000 promptimize-0.2.2/promptimize/simple_jinja.py
+-rw-r--r--   0 max        (501) staff       (20)     5910 2023-04-25 01:25:06.000000 promptimize-0.2.2/promptimize/suite.py
+-rw-r--r--   0 max        (501) staff       (20)     9068 2023-04-25 01:25:49.000000 promptimize-0.2.2/promptimize/utils.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.938893 promptimize-0.2.2/promptimize.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)    13056 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      743 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       71 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)       65 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       12 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)       31 2023-04-25 01:19:56.000000 promptimize-0.2.2/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       97 2023-04-25 01:11:21.000000 promptimize-0.2.2/requirements-dev.txt
+-rw-r--r--   0 max        (501) staff       (20)       65 2023-04-19 00:07:38.000000 promptimize-0.2.2/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-04-25 16:55:17.941028 promptimize-0.2.2/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      899 2023-04-25 16:54:48.000000 promptimize-0.2.2/setup.py
```

### Comparing `promptimize-0.2.1/.pre-commit-config.yaml` & `promptimize-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/LICENSE` & `promptimize-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/PKG-INFO` & `promptimize-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptimize
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python toolkit to generate and evaluate prompts for GPT at scale
 Home-page: UNKNOWN
 Author: Maxime Beauchemin
 Author-email: maximebeauchemin@gmail.com
 License: Apache License, Version 2.0
 Description: # 💡 ¡promptimize! 💡
         [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -266,13 +266,13 @@
         This project is in its super early stages as of `0.2.0`, and contributions,
         contributors, and maintainers are highly encouraged. While it's a great time
         to onboard and influence the direction of the project, things are still
         evolving quickly. To get involved, open a GitHub issue
         or submit a pull request!
         
         ## Links
-        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/)
+        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
         * [Preset Blog](https://preset.io/blog/)
         * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `promptimize-0.2.1/README.md` & `promptimize-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,10 @@
 This project is in its super early stages as of `0.2.0`, and contributions,
 contributors, and maintainers are highly encouraged. While it's a great time
 to onboard and influence the direction of the project, things are still
 evolving quickly. To get involved, open a GitHub issue
 or submit a pull request!
 
 ## Links
-* [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/)
+* [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
 * [Preset Blog](https://preset.io/blog/)
 * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
```

### Comparing `promptimize-0.2.1/docs/Makefile` & `promptimize-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/docs/publish.sh` & `promptimize-0.2.2/docs/publish.sh`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/docs/source/README.md` & `promptimize-0.2.2/docs/source/README.md`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/docs/source/conf.py` & `promptimize-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/examples/__pycache__/use_cases.cpython-38.pyc` & `promptimize-0.2.2/examples/__pycache__/use_cases.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/examples/readme_examples.py` & `promptimize-0.2.2/examples/readme_examples.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/examples/readme_hello_world.py` & `promptimize-0.2.2/examples/readme_hello_world.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/cli.py` & `promptimize-0.2.2/promptimize/cli.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/crawler.py` & `promptimize-0.2.2/promptimize/crawler.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/evals.py` & `promptimize-0.2.2/promptimize/evals.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/prompt_cases.py` & `promptimize-0.2.2/promptimize/prompt_cases.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/reports.py` & `promptimize-0.2.2/promptimize/reports.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/suite.py` & `promptimize-0.2.2/promptimize/suite.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize/utils.py` & `promptimize-0.2.2/promptimize/utils.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/promptimize.egg-info/PKG-INFO` & `promptimize-0.2.2/promptimize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptimize
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python toolkit to generate and evaluate prompts for GPT at scale
 Home-page: UNKNOWN
 Author: Maxime Beauchemin
 Author-email: maximebeauchemin@gmail.com
 License: Apache License, Version 2.0
 Description: # 💡 ¡promptimize! 💡
         [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -266,13 +266,13 @@
         This project is in its super early stages as of `0.2.0`, and contributions,
         contributors, and maintainers are highly encouraged. While it's a great time
         to onboard and influence the direction of the project, things are still
         evolving quickly. To get involved, open a GitHub issue
         or submit a pull request!
         
         ## Links
-        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/)
+        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
         * [Preset Blog](https://preset.io/blog/)
         * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `promptimize-0.2.1/promptimize.egg-info/SOURCES.txt` & `promptimize-0.2.2/promptimize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.1/setup.py` & `promptimize-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="promptimize",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "promptimize=promptimize:cli",
             "p9e=promptimize:cli",
```

