# Comparing `tmp/pymavlog-0.1.1.tar.gz` & `tmp/pymavlog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymavlog-0.1.1.tar", max compression
+gzip compressed data, was "pymavlog-0.1.2.tar", max compression
```

## Comparing `pymavlog-0.1.1.tar` & `pymavlog-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-18 18:08:48.698553 pymavlog-0.1.1/LICENSE
--rw-r--r--   0        0        0     1651 2023-04-18 18:08:48.698553 pymavlog-0.1.1/README.md
--rw-r--r--   0        0        0      176 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/__init__.py
--rw-r--r--   0        0        0     5914 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/core.py
--rw-r--r--   0        0        0      137 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/errors.py
--rw-r--r--   0        0        0      121 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/helpers.py
--rw-r--r--   0        0        0     1072 2023-04-18 18:08:57.818637 pymavlog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 pymavlog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-26 07:41:51.286790 pymavlog-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1657 2023-04-26 07:41:51.286790 pymavlog-0.1.2/README.md
+-rw-r--r--   0        0        0      176 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/__init__.py
+-rw-r--r--   0        0        0     5976 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/core.py
+-rw-r--r--   0        0        0      137 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/errors.py
+-rw-r--r--   0        0        0      121 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/helpers.py
+-rw-r--r--   0        0        0     1072 2023-04-26 07:42:04.966868 pymavlog-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 pymavlog-0.1.2/PKG-INFO
```

### Comparing `pymavlog-0.1.1/LICENSE` & `pymavlog-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymavlog-0.1.1/README.md` & `pymavlog-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [![codecov](https://codecov.io/gh/rmargar/pymavlog/branch/main/graph/badge.svg?token=0APOFRD0BT)](https://codecov.io/gh/rmargar/pymavlog)
 ![test](https://github.com/rmargar/pymavlog/actions/workflows/test.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/pymavlog.svg)](https://badge.fury.io/py/pymavlog)
 
-# pyulog
+# pymavlog
 
 A lightweight python library to parse log files from ArduPilot vehicles based on the [MavLink](https://mavlink.io/) protocol. It is built on top of [pymavlink](https://github.com/ArduPilot/pymavlink) and uses [NumPy](https://numpy.org/) under the hood to vectorize messages.
 
 ## Installation
 
 Installation with pip:
 
 ```bash
-pip install pyulog
+pip install pymavlog
 ```
 
 or via Poetry
 
 ```bash
-poetry add pyulog
+poetry add pymavlog
 ```
 
 ## Development
 
 Install the package in editable mode:
 
 ```bash
```

### Comparing `pymavlog-0.1.1/pymavlog/core.py` & `pymavlog-0.1.2/pymavlog/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,19 +164,22 @@
     def parse(self):
         """
         Parses the log file in-memory
         """
         message: DFMessage
 
         while True:
-            message = self._mlog.recv_match(type=self._types)
+            message = self._mlog.recv_msg()
 
             if message is None:
                 break
 
+            if message.get_type() not in self._types:
+                continue
+
             message: DFMessage
 
             msg_dict = message.to_dict()
 
             self._parsed_data[message.get_type()].append_message(msg_dict)
 
             try:
```

### Comparing `pymavlog-0.1.1/pyproject.toml` & `pymavlog-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymavlog"
-version = "0.1.1"
+version = "0.1.2"
 description = "A lightweight python library to parse MavLink log files"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Ricardo Martinez <rik@rmargar.net>"
 ]
 classifiers = [
```

### Comparing `pymavlog-0.1.1/PKG-INFO` & `pymavlog-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymavlog
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight python library to parse MavLink log files
 Home-page: https://github.com/rmargar/pymavlog
 License: MIT
 Author: Ricardo Martinez
 Author-email: rik@rmargar.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -26,30 +26,30 @@
 Project-URL: Repository, https://github.com/rmargar/pymavlog
 Description-Content-Type: text/markdown
 
 [![codecov](https://codecov.io/gh/rmargar/pymavlog/branch/main/graph/badge.svg?token=0APOFRD0BT)](https://codecov.io/gh/rmargar/pymavlog)
 ![test](https://github.com/rmargar/pymavlog/actions/workflows/test.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/pymavlog.svg)](https://badge.fury.io/py/pymavlog)
 
-# pyulog
+# pymavlog
 
 A lightweight python library to parse log files from ArduPilot vehicles based on the [MavLink](https://mavlink.io/) protocol. It is built on top of [pymavlink](https://github.com/ArduPilot/pymavlink) and uses [NumPy](https://numpy.org/) under the hood to vectorize messages.
 
 ## Installation
 
 Installation with pip:
 
 ```bash
-pip install pyulog
+pip install pymavlog
 ```
 
 or via Poetry
 
 ```bash
-poetry add pyulog
+poetry add pymavlog
 ```
 
 ## Development
 
 Install the package in editable mode:
 
 ```bash
```

