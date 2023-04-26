# Comparing `tmp/exc_handler-1.0.3.tar.gz` & `tmp/exc_handler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exc_handler-1.0.3.tar", last modified: Tue Apr 25 14:46:11 2023, max compression
+gzip compressed data, was "exc_handler-1.0.4.tar", last modified: Tue Apr 25 15:35:43 2023, max compression
```

## Comparing `exc_handler-1.0.3.tar` & `exc_handler-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 14:46:11.558296 exc_handler-1.0.3/
--rw-rw-rw-   0        0        0      427 2023-04-25 14:46:11.557295 exc_handler-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 14:46:11.505329 exc_handler-1.0.3/exc_handler/
--rw-rw-rw-   0        0        0     1358 2023-04-25 14:24:07.000000 exc_handler-1.0.3/exc_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:46:11.553299 exc_handler-1.0.3/exc_handler.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-25 14:46:10.000000 exc_handler-1.0.3/exc_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-25 14:46:10.000000 exc_handler-1.0.3/exc_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 14:46:10.000000 exc_handler-1.0.3/exc_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 14:46:10.000000 exc_handler-1.0.3/exc_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 14:46:11.559295 exc_handler-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-04-25 14:44:55.000000 exc_handler-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:35:43.341974 exc_handler-1.0.4/
+-rw-rw-rw-   0        0        0      427 2023-04-25 15:35:43.339973 exc_handler-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-04-25 13:55:46.000000 exc_handler-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 15:35:43.302997 exc_handler-1.0.4/exc_handler/
+-rw-rw-rw-   0        0        0     1345 2023-04-25 15:34:20.000000 exc_handler-1.0.4/exc_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:35:43.336978 exc_handler-1.0.4/exc_handler.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 15:35:43.000000 exc_handler-1.0.4/exc_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 15:35:43.342974 exc_handler-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-04-25 15:34:25.000000 exc_handler-1.0.4/setup.py
```

### Comparing `exc_handler-1.0.3/README.md` & `exc_handler-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `exc_handler-1.0.3/exc_handler/__init__.py` & `exc_handler-1.0.4/exc_handler/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 from types import TracebackType
 from termcolor import colored
 
 def exc_handler(exc: Exception, value, tb: TracebackType):
 
 	current_time = dt.strftime(dt.now(), '%d.%m.%Y %H:%M:%S')
 
-	print(value)
 	tb: StackSummary = extract_tb(tb)
 
 	print()
 	for frame in tb:
 		raised = colored(f"file '{frame.filename}', line {frame.lineno}:", 'dark_grey')
 		print(raised, frame.line)
 
 	message = current_time + ' > ' + colored(f'{exc.__name__}', 'blue') + ': ' + colored(f'{value}', 'red')
 	print(message)
 	return f"{exc.__class__.__name__}: {exc}"
 
-sys.excepthook = exc_handler
+sys.excepthook = exc_handler
```

### Comparing `exc_handler-1.0.3/setup.py` & `exc_handler-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 Usage:
     - Just import this module
 """
 
 setup(
     name="exc_handler",
-    version="1.0.3",
+    version="1.0.4",
     description=doc,
     author="iineolineii",
     packages=["exc_handler"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
 	]
-)
+)
```

