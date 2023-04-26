# Comparing `tmp/async_tkinter_loop-0.8.0.tar.gz` & `tmp/async_tkinter_loop-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_tkinter_loop-0.8.0.tar", max compression
+gzip compressed data, was "async_tkinter_loop-0.8.1.tar", max compression
```

## Comparing `async_tkinter_loop-0.8.0.tar` & `async_tkinter_loop-0.8.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-24 18:22:36.143923 async_tkinter_loop-0.8.0/LICENSE
--rw-r--r--   0        0        0     6448 2023-04-24 18:22:36.143923 async_tkinter_loop-0.8.0/README.md
--rw-r--r--   0        0        0     2498 2023-04-24 18:22:36.143923 async_tkinter_loop-0.8.0/async_tkinter_loop.py
--rw-r--r--   0        0        0     1292 2023-04-24 18:22:36.147923 async_tkinter_loop-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 async_tkinter_loop-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-25 14:32:47.861661 async_tkinter_loop-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6448 2023-04-25 14:32:47.861661 async_tkinter_loop-0.8.1/README.md
+-rw-r--r--   0        0        0     2502 2023-04-25 14:32:47.861661 async_tkinter_loop-0.8.1/async_tkinter_loop.py
+-rw-r--r--   0        0        0     1292 2023-04-25 14:32:47.865661 async_tkinter_loop-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 async_tkinter_loop-0.8.1/PKG-INFO
```

### Comparing `async_tkinter_loop-0.8.0/LICENSE` & `async_tkinter_loop-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_tkinter_loop-0.8.0/README.md` & `async_tkinter_loop-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `async_tkinter_loop-0.8.0/async_tkinter_loop.py` & `async_tkinter_loop-0.8.1/async_tkinter_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     An asynchronous implementation of tkinter mainloop
     :param root: tkinter root object
     :return: nothing
     """
     while True:
         # Process all pending events
-        while root.dooneevent(_tkinter.DONT_WAIT):
+        while root.dooneevent(_tkinter.DONT_WAIT) > 0:
             pass
 
         try:
             root.winfo_exists()  # Will throw TclError if the main window is destroyed
         except TclError:
             break
```

### Comparing `async_tkinter_loop-0.8.0/pyproject.toml` & `async_tkinter_loop-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-tkinter-loop"
-version = "0.8.0"
+version = "0.8.1"
 description = "Asynchronous mainloop implementation for tkinter"
 authors = ["insolor <insolor@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/insolor/async-tkinter-loop"
 repository = "https://github.com/insolor/async-tkinter-loop"
 keywords = ["tkinter", "async", "async-await", "asyncio", "aiohttp"]
```

### Comparing `async_tkinter_loop-0.8.0/PKG-INFO` & `async_tkinter_loop-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-tkinter-loop
-Version: 0.8.0
+Version: 0.8.1
 Summary: Asynchronous mainloop implementation for tkinter
 Home-page: https://github.com/insolor/async-tkinter-loop
 License: MIT
 Keywords: tkinter,async,async-await,asyncio,aiohttp
 Author: insolor
 Author-email: insolor@gmail.com
 Requires-Python: >=3.7,<4.0
```

