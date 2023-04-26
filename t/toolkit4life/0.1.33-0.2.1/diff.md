# Comparing `tmp/toolkit4life-0.1.33.tar.gz` & `tmp/toolkit4life-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolkit4life-0.1.33.tar", last modified: Mon Feb 20 10:52:30 2023, max compression
+gzip compressed data, was "toolkit4life-0.2.1.tar", last modified: Wed Apr 26 15:24:42 2023, max compression
```

## Comparing `toolkit4life-0.1.33.tar` & `toolkit4life-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-02-20 10:52:30.657183 toolkit4life-0.1.33/
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     1074 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/LICENSE
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)       24 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/MANIFEST.in
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      789 2023-02-20 10:52:30.657183 toolkit4life-0.1.33/PKG-INFO
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      371 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/README.md
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      217 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/requirements.txt
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)       38 2023-02-20 10:52:30.657183 toolkit4life-0.1.33/setup.cfg
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     1630 2023-02-20 10:51:40.000000 toolkit4life-0.1.33/setup.py
-drwxrwxr-x   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-02-20 10:52:30.653183 toolkit4life-0.1.33/toolkit4life/
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/__init__.py
-drwxrwxr-x   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-02-20 10:52:30.657183 toolkit4life-0.1.33/toolkit4life/clients/
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/clients/__init__.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     2613 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/clients/_sqlalchemy.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     1277 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/clients/postgres.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     4109 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/clients/redis.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     1347 2023-02-20 10:50:54.000000 toolkit4life-0.1.33/toolkit4life/clients/trino.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     4554 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/logger.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     3117 2023-01-29 07:50:57.000000 toolkit4life-0.1.33/toolkit4life/requests.py
-drwxrwxr-x   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-02-20 10:52:30.657183 toolkit4life-0.1.33/toolkit4life/telegram/
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     2768 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/telegram/restrictors.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)     1746 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/threads.py
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      268 2023-01-29 07:47:26.000000 toolkit4life-0.1.33/toolkit4life/utils.py
-drwxrwxr-x   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        0 2023-02-20 10:52:30.653183 toolkit4life-0.1.33/toolkit4life.egg-info/
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      789 2023-02-20 10:52:30.000000 toolkit4life-0.1.33/toolkit4life.egg-info/PKG-INFO
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      552 2023-02-20 10:52:30.000000 toolkit4life-0.1.33/toolkit4life.egg-info/SOURCES.txt
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)        1 2023-02-20 10:52:30.000000 toolkit4life-0.1.33/toolkit4life.egg-info/dependency_links.txt
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)      218 2023-02-20 10:52:30.000000 toolkit4life-0.1.33/toolkit4life.egg-info/requires.txt
--rw-rw-r--   0 keivanipchihagh  (1000) keivanipchihagh  (1000)       13 2023-02-20 10:52:30.000000 toolkit4life-0.1.33/toolkit4life.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.777644 toolkit4life-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 15:24:42.773645 toolkit4life-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:24:42.777644 toolkit4life-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.757650 toolkit4life-0.2.1/toolkit4life/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.761649 toolkit4life-0.2.1/toolkit4life/clients/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/_sqlalchemy.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/redis.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.761649 toolkit4life-0.2.1/toolkit4life/telegram/
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/telegram/restrictors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.773645 toolkit4life-0.2.1/toolkit4life/utils/
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5397 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/utils/requests.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/utils/threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.757650 toolkit4life-0.2.1/toolkit4life.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/top_level.txt
```

### Comparing `toolkit4life-0.1.33/LICENSE` & `toolkit4life-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.1.33/PKG-INFO` & `toolkit4life-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolkit4life
-Version: 0.1.33
+Version: 0.2.1
 Summary: Faster deployment is what we want!
 Home-page: https://github.com/keivanipchihagh/toolkit4life
 Author: Keivan Ipchi Hagh
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `toolkit4life-0.1.33/setup.py` & `toolkit4life-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,25 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name = "toolkit4life",                                      # This is the name of the package
-    version = "0.1.33",                                         # The initial release version
+    version = "0.2.01",                                         # The initial release version
     author = "Keivan Ipchi Hagh",                               # Full name of the author
     url = "https://github.com/keivanipchihagh/toolkit4life",    # URL to the github repository
     description = "Faster deployment is what we want!",
     long_description = long_description,                        # Long description read from the the readme file
     long_description_content_type = "text/markdown",
-    packages = find_namespace_packages(include = ["toolkit4life", "toolkit4life.*"]),   # List of all python modules to be installed
+    packages = find_namespace_packages(
+        include = ["toolkit4life", "toolkit4life.*"]            # List of all python modules to be installed
+    ),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                                          # Information to filter the project on PyPi website
     python_requires = '>=3.6',                                  # Minimum version requirement of the package
     py_modules = ["toolkit4life"],                              # Name of the python package
-    # package_dir = {'':'toolkit4life'},                        # Directory of the source code of the package
     install_requires = required                                 # Install other dependencies if any
-)
+)
```

### Comparing `toolkit4life-0.1.33/toolkit4life/clients/_sqlalchemy.py` & `toolkit4life-0.2.1/toolkit4life/clients/_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.1.33/toolkit4life/clients/postgres.py` & `toolkit4life-0.2.1/toolkit4life/clients/postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 
 # Third-party imports
 from ._sqlalchemy import SQLAlchemy
 
 
 class PostgresClient(SQLAlchemy):
 
-    def __init__(self, host: str, port: str, username: str, password: str, database: str, schema: str = "public") -> None:
+    def __init__(self, host: str, port: str, username: str, password: str, database: str) -> None:
         """
             Creates and initializes a PostgreSQL engine instance that connects to the database
 
             Parameters:
                 host (str): Host IP address
                 port (str): Port number                
                 username (str): Username for authentication/privileges
                 password (str): Password for authentication
                 database (str): Name of the database
-                schema (str): Schema for the database
         """
         super().__init__(engine = "postgresql", host = host, port = port, database = database, username = username, password = password)
-        self.engine = create_engine(self.connection_string, connect_args = {"options": f"-csearch_path={schema}"})
+        self.engine = create_engine(self.connection_string)
 
 
     @property
     def connection_string(self) -> str:
         """ Returns the connection string """
         return f"{self.engine}://{self.username}:%s@{self.host}:{self.port}/{self.database}" % urlquote(self.password)
```

### Comparing `toolkit4life-0.1.33/toolkit4life/clients/redis.py` & `toolkit4life-0.2.1/toolkit4life/clients/redis.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.1.33/toolkit4life/clients/trino.py` & `toolkit4life-0.2.1/toolkit4life/clients/trino.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.1.33/toolkit4life/logger.py` & `toolkit4life-0.2.1/toolkit4life/utils/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,51 @@
-# https://stackoverflow.com/questions/1288498/using-the-same-decorator-with-arguments-with-functions-and-methods/1288936#1288936
-
 # Standard imports
 from time import time
 from typing import Callable
 from datetime import datetime
 
 
 def __now() -> str:
     """ Returns the current datetime as string """
     return datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
+
+
 def __run(func: Callable, *args, **kwargs) -> tuple:
     """ Runs the given function with args and kwargs and returns the result and execution time """
     start_time = time()
     result = func(*args, **kwargs)
     return result, round(time() - start_time, 2)
 
 
 
+def info(message: str) -> None:
+    """ Prints a message as Info """
+    print(f"[INFO - {__now()}] {message}")
+
+
+
+def success(message: str) -> None:
+    """ Prints a message as Success """
+    print(f"[SUCCESS - {__now()}] {message}")
+
+
+
+def error(message: str) -> None:
+    """ Prints a message as error """
+    print(f"[ERROR - {__now()}] {message}")
+
+
+
+def warning(message: str) -> None:
+    """ Prints a message as warning """
+    print(f"[WARNING - {__now()}] {message}")
+
+
+
 class _MethodDecoratorAdaptor(object):
 
     def __init__(self, decorator, func):
         self.decorator = decorator
         self.func = func
 
 
@@ -44,20 +68,20 @@
 
 def status():
     """ A decorator that notifies state of the function execution and its duration """
     @auto_adapt_to_methods
     def wrapper(func: Callable):
         def wrapped(*args, **kwargs):
             try:
-                print(f"[INFO - {__now()}] '{func.__name__}' started..")
+                info(f"Executing '{func.__name__}'..")
                 result, duration = __run(func, *args, **kwargs)
-                print(f"[SUCCESS - {__now()}] '{func.__name__}' executed successfully. (Took {duration} seconds)")
+                success(f"Finished executing '{func.__name__}'. (Took {duration} seconds)")
                 return result
             except Exception as ex:            
-                print(f"[ERROR - {__now()}] '{func.__name__}' failed to execute. (details: {ex})")
+                error(f"Failed to execute '{func.__name__}'. (details: {ex})")
         return wrapped
     return wrapper
 
 
 
 def text(on_success: str, on_failure: str):
     """
@@ -68,18 +92,18 @@
             on_failure: Message to be shown when the function throws and exception
     """
     @auto_adapt_to_methods
     def wrapper(func: Callable):
         def wrapped(*args, **kwargs):
             try:
                 result, duration = __run(func, *args, **kwargs)
-                print(f"SUCCESS - [{__now()}] {on_success}. (Took {duration} seconds)")
+                success(f"SUCCESS - [{__now()}] {on_success}. (Took {duration} seconds)")
                 return result
             except Exception as ex:            
-                print(f"[ERROR - {__now()}] {on_failure}. (details: {ex})")
+                error(f"ERROR - [{__now()}] {on_failure}. (details: {ex})")
         return wrapped
     return wrapper
 
 
 
 def restart_on_crash(warn_on_exception: bool = True, retries: int = None):
     """
@@ -96,37 +120,16 @@
             while True:
                 try:
                     return func(*args, **kwargs)
                 except Exception as ex:
                     if retries is None: raise Exception(ex)
 
                     if warn_on_exception:
-                        print(f"[WARNING - {__now()}] '{func.__name__}' threw an exception! restarting {_retries + 1 }/{retries} ... (details: {ex})")
+                        warning(f"WARNING - [{__now()}] {func.__name__} threw an exception! restarting {_retries + 1 }/{retries} ... (details: {ex})")
                     _retries += 1   # Increment the number of retries
 
                 # Abort the function if the number of retries is greater than the maximum number of retries
                 if _retries >= retries:
-                    print(f"[ERROR - {__now()}] '{func.__name__}' was retried {retries} with no lucks! aborting... (max tries: {retries})")
+                    error(f"'{func.__name__}' threw an exception! aborting... (max tries: {retries})")
                     break
         return wrapped
     return wrapper
-
-
-
-def info(message: str) -> None:
-    """ Prints a message as Info """
-    print(f"[INFO - {__now()}] {message}")
-
-
-def success(message: str) -> None:
-    """ Prints a message as Success """
-    print(f"[SUCCESS - {__now()}] {message}")
-
-
-def error(message: str) -> None:
-    """ Prints a message as error """
-    print(f"[ERROR - {__now()}] {message}")
-
-
-def warning(message: str) -> None:
-    """ Prints a message as warning """
-    print(f"[WARNING - {__now()}] {message}")
```

### Comparing `toolkit4life-0.1.33/toolkit4life/telegram/restrictors.py` & `toolkit4life-0.2.1/toolkit4life/telegram/restrictors.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.1.33/toolkit4life.egg-info/PKG-INFO` & `toolkit4life-0.2.1/toolkit4life.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolkit4life
-Version: 0.1.33
+Version: 0.2.1
 Summary: Faster deployment is what we want!
 Home-page: https://github.com/keivanipchihagh/toolkit4life
 Author: Keivan Ipchi Hagh
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

