# Comparing `tmp/shindan_cli-1.1.0.tar.gz` & `tmp/shindan_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shindan_cli-1.1.0.tar", max compression
+gzip compressed data, was "shindan_cli-1.2.0.tar", max compression
```

## Comparing `shindan_cli-1.1.0.tar` & `shindan_cli-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-03-29 17:22:30.621952 shindan_cli-1.1.0/LICENSE
--rw-r--r--   0        0        0     3795 2023-03-29 17:22:30.621952 shindan_cli-1.1.0/README.md
--rw-r--r--   0        0        0     2037 2023-03-29 17:22:30.625952 shindan_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      210 2023-03-29 17:22:30.625952 shindan_cli-1.1.0/shindan_cli/__init__.py
--rw-r--r--   0        0        0     1630 2023-03-29 17:22:30.625952 shindan_cli-1.1.0/shindan_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-29 17:22:30.625952 shindan_cli-1.1.0/shindan_cli/py.typed
--rw-r--r--   0        0        0     2599 2023-03-29 17:22:30.625952 shindan_cli-1.1.0/shindan_cli/shindan.py
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 shindan_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3795 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/README.md
+-rw-r--r--   0        0        0     2037 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/main.py
+-rw-r--r--   0        0        0        0 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/py.typed
+-rw-r--r--   0        0        0     2678 2023-04-26 02:02:10.678422 shindan_cli-1.2.0/shindan_cli/shindan.py
+-rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 shindan_cli-1.2.0/PKG-INFO
```

### Comparing `shindan_cli-1.1.0/LICENSE` & `shindan_cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.1.0/README.md` & `shindan_cli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.1.0/pyproject.toml` & `shindan_cli-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -52,25 +52,25 @@
 description = "ShindanMaker (https://shindanmaker.com) CLI"
 keywords = ["shindanmaker", "cli"]
 name = "shindan_cli"
 packages = [{include = "shindan_cli"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/shindan-cli"
-version = "1.1.0"
+version = "1.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 beautifulsoup4 = "^4.11.2"
 lxml = "^4.9.2"
 requests = "^2.28.2"
 
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.2"
+mypy = ">=0.991,<1.3"
 pre-commit = "^2.20.0"
 taskipy = "^1.10.3"
 types-beautifulsoup4 = "^4.11.6.7"
 types-requests = "^2.28.11.14"
 lxml-stubs = "^0.4.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
```

### Comparing `shindan_cli-1.1.0/shindan_cli/main.py` & `shindan_cli-1.2.0/shindan_cli/main.py`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.1.0/shindan_cli/shindan.py` & `shindan_cli-1.2.0/shindan_cli/shindan.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,19 @@
 
     session = requests.session()
     s = session.get(url, headers=headers)
     if s.status_code != requests.codes.ok:
         raise ShindanError(s.status_code)
 
     source = BeautifulSoup(s.text, features="lxml")
+
+    # _token, shindanName, hiddenName=, type=name
     params = {i["name"]: i["value"] for i in source.find_all("input")[1:4]}
     params["shindanName"] = shindan_name
+    params["type"] = "name"
 
     login = session.post(url, data=params, headers=headers)
     if wait:
         time.sleep(random.uniform(2, 5))  # noqa: S311
 
     soup = BeautifulSoup(login.text, features="lxml")
     result_tag = soup.find(class_="flex-fill")
```

### Comparing `shindan_cli-1.1.0/PKG-INFO` & `shindan_cli-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shindan-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: ShindanMaker (https://shindanmaker.com) CLI
 Home-page: https://github.com/eggplants/shindan-cli
 License: MIT
 Keywords: shindanmaker,cli
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.7,<4
```

