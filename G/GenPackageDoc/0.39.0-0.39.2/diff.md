# Comparing `tmp/GenPackageDoc-0.39.0.tar.gz` & `tmp/GenPackageDoc-0.39.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenPackageDoc-0.39.0.tar", last modified: Mon Apr 24 14:18:03 2023, max compression
+gzip compressed data, was "GenPackageDoc-0.39.2.tar", last modified: Wed Apr 26 12:05:48 2023, max compression
```

## Comparing `GenPackageDoc-0.39.0.tar` & `GenPackageDoc-0.39.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/GenPackageDoc/
--rw-r--r--   0 runner    (1001) docker     (123)    40053 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CDocBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    25033 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CPackageDocConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CPatterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/CSourceParser.py
--rw-r--r--   0 runner    (1001) docker     (123)   283914 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/GenPackageDoc.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/GenPackageDoc/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/admonitions.sty
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/common.sty
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/pandoc.sty
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/preamble.tex
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/styles/robotframeworkaio.sty
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/GenPackageDoc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 14:18:03.000000 GenPackageDoc-0.39.0/GenPackageDoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:18:03.739369 GenPackageDoc-0.39.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-24 14:16:10.000000 GenPackageDoc-0.39.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/GenPackageDoc/
+-rw-r--r--   0 runner    (1001) docker     (123)    40053 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CDocBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25033 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CPackageDocConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CPatterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/CSourceParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283914 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/GenPackageDoc.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/GenPackageDoc/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/admonitions.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/common.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/pandoc.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/preamble.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/styles/robotframeworkaio.sty
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/GenPackageDoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 12:05:48.000000 GenPackageDoc-0.39.2/GenPackageDoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:05:48.920098 GenPackageDoc-0.39.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-26 12:02:26.000000 GenPackageDoc-0.39.2/setup.py
```

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/CDocBuilder.py` & `GenPackageDoc-0.39.2/GenPackageDoc/CDocBuilder.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/CInterface.py` & `GenPackageDoc-0.39.2/GenPackageDoc/CInterface.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/CPackageDocConfig.py` & `GenPackageDoc-0.39.2/GenPackageDoc/CPackageDocConfig.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/CPatterns.py` & `GenPackageDoc-0.39.2/GenPackageDoc/CPatterns.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/CSourceParser.py` & `GenPackageDoc-0.39.2/GenPackageDoc/CSourceParser.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/GenPackageDoc.pdf` & `GenPackageDoc-0.39.2/GenPackageDoc/GenPackageDoc.pdf`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/__init__.py` & `GenPackageDoc-0.39.2/GenPackageDoc/__init__.py`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/styles/admonitions.sty` & `GenPackageDoc-0.39.2/GenPackageDoc/styles/admonitions.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/styles/common.sty` & `GenPackageDoc-0.39.2/GenPackageDoc/styles/common.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/styles/pandoc.sty` & `GenPackageDoc-0.39.2/GenPackageDoc/styles/pandoc.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/styles/preamble.tex` & `GenPackageDoc-0.39.2/GenPackageDoc/styles/preamble.tex`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/styles/robotframeworkaio.sty` & `GenPackageDoc-0.39.2/GenPackageDoc/styles/robotframeworkaio.sty`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc/version.py` & `GenPackageDoc-0.39.2/GenPackageDoc/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of GenPackageDoc
 #
-VERSION      = "0.39.0"
-VERSION_DATE = "06.01.2023"
+VERSION      = "0.39.2"
+VERSION_DATE = "26.04.2023"
```

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc.egg-info/PKG-INFO` & `GenPackageDoc-0.39.2/GenPackageDoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.39.0
+Version: 0.39.2
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GenPackageDoc-0.39.0/GenPackageDoc.egg-info/SOURCES.txt` & `GenPackageDoc-0.39.2/GenPackageDoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/LICENSE` & `GenPackageDoc-0.39.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/PKG-INFO` & `GenPackageDoc-0.39.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenPackageDoc
-Version: 0.39.0
+Version: 0.39.2
 Summary: Documentation builder for Python packages
 Home-page: https://github.com/test-fullautomation/python-genpackagedoc
 Author: Holger Queckenstedt
 Author-email: Holger.Queckenstedt@de.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GenPackageDoc-0.39.0/README.rst` & `GenPackageDoc-0.39.2/README.rst`

 * *Files identical despite different names*

### Comparing `GenPackageDoc-0.39.0/setup.py` & `GenPackageDoc-0.39.2/setup.py`

 * *Files identical despite different names*

