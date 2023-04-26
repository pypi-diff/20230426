# Comparing `tmp/tcmb-0.2.0.tar.gz` & `tmp/tcmb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcmb-0.2.0.tar", last modified: Wed Jan 25 22:36:30 2023, max compression
+gzip compressed data, was "tcmb-0.3.0.tar", last modified: Tue Apr 25 23:42:24 2023, max compression
```

## Comparing `tcmb-0.2.0.tar` & `tcmb-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-01-25 22:36:30.596074 tcmb-0.2.0/
--rw-r--r--   0 stba       (501) staff       (20)     2736 2023-01-12 22:31:50.000000 tcmb-0.2.0/.gitignore
--rw-r--r--   0 stba       (501) staff       (20)      602 2023-01-25 22:29:47.000000 tcmb-0.2.0/CHANGELOG.md
--rw-r--r--   0 stba       (501) staff       (20)     1065 2023-01-12 21:37:38.000000 tcmb-0.2.0/LICENSE
--rw-r--r--   0 stba       (501) staff       (20)     5963 2023-01-25 22:36:30.595919 tcmb-0.2.0/PKG-INFO
--rw-r--r--   0 stba       (501) staff       (20)     4120 2023-01-19 23:12:56.000000 tcmb-0.2.0/README.md
--rw-r--r--   0 stba       (501) staff       (20)      513 2023-01-25 22:29:47.000000 tcmb-0.2.0/TODO.md
--rw-r--r--   0 stba       (501) staff       (20)      793 2023-01-25 22:29:47.000000 tcmb-0.2.0/pyproject.toml
--rw-r--r--   0 stba       (501) staff       (20)      167 2023-01-19 23:12:56.000000 tcmb-0.2.0/requirements.txt
--rw-r--r--   0 stba       (501) staff       (20)       38 2023-01-25 22:36:30.596110 tcmb-0.2.0/setup.cfg
--rw-r--r--   0 stba       (501) staff       (20)       37 2023-01-12 21:38:29.000000 tcmb-0.2.0/setup.py
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-01-25 22:36:30.594416 tcmb-0.2.0/tcmb/
--rw-r--r--   0 stba       (501) staff       (20)       52 2023-01-25 22:29:47.000000 tcmb-0.2.0/tcmb/__init__.py
--rw-r--r--   0 stba       (501) staff       (20)      845 2023-01-19 22:56:29.000000 tcmb-0.2.0/tcmb/auth.py
--rw-r--r--   0 stba       (501) staff       (20)      331 2023-01-12 22:32:13.000000 tcmb-0.2.0/tcmb/const.py
--rw-r--r--   0 stba       (501) staff       (20)    12543 2023-01-25 22:22:32.000000 tcmb-0.2.0/tcmb/core.py
--rw-r--r--   0 stba       (501) staff       (20)      200 2023-01-05 21:54:29.000000 tcmb-0.2.0/tcmb/errors.py
--rw-r--r--   0 stba       (501) staff       (20)     1046 2023-01-25 22:22:32.000000 tcmb-0.2.0/tcmb/utils.py
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-01-25 22:36:30.595164 tcmb-0.2.0/tcmb.egg-info/
--rw-r--r--   0 stba       (501) staff       (20)     5963 2023-01-25 22:36:30.000000 tcmb-0.2.0/tcmb.egg-info/PKG-INFO
--rw-r--r--   0 stba       (501) staff       (20)      371 2023-01-25 22:36:30.000000 tcmb-0.2.0/tcmb.egg-info/SOURCES.txt
--rw-r--r--   0 stba       (501) staff       (20)        1 2023-01-25 22:36:30.000000 tcmb-0.2.0/tcmb.egg-info/dependency_links.txt
--rw-r--r--   0 stba       (501) staff       (20)       22 2023-01-25 22:36:30.000000 tcmb-0.2.0/tcmb.egg-info/requires.txt
--rw-r--r--   0 stba       (501) staff       (20)        5 2023-01-25 22:36:30.000000 tcmb-0.2.0/tcmb.egg-info/top_level.txt
-drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-01-25 22:36:30.595622 tcmb-0.2.0/tests/
--rw-r--r--   0 stba       (501) staff       (20)        0 2023-01-07 22:09:47.000000 tcmb-0.2.0/tests/__init__.py
--rw-r--r--   0 stba       (501) staff       (20)      167 2023-01-25 21:50:00.000000 tcmb-0.2.0/tests/test_auth.py
--rw-r--r--   0 stba       (501) staff       (20)     1449 2023-01-25 21:50:00.000000 tcmb-0.2.0/tests/test_core.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-04-25 23:42:24.749347 tcmb-0.3.0/
+-rw-r--r--   0 stba       (501) staff       (20)     2736 2023-01-12 22:31:50.000000 tcmb-0.3.0/.gitignore
+-rw-r--r--   0 stba       (501) staff       (20)     1186 2023-04-25 23:39:26.000000 tcmb-0.3.0/CHANGELOG.md
+-rw-r--r--   0 stba       (501) staff       (20)     1065 2023-01-12 21:37:38.000000 tcmb-0.3.0/LICENSE
+-rw-r--r--   0 stba       (501) staff       (20)     6912 2023-04-25 23:42:24.749202 tcmb-0.3.0/PKG-INFO
+-rw-r--r--   0 stba       (501) staff       (20)     5020 2023-04-25 23:35:52.000000 tcmb-0.3.0/README.md
+-rw-r--r--   0 stba       (501) staff       (20)      684 2023-04-25 23:39:26.000000 tcmb-0.3.0/TODO.md
+-rw-r--r--   0 stba       (501) staff       (20)      920 2023-04-25 23:35:52.000000 tcmb-0.3.0/pyproject.toml
+-rw-r--r--   0 stba       (501) staff       (20)      167 2023-01-19 23:12:56.000000 tcmb-0.3.0/requirements.txt
+-rw-r--r--   0 stba       (501) staff       (20)       38 2023-04-25 23:42:24.749391 tcmb-0.3.0/setup.cfg
+-rw-r--r--   0 stba       (501) staff       (20)       37 2023-01-12 21:38:29.000000 tcmb-0.3.0/setup.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-04-25 23:42:24.746090 tcmb-0.3.0/tcmb/
+-rw-r--r--   0 stba       (501) staff       (20)       58 2023-04-25 23:39:26.000000 tcmb-0.3.0/tcmb/__init__.py
+-rw-r--r--   0 stba       (501) staff       (20)     1360 2023-04-25 23:35:52.000000 tcmb-0.3.0/tcmb/_data.py
+-rw-r--r--   0 stba       (501) staff       (20)     2093 2023-04-25 23:35:52.000000 tcmb-0.3.0/tcmb/auth.py
+-rw-r--r--   0 stba       (501) staff       (20)      331 2023-01-12 22:32:13.000000 tcmb-0.3.0/tcmb/const.py
+-rw-r--r--   0 stba       (501) staff       (20)    13564 2023-04-25 23:35:52.000000 tcmb-0.3.0/tcmb/core.py
+-rw-r--r--   0 stba       (501) staff       (20)      562 2023-04-25 23:35:52.000000 tcmb-0.3.0/tcmb/errors.py
+-rw-r--r--   0 stba       (501) staff       (20)     2017 2023-04-25 22:58:22.000000 tcmb-0.3.0/tcmb/fetch.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-04-25 23:42:24.746899 tcmb-0.3.0/tcmb/resources/
+-rw-r--r--   0 stba       (501) staff       (20)   717585 2023-04-25 23:35:52.000000 tcmb-0.3.0/tcmb/resources/series.json
+-rw-r--r--   0 stba       (501) staff       (20)     4512 2023-04-25 23:35:52.000000 tcmb-0.3.0/tcmb/utils.py
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-04-25 23:42:24.746778 tcmb-0.3.0/tcmb.egg-info/
+-rw-r--r--   0 stba       (501) staff       (20)     6912 2023-04-25 23:42:24.000000 tcmb-0.3.0/tcmb.egg-info/PKG-INFO
+-rw-r--r--   0 stba       (501) staff       (20)      426 2023-04-25 23:42:24.000000 tcmb-0.3.0/tcmb.egg-info/SOURCES.txt
+-rw-r--r--   0 stba       (501) staff       (20)        1 2023-04-25 23:42:24.000000 tcmb-0.3.0/tcmb.egg-info/dependency_links.txt
+-rw-r--r--   0 stba       (501) staff       (20)       22 2023-04-25 23:42:24.000000 tcmb-0.3.0/tcmb.egg-info/requires.txt
+-rw-r--r--   0 stba       (501) staff       (20)        5 2023-04-25 23:42:24.000000 tcmb-0.3.0/tcmb.egg-info/top_level.txt
+drwxr-xr-x   0 stba       (501) staff       (20)        0 2023-04-25 23:42:24.748874 tcmb-0.3.0/tests/
+-rw-r--r--   0 stba       (501) staff       (20)        0 2023-01-07 22:09:47.000000 tcmb-0.3.0/tests/__init__.py
+-rw-r--r--   0 stba       (501) staff       (20)      167 2023-01-25 21:50:00.000000 tcmb-0.3.0/tests/test_auth.py
+-rw-r--r--   0 stba       (501) staff       (20)     1449 2023-01-25 21:50:00.000000 tcmb-0.3.0/tests/test_core.py
```

### Comparing `tcmb-0.2.0/.gitignore` & `tcmb-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tcmb-0.2.0/LICENSE` & `tcmb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcmb-0.2.0/PKG-INFO` & `tcmb-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcmb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Central Bank of the Republic of Türkiye (TCMB) Python API.
 Author-email: Kaymal <gutkyle@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 T.Kaymal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/kaymal/tcmb-py
+Project-URL: pypi, https://pypi.org/project/tcmb
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
@@ -62,21 +63,24 @@
 client = tcmb.Client(api_key="...")
 
 data = client.read(series="TP.DK.USD.S.YTL")
 ```
 
 ## Overview
 
-### Data Hiearchy
+### Data Hierarchy
+
 1. Categories:
 
-Categories are at the top level of the TCMB data hiearchy.
+Categories are at the top level of the TCMB data hierarchy.
 
 ```python
 client = tcmb.Client(api_key="...")
+
+# show categories
 Client.categories
 
 {'CATEGORY_ID': 1.0,
  'TOPIC_TITLE_ENG': 'MARKET STATISTICS',
  'TOPIC_TITLE_TR': 'PİYASA VERİLERİ'}
 ```
 
@@ -84,14 +88,16 @@
 
 2. Data Groups: 
 
 Each category consists of a number of data groups.
 
 ```python
 client = tcmb.Client(api_key="...")
+
+# show data groups
 Client.datagroups
 
 [{'DATAGROUP_CODE': 'bie_pyrepo',
   'CATEGORY_ID': 1,
   'DATAGROUP_NAME': 'Açık Piyasa Repo ve Ters Repo İşlemleri',
   'DATAGROUP_NAME_ENG': 'Open Market Repo and Reverse Repo Transactions',
   ...}
@@ -105,21 +111,37 @@
 It is also possible to filter the datagroups metadata using the `client.get_datagroups_metadata()` method.
 
 3. Series
 
 Datagroups consist of time series, each having a series key such as `TP.YSSK.A1` or `TP.DK.USD.S.YTL`. Series is read using the `.read()` method.
 
 ```python
+import tcmb
+
+client = tcmb.Client(api_key="...")
+
 # read one time series
 data = client.read("TP.YSSK.A1")
 
 # read multiple time series
 data = client.read(["TP.YSSK.A1", "TP.YSSK.A2", "TP.YSSK.A3"])
 ```
 
+A convenient way to read time series without initializing the Client instance is using the `read()` function in the `core.py` module.
+
+```python
+import tcmb
+
+# read one time series
+data = tcmb.read("TP.YSSK.A1", api_key="...")
+
+# read multiple time series
+data = tcmb.read(["TP.YSSK.A1", "TP.YSSK.A2", "TP.YSSK.A3"], api_key="...")
+```
+
 Series metadata can be fetched with `.get_series_metadata()` method.
 
 ```python
 # show metadata of each series within a data group
 client.get_series_metadata(datagroup="bie_yssk")
 
 [{'SERIE_CODE': 'TP.YSSK.A1',
@@ -139,35 +161,41 @@
 [{'SERIE_CODE': 'TP.YSSK.A1',
   'DATAGROUP_CODE': 'bie_yssk',
   'SERIE_NAME': '1-2 Yıl(ABD doları)',
   'SERIE_NAME_ENG': '1-2 Years(USD)',
   ...}]
 ```
 
+## Wildcard Characters
+
+The wildcard characters are represented as an asterisk `*` or a question mark `?`. The asterisk `*` represents any number of characters, while the question mark `?` represents a single character. Additionally, omitting the value has the same effect as using an asterisk. Note that, wildcard character option is not a feature of TCMB web service. Wildcard pattern search is implemented within the `tcmb` package and depends on the package data.
+
 ## Installation
 
 ```sh
 pip install tcmb
 ```
 
 ## Authentication
 
 An API key is required to access the Web Service. Users can sign up from the [login](https://evds2.tcmb.gov.tr/index.php?/evds/login) page. Once logged in, API Key is generated from the Profile page.
 
 There are two ways of providing API key to the `tcmb` client.
 - Using environment variables:
+
 ```shell
 $ export TCMB_API_KEY="..."
 ```
 
 ```python
 import os
 os.environ["TCMB_API_KEY"] = "..."
 ```
 
 - Passing `api_key` when initializing the `Client` class.
+
 ```python
 client = Client(api_key="...")
 ```
 
 ## Disclaimer
 `tcmb` is an **unofficial** open-source package intended for personal use and research purposes. Please see TCMB's [EVDS Disclaimer](https://evds2.tcmb.gov.tr/help/videos/EVDS_Disclaimer.pdf) for the official terms of use of the EVDS Web Service.
```

### Comparing `tcmb-0.2.0/README.md` & `tcmb-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,21 +24,24 @@
 client = tcmb.Client(api_key="...")
 
 data = client.read(series="TP.DK.USD.S.YTL")
 ```
 
 ## Overview
 
-### Data Hiearchy
+### Data Hierarchy
+
 1. Categories:
 
-Categories are at the top level of the TCMB data hiearchy.
+Categories are at the top level of the TCMB data hierarchy.
 
 ```python
 client = tcmb.Client(api_key="...")
+
+# show categories
 Client.categories
 
 {'CATEGORY_ID': 1.0,
  'TOPIC_TITLE_ENG': 'MARKET STATISTICS',
  'TOPIC_TITLE_TR': 'PİYASA VERİLERİ'}
 ```
 
@@ -46,14 +49,16 @@
 
 2. Data Groups: 
 
 Each category consists of a number of data groups.
 
 ```python
 client = tcmb.Client(api_key="...")
+
+# show data groups
 Client.datagroups
 
 [{'DATAGROUP_CODE': 'bie_pyrepo',
   'CATEGORY_ID': 1,
   'DATAGROUP_NAME': 'Açık Piyasa Repo ve Ters Repo İşlemleri',
   'DATAGROUP_NAME_ENG': 'Open Market Repo and Reverse Repo Transactions',
   ...}
@@ -67,21 +72,37 @@
 It is also possible to filter the datagroups metadata using the `client.get_datagroups_metadata()` method.
 
 3. Series
 
 Datagroups consist of time series, each having a series key such as `TP.YSSK.A1` or `TP.DK.USD.S.YTL`. Series is read using the `.read()` method.
 
 ```python
+import tcmb
+
+client = tcmb.Client(api_key="...")
+
 # read one time series
 data = client.read("TP.YSSK.A1")
 
 # read multiple time series
 data = client.read(["TP.YSSK.A1", "TP.YSSK.A2", "TP.YSSK.A3"])
 ```
 
+A convenient way to read time series without initializing the Client instance is using the `read()` function in the `core.py` module.
+
+```python
+import tcmb
+
+# read one time series
+data = tcmb.read("TP.YSSK.A1", api_key="...")
+
+# read multiple time series
+data = tcmb.read(["TP.YSSK.A1", "TP.YSSK.A2", "TP.YSSK.A3"], api_key="...")
+```
+
 Series metadata can be fetched with `.get_series_metadata()` method.
 
 ```python
 # show metadata of each series within a data group
 client.get_series_metadata(datagroup="bie_yssk")
 
 [{'SERIE_CODE': 'TP.YSSK.A1',
@@ -101,35 +122,41 @@
 [{'SERIE_CODE': 'TP.YSSK.A1',
   'DATAGROUP_CODE': 'bie_yssk',
   'SERIE_NAME': '1-2 Yıl(ABD doları)',
   'SERIE_NAME_ENG': '1-2 Years(USD)',
   ...}]
 ```
 
+## Wildcard Characters
+
+The wildcard characters are represented as an asterisk `*` or a question mark `?`. The asterisk `*` represents any number of characters, while the question mark `?` represents a single character. Additionally, omitting the value has the same effect as using an asterisk. Note that, wildcard character option is not a feature of TCMB web service. Wildcard pattern search is implemented within the `tcmb` package and depends on the package data.
+
 ## Installation
 
 ```sh
 pip install tcmb
 ```
 
 ## Authentication
 
 An API key is required to access the Web Service. Users can sign up from the [login](https://evds2.tcmb.gov.tr/index.php?/evds/login) page. Once logged in, API Key is generated from the Profile page.
 
 There are two ways of providing API key to the `tcmb` client.
 - Using environment variables:
+
 ```shell
 $ export TCMB_API_KEY="..."
 ```
 
 ```python
 import os
 os.environ["TCMB_API_KEY"] = "..."
 ```
 
 - Passing `api_key` when initializing the `Client` class.
+
 ```python
 client = Client(api_key="...")
 ```
 
 ## Disclaimer
 `tcmb` is an **unofficial** open-source package intended for personal use and research purposes. Please see TCMB's [EVDS Disclaimer](https://evds2.tcmb.gov.tr/help/videos/EVDS_Disclaimer.pdf) for the official terms of use of the EVDS Web Service.
```

### Comparing `tcmb-0.2.0/TODO.md` & `tcmb-0.3.0/TODO.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # tcmb
 
 ### TODO
-- [x] Update documentation
-    - [x] Add badges
-    - [x] Improve method docstrings
-- [x] Mock response with fixtures 
-- [x] Accept `start` and `end` in the `YYYY-MM-DD` format as well as the `DD-MM-YYYY` format.
-- [x] Release 0.2.0
+- [ ] Add CLI download option (csv, long/wide format)
+
 
 ### BACKLOG
-- [ ] Wildcard option for series
-- [ ] Save categories and datagroups metadata as package data for quicker lookup
-- [ ] Consider using requests Session
-- [ ] Add CLI download option
 - [ ] Add plotting module
+- [ ] Consider using requests Session
+- [ ] Consider adding asyncio support
 
 ### Done
 - [x] Initial release
-- [x] PyPI
+- [x] PyPI
+- [x] Update documentation
+    - [x] Add badges
+    - [x] Improve method docstrings
+- [x] Mock response with fixtures 
+- [x] Accept `start` and `end` in the `YYYY-MM-DD` format as well as the `DD-MM-YYYY` format.
+- [x] Release 0.2.0
+- [x] Add standalone reader that would work without creating the Client class instance
+- [x] Save categories and datagroups metadata as package data for quicker lookup
+- [x] Wildcard option for series
+- [x] Release 0.3.0
```

### Comparing `tcmb-0.2.0/pyproject.toml` & `tcmb-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tcmb"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = "Kaymal", email = "gutkyle@gmail.com" }]
 description = "Central Bank of the Republic of Türkiye (TCMB) Python API."
 readme = "README.md"
 license = { file = 'LICENSE' }
 requires-python = ">=3.8"
 classifiers = [
     'Operating System :: OS Independent',
@@ -18,10 +18,15 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = ["pandas", "numpy", "requests"]
 
 [project.urls]
 repository = "https://github.com/kaymal/tcmb-py"
+pypi = "https://pypi.org/project/tcmb"
 
-[tool.setuptools]
-packages = ["tcmb"]
+[tool.setuptools.packages.find]
+include = ["tcmb"]
+namespaces = true
+
+[tool.setuptools.package-data]
+"tcmb.resources" = ["*"]
```

### Comparing `tcmb-0.2.0/tcmb.egg-info/PKG-INFO` & `tcmb-0.3.0/tcmb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcmb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Central Bank of the Republic of Türkiye (TCMB) Python API.
 Author-email: Kaymal <gutkyle@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 T.Kaymal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/kaymal/tcmb-py
+Project-URL: pypi, https://pypi.org/project/tcmb
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
@@ -62,21 +63,24 @@
 client = tcmb.Client(api_key="...")
 
 data = client.read(series="TP.DK.USD.S.YTL")
 ```
 
 ## Overview
 
-### Data Hiearchy
+### Data Hierarchy
+
 1. Categories:
 
-Categories are at the top level of the TCMB data hiearchy.
+Categories are at the top level of the TCMB data hierarchy.
 
 ```python
 client = tcmb.Client(api_key="...")
+
+# show categories
 Client.categories
 
 {'CATEGORY_ID': 1.0,
  'TOPIC_TITLE_ENG': 'MARKET STATISTICS',
  'TOPIC_TITLE_TR': 'PİYASA VERİLERİ'}
 ```
 
@@ -84,14 +88,16 @@
 
 2. Data Groups: 
 
 Each category consists of a number of data groups.
 
 ```python
 client = tcmb.Client(api_key="...")
+
+# show data groups
 Client.datagroups
 
 [{'DATAGROUP_CODE': 'bie_pyrepo',
   'CATEGORY_ID': 1,
   'DATAGROUP_NAME': 'Açık Piyasa Repo ve Ters Repo İşlemleri',
   'DATAGROUP_NAME_ENG': 'Open Market Repo and Reverse Repo Transactions',
   ...}
@@ -105,21 +111,37 @@
 It is also possible to filter the datagroups metadata using the `client.get_datagroups_metadata()` method.
 
 3. Series
 
 Datagroups consist of time series, each having a series key such as `TP.YSSK.A1` or `TP.DK.USD.S.YTL`. Series is read using the `.read()` method.
 
 ```python
+import tcmb
+
+client = tcmb.Client(api_key="...")
+
 # read one time series
 data = client.read("TP.YSSK.A1")
 
 # read multiple time series
 data = client.read(["TP.YSSK.A1", "TP.YSSK.A2", "TP.YSSK.A3"])
 ```
 
+A convenient way to read time series without initializing the Client instance is using the `read()` function in the `core.py` module.
+
+```python
+import tcmb
+
+# read one time series
+data = tcmb.read("TP.YSSK.A1", api_key="...")
+
+# read multiple time series
+data = tcmb.read(["TP.YSSK.A1", "TP.YSSK.A2", "TP.YSSK.A3"], api_key="...")
+```
+
 Series metadata can be fetched with `.get_series_metadata()` method.
 
 ```python
 # show metadata of each series within a data group
 client.get_series_metadata(datagroup="bie_yssk")
 
 [{'SERIE_CODE': 'TP.YSSK.A1',
@@ -139,35 +161,41 @@
 [{'SERIE_CODE': 'TP.YSSK.A1',
   'DATAGROUP_CODE': 'bie_yssk',
   'SERIE_NAME': '1-2 Yıl(ABD doları)',
   'SERIE_NAME_ENG': '1-2 Years(USD)',
   ...}]
 ```
 
+## Wildcard Characters
+
+The wildcard characters are represented as an asterisk `*` or a question mark `?`. The asterisk `*` represents any number of characters, while the question mark `?` represents a single character. Additionally, omitting the value has the same effect as using an asterisk. Note that, wildcard character option is not a feature of TCMB web service. Wildcard pattern search is implemented within the `tcmb` package and depends on the package data.
+
 ## Installation
 
 ```sh
 pip install tcmb
 ```
 
 ## Authentication
 
 An API key is required to access the Web Service. Users can sign up from the [login](https://evds2.tcmb.gov.tr/index.php?/evds/login) page. Once logged in, API Key is generated from the Profile page.
 
 There are two ways of providing API key to the `tcmb` client.
 - Using environment variables:
+
 ```shell
 $ export TCMB_API_KEY="..."
 ```
 
 ```python
 import os
 os.environ["TCMB_API_KEY"] = "..."
 ```
 
 - Passing `api_key` when initializing the `Client` class.
+
 ```python
 client = Client(api_key="...")
 ```
 
 ## Disclaimer
 `tcmb` is an **unofficial** open-source package intended for personal use and research purposes. Please see TCMB's [EVDS Disclaimer](https://evds2.tcmb.gov.tr/help/videos/EVDS_Disclaimer.pdf) for the official terms of use of the EVDS Web Service.
```

### Comparing `tcmb-0.2.0/tests/test_core.py` & `tcmb-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

