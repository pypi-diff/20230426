# Comparing `tmp/pyfed-0.0.2.tar.gz` & `tmp/pyfed-0.0.3.tar.gz`

## Comparing `pyfed-0.0.2.tar` & `pyfed-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed-0.0.2/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed-0.0.2/src/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed-0.0.2/src/ml_socket.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed-0.0.2/src/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed-0.0.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed-0.0.2/LICENSE
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 pyfed-0.0.2/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyfed-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyfed-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed-0.0.3/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/ml_socket.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed-0.0.3/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfed-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 pyfed-0.0.3/PKG-INFO
```

### Comparing `pyfed-0.0.2/.DS_Store` & `pyfed-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.2/src/ml_socket.py` & `pyfed-0.0.3/src/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.2/src/pyfed.py` & `pyfed-0.0.3/src/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.2/.gitignore` & `pyfed-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.2/LICENSE` & `pyfed-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.2/README.md` & `pyfed-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 PyFed implements FL using sockets, processes, and threads. Simply put, each client will run its particular process and tries to establish a socket connection with the server, which also has its specific process. 
 Once initiated, each connection will be handled by one thread of the server's process. Each thread will communicate with its respective client to receive the trained weights per round. 
 Once they receive the result of one round, threads will return the weights to the server's process, which will arrive at a new model using the mentioned weights. The server will send the new model to the clients using newly initiated threads.
  
 PyFed is mainly based on two classes:
  
--> FL_Server: which represents the server to which clients communicate in a federated learning problem. The __train()__ function of this class handles socket connections and the FL policy. </br>
--> FL_Client: which represents each client in a federated learning network. An object of this class handles training procedure any global model on any local data.
+- __FL_Server__: which represents the server to which clients communicate in a federated learning problem. The __train()__ function of this class handles socket connections and the FL policy. </br>
+- __FL_Client__: which represents each client in a federated learning network. An object of this class handles training procedure any global model on any local data.
 
 Currently, PyFed is limited to FedAvg as its only federated learning policy; however, we will introduce a broader range of configurations for FL experiments in the coming versions.
 
 # Features
 PyFed contains two critical classes: FL_Server and FL_Client, which are responsible for server and client actions in a federated learning problem, respectively. </br>
 * __FL_Server.train()__ establishes a socket connections with clients and handles weight averaging. In addition, at the end of all rounds a tensorboard session will be started to reveal the efficancy of each client.
 * __FL_Server.test()__ will test the final model on the given test data.
```

### Comparing `pyfed-0.0.2/pyproject.toml` & `pyfed-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Amirreza Sokhankhosh", email="amirreza.sokhankhosh@gmail.com" },
 ]
 description = "PyFed is an open-source framework for federated learning algorithms." 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/amirrezasokhankhosh/PyFL"
-"Bug Tracker" = "https://github.com/amirrezasokhankhosh/PyFL/issues"
+"Homepage" = "https://github.com/amirrezasokhankhosh/PyFed"
+"Bug Tracker" = "https://github.com/amirrezasokhankhosh/PyFed/issues"
```

### Comparing `pyfed-0.0.2/PKG-INFO` & `pyfed-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyFed
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyFed is an open-source framework for federated learning algorithms.
-Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFL
-Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFL/issues
+Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
+Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -19,16 +19,16 @@
 
 PyFed implements FL using sockets, processes, and threads. Simply put, each client will run its particular process and tries to establish a socket connection with the server, which also has its specific process. 
 Once initiated, each connection will be handled by one thread of the server's process. Each thread will communicate with its respective client to receive the trained weights per round. 
 Once they receive the result of one round, threads will return the weights to the server's process, which will arrive at a new model using the mentioned weights. The server will send the new model to the clients using newly initiated threads.
  
 PyFed is mainly based on two classes:
  
--> FL_Server: which represents the server to which clients communicate in a federated learning problem. The __train()__ function of this class handles socket connections and the FL policy. </br>
--> FL_Client: which represents each client in a federated learning network. An object of this class handles training procedure any global model on any local data.
+- __FL_Server__: which represents the server to which clients communicate in a federated learning problem. The __train()__ function of this class handles socket connections and the FL policy. </br>
+- __FL_Client__: which represents each client in a federated learning network. An object of this class handles training procedure any global model on any local data.
 
 Currently, PyFed is limited to FedAvg as its only federated learning policy; however, we will introduce a broader range of configurations for FL experiments in the coming versions.
 
 # Features
 PyFed contains two critical classes: FL_Server and FL_Client, which are responsible for server and client actions in a federated learning problem, respectively. </br>
 * __FL_Server.train()__ establishes a socket connections with clients and handles weight averaging. In addition, at the end of all rounds a tensorboard session will be started to reveal the efficancy of each client.
 * __FL_Server.test()__ will test the final model on the given test data.
```

