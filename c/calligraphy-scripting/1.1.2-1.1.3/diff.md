# Comparing `tmp/calligraphy-scripting-1.1.2.tar.gz` & `tmp/calligraphy_scripting-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calligraphy-scripting-1.1.2.tar", max compression
+gzip compressed data, was "calligraphy_scripting-1.1.3.tar", max compression
```

## Comparing `calligraphy-scripting-1.1.2.tar` & `calligraphy_scripting-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1068 2022-03-07 22:50:26.146824 calligraphy-scripting-1.1.2/LICENSE
--rw-r--r--   0        0        0     2199 2022-03-07 22:50:26.146824 calligraphy-scripting-1.1.2/README.md
--rw-r--r--   0        0        0       97 2022-05-05 22:40:45.385662 calligraphy-scripting-1.1.2/calligraphy_scripting/__init__.py
--rw-r--r--   0        0        0     6395 2022-05-05 22:39:53.835662 calligraphy-scripting-1.1.2/calligraphy_scripting/cli.py
--rw-r--r--   0        0        0     7596 2022-03-22 15:31:13.712149 calligraphy-scripting-1.1.2/calligraphy_scripting/data/header.py
--rw-r--r--   0        0        0    11011 2022-05-05 22:22:36.675662 calligraphy-scripting-1.1.2/calligraphy_scripting/parser.py
--rw-r--r--   0        0        0     1536 2022-05-05 22:40:11.905662 calligraphy-scripting-1.1.2/calligraphy_scripting/runner.py
--rw-r--r--   0        0        0     4318 2022-03-08 16:20:36.089213 calligraphy-scripting-1.1.2/calligraphy_scripting/transpiler.py
--rw-r--r--   0        0        0      449 2022-05-05 22:21:51.975662 calligraphy-scripting-1.1.2/calligraphy_scripting/utils.py
--rw-r--r--   0        0        0      657 2022-05-05 22:40:50.965662 calligraphy-scripting-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3043 2022-05-05 22:50:18.685075 calligraphy-scripting-1.1.2/setup.py
--rw-r--r--   0        0        0     2878 2022-05-05 22:50:18.685307 calligraphy-scripting-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-03-07 22:50:26.146824 calligraphy_scripting-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2199 2022-03-07 22:50:26.146824 calligraphy_scripting-1.1.3/README.md
+-rw-r--r--   0        0        0       97 2023-04-25 16:28:43.423407 calligraphy_scripting-1.1.3/calligraphy_scripting/__init__.py
+-rw-r--r--   0        0        0     6395 2022-05-05 22:39:53.835662 calligraphy_scripting-1.1.3/calligraphy_scripting/cli.py
+-rw-r--r--   0        0        0     7596 2022-03-22 15:31:13.712149 calligraphy_scripting-1.1.3/calligraphy_scripting/data/header.py
+-rw-r--r--   0        0        0    11011 2022-05-05 22:22:36.675662 calligraphy_scripting-1.1.3/calligraphy_scripting/parser.py
+-rw-r--r--   0        0        0     1536 2022-05-05 22:40:11.905662 calligraphy_scripting-1.1.3/calligraphy_scripting/runner.py
+-rw-r--r--   0        0        0     4318 2022-03-08 16:20:36.089213 calligraphy_scripting-1.1.3/calligraphy_scripting/transpiler.py
+-rw-r--r--   0        0        0      449 2022-05-05 22:21:51.975662 calligraphy_scripting-1.1.3/calligraphy_scripting/utils.py
+-rw-r--r--   0        0        0      657 2023-04-25 16:28:45.934103 calligraphy_scripting-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 calligraphy_scripting-1.1.3/PKG-INFO
```

### Comparing `calligraphy-scripting-1.1.2/LICENSE` & `calligraphy_scripting-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/README.md` & `calligraphy_scripting-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/calligraphy_scripting/cli.py` & `calligraphy_scripting-1.1.3/calligraphy_scripting/cli.py`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/calligraphy_scripting/data/header.py` & `calligraphy_scripting-1.1.3/calligraphy_scripting/data/header.py`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/calligraphy_scripting/parser.py` & `calligraphy_scripting-1.1.3/calligraphy_scripting/parser.py`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/calligraphy_scripting/runner.py` & `calligraphy_scripting-1.1.3/calligraphy_scripting/runner.py`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/calligraphy_scripting/transpiler.py` & `calligraphy_scripting-1.1.3/calligraphy_scripting/transpiler.py`

 * *Files identical despite different names*

### Comparing `calligraphy-scripting-1.1.2/pyproject.toml` & `calligraphy_scripting-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calligraphy-scripting"
-version = "1.1.2"
+version = "1.1.3"
 description = "A hybrid language for a modern approach to shell scripting"
 authors = ["John Carter <jfcarter2358@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jfcarter2358/calligraphy"
 keywords = ["scripting", "calligraphy"]
```

### Comparing `calligraphy-scripting-1.1.2/setup.py` & `calligraphy_scripting-1.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: calligraphy-scripting
+Version: 1.1.3
+Summary: A hybrid language for a modern approach to shell scripting
+Home-page: https://github.com/jfcarter2358/calligraphy
+License: MIT
+Keywords: scripting,calligraphy
+Author: John Carter
+Author-email: jfcarter2358@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/jfcarter2358/calligraphy
+Description-Content-Type: text/markdown
 
-packages = \
-['calligraphy_scripting', 'calligraphy_scripting.data']
+# Calligraphy
+---
+[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![CI](https://github.com/jfcarter2358/calligraphy/actions/workflows/makefile.yml/badge.svg)](https://github.com/jfcarter2358/calligraphy/actions/workflows/makefile.yml)
+![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jfcarter2358/a5b95abd1dc360c13da66165ff482d5e/raw/calligraphy__heads_main.json)
 
-package_data = \
-{'': ['*']}
+**Shell scripting for the modern age**
 
-entry_points = \
-{'console_scripts': ['calligraphy = calligraphy_scripting.cli:cli']}
-
-setup_kwargs = {
-    'name': 'calligraphy-scripting',
-    'version': '1.1.2',
-    'description': 'A hybrid language for a modern approach to shell scripting',
-    'long_description': "# Calligraphy\n---\n[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/jfcarter2358/calligraphy/actions/workflows/makefile.yml/badge.svg)](https://github.com/jfcarter2358/calligraphy/actions/workflows/makefile.yml)\n![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jfcarter2358/a5b95abd1dc360c13da66165ff482d5e/raw/calligraphy__heads_main.json)\n\n**Shell scripting for the modern age**\n\nCalligraphy is a hybrid scripting language that allows you to mix Python and Bash code\nin the same file. This gives you the advantages of bash when working with other\nprocesses while also giving you the advantages of a modern language like Python.\n\nIt's a free software distributed under the MIT Licence unless\notherwise specified.\n\nDevelopment is hosted on GitHub: https://github.com/jfcarter2358/calligraphy/\n\nPull requests are amazing and most welcome.\n\n## Install\n\nCalligraphy can be simply installed by running\n\n```\npip install calligraphy-scripting\n```\n\nIf you want to install from a source distribution, extract the tarball and run\nthe following command (this requires poetry to be installed)\n\n```\npoetry install --no-dev\n```\n\n## Documentation\n\nThe documentation lives at https://calligraphy.readthedocs.io/.\n\n## Testing\n\nWe use `pytest` and `pytest-cov` for running the test suite. You should be able to install them with\n\n```\npip install pytest pytest-cov\n```\n\nor you can install calligraphy alongside those packages with\n\n```\npoetry install\n```\n\nTo run the test suite, you can do\n\n```\nmake test\n```\n\nThis will produce an html coverage report under the `htmlcov` directory.\n\n## Roadmap\n\nYou can find the Calligraphy roadmap [here](https://jfcarter2358.notion.site/5081d4214297401db15a43e47a974521?v=9858c59c7ecd4eefa09bf75158c47448)\n\n## License\n\nCalligraphy is under the [MIT license](https://opensource.org/licenses/MIT).\n\n## Contact\n\nIf you have any questions or concerns please reach out to me (John Carter) at [jfcarter2358@gmail.com](mailto:jfcarter2358@gmail.com)\n",
-    'author': 'John Carter',
-    'author_email': 'jfcarter2358@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/jfcarter2358/calligraphy',
-    'packages': packages,
-    'package_data': package_data,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Calligraphy is a hybrid scripting language that allows you to mix Python and Bash code
+in the same file. This gives you the advantages of bash when working with other
+processes while also giving you the advantages of a modern language like Python.
 
+It's a free software distributed under the MIT Licence unless
+otherwise specified.
+
+Development is hosted on GitHub: https://github.com/jfcarter2358/calligraphy/
+
+Pull requests are amazing and most welcome.
+
+## Install
+
+Calligraphy can be simply installed by running
+
+```
+pip install calligraphy-scripting
+```
+
+If you want to install from a source distribution, extract the tarball and run
+the following command (this requires poetry to be installed)
+
+```
+poetry install --no-dev
+```
+
+## Documentation
+
+The documentation lives at https://calligraphy.readthedocs.io/.
+
+## Testing
+
+We use `pytest` and `pytest-cov` for running the test suite. You should be able to install them with
+
+```
+pip install pytest pytest-cov
+```
+
+or you can install calligraphy alongside those packages with
+
+```
+poetry install
+```
+
+To run the test suite, you can do
+
+```
+make test
+```
+
+This will produce an html coverage report under the `htmlcov` directory.
+
+## Roadmap
+
+You can find the Calligraphy roadmap [here](https://jfcarter2358.notion.site/5081d4214297401db15a43e47a974521?v=9858c59c7ecd4eefa09bf75158c47448)
+
+## License
+
+Calligraphy is under the [MIT license](https://opensource.org/licenses/MIT).
+
+## Contact
+
+If you have any questions or concerns please reach out to me (John Carter) at [jfcarter2358@gmail.com](mailto:jfcarter2358@gmail.com)
 
-setup(**setup_kwargs)
```

