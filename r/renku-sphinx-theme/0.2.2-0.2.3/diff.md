# Comparing `tmp/renku-sphinx-theme-0.2.2.tar.gz` & `tmp/renku-sphinx-theme-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/renku-sphinx-theme-0.2.2.tar", last modified: Fri Jul  9 12:48:28 2021, max compression
+gzip compressed data, was "renku-sphinx-theme-0.2.3.tar", last modified: Wed Apr 26 11:46:51 2023, max compression
```

## Comparing `renku-sphinx-theme-0.2.2.tar` & `renku-sphinx-theme-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      874 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)      908 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/CHANGES.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (121)     5344 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/custom.scss
--rw-r--r--   0 runner    (1001) docker     (121)     5477 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/
--rw-r--r--   0 runner    (1001) docker     (121)   143212 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.svg
--rw-r--r--   0 runner    (1001) docker     (121)    32025 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.eot
--rw-r--r--   0 runner    (1001) docker     (121)    33521 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.eot
--rw-r--r--   0 runner    (1001) docker     (121)   184627 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.svg
--rw-r--r--   0 runner    (1001) docker     (121)    39796 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (121)    27428 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    97400 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    34008 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    64400 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.otf
--rw-r--r--   0 runner    (1001) docker     (121)   104412 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    68328 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (121)    67588 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.otf
--rw-r--r--   0 runner    (1001) docker     (121)    42368 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    41929 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (121)   218393 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4795 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/compile_scss_config.json
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)      980 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/about.html
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6980 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10731 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-09 12:48:11.000000 renku-sphinx-theme-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6980 2021-07-09 12:48:28.000000 renku-sphinx-theme-0.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.323021 renku-sphinx-theme-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-26 11:46:51.323021 renku-sphinx-theme-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.319021 renku-sphinx-theme-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.319021 renku-sphinx-theme-0.2.3/renku_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/compile_scss_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.323021 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/custom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.319021 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.323021 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/
+-rw-r--r--   0 runner    (1001) docker     (123)    41929 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    64400 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   143212 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34008 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    27428 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    32025 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    67588 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   184627 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    97400 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    39796 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    33521 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    68328 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   218393 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   104412 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    42368 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:46:51.319021 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-26 11:46:51.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-26 11:46:51.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:46:51.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 11:46:51.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 11:46:51.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 11:46:51.000000 renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      908 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-26 11:46:51.323021 renku-sphinx-theme-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-26 11:46:29.000000 renku-sphinx-theme-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `renku-sphinx-theme-0.2.2/AUTHORS.rst` & `renku-sphinx-theme-0.2.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/MANIFEST.in` & `renku-sphinx-theme-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/setup.py` & `renku-sphinx-theme-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,32 +25,36 @@
 readme = open('README.rst').read()
 history = open('CHANGES.rst').read()
 
 tests_require = [
     'check-manifest>=0.25',
     'isort>=4.2.2',
     'pydocstyle>=1.0.0',
+    'twine>=4.0,<5.0',
+    'pkginfo<1.9',
+    'setuptools',
+    'wheel',
 ]
 
 extras_require = {
     'docs': [
         'Sphinx>=1.6.3,<5.0.0',
-        'sphinx-rtd-theme>=0.5.0,<0.6',
-    ],
-    'dev': [
-        'compile-scss~=1.0.1',
+        'sphinx-rtd-theme>=0.5.0,<1.2',
     ],
+    'dev': [ ],
+    #     'compile-scss~=1.0.1', NOTE: This package does not exist anymore, need to find a replacement!
+    # ],
     'tests': tests_require,
 }
 
 extras_require['all'] = extras_require['docs'] + extras_require['dev'] + extras_require['tests']
 
 install_requires = [
     'Sphinx>=1.6.3,<5.0.0',
-    'sphinx-rtd-theme>=0.5.0,<0.6',
+    'sphinx-rtd-theme>=0.5.0,<1.2',
 ]
 
 # Get the version string. Cannot be done with import!
 g = {}
 with open(os.path.join('renku_sphinx_theme', 'version.py'), 'rt') as fp:
     exec(fp.read(), g)
     version = g['__version__']
```

### Comparing `renku-sphinx-theme-0.2.2/LICENSE` & `renku-sphinx-theme-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/run-tests.sh` & `renku-sphinx-theme-0.2.3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/.editorconfig` & `renku-sphinx-theme-0.2.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/README.rst` & `renku-sphinx-theme-0.2.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
 =================================
  Sphinx Theme for Renku Projects
 =================================
 
-.. image:: https://img.shields.io/travis/SwissDataScienceCenter/renku-sphinx-theme.svg
-        :target: https://travis-ci.org/SwissDataScienceCenter/renku-sphinx-theme
+.. image:: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/actions/workflows/test.yml/badge.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/actions?query=branch%3Amaster
 
 .. image:: https://img.shields.io/github/tag/SwissDataScienceCenter/renku-sphinx-theme.svg
         :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases
 
 .. image:: https://img.shields.io/pypi/dm/renku-sphinx-theme.svg
         :target: https://pypi.python.org/pypi/renku-sphinx-theme
```

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/custom.scss` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/custom.scss`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,24 @@
 $rk-info-font: #003274;
 $rk-light-blue: #566673;
 $rk-gray: #838383;
 $rk-light-gray: #e4e7ea;
 $rk-pink: #d26a98;
 
 //side background
-.wy-nav-content-wrap {
+.wy-nav-side {
   background: $rk-blue;
 }
 
+@media screen and (min-width: 1100px) {
+  .wy-nav-content-wrap {
+      background:$rk-blue;
+  }
+}
+
 //all links are green
 a {
   color: $rk-green;
   &:hover {
     color: $rk-green-lighter;
   }
   &:visited {
```

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/favicon.png` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/favicon.png`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts.css` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.svg` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.svg`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.eot` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.eot`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.eot` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.eot`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.svg` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.svg`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.woff` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.woff`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.woff` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.woff`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.ttf` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.ttf`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.ttf` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.ttf`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.otf` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.otf`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.ttf` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.ttf`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.otf` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.otf`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.otf` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Medium.otf`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.woff` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.woff`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.eot` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Bold.eot`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.svg` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/fonts/calcutta/Calcutta-Regular.svg`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/static/custom.css` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/static/custom.css`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,24 @@
   - Run:  compile_scss --watch from inside /renku_sphinx_theme
 
   - That command will compile scss changes into css.
 
   - After doing changes commit scss and css files.
 
 */
-.wy-nav-content-wrap {
+.wy-nav-side {
   background: #01192d;
 }
 
+@media screen and (min-width: 1100px) {
+  .wy-nav-content-wrap {
+      background:#01192d;
+  }
+}
+
 a {
   color: #009568;
 }
 
 a:hover {
   color: #00bd84;
 }
```

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/__init__.py` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/version.py` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 This file is imported by ``renku_sphinx_theme.__init__``,
 and parsed by ``setup.py``.
 """
 
 from __future__ import absolute_import, print_function
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
```

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme/about.html` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme/about.html`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/SOURCES.txt` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 setup.py
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 renku_sphinx_theme/__init__.py
 renku_sphinx_theme/about.html
 renku_sphinx_theme/compile_scss_config.json
-renku_sphinx_theme/layout.html
 renku_sphinx_theme/theme.conf
 renku_sphinx_theme/version.py
 renku_sphinx_theme.egg-info/PKG-INFO
 renku_sphinx_theme.egg-info/SOURCES.txt
 renku_sphinx_theme.egg-info/dependency_links.txt
 renku_sphinx_theme.egg-info/entry_points.txt
 renku_sphinx_theme.egg-info/requires.txt
```

### Comparing `renku-sphinx-theme-0.2.2/renku_sphinx_theme.egg-info/PKG-INFO` & `renku-sphinx-theme-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,173 @@
 Metadata-Version: 2.1
 Name: renku-sphinx-theme
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Sphinx theme for Renku documentation.
 Home-page: https://github.com/SwissDataScienceCenter/renku-sphinx-theme
 Author: Swiss Data Science Center (SDSC)
 Author-email: contact@datascience.ch
 License: Apache License 2.0
-Description: ..
-            Copyright 2017 Swiss Data Science Center (SDSC)
-            A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
-            Eidgenössische Technische Hochschule Zürich (ETHZ).
-        
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-        
-                http://www.apache.org/licenses/LICENSE-2.0
-        
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-        
-        =================================
-         Sphinx Theme for Renku Projects
-        =================================
-        
-        .. image:: https://img.shields.io/travis/SwissDataScienceCenter/renku-sphinx-theme.svg
-                :target: https://travis-ci.org/SwissDataScienceCenter/renku-sphinx-theme
-        
-        .. image:: https://img.shields.io/github/tag/SwissDataScienceCenter/renku-sphinx-theme.svg
-                :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases
-        
-        .. image:: https://img.shields.io/pypi/dm/renku-sphinx-theme.svg
-                :target: https://pypi.python.org/pypi/renku-sphinx-theme
-        
-        .. image:: https://img.shields.io/github/license/SwissDataScienceCenter/renku-sphinx-theme.svg
-                :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/blob/master/LICENSE
-        
-        A Sphinx theme for Renku documentation based on RTD theme.
-        
-        Installation
-        ------------
-        
-        1. Add ``renku-sphinx-theme`` to ``setup.py`` or ``requirements.txt`` used
-           for building your documentation.
-        2. Set ``html_theme`` to ``'renku'`` in ``docs/conf.py``.
-        3. Configure at least ``description`` and ``github_repo`` in
-           ``html_theme_options``.
-        
-        Enjoy your beautiful Renku documentation style.
-        
-        
-        Style (css)
-        -----------
-        
-        This repo contains a scss file that generates a css file.
-        The css file shouldn't be manually modified since it's generated with the scss.
-        Instructions to change and run the scss file are inside the scss file.
-        
-        The easy way of doing style changes in this repository is to go to the renku repo, add a temporary css (custom.css) 
-        in the ``docs/conf.py`` file and follow this steps: 
-        
-        https://renku.readthedocs.io/en/latest/developer/contributing/documentation.html
-        
-        The reason for this is that renku docs is a better repository for testing changes.
-        
-        After doing the changes in the temporary css add this to custom.scss in this repository, build this into 
-        a css file using the instructions and commit the css and scss files.
-        
-        
-        Building
-        --------
-        
-        To build docs after doing changes, and test things inside this repository
-        
-        1. From the base folder... ``pip install -r docs/requirements.txt``
-        2. This should be done in case there where changes in fonts or new css files added ``pip install --editable .``
-        3. There is no Makefile here but in order to do the "make html" action you should do 
-        
-            ``cd docs``
-            ``sphinx-build -b html -d _build/doctrees . _build/html``
-        
-        Docs will be built into ``_build/html...`` open this files with chrome to see the changes.
-        
-        
-        Releasing
-        ---------
-        
-        After doing changes, a new release should be published in pypi under the sdsc-org account.
-        
-        To release a new version, change the version inside version.py, do step 1 and 2 of Building.
-        Then do ``python3 -m twine upload dist/*`` and the new release will be published on pypi.
-        
-        
-        ..
-            Copyright 2017 Swiss Data Science Center (SDSC)
-            A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
-            Eidgenössische Technische Hochschule Zürich (ETHZ).
-        
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-        
-                http://www.apache.org/licenses/LICENSE-2.0
-        
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-        
-        Changes
-        =======
-        
-        `0.2.2 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/compare/v0.1.0...v0.2.2>`__ (2021-07-09)
-        -------------------------------------------------------------------------------------------------------------
-        
-        -  **design:** new design for renku-sphinx
-           (`3cf7ec7 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/3cf7ec746996411408267cb952f500481aac805b>`__)
-        
-        -  **chore:** replace travis CI with github actions
-           (`4056830 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/40568301b0d95865db8835360b6b2ddd873ceccd>`__)
-        
-        `0.1.0 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases/tag/v0.1.0>__ (2018-05-17)`
-        ---------------------------------------------------------------------------------------------------------
-        
-        - Initial public release.
-        
 Keywords: Renku Sphinx theme
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: all
 Provides-Extra: tests
+Provides-Extra: all
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+..
+    Copyright 2017 Swiss Data Science Center (SDSC)
+    A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+    Eidgenössische Technische Hochschule Zürich (ETHZ).
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+=================================
+ Sphinx Theme for Renku Projects
+=================================
+
+.. image:: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/actions/workflows/test.yml/badge.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/actions?query=branch%3Amaster
+
+.. image:: https://img.shields.io/github/tag/SwissDataScienceCenter/renku-sphinx-theme.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases
+
+.. image:: https://img.shields.io/pypi/dm/renku-sphinx-theme.svg
+        :target: https://pypi.python.org/pypi/renku-sphinx-theme
+
+.. image:: https://img.shields.io/github/license/SwissDataScienceCenter/renku-sphinx-theme.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/blob/master/LICENSE
+
+A Sphinx theme for Renku documentation based on RTD theme.
+
+Installation
+------------
+
+1. Add ``renku-sphinx-theme`` to ``setup.py`` or ``requirements.txt`` used
+   for building your documentation.
+2. Set ``html_theme`` to ``'renku'`` in ``docs/conf.py``.
+3. Configure at least ``description`` and ``github_repo`` in
+   ``html_theme_options``.
+
+Enjoy your beautiful Renku documentation style.
+
+
+Style (css)
+-----------
+
+This repo contains a scss file that generates a css file.
+The css file shouldn't be manually modified since it's generated with the scss.
+Instructions to change and run the scss file are inside the scss file.
+
+The easy way of doing style changes in this repository is to go to the renku repo, add a temporary css (custom.css) 
+in the ``docs/conf.py`` file and follow this steps: 
+
+https://renku.readthedocs.io/en/latest/developer/contributing/documentation.html
+
+The reason for this is that renku docs is a better repository for testing changes.
+
+After doing the changes in the temporary css add this to custom.scss in this repository, build this into 
+a css file using the instructions and commit the css and scss files.
+
+
+Building
+--------
+
+To build docs after doing changes, and test things inside this repository
+
+1. From the base folder... ``pip install -r docs/requirements.txt``
+2. This should be done in case there where changes in fonts or new css files added ``pip install --editable .``
+3. There is no Makefile here but in order to do the "make html" action you should do 
+
+    ``cd docs``
+    ``sphinx-build -b html -d _build/doctrees . _build/html``
+
+Docs will be built into ``_build/html...`` open this files with chrome to see the changes.
+
+
+Releasing
+---------
+
+After doing changes, a new release should be published in pypi under the sdsc-org account.
+
+To release a new version, change the version inside version.py, do step 1 and 2 of Building.
+Then do ``python3 -m twine upload dist/*`` and the new release will be published on pypi.
+
+
+..
+    Copyright 2017 Swiss Data Science Center (SDSC)
+    A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+    Eidgenössische Technische Hochschule Zürich (ETHZ).
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+Changes
+=======
+
+`0.2.3 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/compare/v0.2.2...v0.2.3>`__ (2023-04-26)
+-------------------------------------------------------------------------------------------------------------
+
+-  **chore:** add dependabot.yml
+   (`76baee5 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/76baee53a3dea65e44c862e3d39836bced35f205>`__)
+
+-  **chore:** remove dependency on non-existent compile-scss
+   (`617e566 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/617e566bc4821c31e42d544c6abda9399c5cbde5>`__)
+ 
+-  **chore:** fix pypi description
+   (`23536d9 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/23536d9e40efdd3701a76074e377f2236d336cdf>`__)
+  
+-  **chore(deps):** update sphinx-rtd-theme requirement 
+   (`2ca96ca <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/2ca96ca9b932de2ba2f2434f0bb962d06d0a6620>`__)
+
+-  **chore:** bump python version
+   (`0dd1fe6 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/0dd1fe66db3b1d1c587ca534bb04c9a6c148de92>`__)
+
+-  **chore:** delete layout.html
+   (`5fa988d <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/5fa988d54609cfe3f593ca252af7925acd12eeef>`__)
+
+-  **fix:** update styles to fix sidebar background leaking into main content
+   (`5ab737b <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/5ab737bf48f7757ff1fb4464538f851da5918aa9>`__)
+
+`0.2.2 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/compare/v0.1.0...v0.2.2>`__ (2021-07-09)
+-------------------------------------------------------------------------------------------------------------
+
+-  **design:** new design for renku-sphinx
+   (`3cf7ec7 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/3cf7ec746996411408267cb952f500481aac805b>`__)
+
+-  **chore:** replace travis CI with github actions
+   (`4056830 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/40568301b0d95865db8835360b6b2ddd873ceccd>`__)
+
+`0.1.0 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases/tag/v0.1.0>`__ (2018-05-17)
+---------------------------------------------------------------------------------------------------------
+
+- Initial public release.
```

### Comparing `renku-sphinx-theme-0.2.2/docs/conf.py` & `renku-sphinx-theme-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `renku-sphinx-theme-0.2.2/PKG-INFO` & `renku-sphinx-theme-0.2.3/renku_sphinx_theme.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,173 @@
 Metadata-Version: 2.1
 Name: renku-sphinx-theme
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Sphinx theme for Renku documentation.
 Home-page: https://github.com/SwissDataScienceCenter/renku-sphinx-theme
 Author: Swiss Data Science Center (SDSC)
 Author-email: contact@datascience.ch
 License: Apache License 2.0
-Description: ..
-            Copyright 2017 Swiss Data Science Center (SDSC)
-            A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
-            Eidgenössische Technische Hochschule Zürich (ETHZ).
-        
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-        
-                http://www.apache.org/licenses/LICENSE-2.0
-        
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-        
-        =================================
-         Sphinx Theme for Renku Projects
-        =================================
-        
-        .. image:: https://img.shields.io/travis/SwissDataScienceCenter/renku-sphinx-theme.svg
-                :target: https://travis-ci.org/SwissDataScienceCenter/renku-sphinx-theme
-        
-        .. image:: https://img.shields.io/github/tag/SwissDataScienceCenter/renku-sphinx-theme.svg
-                :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases
-        
-        .. image:: https://img.shields.io/pypi/dm/renku-sphinx-theme.svg
-                :target: https://pypi.python.org/pypi/renku-sphinx-theme
-        
-        .. image:: https://img.shields.io/github/license/SwissDataScienceCenter/renku-sphinx-theme.svg
-                :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/blob/master/LICENSE
-        
-        A Sphinx theme for Renku documentation based on RTD theme.
-        
-        Installation
-        ------------
-        
-        1. Add ``renku-sphinx-theme`` to ``setup.py`` or ``requirements.txt`` used
-           for building your documentation.
-        2. Set ``html_theme`` to ``'renku'`` in ``docs/conf.py``.
-        3. Configure at least ``description`` and ``github_repo`` in
-           ``html_theme_options``.
-        
-        Enjoy your beautiful Renku documentation style.
-        
-        
-        Style (css)
-        -----------
-        
-        This repo contains a scss file that generates a css file.
-        The css file shouldn't be manually modified since it's generated with the scss.
-        Instructions to change and run the scss file are inside the scss file.
-        
-        The easy way of doing style changes in this repository is to go to the renku repo, add a temporary css (custom.css) 
-        in the ``docs/conf.py`` file and follow this steps: 
-        
-        https://renku.readthedocs.io/en/latest/developer/contributing/documentation.html
-        
-        The reason for this is that renku docs is a better repository for testing changes.
-        
-        After doing the changes in the temporary css add this to custom.scss in this repository, build this into 
-        a css file using the instructions and commit the css and scss files.
-        
-        
-        Building
-        --------
-        
-        To build docs after doing changes, and test things inside this repository
-        
-        1. From the base folder... ``pip install -r docs/requirements.txt``
-        2. This should be done in case there where changes in fonts or new css files added ``pip install --editable .``
-        3. There is no Makefile here but in order to do the "make html" action you should do 
-        
-            ``cd docs``
-            ``sphinx-build -b html -d _build/doctrees . _build/html``
-        
-        Docs will be built into ``_build/html...`` open this files with chrome to see the changes.
-        
-        
-        Releasing
-        ---------
-        
-        After doing changes, a new release should be published in pypi under the sdsc-org account.
-        
-        To release a new version, change the version inside version.py, do step 1 and 2 of Building.
-        Then do ``python3 -m twine upload dist/*`` and the new release will be published on pypi.
-        
-        
-        ..
-            Copyright 2017 Swiss Data Science Center (SDSC)
-            A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
-            Eidgenössische Technische Hochschule Zürich (ETHZ).
-        
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-        
-                http://www.apache.org/licenses/LICENSE-2.0
-        
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-        
-        Changes
-        =======
-        
-        `0.2.2 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/compare/v0.1.0...v0.2.2>`__ (2021-07-09)
-        -------------------------------------------------------------------------------------------------------------
-        
-        -  **design:** new design for renku-sphinx
-           (`3cf7ec7 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/3cf7ec746996411408267cb952f500481aac805b>`__)
-        
-        -  **chore:** replace travis CI with github actions
-           (`4056830 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/40568301b0d95865db8835360b6b2ddd873ceccd>`__)
-        
-        `0.1.0 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases/tag/v0.1.0>__ (2018-05-17)`
-        ---------------------------------------------------------------------------------------------------------
-        
-        - Initial public release.
-        
 Keywords: Renku Sphinx theme
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: all
 Provides-Extra: tests
+Provides-Extra: all
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+..
+    Copyright 2017 Swiss Data Science Center (SDSC)
+    A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+    Eidgenössische Technische Hochschule Zürich (ETHZ).
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+=================================
+ Sphinx Theme for Renku Projects
+=================================
+
+.. image:: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/actions/workflows/test.yml/badge.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/actions?query=branch%3Amaster
+
+.. image:: https://img.shields.io/github/tag/SwissDataScienceCenter/renku-sphinx-theme.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases
+
+.. image:: https://img.shields.io/pypi/dm/renku-sphinx-theme.svg
+        :target: https://pypi.python.org/pypi/renku-sphinx-theme
+
+.. image:: https://img.shields.io/github/license/SwissDataScienceCenter/renku-sphinx-theme.svg
+        :target: https://github.com/SwissDataScienceCenter/renku-sphinx-theme/blob/master/LICENSE
+
+A Sphinx theme for Renku documentation based on RTD theme.
+
+Installation
+------------
+
+1. Add ``renku-sphinx-theme`` to ``setup.py`` or ``requirements.txt`` used
+   for building your documentation.
+2. Set ``html_theme`` to ``'renku'`` in ``docs/conf.py``.
+3. Configure at least ``description`` and ``github_repo`` in
+   ``html_theme_options``.
+
+Enjoy your beautiful Renku documentation style.
+
+
+Style (css)
+-----------
+
+This repo contains a scss file that generates a css file.
+The css file shouldn't be manually modified since it's generated with the scss.
+Instructions to change and run the scss file are inside the scss file.
+
+The easy way of doing style changes in this repository is to go to the renku repo, add a temporary css (custom.css) 
+in the ``docs/conf.py`` file and follow this steps: 
+
+https://renku.readthedocs.io/en/latest/developer/contributing/documentation.html
+
+The reason for this is that renku docs is a better repository for testing changes.
+
+After doing the changes in the temporary css add this to custom.scss in this repository, build this into 
+a css file using the instructions and commit the css and scss files.
+
+
+Building
+--------
+
+To build docs after doing changes, and test things inside this repository
+
+1. From the base folder... ``pip install -r docs/requirements.txt``
+2. This should be done in case there where changes in fonts or new css files added ``pip install --editable .``
+3. There is no Makefile here but in order to do the "make html" action you should do 
+
+    ``cd docs``
+    ``sphinx-build -b html -d _build/doctrees . _build/html``
+
+Docs will be built into ``_build/html...`` open this files with chrome to see the changes.
+
+
+Releasing
+---------
+
+After doing changes, a new release should be published in pypi under the sdsc-org account.
+
+To release a new version, change the version inside version.py, do step 1 and 2 of Building.
+Then do ``python3 -m twine upload dist/*`` and the new release will be published on pypi.
+
+
+..
+    Copyright 2017 Swiss Data Science Center (SDSC)
+    A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
+    Eidgenössische Technische Hochschule Zürich (ETHZ).
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+Changes
+=======
+
+`0.2.3 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/compare/v0.2.2...v0.2.3>`__ (2023-04-26)
+-------------------------------------------------------------------------------------------------------------
+
+-  **chore:** add dependabot.yml
+   (`76baee5 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/76baee53a3dea65e44c862e3d39836bced35f205>`__)
+
+-  **chore:** remove dependency on non-existent compile-scss
+   (`617e566 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/617e566bc4821c31e42d544c6abda9399c5cbde5>`__)
+ 
+-  **chore:** fix pypi description
+   (`23536d9 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/23536d9e40efdd3701a76074e377f2236d336cdf>`__)
+  
+-  **chore(deps):** update sphinx-rtd-theme requirement 
+   (`2ca96ca <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/2ca96ca9b932de2ba2f2434f0bb962d06d0a6620>`__)
+
+-  **chore:** bump python version
+   (`0dd1fe6 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/0dd1fe66db3b1d1c587ca534bb04c9a6c148de92>`__)
+
+-  **chore:** delete layout.html
+   (`5fa988d <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/5fa988d54609cfe3f593ca252af7925acd12eeef>`__)
+
+-  **fix:** update styles to fix sidebar background leaking into main content
+   (`5ab737b <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/5ab737bf48f7757ff1fb4464538f851da5918aa9>`__)
+
+`0.2.2 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/compare/v0.1.0...v0.2.2>`__ (2021-07-09)
+-------------------------------------------------------------------------------------------------------------
+
+-  **design:** new design for renku-sphinx
+   (`3cf7ec7 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/3cf7ec746996411408267cb952f500481aac805b>`__)
+
+-  **chore:** replace travis CI with github actions
+   (`4056830 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/commit/40568301b0d95865db8835360b6b2ddd873ceccd>`__)
+
+`0.1.0 <https://github.com/SwissDataScienceCenter/renku-sphinx-theme/releases/tag/v0.1.0>`__ (2018-05-17)
+---------------------------------------------------------------------------------------------------------
+
+- Initial public release.
```

