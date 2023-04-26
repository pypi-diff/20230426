# Comparing `tmp/xiaogpt-1.42.tar.gz` & `tmp/xiaogpt-1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.42.tar", last modified: Wed Apr 19 13:30:55 2023, max compression
+gzip compressed data, was "xiaogpt-1.43.tar", last modified: Wed Apr 26 00:15:07 2023, max compression
```

## Comparing `xiaogpt-1.42.tar` & `xiaogpt-1.43.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-19 13:30:41.945454 xiaogpt-1.42/LICENSE
--rw-r--r--   0        0        0    11110 2023-04-19 13:30:41.945454 xiaogpt-1.42/README.md
--rw-r--r--   0        0        0      919 2023-04-19 13:30:55.297498 xiaogpt-1.42/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/__main__.py
--rw-r--r--   0        0        0      189 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      218 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     2895 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1386 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1732 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/cli.py
--rw-r--r--   0        0        0     5263 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/config.py
--rw-r--r--   0        0        0     1991 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/utils.py
--rw-r--r--   0        0        0    19359 2023-04-19 13:30:41.945454 xiaogpt-1.42/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11696 1970-01-01 00:00:00.000000 xiaogpt-1.42/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-26 00:14:50.347124 xiaogpt-1.43/LICENSE
+-rw-r--r--   0        0        0    11110 2023-04-26 00:14:50.347124 xiaogpt-1.43/README.md
+-rw-r--r--   0        0        0      919 2023-04-26 00:15:07.655227 xiaogpt-1.43/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      639 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      554 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3275 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1605 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1996 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5263 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18548 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    11696 1970-01-01 00:00:00.000000 xiaogpt-1.43/PKG-INFO
```

### Comparing `xiaogpt-1.42/LICENSE` & `xiaogpt-1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.42/README.md` & `xiaogpt-1.43/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.42/pyproject.toml` & `xiaogpt-1.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.42"
+version = "1.43"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.42/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.43/xiaogpt/bot/chatgptapi_bot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+from __future__ import annotations
+
 import openai
 from rich import print
 
 from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.utils import split_sentences
 
 
 class ChatGPTBot(BaseBot):
     default_options = {"model": "gpt-3.5-turbo"}
 
-    def __init__(self, openai_key, api_base=None, proxy=None, deployment_id=None):
+    def __init__(
+        self,
+        openai_key: str,
+        api_base: str | None = None,
+        proxy: str | None = None,
+        deployment_id: str | None = None,
+    ) -> None:
         self.history = []
         openai.api_key = openai_key
         if api_base:
             openai.api_base = api_base
             # if api_base ends with openai.azure.com, then set api_type to azure
             if api_base.endswith(("openai.azure.com/", "openai.azure.com")):
                 openai.api_type = "azure"
@@ -20,14 +28,23 @@
                 self.default_options = {
                     **self.default_options,
                     "engine": deployment_id,
                 }
         if proxy:
             openai.proxy = proxy
 
+    @classmethod
+    def from_config(cls, config):
+        return cls(
+            openai_key=config.openai_key,
+            api_base=config.api_base,
+            proxy=config.proxy,
+            deployment_id=config.deployment_id,
+        )
+
     async def ask(self, query, **options):
         ms = []
         for h in self.history:
             ms.append({"role": "user", "content": h[0]})
             ms.append({"role": "assistant", "content": h[1]})
         ms.append({"role": "user", "content": f"{query}"})
         kwargs = {**self.default_options, **options}
```

### Comparing `xiaogpt-1.42/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.43/xiaogpt/bot/gpt3_bot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import openai
 from rich import print
 
+from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.utils import split_sentences
 
 
-class GPT3Bot:
+class GPT3Bot(BaseBot):
     def __init__(self, openai_key, api_base=None, proxy=None):
         openai.api_key = openai_key
         if api_base:
             openai.api_base = api_base
         if proxy:
             openai.proxy = proxy
         self.history = []
 
+    @classmethod
+    def from_config(cls, config):
+        return cls(
+            openai_key=config.openai_key, api_base=config.api_base, proxy=config.proxy
+        )
+
     async def ask(self, query, **options):
         data = {
             "prompt": query,
             "model": "text-davinci-003",
             "max_tokens": 1024,
             "temperature": 1,
             "top_p": 1,
```

### Comparing `xiaogpt-1.42/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.43/xiaogpt/bot/newbing_bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 from __future__ import annotations
 
 import re
 
 from EdgeGPT import Chatbot, ConversationStyle
 
+from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.utils import split_sentences
 
 _reference_link_re = re.compile(r"\[\d+\]: .+?\n+")
 
 
-class NewBingBot:
+class NewBingBot(BaseBot):
     def __init__(
         self,
         bing_cookie_path: str = "",
         bing_cookies: dict | None = None,
         proxy: str | None = None,
     ):
         self.history = []
         self._bot = Chatbot(
             cookiePath=bing_cookie_path, cookies=bing_cookies, proxy=proxy
         )
 
+    @classmethod
+    def from_config(cls, config):
+        return cls(
+            bing_cookie_path=config.bing_cookie_path,
+            bing_cookies=config.bing_cookies,
+            proxy=config.proxy,
+        )
+
     @staticmethod
     def clean_text(s):
         s = s.replace("**", "")
         s = _reference_link_re.sub("", s)
         s = re.sub(r"\[[\^\d]+\]", "", s)
         return s.strip()
```

### Comparing `xiaogpt-1.42/xiaogpt/cli.py` & `xiaogpt-1.43/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.42/xiaogpt/config.py` & `xiaogpt-1.43/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.42/xiaogpt/utils.py` & `xiaogpt-1.43/xiaogpt/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import os
 import re
 import socket
 from http.cookies import SimpleCookie
+from typing import AsyncIterator
 from urllib.parse import urlparse
 
 from requests.utils import cookiejar_from_dict
 
 
 ### HELP FUNCTION ###
 def parse_cookie_string(cookie_string):
     cookie = SimpleCookie()
     cookie.load(cookie_string)
-    cookies_dict = {}
-    cookiejar = None
-    for k, m in cookie.items():
-        cookies_dict[k] = m.value
-        cookiejar = cookiejar_from_dict(cookies_dict, cookiejar=None, overwrite=True)
-    return cookiejar
+    cookies_dict = {k: m.value for k, m in cookie.items()}
+    return cookiejar_from_dict(cookies_dict, cookiejar=None, overwrite=True)
 
 
 _no_elapse_chars = re.compile(r"([「」『』《》“”'\"()（）]|(?<!-)-(?!-))", re.UNICODE)
 
 
-def calculate_tts_elapse(text):
+def calculate_tts_elapse(text: str) -> float:
     # for simplicity, we use a fixed speed
     speed = 4.5  # this value is picked by trial and error
     # Exclude quotes and brackets that do not affect the total elapsed time
     return len(_no_elapse_chars.sub("", text)) / speed
 
 
 _ending_punctuations = ("。", "？", "！", "；", ".", "?", "!", ";")
 
 
-async def split_sentences(text_stream):
+async def split_sentences(text_stream: AsyncIterator[str]) -> AsyncIterator[str]:
     cur = ""
     async for text in text_stream:
         cur += text
         if cur.endswith(_ending_punctuations):
             yield cur
             cur = ""
     if cur:
         yield cur
 
 
 ### for edge-tts utils ###
-def find_key_by_partial_string(dictionary, partial_key):
+def find_key_by_partial_string(dictionary: dict[str, str], partial_key: str) -> str:
     for key, value in dictionary.items():
         if key in partial_key:
             return value
 
 
 def validate_proxy(proxy_str: str) -> bool:
     """Do a simple validation of the http proxy string."""
@@ -59,14 +58,14 @@
         raise ValueError("Proxy scheme must be http or https")
     if not (parsed.hostname and parsed.port):
         raise ValueError("Proxy hostname and port must be set")
 
     return True
 
 
-def get_hostname():
+def get_hostname() -> str:
     if "XIAOGPT_HOSTNAME" in os.environ:
         return os.environ["XIAOGPT_HOSTNAME"]
 
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         s.connect(("8.8.8.8", 80))
         return s.getsockname()[0]
```

### Comparing `xiaogpt-1.42/xiaogpt/xiaogpt.py` & `xiaogpt-1.43/xiaogpt/xiaogpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import edge_tts
 import openai
 from aiohttp import ClientSession
 from miservice import MiAccount, MiIOService, MiNAService, miio_command
 from rich import print
 from rich.logging import RichHandler
 
-from xiaogpt.bot import ChatGPTBot, GPT3Bot, NewBingBot
+from xiaogpt.bot import get_bot
 from xiaogpt.config import (
     COOKIE_TEMPLATE,
     EDGE_TTS_DICT,
     LATEST_ASK_API,
     MI_ASK_SIMULATE_DATA,
     WAKEUP_KEYWORD,
     Config,
@@ -179,33 +179,15 @@
                 device_id=self.device_id, service_token=service_token, user_id=user_id
             )
             return parse_cookie_string(cookie_string)
 
     @property
     def chatbot(self):
         if self._chatbot is None:
-            if self.config.bot == "gpt3":
-                self._chatbot = GPT3Bot(
-                    self.config.openai_key, self.config.api_base, self.config.proxy
-                )
-            elif self.config.bot == "chatgptapi":
-                self._chatbot = ChatGPTBot(
-                    self.config.openai_key,
-                    self.config.api_base,
-                    self.config.proxy,
-                    self.config.deployment_id,
-                )
-            elif self.config.bot == "newbing":
-                self._chatbot = NewBingBot(
-                    bing_cookie_path=self.config.bing_cookie_path,
-                    bing_cookies=self.config.bing_cookies,
-                    proxy=self.config.proxy,
-                )
-            else:
-                raise Exception(f"Do not support {self.config.bot}")
+            self._chatbot = get_bot(self.config)
         return self._chatbot
 
     async def simulate_xiaoai_question(self):
         data = MI_ASK_SIMULATE_DATA
         # Convert the data['data'] value from a string to a dictionary
         data_dict = json.loads(data["data"])
         # Get the first item in the records list
```

### Comparing `xiaogpt-1.42/PKG-INFO` & `xiaogpt-1.43/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.42
+Version: 1.43
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

