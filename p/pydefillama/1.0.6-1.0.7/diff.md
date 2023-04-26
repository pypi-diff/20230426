# Comparing `tmp/pydefillama-1.0.6.tar.gz` & `tmp/pydefillama-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydefillama-1.0.6.tar", last modified: Tue Apr 25 21:29:14 2023, max compression
+gzip compressed data, was "pydefillama-1.0.7.tar", last modified: Tue Apr 25 21:58:54 2023, max compression
```

## Comparing `pydefillama-1.0.6.tar` & `pydefillama-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:29:14.137380 pydefillama-1.0.6/
--rw-r--r--   0 nirmal     (501) staff       (20)     1064 2023-04-25 14:06:51.000000 pydefillama-1.0.6/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     2166 2023-04-25 21:29:14.137259 pydefillama-1.0.6/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)     1870 2023-04-25 21:22:11.000000 pydefillama-1.0.6/README.md
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:29:14.134845 pydefillama-1.0.6/pydefillama/
--rw-r--r--   0 nirmal     (501) staff       (20)       41 2023-04-25 15:59:53.000000 pydefillama-1.0.6/pydefillama/__init__.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:29:14.136413 pydefillama-1.0.6/pydefillama/src/
--rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-04-25 16:01:08.000000 pydefillama-1.0.6/pydefillama/src/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)     5897 2023-04-25 21:14:16.000000 pydefillama-1.0.6/pydefillama/src/fetcher.py
--rw-r--r--   0 nirmal     (501) staff       (20)      110 2023-04-25 14:30:17.000000 pydefillama-1.0.6/pydefillama/src/utils.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:29:14.136971 pydefillama-1.0.6/pydefillama/tests/
--rw-r--r--   0 nirmal     (501) staff       (20)       29 2023-04-25 16:07:05.000000 pydefillama-1.0.6/pydefillama/tests/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)     2464 2023-04-25 21:14:16.000000 pydefillama-1.0.6/pydefillama/tests/fetcher_tests.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:29:14.135774 pydefillama-1.0.6/pydefillama.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     2166 2023-04-25 21:29:14.000000 pydefillama-1.0.6/pydefillama.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      403 2023-04-25 21:29:14.000000 pydefillama-1.0.6/pydefillama.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 21:29:14.000000 pydefillama-1.0.6/pydefillama.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 14:46:30.000000 pydefillama-1.0.6/pydefillama.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       28 2023-04-25 21:29:14.000000 pydefillama-1.0.6/pydefillama.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       12 2023-04-25 21:29:14.000000 pydefillama-1.0.6/pydefillama.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-25 21:29:14.137414 pydefillama-1.0.6/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      717 2023-04-25 21:29:09.000000 pydefillama-1.0.6/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.178470 pydefillama-1.0.7/
+-rw-r--r--   0 nirmal     (501) staff       (20)     1064 2023-04-25 14:06:51.000000 pydefillama-1.0.7/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     2304 2023-04-25 21:58:54.178344 pydefillama-1.0.7/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)     2008 2023-04-25 21:56:56.000000 pydefillama-1.0.7/README.md
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.175307 pydefillama-1.0.7/pydefillama/
+-rw-r--r--   0 nirmal     (501) staff       (20)       41 2023-04-25 15:59:53.000000 pydefillama-1.0.7/pydefillama/__init__.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.177450 pydefillama-1.0.7/pydefillama/src/
+-rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-04-25 16:01:08.000000 pydefillama-1.0.7/pydefillama/src/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)     5799 2023-04-25 21:57:37.000000 pydefillama-1.0.7/pydefillama/src/fetcher.py
+-rw-r--r--   0 nirmal     (501) staff       (20)      110 2023-04-25 14:30:17.000000 pydefillama-1.0.7/pydefillama/src/utils.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.178080 pydefillama-1.0.7/pydefillama/tests/
+-rw-r--r--   0 nirmal     (501) staff       (20)       29 2023-04-25 16:07:05.000000 pydefillama-1.0.7/pydefillama/tests/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)     3658 2023-04-25 21:56:46.000000 pydefillama-1.0.7/pydefillama/tests/fetcher_tests.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.176593 pydefillama-1.0.7/pydefillama.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     2304 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      403 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 14:46:30.000000 pydefillama-1.0.7/pydefillama.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       28 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       12 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-25 21:58:54.178502 pydefillama-1.0.7/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      717 2023-04-25 21:58:41.000000 pydefillama-1.0.7/setup.py
```

### Comparing `pydefillama-1.0.6/LICENSE` & `pydefillama-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydefillama-1.0.6/PKG-INFO` & `pydefillama-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pydefillama
-Version: 1.0.6
-Summary: Python Wrapper for DefiLlama endpoints
-Home-page: https://github.com/Artemis-xyz/DefiLlama-Python-Client
-Author: Artemis.xyz
-Author-email: team@artemis.xyz
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pydefillama: a DefiLlama Python client
 
 [![PyPi](https://github.com/Artemis-xyz/pydefillama/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Artemis-xyz/pydefillama/actions/workflows/python-package.yml)
 [![PyPi](https://img.shields.io/pypi/v/pydefillama)](https://pypi.org/project/pydefillama/)
 
 An unofficial DeFiLlama wrapper built for data science workflows.
 
@@ -41,15 +30,15 @@
 ```
 
 Full list of supported functions [here](https://github.com/Artemis-xyz/pydefillama/blob/main/pydefillama/src/fetcher.py).
 
 ## Run Tests
 
 ```
- python -m unittest discover
+python -m unittest discover
 ```
 
 ## Developing Locally
 
 ```
 # install module without pip
 python setup.py develop
@@ -64,14 +53,22 @@
 
 ## Contributing
 
 If you would like to contribute to this project, please open an issue or submit a PR.
 While we are open to all contributions, we would like to keep this project focused on data science workflows, which is why functions often return a pandas dataframe.
 If you would like to use this API for other purposes, please consider forking this repo.
 
+## Maintainers
+
+To push to PyPi, follow the following steps:
+
+- Update version in `setup.py`
+- Push to main branch
+- Run `./updatepip.sh`
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgements
 
 We are thankful for the DefiLlama team for providing this open API. If you would like to support them, consider donating to them [here](https://defillama.com/donations).
```

### Comparing `pydefillama-1.0.6/README.md` & `pydefillama-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pydefillama
+Version: 1.0.7
+Summary: Python Wrapper for DefiLlama endpoints
+Home-page: https://github.com/Artemis-xyz/DefiLlama-Python-Client
+Author: Artemis.xyz
+Author-email: team@artemis.xyz
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pydefillama: a DefiLlama Python client
 
 [![PyPi](https://github.com/Artemis-xyz/pydefillama/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Artemis-xyz/pydefillama/actions/workflows/python-package.yml)
 [![PyPi](https://img.shields.io/pypi/v/pydefillama)](https://pypi.org/project/pydefillama/)
 
 An unofficial DeFiLlama wrapper built for data science workflows.
 
@@ -30,15 +41,15 @@
 ```
 
 Full list of supported functions [here](https://github.com/Artemis-xyz/pydefillama/blob/main/pydefillama/src/fetcher.py).
 
 ## Run Tests
 
 ```
- python -m unittest discover
+python -m unittest discover
 ```
 
 ## Developing Locally
 
 ```
 # install module without pip
 python setup.py develop
@@ -53,14 +64,22 @@
 
 ## Contributing
 
 If you would like to contribute to this project, please open an issue or submit a PR.
 While we are open to all contributions, we would like to keep this project focused on data science workflows, which is why functions often return a pandas dataframe.
 If you would like to use this API for other purposes, please consider forking this repo.
 
+## Maintainers
+
+To push to PyPi, follow the following steps:
+
+- Update version in `setup.py`
+- Push to main branch
+- Run `./updatepip.sh`
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgements
 
 We are thankful for the DefiLlama team for providing this open API. If you would like to support them, consider donating to them [here](https://defillama.com/donations).
```

### Comparing `pydefillama-1.0.6/pydefillama/src/fetcher.py` & `pydefillama-1.0.7/pydefillama/src/fetcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,23 +145,21 @@
 
 def fetch_protocol_dex_volumes(protocol_slug: str) -> pd.DataFrame:
     url = f"https://api.llama.fi/summary/dexs/{protocol_slug}?excludeTotalDataChart=false&excludeTotalDataChartBreakdown=true&dataType=dailyVolume"
     r = requests.get(url)
     results = r.json()["totalDataChart"]
     df = pd.DataFrame(results)
     df.columns = ["date", "volume"]
-    df = df.set_index("date")
-    df.index = pd.to_datetime(df.index, unit="s").date
-    df = df.fillna(np.nan).replace([np.nan], [None]).reset_index()
+    df = _convert_df_column_to_date(df, unit="s")
+    df = df.fillna(np.nan).replace([np.nan], [None])
     return df
 
 
 def fetch_chain_dex_volumes(chain_name) -> pd.DataFrame:
     url = f"https://api.llama.fi/overview/dexs/{chain_name}?excludeTotalDataChart=false&excludeTotalDataChartBreakdown=true&dataType=dailyVolume"
     r = requests.get(url)
     results = r.json()["totalDataChart"]
     df = pd.DataFrame(results)
     df.columns = ["date", "volume"]
-    df = df.set_index("date")
-    df.index = pd.to_datetime(df.index, unit="s").date
-    df = df.fillna(np.nan).replace([np.nan], [None]).reset_index()
+    df = _convert_df_column_to_date(df, unit="s")
+    df = df.fillna(np.nan).replace([np.nan], [None])
     return df
```

### Comparing `pydefillama-1.0.6/pydefillama.egg-info/PKG-INFO` & `pydefillama-1.0.7/pydefillama.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydefillama
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python Wrapper for DefiLlama endpoints
 Home-page: https://github.com/Artemis-xyz/DefiLlama-Python-Client
 Author: Artemis.xyz
 Author-email: team@artemis.xyz
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 ```
 
 Full list of supported functions [here](https://github.com/Artemis-xyz/pydefillama/blob/main/pydefillama/src/fetcher.py).
 
 ## Run Tests
 
 ```
- python -m unittest discover
+python -m unittest discover
 ```
 
 ## Developing Locally
 
 ```
 # install module without pip
 python setup.py develop
@@ -64,14 +64,22 @@
 
 ## Contributing
 
 If you would like to contribute to this project, please open an issue or submit a PR.
 While we are open to all contributions, we would like to keep this project focused on data science workflows, which is why functions often return a pandas dataframe.
 If you would like to use this API for other purposes, please consider forking this repo.
 
+## Maintainers
+
+To push to PyPi, follow the following steps:
+
+- Update version in `setup.py`
+- Push to main branch
+- Run `./updatepip.sh`
+
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgements
 
 We are thankful for the DefiLlama team for providing this open API. If you would like to support them, consider donating to them [here](https://defillama.com/donations).
```

### Comparing `pydefillama-1.0.6/setup.py` & `pydefillama-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r") as requirements_file:
     requirements_text = requirements_file.read()
 
 requirements = requirements_text.split()
 
 setuptools.setup(
     name="pydefillama",
-    version="1.0.6",
+    version="1.0.7",
     description="Python Wrapper for DefiLlama endpoints",
     url="https://github.com/Artemis-xyz/DefiLlama-Python-Client",
     author="Artemis.xyz",
     author_email="team@artemis.xyz",
     license="MIT",
     packages=setuptools.find_packages(exclude="tests"),
     zip_safe=False,
```

