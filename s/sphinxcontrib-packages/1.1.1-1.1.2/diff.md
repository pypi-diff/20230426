# Comparing `tmp/sphinxcontrib-packages-1.1.1.tar.gz` & `tmp/sphinxcontrib-packages-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-packages-1.1.1.tar", last modified: Fri Apr 21 14:52:33 2023, max compression
+gzip compressed data, was "sphinxcontrib-packages-1.1.2.tar", last modified: Wed Apr 26 18:51:32 2023, max compression
```

## Comparing `sphinxcontrib-packages-1.1.1.tar` & `sphinxcontrib-packages-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/
--rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.1/AUTHORS
--rw-r--r--   0 louis     (1000) louis     (1000)    34520 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.1/LICENSE
--rw-r--r--   0 louis     (1000) louis     (1000)     3091 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)     1576 2021-05-21 17:49:20.000000 sphinxcontrib-packages-1.1.1/README.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      257 2023-04-21 13:09:34.000000 sphinxcontrib-packages-1.1.1/pyproject.toml
--rw-r--r--   0 louis     (1000) louis     (1000)     1538 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/setup.cfg
--rw-r--r--   0 louis     (1000) louis     (1000)       93 2023-04-21 09:24:16.000000 sphinxcontrib-packages-1.1.1/setup.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.093986 sphinxcontrib-packages-1.1.1/sphinxcontrib/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/sphinxcontrib/packages/
--rw-r--r--   0 louis     (1000) louis     (1000)    14193 2023-04-21 14:49:13.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib/packages/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/
--rw-r--r--   0 louis     (1000) louis     (1000)     3091 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)      387 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       14 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/requires.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       14 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/top_level.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-04-21 14:52:32.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/zip-safe
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/test/
--rw-r--r--   0 louis     (1000) louis     (1000)     1541 2022-01-31 20:51:08.000000 sphinxcontrib-packages-1.1.1/test/test_doctests.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-26 18:51:32.763298 sphinxcontrib-packages-1.1.2/
+-rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.2/AUTHORS
+-rw-r--r--   0 louis     (1000) louis     (1000)    34520 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.2/LICENSE
+-rw-r--r--   0 louis     (1000) louis     (1000)     3091 2023-04-26 18:51:32.763298 sphinxcontrib-packages-1.1.2/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)     1576 2021-05-21 17:49:20.000000 sphinxcontrib-packages-1.1.2/README.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      257 2023-04-21 13:09:34.000000 sphinxcontrib-packages-1.1.2/pyproject.toml
+-rw-r--r--   0 louis     (1000) louis     (1000)     1538 2023-04-26 18:51:32.763298 sphinxcontrib-packages-1.1.2/setup.cfg
+-rw-r--r--   0 louis     (1000) louis     (1000)       93 2023-04-21 09:24:16.000000 sphinxcontrib-packages-1.1.2/setup.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-26 18:51:32.759298 sphinxcontrib-packages-1.1.2/sphinxcontrib/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-26 18:51:32.759298 sphinxcontrib-packages-1.1.2/sphinxcontrib/packages/
+-rw-r--r--   0 louis     (1000) louis     (1000)    14201 2023-04-26 18:50:08.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib/packages/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-26 18:51:32.763298 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/
+-rw-r--r--   0 louis     (1000) louis     (1000)     3091 2023-04-26 18:51:32.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)      387 2023-04-26 18:51:32.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-04-26 18:51:32.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       14 2023-04-26 18:51:32.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/requires.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       14 2023-04-26 18:51:32.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/top_level.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-04-21 14:52:32.000000 sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/zip-safe
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-26 18:51:32.763298 sphinxcontrib-packages-1.1.2/test/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1541 2022-01-31 20:51:08.000000 sphinxcontrib-packages-1.1.2/test/test_doctests.py
```

### Comparing `sphinxcontrib-packages-1.1.1/LICENSE` & `sphinxcontrib-packages-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-packages-1.1.1/PKG-INFO` & `sphinxcontrib-packages-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-packages
-Version: 1.1.1
+Version: 1.1.2
 Summary: This packages contains the Packages sphinx extension, which provides directives to display packages installed on the host machine
 Home-page: https://framagit.org/spalax/sphinxcontrib-packages
 Author: Louis Paternault
 Author-email: spalax@gresille.org
 License: AGPLv3 or any later version
 Project-URL: Documentation, http://packages.readthedocs.io
 Project-URL: Source, https://framagit.org/spalax/sphinxcontrib-packages
```

### Comparing `sphinxcontrib-packages-1.1.1/README.rst` & `sphinxcontrib-packages-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-packages-1.1.1/setup.cfg` & `sphinxcontrib-packages-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sphinxcontrib-packages
-version = 1.1.1
+version = 1.1.2
 author = Louis Paternault
 author_email = spalax@gresille.org
 license = AGPLv3 or any later version
 description = This packages contains the Packages sphinx extension, which provides directives to display packages installed on the host machine
 keywords = sphinx package system
 url = https://framagit.org/spalax/sphinxcontrib-packages
 project_urls =
```

### Comparing `sphinxcontrib-packages-1.1.1/sphinxcontrib/packages/__init__.py` & `sphinxcontrib-packages-1.1.2/sphinxcontrib/packages/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,18 @@
 
 import distro
 import pkg_resources
 from docutils import nodes
 from docutils.parsers.rst import Directive, directives
 from docutils.parsers.rst.directives import flag, unchanged
 from docutils.statemachine import StringList
+from sphinx.domains import Domain
 from sphinx.util.nodes import nested_parse_with_titles
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 def node_or_str(text):
     """Return argument, converted to a node if necessary."""
     if isinstance(text, str):
         return nodes.paragraph(text=text)
     return text
@@ -449,18 +450,28 @@
                 item = item[2:]
             yield from [
                 dict([("package", file), ("type", self._sty_or_cls(file))])
                 for file in self._find(item)
             ]
 
 
+class PackagesDomain(Domain):
+    """Gather directives."""
+
+    name = "packages"
+    label = "Sphinxcontrib-packages"
+    directives = {
+        "platform": PlatformDirective,
+        "pyversions": PythonVersionsDirective,
+        "bin": BinDirective,
+        "deb": DebDirective,
+        "python": PyDirective,
+        "python2": Py2Directive,
+        "python3": Py3Directive,
+        "c": CDirective,
+        "latex": LatexDirective,
+    }
+
+
 def setup(app):
     """Register directives."""
-    app.add_directive("packages:platform", PlatformDirective)
-    app.add_directive("packages:pyversions", PythonVersionsDirective)
-    app.add_directive("packages:bin", BinDirective)
-    app.add_directive("packages:deb", DebDirective)
-    app.add_directive("packages:python", PyDirective)
-    app.add_directive("packages:python2", Py2Directive)
-    app.add_directive("packages:python3", Py3Directive)
-    app.add_directive("packages:c", CDirective)
-    app.add_directive("packages:latex", LatexDirective)
+    app.add_domain(PackagesDomain)
```

### Comparing `sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/PKG-INFO` & `sphinxcontrib-packages-1.1.2/sphinxcontrib_packages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-packages
-Version: 1.1.1
+Version: 1.1.2
 Summary: This packages contains the Packages sphinx extension, which provides directives to display packages installed on the host machine
 Home-page: https://framagit.org/spalax/sphinxcontrib-packages
 Author: Louis Paternault
 Author-email: spalax@gresille.org
 License: AGPLv3 or any later version
 Project-URL: Documentation, http://packages.readthedocs.io
 Project-URL: Source, https://framagit.org/spalax/sphinxcontrib-packages
```

### Comparing `sphinxcontrib-packages-1.1.1/test/test_doctests.py` & `sphinxcontrib-packages-1.1.2/test/test_doctests.py`

 * *Files identical despite different names*

