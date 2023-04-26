# Comparing `tmp/py-ai-cli-0.3.2.tar.gz` & `tmp/py-ai-cli-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ai-cli-0.3.2.tar", last modified: Wed Apr 26 03:39:44 2023, max compression
+gzip compressed data, was "py-ai-cli-0.3.3.tar", last modified: Wed Apr 26 05:19:29 2023, max compression
```

## Comparing `py-ai-cli-0.3.2.tar` & `py-ai-cli-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1729 2023-04-26 03:39:25.591105 py-ai-cli-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     3155 2023-04-26 03:39:25.591105 py-ai-cli-0.3.2/README.md
--rw-r--r--   0        0        0     3940 2023-04-26 03:39:25.591105 py-ai-cli-0.3.2/README_ja.md
--rw-r--r--   0        0        0     2922 2023-04-26 03:39:25.591105 py-ai-cli-0.3.2/README_zh.md
--rw-r--r--   0        0        0     2021 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      680 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/src/ai_cli/__init__.py
--rw-r--r--   0        0        0     8231 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/src/ai_cli/bot/__init__.py
--rw-r--r--   0        0        0      195 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/src/ai_cli/bot/token.py
--rwxr-xr-x   0        0        0    13577 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/src/ai_cli/cli.py
--rw-r--r--   0        0        0     4468 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/src/ai_cli/git.py
--rw-r--r--   0        0        0     2882 2023-04-26 03:39:25.935111 py-ai-cli-0.3.2/src/ai_cli/setting.py
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 py-ai-cli-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1729 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3155 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/README.md
+-rw-r--r--   0        0        0     3940 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/README_ja.md
+-rw-r--r--   0        0        0     2922 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/README_zh.md
+-rw-r--r--   0        0        0     2021 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      680 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/src/ai_cli/__init__.py
+-rw-r--r--   0        0        0     8231 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/src/ai_cli/bot/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/src/ai_cli/bot/token.py
+-rwxr-xr-x   0        0        0    13577 2023-04-26 05:19:10.283737 py-ai-cli-0.3.3/src/ai_cli/cli.py
+-rw-r--r--   0        0        0     4468 2023-04-26 05:19:10.283737 py-ai-cli-0.3.3/src/ai_cli/git.py
+-rw-r--r--   0        0        0     2873 2023-04-26 05:19:10.283737 py-ai-cli-0.3.3/src/ai_cli/setting.py
+-rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 py-ai-cli-0.3.3/PKG-INFO
```

### Comparing `py-ai-cli-0.3.2/CHANGELOG.md` & `py-ai-cli-0.3.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/README.md` & `py-ai-cli-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/README_ja.md` & `py-ai-cli-0.3.3/README_ja.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/README_zh.md` & `py-ai-cli-0.3.3/README_zh.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/pyproject.toml` & `py-ai-cli-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     "pysocks>=1.7.1",
     "pyperclip>=1.8.2",
     "EdgeGPT>=0.1.22.1",
     "tiktoken>=0.3.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.2"
+version = "0.3.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/yufeikang/ai-cli"
 Documentation = "https://github.com/yufeikang/ai-cli/blob/main/README.md"
```

### Comparing `py-ai-cli-0.3.2/src/ai_cli/__init__.py` & `py-ai-cli-0.3.3/src/ai_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 import logging
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 
 HOME = Path.home()
```

### Comparing `py-ai-cli-0.3.2/src/ai_cli/bot/__init__.py` & `py-ai-cli-0.3.3/src/ai_cli/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/src/ai_cli/cli.py` & `py-ai-cli-0.3.3/src/ai_cli/cli.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/src/ai_cli/git.py` & `py-ai-cli-0.3.3/src/ai_cli/git.py`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.2/src/ai_cli/setting.py` & `py-ai-cli-0.3.3/src/ai_cli/setting.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 if old_setting_file.exists() and not setting_file.exists():
     setting_file.parent.mkdir(parents=True, exist_ok=True)
     old_setting_file.rename(setting_file)
 
 
 class Setting:
     api_key = None
-    endpoint = "https://api.openai.com/v1"
+    endpoint = None
     model = "gpt-3.5-turbo"
     no_stream = False
     bot = "GPTBot"  # GPTBot, BingBot,
     raw = False
     log_level = "INFO"
     debug = False
     proxy = None
@@ -44,16 +44,16 @@
 
     def __dict__(self):
         return {k: v for k, v in self.__iter__()}
 
     def set(self, k, v):
         if not hasattr(self, k):
             return
-        if v is None:
-            return
+        if v in ["None", "none"]:
+            v = None
         setattr(self, k, v)
 
     @classmethod
     def from_dict(cls, d):
         obj = cls()
         for k, v in d.items():
             if not hasattr(obj, k):
```

### Comparing `py-ai-cli-0.3.2/PKG-INFO` & `py-ai-cli-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ai_cli
-Version: 0.3.2
+Version: 0.3.3
 Summary: This CLI tool allows you to easily chat with chatGPT in the command line. You can chat with it, ask questions, and even translate text. It also
 License: MIT
 Author-email: Yufei Kang <kou.uhi.x@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Documentation, https://github.com/yufeikang/ai-cli/blob/main/README.md
 Project-URL: Repository, https://github.com/yufeikang/ai-cli
 Description-Content-Type: text/markdown
```

