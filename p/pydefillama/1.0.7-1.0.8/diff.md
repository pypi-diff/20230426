# Comparing `tmp/pydefillama-1.0.7.tar.gz` & `tmp/pydefillama-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydefillama-1.0.7.tar", last modified: Tue Apr 25 21:58:54 2023, max compression
+gzip compressed data, was "pydefillama-1.0.8.tar", last modified: Wed Apr 26 19:10:17 2023, max compression
```

## Comparing `pydefillama-1.0.7.tar` & `pydefillama-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.178470 pydefillama-1.0.7/
--rw-r--r--   0 nirmal     (501) staff       (20)     1064 2023-04-25 14:06:51.000000 pydefillama-1.0.7/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     2304 2023-04-25 21:58:54.178344 pydefillama-1.0.7/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)     2008 2023-04-25 21:56:56.000000 pydefillama-1.0.7/README.md
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.175307 pydefillama-1.0.7/pydefillama/
--rw-r--r--   0 nirmal     (501) staff       (20)       41 2023-04-25 15:59:53.000000 pydefillama-1.0.7/pydefillama/__init__.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.177450 pydefillama-1.0.7/pydefillama/src/
--rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-04-25 16:01:08.000000 pydefillama-1.0.7/pydefillama/src/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)     5799 2023-04-25 21:57:37.000000 pydefillama-1.0.7/pydefillama/src/fetcher.py
--rw-r--r--   0 nirmal     (501) staff       (20)      110 2023-04-25 14:30:17.000000 pydefillama-1.0.7/pydefillama/src/utils.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.178080 pydefillama-1.0.7/pydefillama/tests/
--rw-r--r--   0 nirmal     (501) staff       (20)       29 2023-04-25 16:07:05.000000 pydefillama-1.0.7/pydefillama/tests/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)     3658 2023-04-25 21:56:46.000000 pydefillama-1.0.7/pydefillama/tests/fetcher_tests.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-25 21:58:54.176593 pydefillama-1.0.7/pydefillama.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     2304 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      403 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 14:46:30.000000 pydefillama-1.0.7/pydefillama.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       28 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       12 2023-04-25 21:58:54.000000 pydefillama-1.0.7/pydefillama.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-25 21:58:54.178502 pydefillama-1.0.7/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      717 2023-04-25 21:58:41.000000 pydefillama-1.0.7/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.583180 pydefillama-1.0.8/
+-rw-r--r--   0 nirmal     (501) staff       (20)     1064 2023-04-25 14:06:51.000000 pydefillama-1.0.8/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     2307 2023-04-26 19:10:17.583050 pydefillama-1.0.8/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)     2011 2023-04-26 19:10:13.000000 pydefillama-1.0.8/README.md
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.580437 pydefillama-1.0.8/pydefillama/
+-rw-r--r--   0 nirmal     (501) staff       (20)       41 2023-04-25 15:59:53.000000 pydefillama-1.0.8/pydefillama/__init__.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.582426 pydefillama-1.0.8/pydefillama/src/
+-rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-04-25 16:01:08.000000 pydefillama-1.0.8/pydefillama/src/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)     5910 2023-04-26 19:10:13.000000 pydefillama-1.0.8/pydefillama/src/fetcher.py
+-rw-r--r--   0 nirmal     (501) staff       (20)      110 2023-04-25 14:30:17.000000 pydefillama-1.0.8/pydefillama/src/utils.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.582849 pydefillama-1.0.8/pydefillama/tests/
+-rw-r--r--   0 nirmal     (501) staff       (20)       29 2023-04-25 16:07:05.000000 pydefillama-1.0.8/pydefillama/tests/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)     3658 2023-04-26 19:10:13.000000 pydefillama-1.0.8/pydefillama/tests/fetcher_tests.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-26 19:10:17.581805 pydefillama-1.0.8/pydefillama.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     2307 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      403 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-25 14:46:30.000000 pydefillama-1.0.8/pydefillama.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       28 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       12 2023-04-26 19:10:17.000000 pydefillama-1.0.8/pydefillama.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-26 19:10:17.583219 pydefillama-1.0.8/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      717 2023-04-26 19:10:13.000000 pydefillama-1.0.8/setup.py
```

### Comparing `pydefillama-1.0.7/LICENSE` & `pydefillama-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydefillama-1.0.7/PKG-INFO` & `pydefillama-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydefillama
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python Wrapper for DefiLlama endpoints
 Home-page: https://github.com/Artemis-xyz/DefiLlama-Python-Client
 Author: Artemis.xyz
 Author-email: team@artemis.xyz
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -62,15 +62,15 @@
 ...
 ```
 
 ## Contributing
 
 If you would like to contribute to this project, please open an issue or submit a PR.
 While we are open to all contributions, we would like to keep this project focused on data science workflows, which is why functions often return a pandas dataframe.
-If you would like to use this API for other purposes, please consider forking this repo.
+If you would like to use this module for other purposes, please consider forking this repo.
 
 ## Maintainers
 
 To push to PyPi, follow the following steps:
 
 - Update version in `setup.py`
 - Push to main branch
```

### Comparing `pydefillama-1.0.7/README.md` & `pydefillama-1.0.8/pydefillama.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pydefillama
+Version: 1.0.8
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
 
@@ -51,15 +62,15 @@
 ...
 ```
 
 ## Contributing
 
 If you would like to contribute to this project, please open an issue or submit a PR.
 While we are open to all contributions, we would like to keep this project focused on data science workflows, which is why functions often return a pandas dataframe.
-If you would like to use this API for other purposes, please consider forking this repo.
+If you would like to use this module for other purposes, please consider forking this repo.
 
 ## Maintainers
 
 To push to PyPi, follow the following steps:
 
 - Update version in `setup.py`
 - Push to main branch
```

### Comparing `pydefillama-1.0.7/pydefillama/src/fetcher.py` & `pydefillama-1.0.8/pydefillama/src/fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 def fetch_protocol_tvl(protocol_slug: str) -> pd.DataFrame:
     url = f"https://api.llama.fi/protocol/{protocol_slug}"
     r = requests.get(url)
     data = r.json()
     df = pd.DataFrame(data["tvl"])
     df.columns = ["date", "tvl"]
     df = _convert_df_column_to_date(df, unit="s")
+    # get latest for each date
+    df = df.groupby("date").max().reset_index()
+    df = df.sort_values("date")
     return df
 
 
 def fetch_all_chains() -> list[dict]:
     def _transform_raw_chain(raw_chain):
         return {
             "gecko_id": raw_chain.get("gecko_id"),
```

### Comparing `pydefillama-1.0.7/pydefillama/tests/fetcher_tests.py` & `pydefillama-1.0.8/pydefillama/tests/fetcher_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         )
         self.assertTrue(len(uniswap_v3_entry) == 1)
         uniswap_v3_entry = uniswap_v3_entry[0]
         self.assertTrue(uniswap_v3_entry["symbol"] == "UNI")
         self.assertTrue(uniswap_v3_entry["parentProtocol"] == "parent#uniswap")
 
     def test_fetch_protocol_tvl(self):
-        df = llama.fetch_protocol_tvl("uniswap-v3")
+        df = llama.fetch_protocol_tvl("uniswap-v2")
         self.assertIsInstance(df, pd.DataFrame)
         self.assertTrue(df.columns[0] == "date")
         self.assertTrue(df.columns[1] == "tvl")
         self.assertTrue(df.iloc[-1]["tvl"] > 0)
 
     def test_fetch_chain_tvl(self):
         df = llama.fetch_chain_tvl("ethereum")
```

### Comparing `pydefillama-1.0.7/pydefillama.egg-info/PKG-INFO` & `pydefillama-1.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pydefillama
-Version: 1.0.7
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
 
@@ -62,15 +51,15 @@
 ...
 ```
 
 ## Contributing
 
 If you would like to contribute to this project, please open an issue or submit a PR.
 While we are open to all contributions, we would like to keep this project focused on data science workflows, which is why functions often return a pandas dataframe.
-If you would like to use this API for other purposes, please consider forking this repo.
+If you would like to use this module for other purposes, please consider forking this repo.
 
 ## Maintainers
 
 To push to PyPi, follow the following steps:
 
 - Update version in `setup.py`
 - Push to main branch
```

### Comparing `pydefillama-1.0.7/setup.py` & `pydefillama-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r") as requirements_file:
     requirements_text = requirements_file.read()
 
 requirements = requirements_text.split()
 
 setuptools.setup(
     name="pydefillama",
-    version="1.0.7",
+    version="1.0.8",
     description="Python Wrapper for DefiLlama endpoints",
     url="https://github.com/Artemis-xyz/DefiLlama-Python-Client",
     author="Artemis.xyz",
     author_email="team@artemis.xyz",
     license="MIT",
     packages=setuptools.find_packages(exclude="tests"),
     zip_safe=False,
```

