# Comparing `tmp/fling_start-0.1.2.tar.gz` & `tmp/fling_start-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_start-0.1.2.tar", max compression
+gzip compressed data, was "fling_start-0.1.3.tar", max compression
```

## Comparing `fling_start-0.1.2.tar` & `fling_start-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.2/README.md
--rw-r--r--   0        0        0        6 2023-04-26 18:25:30.486564 fling_start-0.1.2/VERSION
--rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.2/fling/__init__.py
--rw-r--r--   0        0        0      427 2023-04-26 01:56:02.255573 fling_start-0.1.2/fling/start.py
--rw-r--r--   0        0        0      456 2023-04-26 18:23:34.476329 fling_start-0.1.2/fling/static/start/styles.css
--rw-r--r--   0        0        0     8363 2023-04-26 18:24:38.168476 fling_start-0.1.2/fling/templates/start/index.html
--rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.2/fling/templates/start/x3d.html
--rw-r--r--   0        0        0      600 2023-04-26 18:25:20.474919 fling_start-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 fling_start-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.3/README.md
+-rw-r--r--   0        0        0        6 2023-04-26 18:37:10.643832 fling_start-0.1.3/VERSION
+-rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.3/fling/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-26 01:56:02.255573 fling_start-0.1.3/fling/start.py
+-rw-r--r--   0        0        0      456 2023-04-26 18:23:34.476329 fling_start-0.1.3/fling/static/start/styles.css
+-rw-r--r--   0        0        0     8408 2023-04-26 18:33:51.929637 fling_start-0.1.3/fling/templates/start/index.html
+-rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.3/fling/templates/start/x3d.html
+-rw-r--r--   0        0        0      600 2023-04-26 18:37:08.260557 fling_start-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 fling_start-0.1.3/PKG-INFO
```

### Comparing `fling_start-0.1.2/fling/templates/start/index.html` & `fling_start-0.1.3/fling/templates/start/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       </p>
     <![endif]-->
 
   <div class="stacked">
     <div id="loading">
       <svg height="100%" width="100%" viewBox="-250 -250 250 250">
         <defs>
-          <filter id="blur">
+          <filter id="blur" x="-30%" y="-30%" width="160%" height="160%">
             <feDropShadow dx="10" dy="10" stdDeviation="2">
               <animate attributeName="stdDeviation" values="2 0; 0 2; 2 0; 0 2; 2 0; " dur="10s" repeatCount="indefinite" fill="freeze" />
               <animate attributeName="dx" values="0;5;0;-5;0" dur="10s" repeatCount="indefinite" fill="freeze" />
               <animate attributeName="dy" values="5;0;-5;0;5" dur="10s" repeatCount="indefinite" fill="freeze" />
             </feDropShadow>
           </filter>
           <!-- <path
```

### Comparing `fling_start-0.1.2/fling/templates/start/x3d.html` & `fling_start-0.1.3/fling/templates/start/x3d.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.2/pyproject.toml` & `fling_start-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-start"
-version = "0.1.2"
+version = "0.1.3"
 description = "Side Project Management from the command line"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" }, { path = "README.md" },
```

### Comparing `fling_start-0.1.2/PKG-INFO` & `fling_start-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-start
-Version: 0.1.2
+Version: 0.1.3
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

