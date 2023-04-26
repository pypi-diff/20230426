# Comparing `tmp/fileup-1.0.0.tar.gz` & `tmp/fileup-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fileup-1.0.0.tar", last modified: Mon Apr 24 17:56:36 2023, max compression
+gzip compressed data, was "fileup-1.1.0.tar", last modified: Wed Apr 26 17:55:30 2023, max compression
```

## Comparing `fileup-1.0.0.tar` & `fileup-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-24 17:56:36.616970 fileup-1.0.0/
--rw-r--r--   0 basnijholt   (501) staff       (20)     1511 2020-06-12 12:23:27.000000 fileup-1.0.0/LICENSE
--rw-r--r--   0 basnijholt   (501) staff       (20)     2474 2023-04-24 17:56:36.616595 fileup-1.0.0/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)     2148 2023-04-24 17:47:18.000000 fileup-1.0.0/README.md
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-24 17:56:36.612486 fileup-1.0.0/fileup.egg-info/
--rw-r--r--   0 basnijholt   (501) staff       (20)     2474 2023-04-24 17:56:36.000000 fileup-1.0.0/fileup.egg-info/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)      245 2023-04-24 17:56:36.000000 fileup-1.0.0/fileup.egg-info/SOURCES.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-04-24 17:56:36.000000 fileup-1.0.0/fileup.egg-info/dependency_links.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       35 2023-04-24 17:56:36.000000 fileup-1.0.0/fileup.egg-info/entry_points.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       58 2023-04-24 17:56:36.000000 fileup-1.0.0/fileup.egg-info/requires.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        7 2023-04-24 17:56:36.000000 fileup-1.0.0/fileup.egg-info/top_level.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)     5050 2023-04-24 17:43:02.000000 fileup-1.0.0/fileup.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     2008 2023-04-24 17:50:15.000000 fileup-1.0.0/pyproject.toml
--rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-04-24 17:56:36.617058 fileup-1.0.0/setup.cfg
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-24 17:56:36.616006 fileup-1.0.0/tests/
--rw-r--r--   0 basnijholt   (501) staff       (20)     3941 2023-04-24 17:45:09.000000 fileup-1.0.0/tests/test_fileup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:55:30.024330 fileup-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-26 17:55:02.000000 fileup-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-26 17:55:30.024330 fileup-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-26 17:55:02.000000 fileup-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:55:30.024330 fileup-1.1.0/fileup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-26 17:55:30.000000 fileup-1.1.0/fileup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-26 17:55:30.000000 fileup-1.1.0/fileup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:55:30.000000 fileup-1.1.0/fileup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 17:55:30.000000 fileup-1.1.0/fileup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 17:55:30.000000 fileup-1.1.0/fileup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 17:55:30.000000 fileup-1.1.0/fileup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-26 17:55:02.000000 fileup-1.1.0/fileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 17:55:02.000000 fileup-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:55:30.024330 fileup-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:55:30.024330 fileup-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-26 17:55:02.000000 fileup-1.1.0/tests/test_fileup.py
```

### Comparing `fileup-1.0.0/LICENSE` & `fileup-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fileup-1.0.0/PKG-INFO` & `fileup-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-Metadata-Version: 2.1
-Name: fileup
-Version: 1.0.0
-Summary: Easily upload files to an FTP-server and get back the url.
-Author-email: Bas Nijholt <bas@nijho.lt>
-Project-URL: Homepage, https://github.com/basnijholt/fileup
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 
 # :rocket: fileup - Effortless File Sharing for Command-Line Enthusiasts :rocket:
 
+[![PyPI](https://img.shields.io/pypi/v/fileup.svg)](https://pypi.python.org/pypi/fileup)
+[![Build Status](https://github.com/basnijholt/fileup/actions/workflows/pytest.yml/badge.svg)](https://github.com/basnijholt/fileup/actions/workflows/pytest.yml)
+[![CodeCov](https://codecov.io/gh/basnijholt/fileup/branch/main/graph/badge.svg)](https://codecov.io/gh/basnijholt/fileup)
+
+
 `fileup` is your go-to Python package for hassle-free uploading and sharing of files right from your command-line interface! 🖥️🔥 You can set a time limit after which the file will be automatically removed, ensuring the security of your data. 🕒🔒
 
 ## :books: Table of Contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
@@ -29,15 +23,15 @@
 
 
 ## :package: Installation
 
 To install `fileup`, simply run the following command:
 
 ```bash
-pip install -U https://github.com/basnijholt/fileup/archive/master.zip
+pip install -U fileup
 ```
 
 ## :memo: Configuration
 
 Before you can start sharing your files, you'll need to create a configuration file at `~/.config/fileup/config` with the following structure:
 
 ```less
```

### Comparing `fileup-1.0.0/README.md` & `fileup-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.1
+Name: fileup
+Version: 1.1.0
+Summary: Easily upload files to an FTP-server and get back the url.
+Author-email: Bas Nijholt <bas@nijho.lt>
+Project-URL: Homepage, https://github.com/basnijholt/fileup
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 
 # :rocket: fileup - Effortless File Sharing for Command-Line Enthusiasts :rocket:
 
+[![PyPI](https://img.shields.io/pypi/v/fileup.svg)](https://pypi.python.org/pypi/fileup)
+[![Build Status](https://github.com/basnijholt/fileup/actions/workflows/pytest.yml/badge.svg)](https://github.com/basnijholt/fileup/actions/workflows/pytest.yml)
+[![CodeCov](https://codecov.io/gh/basnijholt/fileup/branch/main/graph/badge.svg)](https://codecov.io/gh/basnijholt/fileup)
+
+
 `fileup` is your go-to Python package for hassle-free uploading and sharing of files right from your command-line interface! 🖥️🔥 You can set a time limit after which the file will be automatically removed, ensuring the security of your data. 🕒🔒
 
 ## :books: Table of Contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
@@ -18,15 +34,15 @@
 
 
 ## :package: Installation
 
 To install `fileup`, simply run the following command:
 
 ```bash
-pip install -U https://github.com/basnijholt/fileup/archive/master.zip
+pip install -U fileup
 ```
 
 ## :memo: Configuration
 
 Before you can start sharing your files, you'll need to create a configuration file at `~/.config/fileup/config` with the following structure:
 
 ```less
```

### Comparing `fileup-1.0.0/fileup.egg-info/PKG-INFO` & `fileup-1.1.0/fileup.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: fileup
-Version: 1.0.0
+Version: 1.1.0
 Summary: Easily upload files to an FTP-server and get back the url.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/fileup
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 
 # :rocket: fileup - Effortless File Sharing for Command-Line Enthusiasts :rocket:
 
+[![PyPI](https://img.shields.io/pypi/v/fileup.svg)](https://pypi.python.org/pypi/fileup)
+[![Build Status](https://github.com/basnijholt/fileup/actions/workflows/pytest.yml/badge.svg)](https://github.com/basnijholt/fileup/actions/workflows/pytest.yml)
+[![CodeCov](https://codecov.io/gh/basnijholt/fileup/branch/main/graph/badge.svg)](https://codecov.io/gh/basnijholt/fileup)
+
+
 `fileup` is your go-to Python package for hassle-free uploading and sharing of files right from your command-line interface! 🖥️🔥 You can set a time limit after which the file will be automatically removed, ensuring the security of your data. 🕒🔒
 
 ## :books: Table of Contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
@@ -29,15 +34,15 @@
 
 
 ## :package: Installation
 
 To install `fileup`, simply run the following command:
 
 ```bash
-pip install -U https://github.com/basnijholt/fileup/archive/master.zip
+pip install -U fileup
 ```
 
 ## :memo: Configuration
 
 Before you can start sharing your files, you'll need to create a configuration file at `~/.config/fileup/config` with the following structure:
 
 ```less
```

### Comparing `fileup-1.0.0/fileup.py` & `fileup-1.1.0/fileup.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,21 @@
             try:
                 ftp.delete(file_name)
             except Exception as e:  # noqa: BLE001
                 print(f"Error: {e}")
             ftp.delete(file_name + "_delete_on_" + date)
 
 
-def file_up(filename: str | Path, *, time: float, direct: bool, img: bool) -> str:
+def fileup(
+    filename: str | Path,
+    *,
+    time: float = 90.0,
+    direct: bool = False,
+    img: bool = False,
+) -> str:
     """Upload a file to a server and return the url."""
     path = Path(filename).resolve()
     filename_base = path.name
 
     base_url, base_folder, folder, user, pw = read_config()
 
     # Connect to server
@@ -135,15 +141,15 @@
         default=90,
         help="If time is 0 the file will never be deleted, default is 90 days.",
     )
     parser.add_argument("-d", "--direct", action="store_true")
     parser.add_argument("-i", "--img", action="store_true")
     args = parser.parse_args()
 
-    url = file_up(args.filename, time=args.time, direct=args.direct, img=args.img)
+    url = fileup(args.filename, time=args.time, direct=args.direct, img=args.img)
 
     # Put a URL into clipboard only works on OS X
     with contextlib.suppress(Exception):
         process = subprocess.Popen(
             "pbcopy",
             env={"LANG": "en_US.UTF-8"},
             stdin=subprocess.PIPE,
```

### Comparing `fileup-1.0.0/pyproject.toml` & `fileup-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileup-1.0.0/tests/test_fileup.py` & `fileup-1.1.0/tests/test_fileup.py`

 * *Files identical despite different names*

