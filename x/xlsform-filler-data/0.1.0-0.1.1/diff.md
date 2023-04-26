# Comparing `tmp/xlsform_filler_data-0.1.0.tar.gz` & `tmp/xlsform_filler_data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsform_filler_data-0.1.0.tar", max compression
+gzip compressed data, was "xlsform_filler_data-0.1.1.tar", max compression
```

## Comparing `xlsform_filler_data-0.1.0.tar` & `xlsform_filler_data-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-18 18:35:03.705789 xlsform_filler_data-0.1.0/README.md
--rw-r--r--   0        0        0      559 2023-04-25 20:09:34.175064 xlsform_filler_data-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-18 18:35:03.705672 xlsform_filler_data-0.1.0/xlsform_filler_data/__init__.py
--rw-r--r--   0        0        0     2043 2023-04-25 20:01:24.661693 xlsform_filler_data-0.1.0/xlsform_filler_data/xlsform_filler_data.py
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.0/setup.py
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-04-26 05:46:10.327908 xlsform_filler_data-0.1.1/README.md
+-rw-r--r--   0        0        0      557 2023-04-26 06:03:30.905260 xlsform_filler_data-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 18:35:03.705672 xlsform_filler_data-0.1.1/xlsform_filler_data/__init__.py
+-rw-r--r--   0        0        0     2043 2023-04-25 20:01:24.661693 xlsform_filler_data-0.1.1/xlsform_filler_data/xlsform_filler_data.py
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.1/setup.py
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.1/PKG-INFO
```

### Comparing `xlsform_filler_data-0.1.0/pyproject.toml` & `xlsform_filler_data-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "xlsform-filler-data"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool for generating fake testing data based on an XLSform. "
 authors = ["Brian Mc Donald <brian@brianmcdonald.me>"]
 readme = "README.md"
 packages = [{include = "xlsform_filler_data"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 pandas = "^2.0.0"
 openpyxl = "^3.1.2"
 click = "^8.1.3"
 lorem-text = "^2.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-xlsform_filler_data = "xlsform_filler_data.xlsform_filler_data:cli"
+xlsform-filler-data = "xlsform_filler_data.xlsform_filler_data:cli"
```

### Comparing `xlsform_filler_data-0.1.0/xlsform_filler_data/xlsform_filler_data.py` & `xlsform_filler_data-0.1.1/xlsform_filler_data/xlsform_filler_data.py`

 * *Files identical despite different names*

### Comparing `xlsform_filler_data-0.1.0/setup.py` & `xlsform_filler_data-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'lorem-text>=2.1,<3.0',
  'openpyxl>=3.1.2,<4.0.0',
  'pandas>=2.0.0,<3.0.0']
 
 entry_points = \
-{'console_scripts': ['xlsform_filler_data = '
+{'console_scripts': ['xlsform-filler-data = '
                      'xlsform_filler_data.xlsform_filler_data:cli']}
 
 setup_kwargs = {
     'name': 'xlsform-filler-data',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A tool for generating fake testing data based on an XLSform. ',
-    'long_description': '',
+    'long_description': '# XLSfrom filler data\n\n## Installation\n```pip install xlsform-filler-data```',
     'author': 'Brian Mc Donald',
     'author_email': 'brian@brianmcdonald.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

