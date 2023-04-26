# Comparing `tmp/semantra-0.1.2.tar.gz` & `tmp/semantra-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantra-0.1.2.tar", last modified: Sun Apr 23 22:22:01 2023, max compression
+gzip compressed data, was "semantra-0.1.3.tar", last modified: Wed Apr 26 04:21:20 2023, max compression
```

## Comparing `semantra-0.1.2.tar` & `semantra-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.226478 semantra-0.1.2/
--rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.2/LICENSE
--rw-r--r--   0 freedmand   (501) staff       (20)    10623 2023-04-23 22:22:01.226032 semantra-0.1.2/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)    10080 2023-04-23 21:52:03.000000 semantra-0.1.2/README.md
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.207963 semantra-0.1.2/client/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.209895 semantra-0.1.2/client/public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.211944 semantra-0.1.2/client/public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-23 21:34:21.000000 semantra-0.1.2/client/public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-23 21:34:21.000000 semantra-0.1.2/client/public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-23 21:34:21.000000 semantra-0.1.2/client/public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.2/client/public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.2/client/public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.2/client/public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-23 22:21:45.000000 semantra-0.1.2/pyproject.toml
--rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-23 22:22:01.226525 semantra-0.1.2/setup.cfg
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.208245 semantra-0.1.2/src/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.216795 semantra-0.1.2/src/semantra/
--rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.2/src/semantra/__init__.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.219659 semantra-0.1.2/src/semantra/__pycache__/
--rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.2/src/semantra/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.2/src/semantra/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.2/src/semantra/__pycache__/pdf.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.2/src/semantra/__pycache__/semantra.cpython-39.pyc
--rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.2/src/semantra/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.220807 semantra-0.1.2/src/semantra/client_public/
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.221883 semantra-0.1.2/src/semantra/client_public/build/
--rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-23 21:34:21.000000 semantra-0.1.2/src/semantra/client_public/build/bundle.css
--rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-23 21:34:21.000000 semantra-0.1.2/src/semantra/client_public/build/bundle.js
--rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-23 21:34:21.000000 semantra-0.1.2/src/semantra/client_public/build/bundle.js.map
--rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.2/src/semantra/client_public/favicon.png
--rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.2/src/semantra/client_public/global.css
--rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.2/src/semantra/client_public/index.html
--rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-23 13:37:42.000000 semantra-0.1.2/src/semantra/models.py
--rw-r--r--   0 freedmand   (501) staff       (20)     3118 2023-04-23 04:31:52.000000 semantra-0.1.2/src/semantra/pdf.py
--rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-23 12:49:54.000000 semantra-0.1.2/src/semantra/semantra.py
--rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-22 20:05:23.000000 semantra-0.1.2/src/semantra/util.py
-drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-23 22:22:01.218164 semantra-0.1.2/src/semantra.egg-info/
--rw-r--r--   0 freedmand   (501) staff       (20)    10623 2023-04-23 22:22:01.000000 semantra-0.1.2/src/semantra.egg-info/PKG-INFO
--rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-23 22:22:01.000000 semantra-0.1.2/src/semantra.egg-info/SOURCES.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-23 22:22:01.000000 semantra-0.1.2/src/semantra.egg-info/dependency_links.txt
--rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-23 22:22:01.000000 semantra-0.1.2/src/semantra.egg-info/entry_points.txt
--rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-23 22:22:01.000000 semantra-0.1.2/src/semantra.egg-info/requires.txt
--rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-23 22:22:01.000000 semantra-0.1.2/src/semantra.egg-info/top_level.txt
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.028869 semantra-0.1.3/
+-rw-r--r--   0 freedmand   (501) staff       (20)     1071 2023-03-31 03:28:18.000000 semantra-0.1.3/LICENSE
+-rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-26 04:21:20.028656 semantra-0.1.3/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)    10075 2023-04-26 04:20:51.000000 semantra-0.1.3/README.md
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.016445 semantra-0.1.3/client/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.018545 semantra-0.1.3/client/public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.020494 semantra-0.1.3/client/public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-23 21:34:21.000000 semantra-0.1.3/client/public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-23 21:34:21.000000 semantra-0.1.3/client/public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-23 21:34:21.000000 semantra-0.1.3/client/public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.3/client/public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.3/client/public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.3/client/public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)     1020 2023-04-26 04:20:51.000000 semantra-0.1.3/pyproject.toml
+-rw-r--r--   0 freedmand   (501) staff       (20)       38 2023-04-26 04:21:20.028907 semantra-0.1.3/setup.cfg
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.016707 semantra-0.1.3/src/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.024271 semantra-0.1.3/src/semantra/
+-rw-r--r--   0 freedmand   (501) staff       (20)        0 2023-04-23 04:39:23.000000 semantra-0.1.3/src/semantra/__init__.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.026286 semantra-0.1.3/src/semantra/__pycache__/
+-rw-r--r--   0 freedmand   (501) staff       (20)      148 2023-04-23 04:39:41.000000 semantra-0.1.3/src/semantra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    10961 2023-04-23 04:37:57.000000 semantra-0.1.3/src/semantra/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     3086 2023-04-23 04:37:58.000000 semantra-0.1.3/src/semantra/__pycache__/pdf.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)    19561 2023-04-23 12:15:19.000000 semantra-0.1.3/src/semantra/__pycache__/semantra.cpython-39.pyc
+-rw-r--r--   0 freedmand   (501) staff       (20)     4744 2023-04-23 04:37:58.000000 semantra-0.1.3/src/semantra/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.026717 semantra-0.1.3/src/semantra/client_public/
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.027418 semantra-0.1.3/src/semantra/client_public/build/
+-rw-r--r--   0 freedmand   (501) staff       (20)    14304 2023-04-23 21:34:21.000000 semantra-0.1.3/src/semantra/client_public/build/bundle.css
+-rw-r--r--   0 freedmand   (501) staff       (20)   449083 2023-04-23 21:34:21.000000 semantra-0.1.3/src/semantra/client_public/build/bundle.js
+-rw-r--r--   0 freedmand   (501) staff       (20)  1495725 2023-04-23 21:34:21.000000 semantra-0.1.3/src/semantra/client_public/build/bundle.js.map
+-rw-r--r--   0 freedmand   (501) staff       (20)     3300 2023-04-09 04:23:49.000000 semantra-0.1.3/src/semantra/client_public/favicon.png
+-rw-r--r--   0 freedmand   (501) staff       (20)      890 2023-02-15 22:52:41.000000 semantra-0.1.3/src/semantra/client_public/global.css
+-rw-r--r--   0 freedmand   (501) staff       (20)      434 2023-04-09 20:49:05.000000 semantra-0.1.3/src/semantra/client_public/index.html
+-rw-r--r--   0 freedmand   (501) staff       (20)    11501 2023-04-26 04:12:41.000000 semantra-0.1.3/src/semantra/models.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     3325 2023-04-26 04:20:51.000000 semantra-0.1.3/src/semantra/pdf.py
+-rw-r--r--   0 freedmand   (501) staff       (20)    28701 2023-04-26 04:12:41.000000 semantra-0.1.3/src/semantra/semantra.py
+-rw-r--r--   0 freedmand   (501) staff       (20)     4524 2023-04-26 04:12:41.000000 semantra-0.1.3/src/semantra/util.py
+drwxr-xr-x   0 freedmand   (501) staff       (20)        0 2023-04-26 04:21:20.025097 semantra-0.1.3/src/semantra.egg-info/
+-rw-r--r--   0 freedmand   (501) staff       (20)    10618 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/PKG-INFO
+-rw-r--r--   0 freedmand   (501) staff       (20)     1018 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/SOURCES.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        1 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/dependency_links.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)       52 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/entry_points.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)      176 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/requires.txt
+-rw-r--r--   0 freedmand   (501) staff       (20)        9 2023-04-26 04:21:20.000000 semantra-0.1.3/src/semantra.egg-info/top_level.txt
```

### Comparing `semantra-0.1.2/LICENSE` & `semantra-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/PKG-INFO` & `semantra-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.2
+Version: 0.1.3
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Semantra
 
-
-
 https://user-images.githubusercontent.com/306095/233867821-601db8b0-19c6-4bae-8e93-720b324dc199.mov
 
-
-
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
 
 The tool, made to run on the command line, analyzes specified text and PDF files on your computer and launches a local web search application for interactively querying them. The purpose of Semantra is to make running a specialized semantic search engine easy, friendly, configurable, and private/secure.
 
 Semantra is built for individuals seeking needles in haystacks — journalists sifting through leaked documents on deadline, researchers seeking insights within papers, students engaging with literature by querying themes, historians connecting events across books, and so forth.
 
 ## Resources
@@ -165,12 +161,12 @@
 
 The Python app is in `src/semantra/semantra.py` and is managed as a standard Python command-line project with `pyproject.toml`.
 
 The local web app is written in [Svelte](https://svelte.dev/) and managed as a standard npm application.
 
 To develop for the web app `cd` into `client` and then run `npm install`.
 
-To build the web app, run `npm run build`. The build the web app in watch mode and rebuild when there's changes, run `npm run build:watch`.
+To build the web app, run `npm run build`. To build the web app in watch mode and rebuild when there's changes, run `npm run build:watch`.
 
 ## Contributions
 
 The app is still in early stages, but contributions are welcome. Please feel free to submit an issue for any bugs or feature requests.
```

### Comparing `semantra-0.1.2/README.md` & `semantra-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # Semantra
 
-
-
 https://user-images.githubusercontent.com/306095/233867821-601db8b0-19c6-4bae-8e93-720b324dc199.mov
 
-
-
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
 
 The tool, made to run on the command line, analyzes specified text and PDF files on your computer and launches a local web search application for interactively querying them. The purpose of Semantra is to make running a specialized semantic search engine easy, friendly, configurable, and private/secure.
 
 Semantra is built for individuals seeking needles in haystacks — journalists sifting through leaked documents on deadline, researchers seeking insights within papers, students engaging with literature by querying themes, historians connecting events across books, and so forth.
 
 ## Resources
@@ -151,12 +147,12 @@
 
 The Python app is in `src/semantra/semantra.py` and is managed as a standard Python command-line project with `pyproject.toml`.
 
 The local web app is written in [Svelte](https://svelte.dev/) and managed as a standard npm application.
 
 To develop for the web app `cd` into `client` and then run `npm install`.
 
-To build the web app, run `npm run build`. The build the web app in watch mode and rebuild when there's changes, run `npm run build:watch`.
+To build the web app, run `npm run build`. To build the web app in watch mode and rebuild when there's changes, run `npm run build:watch`.
 
 ## Contributions
 
 The app is still in early stages, but contributions are welcome. Please feel free to submit an issue for any bugs or feature requests.
```

### Comparing `semantra-0.1.2/client/public/build/bundle.css` & `semantra-0.1.3/client/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/client/public/build/bundle.js` & `semantra-0.1.3/client/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/client/public/build/bundle.js.map` & `semantra-0.1.3/client/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/client/public/favicon.png` & `semantra-0.1.3/client/public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/client/public/global.css` & `semantra-0.1.3/client/public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/pyproject.toml` & `semantra-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantra"
-version = "0.1.2"
+version = "0.1.3"
 description = "A semantic search CLI tool"
 authors = [{name = "Dylan Freedman", email = "freedmand@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `semantra-0.1.2/src/semantra/__pycache__/models.cpython-39.pyc` & `semantra-0.1.3/src/semantra/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/__pycache__/pdf.cpython-39.pyc` & `semantra-0.1.3/src/semantra/__pycache__/pdf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/__pycache__/semantra.cpython-39.pyc` & `semantra-0.1.3/src/semantra/__pycache__/semantra.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/__pycache__/util.cpython-39.pyc` & `semantra-0.1.3/src/semantra/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/client_public/build/bundle.css` & `semantra-0.1.3/src/semantra/client_public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/client_public/build/bundle.js` & `semantra-0.1.3/src/semantra/client_public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/client_public/build/bundle.js.map` & `semantra-0.1.3/src/semantra/client_public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/client_public/favicon.png` & `semantra-0.1.3/src/semantra/client_public/favicon.png`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/client_public/global.css` & `semantra-0.1.3/src/semantra/client_public/global.css`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/models.py` & `semantra-0.1.3/src/semantra/models.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/pdf.py` & `semantra-0.1.3/src/semantra/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     pdf = pdfium.PdfDocument(filename)
     n_pages = len(pdf)
 
     if force or not os.path.exists(converted_txt) or not os.path.exists(position_index):
         positions = []
         position = 0
         # newline="" ensures pdfium's \r is preserved
-        with open(converted_txt, "w", newline="") as f:
+        with open(
+            converted_txt, "w", newline="", encoding="utf-8", errors="ignore"
+        ) as f:
             for page_index in tqdm(
                 range(n_pages),
                 desc="Extracting PDF contents",
                 leave=False,
                 disable=silent,
             ):
                 page = pdf[page_index]
@@ -74,19 +76,23 @@
                         "char_index": position,
                         "page_width": page_width,
                         "page_height": page_height,
                     }
                 )
                 position += f.write(pagetext)
                 position += f.write(LINE_FEED)
-        with open(position_index, "w") as f:
+        with open(position_index, "w", encoding="utf-8") as f:
             json.dump(positions, f)
-        with open(converted_txt, "r", newline="") as f:
+        with open(
+            converted_txt, "r", newline="", encoding="utf-8", errors="ignore"
+        ) as f:
             rawtext = f.read()
         return PDFContent(rawtext, filename, positions)
     else:
-        with open(converted_txt, "r", newline="") as f:
+        with open(
+            converted_txt, "r", newline="", encoding="utf-8", errors="ignore"
+        ) as f:
             rawtext = f.read()
-        with open(position_index, "r") as f:
+        with open(position_index, "r", encoding="utf-8") as f:
             positions = json.load(f)
 
         return PDFContent(rawtext, filename, positions)
```

### Comparing `semantra-0.1.2/src/semantra/semantra.py` & `semantra-0.1.3/src/semantra/semantra.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra/util.py` & `semantra-0.1.3/src/semantra/util.py`

 * *Files identical despite different names*

### Comparing `semantra-0.1.2/src/semantra.egg-info/PKG-INFO` & `semantra-0.1.3/src/semantra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: semantra
-Version: 0.1.2
+Version: 0.1.3
 Summary: A semantic search CLI tool
 Author-email: Dylan Freedman <freedmand@gmail.com>
 Project-URL: Homepage, https://github.com/freedmand/semantra
 Project-URL: Repository, https://github.com/freedmand/semantra
 Project-URL: Bug Tracker, https://github.com/freedmand/semantra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Semantra
 
-
-
 https://user-images.githubusercontent.com/306095/233867821-601db8b0-19c6-4bae-8e93-720b324dc199.mov
 
-
-
 Semantra is a multipurpose tool for semantically searching documents. Query by meaning rather than just by matching text.
 
 The tool, made to run on the command line, analyzes specified text and PDF files on your computer and launches a local web search application for interactively querying them. The purpose of Semantra is to make running a specialized semantic search engine easy, friendly, configurable, and private/secure.
 
 Semantra is built for individuals seeking needles in haystacks — journalists sifting through leaked documents on deadline, researchers seeking insights within papers, students engaging with literature by querying themes, historians connecting events across books, and so forth.
 
 ## Resources
@@ -165,12 +161,12 @@
 
 The Python app is in `src/semantra/semantra.py` and is managed as a standard Python command-line project with `pyproject.toml`.
 
 The local web app is written in [Svelte](https://svelte.dev/) and managed as a standard npm application.
 
 To develop for the web app `cd` into `client` and then run `npm install`.
 
-To build the web app, run `npm run build`. The build the web app in watch mode and rebuild when there's changes, run `npm run build:watch`.
+To build the web app, run `npm run build`. To build the web app in watch mode and rebuild when there's changes, run `npm run build:watch`.
 
 ## Contributions
 
 The app is still in early stages, but contributions are welcome. Please feel free to submit an issue for any bugs or feature requests.
```

### Comparing `semantra-0.1.2/src/semantra.egg-info/SOURCES.txt` & `semantra-0.1.3/src/semantra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

