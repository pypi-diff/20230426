# Comparing `tmp/lognflow-0.6.4.tar.gz` & `tmp/lognflow-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.6.4.tar", last modified: Thu Apr  6 03:40:33 2023, max compression
+gzip compressed data, was "lognflow-0.6.5.tar", last modified: Wed Apr 26 02:34:03 2023, max compression
```

## Comparing `lognflow-0.6.4.tar` & `lognflow-0.6.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:40:33.664771 lognflow-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-06 03:40:24.000000 lognflow-0.6.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-06 03:40:24.000000 lognflow-0.6.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-06 03:40:24.000000 lognflow-0.6.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-06 03:40:24.000000 lognflow-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-06 03:40:24.000000 lognflow-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-06 03:40:33.664771 lognflow-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-06 03:40:24.000000 lognflow-0.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:40:33.664771 lognflow-0.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-06 03:40:24.000000 lognflow-0.6.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:40:33.664771 lognflow-0.6.4/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-06 03:40:24.000000 lognflow-0.6.4/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69961 2023-04-06 03:40:24.000000 lognflow-0.6.4/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-06 03:40:24.000000 lognflow-0.6.4/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-06 03:40:24.000000 lognflow-0.6.4/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:40:33.664771 lognflow-0.6.4/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-06 03:40:33.000000 lognflow-0.6.4/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-06 03:40:33.000000 lognflow-0.6.4/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 03:40:33.000000 lognflow-0.6.4/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 03:40:33.000000 lognflow-0.6.4/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 03:40:33.000000 lognflow-0.6.4/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 03:40:33.000000 lognflow-0.6.4/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-06 03:40:33.664771 lognflow-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-06 03:40:24.000000 lognflow-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:40:33.664771 lognflow-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 03:40:24.000000 lognflow-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-06 03:40:24.000000 lognflow-0.6.4/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-06 03:40:24.000000 lognflow-0.6.4/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-06 03:40:24.000000 lognflow-0.6.4/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 02:33:52.000000 lognflow-0.6.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-26 02:33:52.000000 lognflow-0.6.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-26 02:33:52.000000 lognflow-0.6.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-26 02:33:52.000000 lognflow-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 02:33:52.000000 lognflow-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-26 02:34:03.827967 lognflow-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-26 02:33:52.000000 lognflow-0.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 02:33:52.000000 lognflow-0.6.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70379 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-26 02:33:52.000000 lognflow-0.6.5/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 02:34:03.000000 lognflow-0.6.5/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 02:34:03.827967 lognflow-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 02:33:52.000000 lognflow-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:34:03.827967 lognflow-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 02:33:52.000000 lognflow-0.6.5/tests/test_printprogress.py
```

### Comparing `lognflow-0.6.4/CONTRIBUTING.rst` & `lognflow-0.6.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/HISTORY.rst` & `lognflow-0.6.5/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 * time_in_file_name has been changed to time_tag, sorry there! but early stages.
 * time_tag is True in the constructor, but could always be set to False
 * All tests passed!
 
 0.6.0 (2023-03-22)
 ------------------
 * This is a stable release
-* All text files are handled by thw with statement
+* All text files are handled by the with statement
 * Renaming bug is fixed
 * all tests run properly.
 * lognflow has all that logviewer has. We will check if dir exists at every use
 
 0.6.1 (2023-03-22)
 ------------------
 * rename had a bug that is fixed
@@ -50,11 +50,17 @@
 * We support Python 3.7+ because of dataclasses
 * printprogress now can disable printing anything and return ETA at the __call__
 
 0.6.3 (2023-04-01)
 ------------------
 * lognflow class does all logviewer does. Maybe it is time to remove logviewer.
 
-0.6.4 (2023-04-10)
+0.6.4 (2023-04-06)
 ------------------
 * Better documentation and examples for readme
-* get_var is added to lognflow
+* get_var is added to lognflow to get buffered variables logged by log_var
+
+0.6.5 (2023-04-26)
+------------------
+* Fixed a bug in the docs to allow sphinx compile it.
+* log_var will log only the valid time stamps.
+* added end keyword argument to log_text
```

### Comparing `lognflow-0.6.4/LICENSE` & `lognflow-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/PKG-INFO` & `lognflow-0.6.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.4
+Version: 0.6.5
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -141,15 +141,15 @@
 * time_in_file_name has been changed to time_tag, sorry there! but early stages.
 * time_tag is True in the constructor, but could always be set to False
 * All tests passed!
 
 0.6.0 (2023-03-22)
 ------------------
 * This is a stable release
-* All text files are handled by thw with statement
+* All text files are handled by the with statement
 * Renaming bug is fixed
 * all tests run properly.
 * lognflow has all that logviewer has. We will check if dir exists at every use
 
 0.6.1 (2023-03-22)
 ------------------
 * rename had a bug that is fixed
@@ -160,11 +160,17 @@
 * We support Python 3.7+ because of dataclasses
 * printprogress now can disable printing anything and return ETA at the __call__
 
 0.6.3 (2023-04-01)
 ------------------
 * lognflow class does all logviewer does. Maybe it is time to remove logviewer.
 
-0.6.4 (2023-04-10)
+0.6.4 (2023-04-06)
 ------------------
 * Better documentation and examples for readme
-* get_var is added to lognflow
+* get_var is added to lognflow to get buffered variables logged by log_var
+
+0.6.5 (2023-04-26)
+------------------
+* Fixed a bug in the docs to allow sphinx compile it.
+* log_var will log only the valid time stamps.
+* added end keyword argument to log_text
```

### Comparing `lognflow-0.6.4/README.rst` & `lognflow-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/docs/Makefile` & `lognflow-0.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/docs/conf.py` & `lognflow-0.6.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'lognflow'
-copyright = "2022, Alireza Sadri"
+copyright = "2023, Alireza Sadri"
 author = "Alireza Sadri"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
```

### Comparing `lognflow-0.6.4/docs/installation.rst` & `lognflow-0.6.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/docs/make.bat` & `lognflow-0.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/lognflow/lognflow.py` & `lognflow-0.6.5/lognflow/lognflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,18 @@
             instance of the lognflow. 
         :type logs_root: pathlib.Path
         
         :param log_dir: 
             This is the final directory path for the log files. 
         :type log_dir: pathlib.Path
     
-        :param exp_prename:
+        :param log_prefix:
             this string will be put before the time tag for log_dir, when
             only logs_root is given.
-        :type exp_prename: str
+        :type log_prefix: str
         
         :param print_text: 
             If True, everything that is logged as text will be printed as well
         :type print_text: bool
         
         :param main_log_name: 
             main log file name, by default: 'main_log'
@@ -123,15 +123,15 @@
             log_... functions.
         :type time_tag: bool
     """
     
     def __init__(self, 
                  logs_root        : pathlib.Path = None,
                  log_dir          : pathlib.Path = None,
-                 exp_prename      : str          = None,
+                 log_prefix       : str          = None,
                  print_text       : bool         = True,
                  main_log_name    : str          = 'main_log',
                  log_flush_period : int          = 10,
                  time_tag         : bool         = True):
         self._init_time = time.time()
         self.time_tag = time_tag
 
@@ -143,16 +143,16 @@
                     logs_root = select_directory(logs_root)
                 except:
                     pass
             
             new_log_dir_found = False
             while(not new_log_dir_found):
                 log_dir_name = ''
-                if(exp_prename is not None):
-                    log_dir_name = str(exp_prename)
+                if(log_prefix is not None):
+                    log_dir_name = str(log_prefix)
                 log_dir_name += f'{self._init_time}/'
                 self.log_dir = \
                     pathlib.Path(logs_root) / log_dir_name
                 if(not self.log_dir.is_dir()):
                     new_log_dir_found = True
                 else:
                     self._init_time = time.time()
@@ -272,15 +272,16 @@
             to_be_logged=[],      
             log_fpath=fpath,         
             log_size_limit=log_size_limit,    
             log_size=0,          
             last_log_flush_time=0,
             log_flush_period=log_flush_period)  
 
-    def log_text_flush(self, log_name = None, flush = False):
+    def log_text_flush(self, log_name = None, 
+                       flush = False):
         """
         Keep str as a list of lines to be logged. This function must take the 
         log name too. Then put the str in the log file.
         """
         """ Flush the text logs
             Writing text to open(file, 'a') does not constantly happen on HDD.
             There is an OS buffer in between. This funciton should be called
@@ -314,14 +315,15 @@
                  to_be_logged = '', 
                  log_time_stamp = True,
                  print_text = None,
                  log_size_limit: int = int(1e+7),
                  time_tag : bool = None,
                  log_flush_period : int = None,
                  flush = False,
+                 end = '\n',
                  new_file = False):
         """ log a string into a text file
             You can shose a name for the log and give the text to put in it.
             Also you can pass a small numpy array. You can ask it to put time
             stamp in the log and in the log file name, you can disable
             printing the text. You can set the log size limit to split it into
             another file with a new time stamp.
@@ -339,17 +341,26 @@
                     Put time stamp for every entry of the log
             :param print_text : bool
                     if False, what is logged will not be printed.
             :param log_size_limit : int
                     log size limit in bytes.
             :param time_tag : bool
                     put time stamp in file names.
+            :param log_flush_period : int
+                    How often flush the log in seconds, if time passes this
+                    given period, it will flush the first time a text is logged,
+                    or if the logger is finilized.
             :param flush : bool
                     force flush into the log file
-            
+            :param end: str
+                    The last charachter for this call.
+            :param new_file: bool
+                    if a new file is needed. If time_tag is True, it will make
+                    a new file with a new name that has a time tag. If False,
+                    it closees the current text file and overwrites on it.
         """
         time_time = time.time() - self._init_time
 
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
         log_name = self.log_name if (log_name is None) else log_name
@@ -362,54 +373,36 @@
             print(to_be_logged)
                 
         if ( (not (log_name in self._loggers_dict)) or new_file):
             self._log_text_handler(log_name, 
                                    log_size_limit = log_size_limit,
                                    time_tag = time_tag)
 
-        ############################################
         curr_textinlog = self._loggers_dict[log_name]
         _logger = []
         if(log_time_stamp):
             _time_str = f'T:{time_time:>6.6f}| '
             _logger.append(_time_str)
-        if isinstance(to_be_logged, np.ndarray):
-            try:
-                _logger.append('numpy.ndarray')
-                if(to_be_logged.size()>100):
-                    _logger.append(', The first and last 50 elements:\n')
-                    to_be_logged = to_be_logged.ravel()
-                    _logstr = np.array2string(to_be_logged[:50])
-                    _logger.append(_logstr)
-                    _logger.append(' ... ')
-                    _logstr = np.array2string(to_be_logged[-50:])
-                    _logger.append(_logstr)
-                else:
-                    _logstr = ':\n' + np.array2string(to_be_logged)
-                    _logger.append(_logstr)
-            except:
-                _logger.append(' not possible to log ' + log_name + '\n')
-        else:
-            if(isinstance(to_be_logged, list)):
-                for _ in to_be_logged:
-                    _tolog = str(_)
-                    _logger.append(_tolog)
-            else:
-                _tolog = str(to_be_logged)
+        if(isinstance(to_be_logged, list)):
+            for _ in to_be_logged:
+                _tolog = str(_)
                 _logger.append(_tolog)
-            _logger.append('\n')
+        else:
+            _tolog = str(to_be_logged)
+            _logger.append(_tolog)
+        if(_logger[-1][-1] != end):
+            _logger.append(end)
         log_size = 0
         for _logger_el in _logger:
             curr_textinlog.to_be_logged.append(_logger_el)
             log_size += len(_logger_el)
         curr_textinlog.log_size += log_size
-        ############################################
         
         self.log_text_flush(log_name, flush)        
-        ############################################
+
         if(log_size >= curr_textinlog.log_size_limit):
             self._log_text_handler(log_name, 
                                    log_size_limit = curr_textinlog.log_size_limit,
                                    time_tag = curr_textinlog.time_tag)
             curr_textinlog = self._loggers_dict[log_name]
         return curr_textinlog.log_fpath
                         
@@ -509,24 +502,26 @@
             examples: myvar or myscript/myvar
                 parameter_name can be just a name e.g. myvar, or could be a
                 path like name such as myscript/myvar.
         """
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         
         _var = self._vars_dict[parameter_name]
+        _var_data_array = _var.data_array[_var.time_array > 0]
+        _var_time_array = _var.time_array[_var.time_array > 0]
         if(_var.save_as == 'npz'):
             fpath = param_dir / f'{param_name}_{_var.file_start_time}.npz'
             np.savez(fpath,
-                time_array = _var.time_array,
-                data_array = _var.data_array)
+                time_array = _var_time_array,
+                data_array = _var_data_array)
         elif(_var.save_as == 'txt'):
             fpath = param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
-            np.savetxt(fpath, _var.time_array)
+            np.savetxt(fpath, _var_time_array)
             fpath = param_dir / f'{param_name}_data_{_var.file_start_time}.txt'
-            np.savetxt(fpath, _var.data_array)
+            np.savetxt(fpath, _var_data_array)
         return fpath
     
     def get_var(self, parameter_name : str):
         """ Get the buffered numpy arrays
             If you need the buffered variable back.
         :param parameter_name : str
             examples: myvar or myscript/myvar
@@ -922,70 +917,73 @@
             self.log_text(self.log_name,
                 f'Cannot make the hexbin for variable {parameter_name}.')
             return None
         
     def log_imshow(self, parameter_name : str, 
                    parameter_value,
                    image_format='jpeg', dpi=1200, cmap = 'jet',
-                   time_tag : bool = None,
+                   time_tag : bool = None, nan_borders = np.nan,
                    **kwargs):
         """log an image
             The image is logged using plt.imshow
             
             Parameters
             ----------
             :param parameter_name : str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             :param parameter_value : np.array
-                    An np array of size n x m, to be shown by imshow
+                    An np array of shape amongst the following:
+                    * (n, m) 
+                    * (n, m, 3)
+                    * (n, m, ch)
+                    * (1, n, m, ch)
+                    * (n, m, 3, ch)
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        parameter_value = np.squeeze(parameter_value)
+        parameter_value = parameter_value.squeeze()
         parameter_value_shape = parameter_value.shape
         n_dims = len(parameter_value_shape)
         
         FLAG_img_ready = False
+        use_multichannel_to_square = False
         if(n_dims == 2):
             FLAG_img_ready = True
         elif(n_dims == 3):
             if(parameter_value_shape[2] == 3):
                 FLAG_img_ready = True
+            else:
+                FLAG_img_ready = True
+                use_multichannel_to_square = True
         elif(n_dims == 4):
-            parameter_value = parameter_value.swapaxes(1,2)
-            new_shape = parameter_value.shape
-            parameter_value = \
-                parameter_value.reshape(new_shape[0] * new_shape[1],
-                                        new_shape[2] * new_shape[3])
-            FLAG_img_ready = True
-        elif(n_dims == 5):
-            if(parameter_value_shape[4] == 3):
-                parameter_value = parameter_value.swapaxes(1,2)
-                new_shape = parameter_value.shape
-                parameter_value = parameter_value.reshape(\
-                    new_shape[0] * new_shape[1],
-                    new_shape[2] * new_shape[3],
-                    new_shape[4])
+            if(parameter_value_shape[2] == 3):
+                FLAG_img_ready = True
+                use_multichannel_to_square = True
+            elif(parameter_value_shape[0] == 1):
                 FLAG_img_ready = True
+                use_multichannel_to_square = True
         
+        if(use_multichannel_to_square):
+            parameter_value = self. multichannel_to_square(
+                parameter_value, nan_borders = nan_borders)
         if(FLAG_img_ready):
+            plt.figure()
             plt.imshow(parameter_value, cmap = cmap, **kwargs)
             plt.colorbar()
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
             return fpath
         else:
-            plt.close()
             self.log_text(
                 self.log_name,
                 f'Cannot plot variable {parameter_name} with shape' + \
                 f'{parameter_value.shape}')
             return
 
     def multichannel_to_square(self, stack, nan_borders = np.nan):
@@ -993,27 +991,40 @@
             This is very useful when lots of images need to be tiled
             against each other.
         
             Parameters
             ----------
             :param stack : np.ndarray
                     It must have the shape of either
+                    n_r x n_c x n_ch
+                    n_r x n_c x  3  x n_ch
                     n_f x n_r x n_c x n_ch
-                    n_f x n_r x n_c x 3 x n_ch
+                    n_f x n_r x n_c x  3  x n_ch
                     
-                In both cases n_ch will be turned into square tile
-                Remember if you have N images to put into a square, you only
-                have n_f = 1 image with n_ch = N, you do not have N images
-                and the shape of the ndarray will be 1 x n_r x n_c x N
+                In both cases n_ch will be turned into a square tile
+                Remember if you have N images to put into a square, the input
+                shape should be 1 x n_r x n_c x N
+            :param nan_borders: literal or np.inf or np.nan
+                When plotting images with matplotlib.pyplot.imshow, there
+                needs to be a border between them. This is the value for the 
+                border elements.
                 
             output
             ---------
-                it produces an np.array of shape n_f x n_r x n_c or
-                n_f x n_r x n_c x 3 in case of RGB input.
-        """
+                Since we have N channels to be laid into a square, the side
+                length woul be ceil(N**0.5)
+                it produces an np.array of shape n_f x n_r * S x n_c * S or
+                n_f x n_r * S x n_c * S x 3 in case of RGB input.
+        """
+        if(len(stack.shape) == 4):
+            if(stack.shape[3] == 3):
+                stack = np.array([stack])
+        if(len(stack.shape) == 3):
+            stack = np.array([stack])
+        
         if((len(stack.shape) == 4) | (len(stack.shape) == 5)):
             if(len(stack.shape) == 4):
                 n_imgs, n_R, n_C, n_ch = stack.shape
             if(len(stack.shape) == 5):
                 n_imgs, n_R, n_C, is_rgb, n_ch = stack.shape
                 if(is_rgb != 3):
                     return None
```

### Comparing `lognflow-0.6.4/lognflow/logviewer.py` & `lognflow-0.6.5/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/lognflow/printprogress.py` & `lognflow-0.6.5/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/lognflow.egg-info/PKG-INFO` & `lognflow-0.6.5/lognflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.6.4
+Version: 0.6.5
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -141,15 +141,15 @@
 * time_in_file_name has been changed to time_tag, sorry there! but early stages.
 * time_tag is True in the constructor, but could always be set to False
 * All tests passed!
 
 0.6.0 (2023-03-22)
 ------------------
 * This is a stable release
-* All text files are handled by thw with statement
+* All text files are handled by the with statement
 * Renaming bug is fixed
 * all tests run properly.
 * lognflow has all that logviewer has. We will check if dir exists at every use
 
 0.6.1 (2023-03-22)
 ------------------
 * rename had a bug that is fixed
@@ -160,11 +160,17 @@
 * We support Python 3.7+ because of dataclasses
 * printprogress now can disable printing anything and return ETA at the __call__
 
 0.6.3 (2023-04-01)
 ------------------
 * lognflow class does all logviewer does. Maybe it is time to remove logviewer.
 
-0.6.4 (2023-04-10)
+0.6.4 (2023-04-06)
 ------------------
 * Better documentation and examples for readme
-* get_var is added to lognflow
+* get_var is added to lognflow to get buffered variables logged by log_var
+
+0.6.5 (2023-04-26)
+------------------
+* Fixed a bug in the docs to allow sphinx compile it.
+* log_var will log only the valid time stamps.
+* added end keyword argument to log_text
```

### Comparing `lognflow-0.6.4/lognflow.egg-info/SOURCES.txt` & `lognflow-0.6.5/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.6.4/setup.py` & `lognflow-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.6.4'
+__version__ = '0.6.5'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.6.4/tests/test_lognflow.py` & `lognflow-0.6.5/tests/test_lognflow.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -293,8 +293,8 @@
     test_log_animation()
     test_log_hist()
     test_log_scatter3()
     test_log_plt()
     test_log_hexbin()
     test_log_imshow()
     test_log_canvas()
-    test_log_confusion_matrix()
+    test_log_confusion_matrix()
```

### Comparing `lognflow-0.6.4/tests/test_logviewer.py` & `lognflow-0.6.5/tests/test_logviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     
     if(flist_A_AB):
         
         dataset_A = logged.get_stack_of_files(flist = flist_A_AB, return_data = True, return_flist = False)
         dataset_B = logged.get_stack_of_files(flist = flist_B_AB, return_data = True, return_flist = False)
         
         logger.log_canvas('data_samples', [dataset_A, dataset_B], dpi = 300)
-        _ = logger._loggers_dict['main_log'][2]
+        _ = logger._loggers_dict['main_log'].log_size
         logger('Size of the log file in bytes is: ' \
                + f'{_}')
 
 def test_replace_time_with_index():
     logger = lognflow(temp_dir)
     logger('Well this is a test for logviewer')
```

### Comparing `lognflow-0.6.4/tests/test_printprogress.py` & `lognflow-0.6.5/tests/test_printprogress.py`

 * *Files identical despite different names*

