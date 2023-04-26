# Comparing `tmp/tap_messagebird-0.0.6.tar.gz` & `tmp/tap_messagebird-0.0.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_messagebird-0.0.6.tar", max compression
+gzip compressed data, was "tap_messagebird-0.0.6a1.tar", max compression
```

## Comparing `tap_messagebird-0.0.6.tar` & `tap_messagebird-0.0.6a1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/LICENSE
--rw-r--r--   0        0        0     3370 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/README.md
--rw-r--r--   0        0        0     1187 2023-04-25 19:14:50.754680 tap_messagebird-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      117 2023-04-25 19:14:50.754680 tap_messagebird-0.0.6/tap_messagebird/__init__.py
--rw-r--r--   0        0        0     3857 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/tap_messagebird/client.py
--rw-r--r--   0        0        0     3044 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/tap_messagebird/schemas/conversation.json
--rw-r--r--   0        0        0      993 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/tap_messagebird/schemas/conversation_message.json
--rw-r--r--   0        0        0     4240 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/tap_messagebird/schemas/message.json
--rw-r--r--   0        0        0     5204 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/tap_messagebird/streams.py
--rw-r--r--   0        0        0     1590 2023-04-25 19:14:25.898576 tap_messagebird-0.0.6/tap_messagebird/tap.py
--rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 tap_messagebird-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/LICENSE
+-rw-r--r--   0        0        0     3370 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/README.md
+-rw-r--r--   0        0        0     1167 2023-04-17 21:25:44.449824 tap_messagebird-0.0.6a1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-04-17 21:25:44.453824 tap_messagebird-0.0.6a1/tap_messagebird/__init__.py
+-rw-r--r--   0        0        0     3857 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/tap_messagebird/client.py
+-rw-r--r--   0        0        0     3044 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/tap_messagebird/schemas/conversation.json
+-rw-r--r--   0        0        0      993 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/tap_messagebird/schemas/conversation_message.json
+-rw-r--r--   0        0        0     4240 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/tap_messagebird/schemas/message.json
+-rw-r--r--   0        0        0     3621 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/tap_messagebird/streams.py
+-rw-r--r--   0        0        0     1590 2023-04-17 21:25:26.741426 tap_messagebird-0.0.6a1/tap_messagebird/tap.py
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 tap_messagebird-0.0.6a1/PKG-INFO
```

### Comparing `tap_messagebird-0.0.6/LICENSE` & `tap_messagebird-0.0.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/README.md` & `tap_messagebird-0.0.6a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/pyproject.toml` & `tap_messagebird-0.0.6a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "tap-messagebird"
-version = "0.0.6"
+version = "0.0.6-a.1"
 description = "`tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Meltano Team <hello@meltano.com>"]
 keywords = [
     "ELT",
     "Messagebird",
 ]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = "<3.11,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = { version=">=0.24,<0.26"}
+singer-sdk = { version="^0.24.0"}
 fs-s3fs = { version = "^1.1.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.extras]
 s3 = ["fs-s3fs"]
@@ -37,15 +37,15 @@
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.ruff]
-ignore = ["ANN101", "PLR2004", "N818"]
+ignore = ["ANN101"]
 select = ["ALL"]
 target-version = "py37"
 
 [tool.ruff.per-file-ignores]
 "scripts/*" = ["ANN", "D", "INP"]
 "tests/*" = ["ANN"]
```

### Comparing `tap_messagebird-0.0.6/tap_messagebird/client.py` & `tap_messagebird-0.0.6a1/tap_messagebird/client.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/tap_messagebird/schemas/conversation.json` & `tap_messagebird-0.0.6a1/tap_messagebird/schemas/conversation.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/tap_messagebird/schemas/conversation_message.json` & `tap_messagebird-0.0.6a1/tap_messagebird/schemas/conversation_message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/tap_messagebird/schemas/message.json` & `tap_messagebird-0.0.6a1/tap_messagebird/schemas/message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/tap_messagebird/tap.py` & `tap_messagebird-0.0.6a1/tap_messagebird/tap.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.6/PKG-INFO` & `tap_messagebird-0.0.6a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tap-messagebird
-Version: 0.0.6
+Version: 0.0.6a1
 Summary: `tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Messagebird
 Author: Meltano Team
 Author-email: hello@meltano.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: s3
 Requires-Dist: fs-s3fs (>=1.1.1,<2.0.0) ; extra == "s3"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: singer-sdk (>=0.24,<0.26)
+Requires-Dist: singer-sdk (>=0.24.0,<0.25.0)
 Description-Content-Type: text/markdown
 
 # `tap-messagebird`
 
 Messagebird tap class.
 
 Built with the [Meltano Singer SDK](https://sdk.meltano.com).
```

