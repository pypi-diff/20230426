# Comparing `tmp/one-api-tool-0.2.0.tar.gz` & `tmp/one-api-tool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.2.0.tar", last modified: Wed Apr 26 09:36:31 2023, max compression
+gzip compressed data, was "one-api-tool-0.2.1.tar", last modified: Wed Apr 26 10:10:41 2023, max compression
```

## Comparing `one-api-tool-0.2.0.tar` & `one-api-tool-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:36:31.175640 one-api-tool-0.2.0/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.0/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-26 09:36:31.175483 one-api-tool-0.2.0/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.0/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:36:31.172486 one-api-tool-0.2.0/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-26 09:36:31.000000 one-api-tool-0.2.0/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      490 2023-04-26 09:36:31.000000 one-api-tool-0.2.0/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-26 09:36:31.000000 one-api-tool-0.2.0/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-26 09:36:31.000000 one-api-tool-0.2.0/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       67 2023-04-26 09:36:31.000000 one-api-tool-0.2.0/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-26 09:36:31.000000 one-api-tool-0.2.0/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:36:31.173337 one-api-tool-0.2.0/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.0/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:36:31.174461 one-api-tool-0.2.0/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.0/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1569 2023-04-26 09:30:39.000000 one-api-tool-0.2.0/oneapi/commands/one_api_eval_file.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1300 2023-04-26 09:30:29.000000 one-api-tool-0.2.0/oneapi/commands/one_api_eval_one.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1108 2023-04-26 09:25:26.000000 one-api-tool-0.2.0/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6162 2023-04-26 09:02:32.000000 one-api-tool-0.2.0/oneapi/one_ai_eval.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9519 2023-04-26 08:55:00.000000 one-api-tool-0.2.0/oneapi/one_api.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:36:31.175131 one-api-tool-0.2.0/oneapi/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-26 09:01:28.000000 one-api-tool-0.2.0/oneapi/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2540 2023-04-26 04:21:33.000000 one-api-tool-0.2.0/oneapi/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-26 09:36:31.175687 one-api-tool-0.2.0/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1184 2023-04-26 09:36:24.000000 one-api-tool-0.2.0/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.144932 one-api-tool-0.2.1/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.2.1/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-26 10:10:41.144676 one-api-tool-0.2.1/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1697 2023-04-18 03:55:54.000000 one-api-tool-0.2.1/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.141544 one-api-tool-0.2.1/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2253 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      490 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)      173 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       67 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-26 10:10:41.000000 one-api-tool-0.2.1/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.142301 one-api-tool-0.2.1/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      172 2023-04-26 09:02:00.000000 one-api-tool-0.2.1/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.143553 one-api-tool-0.2.1/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.2.1/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1569 2023-04-26 09:30:39.000000 one-api-tool-0.2.1/oneapi/commands/one_api_eval_file.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1300 2023-04-26 10:05:38.000000 one-api-tool-0.2.1/oneapi/commands/one_api_eval_one.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1108 2023-04-26 09:25:26.000000 one-api-tool-0.2.1/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6162 2023-04-26 09:02:32.000000 one-api-tool-0.2.1/oneapi/one_ai_eval.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9519 2023-04-26 08:55:00.000000 one-api-tool-0.2.1/oneapi/one_api.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-26 10:10:41.144308 one-api-tool-0.2.1/oneapi/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       25 2023-04-26 09:01:28.000000 one-api-tool-0.2.1/oneapi/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2540 2023-04-26 04:21:33.000000 one-api-tool-0.2.1/oneapi/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-26 10:10:41.145034 one-api-tool-0.2.1/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1184 2023-04-26 10:10:00.000000 one-api-tool-0.2.1/setup.py
```

### Comparing `one-api-tool-0.2.0/LICENSE` & `one-api-tool-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/PKG-INFO` & `one-api-tool-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.0/README.md` & `one-api-tool-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.2.1/one_api_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.2.0/oneapi/commands/one_api_eval_file.py` & `one-api-tool-0.2.1/oneapi/commands/one_api_eval_file.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/oneapi/commands/one_api_eval_one.py` & `one-api-tool-0.2.1/oneapi/commands/one_api_eval_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from oneapi.one_api import OneAPITool
 
 def main():
     parser = argparse.ArgumentParser(description="one-eval-line <command> [<args>]")
     parser.add_argument("--config_file", type=str, help="config file path", required=True)
     parser.add_argument("--prompt", type=str, help="question", required=True)
     parser.add_argument("--answers", help="answer list", nargs='+',required=True)
-    parser.add_argument("--target",type=str, default="standard answer", help="", required=False)
+    parser.add_argument("--target",type=str, default="", help="standard answer", required=False)
     parser.add_argument("--model",type=str, default="", help="evaluate model name, e.g., gpt-35-turbo, gpt-4", required=False)
     parser.add_argument("--detail",type=bool, default=True, help="print every prompt and response detail", required=False)
     args = parser.parse_args()
     tool = OneAPITool.from_config_file(args.config_file)
     result = eval_one(
         prompt=args.prompt, 
         answers=args.answers,
```

### Comparing `one-api-tool-0.2.0/oneapi/commands/one_api_requst.py` & `one-api-tool-0.2.1/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/oneapi/one_ai_eval.py` & `one-api-tool-0.2.1/oneapi/one_ai_eval.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/oneapi/one_api.py` & `one-api-tool-0.2.1/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/oneapi/utils/data_utils.py` & `one-api-tool-0.2.1/oneapi/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.2.0/setup.py` & `one-api-tool-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

