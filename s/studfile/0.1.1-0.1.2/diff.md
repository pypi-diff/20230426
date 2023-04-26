# Comparing `tmp/studfile-0.1.1.tar.gz` & `tmp/studfile-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "studfile-0.1.1.tar", max compression
+gzip compressed data, was "studfile-0.1.2.tar", max compression
```

## Comparing `studfile-0.1.1.tar` & `studfile-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      845 2022-04-30 12:28:17.763638 studfile-0.1.1/README.md
--rw-r--r--   0        0        0      577 2022-06-23 14:26:14.097236 studfile-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2022-06-23 14:25:05.817236 studfile-0.1.1/studfile/__init__.py
--rw-r--r--   0        0        0      582 2022-04-28 21:34:29.273638 studfile-0.1.1/studfile/main.py
--rw-r--r--   0        0        0     1442 2022-04-28 22:22:04.113638 studfile-0.1.1/studfile/parser.py
--rw-r--r--   0        0        0      686 2022-05-20 16:49:33.136746 studfile-0.1.1/studfile/runner.py
--rw-r--r--   0        0        0     1699 2022-06-23 14:27:02.109451 studfile-0.1.1/setup.py
--rw-r--r--   0        0        0     1568 2022-06-23 14:27:02.109642 studfile-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      845 2022-04-30 12:28:17.763638 studfile-0.1.2/README.md
+-rw-r--r--   0        0        0      577 2023-04-25 16:39:33.009420 studfile-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-25 16:39:34.029422 studfile-0.1.2/studfile/__init__.py
+-rw-r--r--   0        0        0      582 2022-04-28 21:34:29.273638 studfile-0.1.2/studfile/main.py
+-rw-r--r--   0        0        0     1442 2022-04-28 22:22:04.113638 studfile-0.1.2/studfile/parser.py
+-rw-r--r--   0        0        0      686 2022-05-20 16:49:33.136746 studfile-0.1.2/studfile/runner.py
+-rw-r--r--   0        0        0     1703 1970-01-01 00:00:00.000000 studfile-0.1.2/setup.py
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 studfile-0.1.2/PKG-INFO
```

### Comparing `studfile-0.1.1/README.md` & `studfile-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `studfile-0.1.1/pyproject.toml` & `studfile-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "studfile"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simplified tool for making easy-to-use build scripts"
 authors = ["John Carter <jfcarter2358@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jfcarter2358/stud"
 keywords = ["build", "studfile"]
```

### Comparing `studfile-0.1.1/studfile/main.py` & `studfile-0.1.2/studfile/main.py`

 * *Files identical despite different names*

### Comparing `studfile-0.1.1/studfile/parser.py` & `studfile-0.1.2/studfile/parser.py`

 * *Files identical despite different names*

### Comparing `studfile-0.1.1/studfile/runner.py` & `studfile-0.1.2/studfile/runner.py`

 * *Files identical despite different names*

### Comparing `studfile-0.1.1/setup.py` & `studfile-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 ['PyYAML>=6.0,<7.0', 'calligraphy-scripting==1.1.2']
 
 entry_points = \
 {'console_scripts': ['stud = studfile.main:main']}
 
 setup_kwargs = {
     'name': 'studfile',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A simplified tool for making easy-to-use build scripts',
     'long_description': '# Stud\n\n## Example Studfile.yaml\n\n```yaml\n.variables:\n  all_services:\n    - foo\n    - bar\n    - baz\nbuild-docker: \n  help: "Build and optionally push docker images"\n  options:\n    - name: -s,--services\n      default: all\n      nargs: \'+\'\n      required: true\n    - name: -p,--push\n      action: store_true\n  cmd: |\n    if \'all\' in services:\n      services = all_services\n\n    for service in services:\n      docker build -t {service} -f src/{service}/Dockerfile .\n      if push:\n        docker push {service}\nbuild-local: \n  help: "Build local versions of services"\n  options:\n    - name: -s,--services\n      default: all\n      nargs: \'+\'\n      required: true\n  cmd: |\n    # notice that the all_services variable is available \n    if \'all\' in services:\n      services = all_services\n\n    for service in services:\n      # do build things here\n```\n',
     'author': 'John Carter',
     'author_email': 'jfcarter2358@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/jfcarter2358/stud',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `studfile-0.1.1/PKG-INFO` & `studfile-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: studfile
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simplified tool for making easy-to-use build scripts
 Home-page: https://github.com/jfcarter2358/stud
 License: MIT
 Keywords: build,studfile
 Author: John Carter
 Author-email: jfcarter2358@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: calligraphy-scripting (==1.1.2)
 Project-URL: Repository, https://github.com/jfcarter2358/stud
 Description-Content-Type: text/markdown
 
 # Stud
```

