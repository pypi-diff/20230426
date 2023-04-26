# Comparing `tmp/pts_keysight_daq-0.0.8.tar.gz` & `tmp/pts_keysight_daq-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_keysight_daq-0.0.8.tar", last modified: Thu Jan 26 15:13:00 2023, max compression
+gzip compressed data, was "pts_keysight_daq-0.0.9.tar", last modified: Thu Feb 23 15:41:28 2023, max compression
```

## Comparing `pts_keysight_daq-0.0.8.tar` & `pts_keysight_daq-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-01-26 15:12:50.000000 pts_keysight_daq-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq/
--rw-rw-rw-   0 root         (0) root         (0)    20283 2023-01-26 15:12:50.000000 pts_keysight_daq-0.0.8/pts_keysight_daq/keysight_daq.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-01-26 15:12:50.000000 pts_keysight_daq-0.0.8/pts_keysight_daq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      291 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-01-26 15:12:50.000000 pts_keysight_daq-0.0.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-01-26 15:12:50.000000 pts_keysight_daq-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:13:00.000000 pts_keysight_daq-0.0.8/setup.cfg
+drwxr-xr-x   0 shuparnadeb   (501) staff       (20)        0 2023-02-23 15:41:28.916234 pts_keysight_daq-0.0.9/
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)     1069 2022-12-06 10:42:12.000000 pts_keysight_daq-0.0.9/LICENSE.txt
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)     2442 2023-02-23 15:41:28.916103 pts_keysight_daq-0.0.9/PKG-INFO
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)     1937 2022-12-06 10:42:12.000000 pts_keysight_daq-0.0.9/README.md
+drwxr-xr-x   0 shuparnadeb   (501) staff       (20)        0 2023-02-23 15:41:28.914944 pts_keysight_daq-0.0.9/pts_keysight_daq/
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)       60 2022-12-06 10:42:12.000000 pts_keysight_daq-0.0.9/pts_keysight_daq/__init__.py
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)    20222 2023-02-23 15:39:58.000000 pts_keysight_daq-0.0.9/pts_keysight_daq/keysight_daq.py
+drwxr-xr-x   0 shuparnadeb   (501) staff       (20)        0 2023-02-23 15:41:28.915940 pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)     2442 2023-02-23 15:41:28.000000 pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/PKG-INFO
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)      291 2023-02-23 15:41:28.000000 pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/SOURCES.txt
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)        1 2023-02-23 15:41:28.000000 pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/dependency_links.txt
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)       72 2023-02-23 15:41:28.000000 pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/requires.txt
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)       17 2023-02-23 15:41:28.000000 pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/top_level.txt
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)       38 2023-02-23 15:41:28.916279 pts_keysight_daq-0.0.9/setup.cfg
+-rw-r--r--   0 shuparnadeb   (501) staff       (20)      925 2023-02-23 15:39:58.000000 pts_keysight_daq-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pts_keysight_daq-0.0.8/PKG-INFO` & `pts_keysight_daq-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pts_keysight_daq
-Version: 0.0.8
+Version: 0.0.9
 Summary: Keysight DAQ 34980A with 34925A-1W Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/keysight34980a-interface
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Keysight34980A Interface
@@ -68,9 +67,7 @@
 E.g. - .virtualenvs/demo_repo_venv/bin/python3
 ```
 After setting up the venv for the repo please install all the 
 requirements and allow some time for the IDE to do indexing. If your repository has a requirements.txt: 
 ```
 pip3 install -r requirements.txt
 ```
-
-
```

### Comparing `pts_keysight_daq-0.0.8/setup.py` & `pts_keysight_daq-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_keysight_daq",
-    version="0.0.8",
+    version="0.0.9",
     author="Pass testing Solutions GmbH",
     description="Keysight DAQ 34980A with 34925A-1W Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/keysight34980a-interface",
     license="MIT",
```

### Comparing `pts_keysight_daq-0.0.8/pts_keysight_daq/keysight_daq.py` & `pts_keysight_daq-0.0.9/pts_keysight_daq/keysight_daq.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,33 +16,31 @@
     """
     Base class for the Keysight 34980A DAQ
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%H:%M:%S',
                         level=logging.INFO)
 
-    def __init__(self, connection_string=None):
+    def __init__(self, connection_string):
         # Supported Devices
         self.cards = None
         self.card_types = None
-        if not connection_string:
-            self.connection_string = os.getenv("DAQ_CONNECTION_STRING", default='TCPIP0::192.168.1.183::INSTR')
-        else:
-            self.connection_string = connection_string
+        self.connection_string = connection_string
         self.supported_list = ["34925A-1W", "34951A"]
         self.resource_manager = None
         self.daq = None
         # Cards Can be discovers with : SYSTem:CTYPe? <slot>
         # Should return AGILENT TECHNOLOGIES,<Modellnummer>,<Seriennummer>,<Firmware-Version>
 
     def open_connection(self):
         """
         Opens a TCP/IP connection to the Keysight DAQ 34980A
         """
         self.resource_manager = pyvisa.ResourceManager()
+        self.connection_string = os.getenv("DAQ_CONNECTION_STRING", default='TCPIP0::192.168.2.183::INSTR')
         try:
             logging.info(f": Opening DAQ Resource at {self.connection_string}")
             self.daq = self.resource_manager.open_resource(self.connection_string)
             self.daq.read_termination = '\n'
             self.daq.write_termination = '\n'
         except Exception as e:
             raise Exception(f": ERROR {e}: Could not open Resource\n")
```

### Comparing `pts_keysight_daq-0.0.8/pts_keysight_daq.egg-info/PKG-INFO` & `pts_keysight_daq-0.0.9/pts_keysight_daq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pts-keysight-daq
-Version: 0.0.8
+Version: 0.0.9
 Summary: Keysight DAQ 34980A with 34925A-1W Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/keysight34980a-interface
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Keysight34980A Interface
@@ -68,9 +67,7 @@
 E.g. - .virtualenvs/demo_repo_venv/bin/python3
 ```
 After setting up the venv for the repo please install all the 
 requirements and allow some time for the IDE to do indexing. If your repository has a requirements.txt: 
 ```
 pip3 install -r requirements.txt
 ```
-
-
```

### Comparing `pts_keysight_daq-0.0.8/LICENSE.txt` & `pts_keysight_daq-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_keysight_daq-0.0.8/README.md` & `pts_keysight_daq-0.0.9/README.md`

 * *Files identical despite different names*

