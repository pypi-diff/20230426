# Comparing `tmp/pygopac-0.3.0.tar.gz` & `tmp/pygopac-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygopac-0.3.0.tar", last modified: Sun Apr  2 17:53:01 2023, max compression
+gzip compressed data, was "pygopac-0.4.0.tar", last modified: Wed Apr 26 07:13:08 2023, max compression
```

## Comparing `pygopac-0.3.0.tar` & `pygopac-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-02 17:53:01.403055 pygopac-0.3.0/
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1074 2023-04-02 16:56:34.000000 pygopac-0.3.0/LICENSE
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1427 2023-04-02 17:53:01.402948 pygopac-0.3.0/PKG-INFO
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      648 2023-04-02 17:27:41.000000 pygopac-0.3.0/README.md
-drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-02 17:53:01.400713 pygopac-0.3.0/extension/
-drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-02 17:53:01.400783 pygopac-0.3.0/extension/src/
-drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-02 17:53:01.401871 pygopac-0.3.0/extension/src/gopaccli/
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      144 2023-04-02 16:56:34.000000 pygopac-0.3.0/extension/src/gopaccli/go.mod
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1780 2023-04-02 16:56:34.000000 pygopac-0.3.0/extension/src/gopaccli/go.sum
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1026 2023-04-02 16:56:34.000000 pygopac-0.3.0/extension/src/gopaccli/gopaccli.go
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      595 2023-04-01 11:07:10.000000 pygopac-0.3.0/extension/src/gopaccli/gopaccli_test.go
-drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-02 17:53:01.402231 pygopac-0.3.0/gopac/
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)       22 2023-04-01 11:07:10.000000 pygopac-0.3.0/gopac/__init__.py
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      298 2023-04-01 11:07:10.000000 pygopac-0.3.0/gopac/exceptions.py
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     3671 2023-04-02 17:27:41.000000 pygopac-0.3.0/gopac/gopac.py
-drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-02 17:53:01.402786 pygopac-0.3.0/pygopac.egg-info/
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1427 2023-04-02 17:53:01.000000 pygopac-0.3.0/pygopac.egg-info/PKG-INFO
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      406 2023-04-02 17:53:01.000000 pygopac-0.3.0/pygopac.egg-info/SOURCES.txt
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)        1 2023-04-02 17:53:01.000000 pygopac-0.3.0/pygopac.egg-info/dependency_links.txt
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)       17 2023-04-02 17:53:01.000000 pygopac-0.3.0/pygopac.egg-info/requires.txt
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)        6 2023-04-02 17:53:01.000000 pygopac-0.3.0/pygopac.egg-info/top_level.txt
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      996 2023-04-02 17:52:54.000000 pygopac-0.3.0/pyproject.toml
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)       38 2023-04-02 17:53:01.403093 pygopac-0.3.0/setup.cfg
--rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      321 2023-04-02 17:49:18.000000 pygopac-0.3.0/setup.py
+drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-26 07:13:08.541252 pygopac-0.4.0/
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1074 2023-04-02 16:56:34.000000 pygopac-0.4.0/LICENSE
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1460 2023-04-26 07:13:08.541112 pygopac-0.4.0/PKG-INFO
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      681 2023-04-26 06:49:56.000000 pygopac-0.4.0/README.md
+drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-26 07:13:08.538584 pygopac-0.4.0/extension/
+drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-26 07:13:08.538643 pygopac-0.4.0/extension/src/
+drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-26 07:13:08.539753 pygopac-0.4.0/extension/src/parser/
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      142 2023-04-23 20:26:09.000000 pygopac-0.4.0/extension/src/parser/go.mod
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1780 2023-04-23 20:26:09.000000 pygopac-0.4.0/extension/src/parser/go.sum
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      982 2023-04-23 20:12:52.000000 pygopac-0.4.0/extension/src/parser/main.go
+drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-26 07:13:08.540290 pygopac-0.4.0/gopac/
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)       22 2023-04-01 11:07:10.000000 pygopac-0.4.0/gopac/__init__.py
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      142 2023-04-23 20:06:43.000000 pygopac-0.4.0/gopac/exceptions.py
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     2800 2023-04-24 19:24:41.000000 pygopac-0.4.0/gopac/gopac.py
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      516 2023-04-23 20:06:43.000000 pygopac-0.4.0/gopac/structures.py
+drwxr-xr-x   0 alekseipetrunnik   (501) staff       (20)        0 2023-04-26 07:13:08.540943 pygopac-0.4.0/pygopac.egg-info/
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)     1460 2023-04-26 07:13:08.000000 pygopac-0.4.0/pygopac.egg-info/PKG-INFO
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      353 2023-04-26 07:13:08.000000 pygopac-0.4.0/pygopac.egg-info/SOURCES.txt
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)        1 2023-04-26 07:13:08.000000 pygopac-0.4.0/pygopac.egg-info/dependency_links.txt
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)       17 2023-04-26 07:13:08.000000 pygopac-0.4.0/pygopac.egg-info/requires.txt
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)        6 2023-04-26 07:13:08.000000 pygopac-0.4.0/pygopac.egg-info/top_level.txt
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      931 2023-04-24 18:58:42.000000 pygopac-0.4.0/pyproject.toml
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)       38 2023-04-26 07:13:08.541287 pygopac-0.4.0/setup.cfg
+-rw-r--r--   0 alekseipetrunnik   (501) staff       (20)      309 2023-04-26 06:57:30.000000 pygopac-0.4.0/setup.py
```

### Comparing `pygopac-0.3.0/LICENSE` & `pygopac-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygopac-0.3.0/PKG-INFO` & `pygopac-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygopac
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple library for working with pac files.
 Author-email: Aleksey Petrunnik <petrunnik.a@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/aleksey925/py-gopac
 Project-URL: repository, https://github.com/aleksey925/py-gopac
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-py-gopac
-========
+pygopac
+=======
 
 A simple library for working with pac files.
 
 ## Examples
 
 ```python
 import gopac
@@ -36,22 +36,22 @@
 
 ## Build wheel
 
 Requirements:
 
 - python
 - pdm (optional)
-- golang (The path to the executable file `go` should be in the PATH environment variable.
+- golang >= 1.20 (The path to the executable file `go` should be in the PATH environment variable.
   If the `go version` command is executed without errors, then everything is correctly configured.)
 - access to the internet
 
-Build with dpm:
+Build dist with pdm:
 
 ```
-make build-whl
+make build-dist-by-pdm
 ```
 
-Build with pip:
+Build dist using standard tools:
 
 ```
-make pip-build-whl
+make build-dist
 ```
```

### Comparing `pygopac-0.3.0/README.md` & `pygopac-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-py-gopac
-========
+pygopac
+=======
 
 A simple library for working with pac files.
 
 ## Examples
 
 ```python
 import gopac
@@ -16,22 +16,22 @@
 
 ## Build wheel
 
 Requirements:
 
 - python
 - pdm (optional)
-- golang (The path to the executable file `go` should be in the PATH environment variable.
+- golang >= 1.20 (The path to the executable file `go` should be in the PATH environment variable.
   If the `go version` command is executed without errors, then everything is correctly configured.)
 - access to the internet
 
-Build with dpm:
+Build dist with pdm:
 
 ```
-make build-whl
+make build-dist-by-pdm
 ```
 
-Build with pip:
+Build dist using standard tools:
 
 ```
-make pip-build-whl
+make build-dist
 ```
```

### Comparing `pygopac-0.3.0/extension/src/gopaccli/go.sum` & `pygopac-0.4.0/extension/src/parser/go.sum`

 * *Files identical despite different names*

### Comparing `pygopac-0.3.0/gopac/gopac.py` & `pygopac-0.4.0/gopac/gopac.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,95 @@
 import base64
+import ctypes
 import json
 import logging
-import os
-import subprocess
-import sys
-from functools import lru_cache
-from locale import getdefaultlocale
-from os.path import dirname, abspath, join
+from pathlib import Path
 from tempfile import gettempdir
 
 import requests
 
-from gopac.exceptions import (
-    CliNotFound, ErrorDecodeOutput, GoPacException, DownloadCancel,
-    DownloadPacFileException, SavePacFileException
-)
+from gopac.exceptions import SharedLibraryNotFound, DownloadCancel, GoPacException
+from gopac.structures import GoStr
 
 __all__ = ['find_proxy', 'download_pac_file', 'terminate_download_pac_file']
 
-EXTENSION_DIR = join(dirname(abspath(__file__)), 'extension')
-ENCODING = (
-    'cp866' if sys.platform in ('win32', 'cygwin') else
-    (getdefaultlocale()[1] if getdefaultlocale()[1] else 'UTF-8')
-)
-SERVICE_INFO = {
-    'pac_path': '',
-    'terminate_download': False
-}
-
 logger = logging.getLogger()
+extension_dir = Path(__file__).parent.absolute() / 'extension'
+_downloader_state = {'terminate_download': False}
+
+
+def get_shared_library() -> Path:
+    list_path = list(
+        filter(
+            lambda i: i.name.startswith('parser.') and not i.name.endswith('.h'),
+            extension_dir.iterdir()
+        )
+    )
+    if len(list_path) != 1:
+        raise SharedLibraryNotFound()
+    return list_path[0]
 
 
-def find_shared_library():
-    shared_library = list(filter(
-        lambda i: not i.endswith('.py') and i != '__pycache__', os.listdir(EXTENSION_DIR)
-    ))
-    if len(shared_library) != 1:
-        raise CliNotFound("CLI not found")
-    return join(EXTENSION_DIR, shared_library[0]).replace(r' ', r'\ ')
+def load_shared_lib(path: Path) -> ctypes.cdll.LoadLibrary:
+    library = ctypes.cdll.LoadLibrary(str(path))
+    library.ParseFile.argtypes = [GoStr, GoStr]
+    library.ParseFile.restype = ctypes.POINTER(ctypes.c_char_p)
+    library.FreePointer.argtypes = [ctypes.POINTER(ctypes.c_char_p)]
+    return library
+
+
+lib = load_shared_lib(get_shared_library())
 
 
 def get_pac_path(url):
-    return join(gettempdir(), base64.b64encode(url.encode()).decode()) + '.pac'
+    return Path(gettempdir()) / f'{base64.b64encode(url.encode()).decode()}.pac'
 
 
-def download_pac_file(url: str) -> str:
+def download_pac_file(url: str, path: Path | None = None) -> Path:
     """
     Downloads pac file to temporary directory
     :param url: url to pac file
+    :param path: path to the location where the downloaded file will be saved.
+    Will be saved to a temporary directory by default.
     :return: path to downloaded file
     """
     def download_hook(*args, **kwargs):
-        if SERVICE_INFO['terminate_download']:
+        if _downloader_state['terminate_download']:
             raise DownloadCancel()
 
-    SERVICE_INFO['terminate_download'] = False
+    _downloader_state['terminate_download'] = False
 
     try:
         response = requests.get(
             url, stream=True, timeout=15, hooks={'response': download_hook}
         )
     except DownloadCancel:
         logger.debug('File PAC download cancelled')
         raise
-    except Exception as e:
-        raise DownloadPacFileException(
-            'Error when downloading a file PAC', e
-        )
 
-    try:
-        SERVICE_INFO['pac_path'] = get_pac_path(url)
-        with open(SERVICE_INFO['pac_path'], mode='wb') as pac:
-            pac.write(response.content)
-        return SERVICE_INFO['pac_path']
-    except Exception as e:
-        message = 'Error in saving the downloaded pac file'
-        logger.exception(message)
-        raise SavePacFileException(message, e)
+    path = path or get_pac_path(url)
+    with open(path, mode='wb') as pac:
+        pac.write(response.content)
+
+    return path
 
 
 def terminate_download_pac_file():
-    SERVICE_INFO['terminate_download'] = True
+    _downloader_state['terminate_download'] = True
 
 
-@lru_cache(maxsize=None)
-def find_proxy(pac_file: str, url: str, encoding=None) -> dict:
+def find_proxy(pac_file: str, url: str) -> dict[str, str]:
     """
     Finds a proxy for a URL
     :param pac_file: path to downloaded file
     :param url: target url
-    :param encoding: system console encoding
     :return: dict like this {'http': 'url:port', 'https': 'url:port'} or
     an empty dict if no proxy is needed
     """
-    cmd = r'{} -pacFile "{}" -url {}'.format(find_shared_library(), pac_file, url)
-    encoding = encoding if encoding else ENCODING
-    try:
-        res = subprocess.check_output(cmd, shell=True).decode(encoding)
-    except subprocess.CalledProcessError:
-        raise ValueError(
-            'The data is not correct, it is not possible to perform a console '
-            'command'
-        )
-    except UnicodeError:
-        raise ErrorDecodeOutput(
-            'It was not possible to determine the encoding of the system '
-            'console and decode the result of the external program'
-        )
-    except Exception as e:
-        raise GoPacException('Unexpected error', e)
-
-    if res.startswith("marshal error"):
-        raise GoPacException(
-            'The external library was unable to form a response'
-        )
-    else:
-        res = json.loads(res)
-
-        if res['Error']:
-            raise GoPacException(res['Error'])
+    result_pointer: ctypes.POINTER(ctypes.c_char_p) = lib.ParseFile(pac_file, url)
+    value: bytes = ctypes.c_char_p.from_buffer(result_pointer).value
+    result = json.loads(value.decode())
+    lib.FreePointer(result_pointer)
+    if result['Error']:
+        raise GoPacException(result['Error'])
 
-        return res['Proxy']
+    return result["Proxy"]
```

### Comparing `pygopac-0.3.0/pygopac.egg-info/PKG-INFO` & `pygopac-0.4.0/pygopac.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygopac
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple library for working with pac files.
 Author-email: Aleksey Petrunnik <petrunnik.a@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/aleksey925/py-gopac
 Project-URL: repository, https://github.com/aleksey925/py-gopac
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-py-gopac
-========
+pygopac
+=======
 
 A simple library for working with pac files.
 
 ## Examples
 
 ```python
 import gopac
@@ -36,22 +36,22 @@
 
 ## Build wheel
 
 Requirements:
 
 - python
 - pdm (optional)
-- golang (The path to the executable file `go` should be in the PATH environment variable.
+- golang >= 1.20 (The path to the executable file `go` should be in the PATH environment variable.
   If the `go version` command is executed without errors, then everything is correctly configured.)
 - access to the internet
 
-Build with dpm:
+Build dist with pdm:
 
 ```
-make build-whl
+make build-dist-by-pdm
 ```
 
-Build with pip:
+Build dist using standard tools:
 
 ```
-make pip-build-whl
+make build-dist
 ```
```

### Comparing `pygopac-0.3.0/pyproject.toml` & `pygopac-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pygopac"
-version = "0.3.0"
+version = "0.4.0"
 description = "A simple library for working with pac files."
 authors = [{name = "Aleksey Petrunnik", email = "petrunnik.a@gmail.com"}]
 license = {text = "MIT"}
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
@@ -23,11 +23,11 @@
 [project.urls]
 homepage = "https://github.com/aleksey925/py-gopac"
 repository = "https://github.com/aleksey925/py-gopac"
 
 [build-system]
 requires = [
     "setuptools>=61.0.0",
-    "setuptools-golang-cli @ git+https://github.com/aleksey925/setuptools-golang-cli.git@0.0.3",
+    "setuptools-golang>=2.7.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
```

