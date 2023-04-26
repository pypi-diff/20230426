# Comparing `tmp/chainbench-0.1.0.tar.gz` & `tmp/chainbench-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.1.0.tar", max compression
+gzip compressed data, was "chainbench-0.1.1.tar", max compression
```

## Comparing `chainbench-0.1.0.tar` & `chainbench-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-04-25 13:55:13.341452 chainbench-0.1.0/LICENSE
--rw-r--r--   0        0        0     5589 2023-04-25 13:55:13.341452 chainbench-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/__main__.py
--rw-r--r--   0        0        0     5241 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3417 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/profile/avalanche.py
--rw-r--r--   0        0        0     2512 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/profile/bsc.py
--rw-r--r--   0        0        0     2794 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/profile/ethereum.py
--rw-r--r--   0        0        0     1829 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/profile/oasis.py
--rw-r--r--   0        0        0     2730 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/profile/polygon.py
--rw-r--r--   0        0        0      168 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2596 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3477 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/user/base.py
--rw-r--r--   0        0        0     1225 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/util/__init__.py
--rw-r--r--   0        0        0     2499 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/util/cli.py
--rw-r--r--   0        0        0     2532 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/util/event.py
--rw-r--r--   0        0        0     3463 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/util/notify.py
--rw-r--r--   0        0        0      320 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-04-25 13:55:13.341452 chainbench-0.1.0/chainbench/util/timer.py
--rw-r--r--   0        0        0      688 2023-04-25 13:55:13.345451 chainbench-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 chainbench-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 15:14:09.028811 chainbench-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6162 2023-04-25 15:14:09.028811 chainbench-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/__main__.py
+-rw-r--r--   0        0        0     5241 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3417 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/avalanche.py
+-rw-r--r--   0        0        0     2512 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/bsc.py
+-rw-r--r--   0        0        0     2794 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/ethereum.py
+-rw-r--r--   0        0        0     1829 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/oasis.py
+-rw-r--r--   0        0        0     2730 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/profile/polygon.py
+-rw-r--r--   0        0        0      168 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     4705 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     2596 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3477 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/user/base.py
+-rw-r--r--   0        0        0     1225 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     2499 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2532 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/event.py
+-rw-r--r--   0        0        0     3463 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/notify.py
+-rw-r--r--   0        0        0      320 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-04-25 15:14:09.028811 chainbench-0.1.1/chainbench/util/timer.py
+-rw-r--r--   0        0        0      746 2023-04-25 15:14:09.028811 chainbench-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 chainbench-0.1.1/PKG-INFO
```

### Comparing `chainbench-0.1.0/LICENSE` & `chainbench-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/README.md` & `chainbench-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: chainbench
+Version: 0.1.1
+Summary: 
+Author: Egor Molodik
+Author-email: egor.molodik@chainstack.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: locust (>=2.15.0,<3.0.0)
+Description-Content-Type: text/markdown
+
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
  <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
 </p>
 
 <p align="center">
@@ -18,14 +33,18 @@
   <a target="_blank" href="https://chainstack.com/blog/">Chainstack blog</a> •
   <a target="_blank" href="https://docs.chainstack.com/quickstart/">Chainstack docs</a> •
   <a target="_blank" href="https://docs.chainstack.com/quickstart/">Blockchain API reference</a> • <br> 
   • <a target="_blank" href="https://console.chainstack.com/user/account/create">Start for free</a> •
 </p>
 
 # Chainbench
+![checks status](https://github.com/chainstacklabs/chainbench/actions/workflows/checks.yml/badge.svg) 
+![build status](https://github.com/chainstacklabs/chainbench/actions/workflows/python-publish.yml/badge.svg)
+![version](https://img.shields.io/pypi/v/chainbench)
+![license](https://img.shields.io/github/license/chainstacklabs/chainbench)
 
 This project allows you to benchmark your blockchain infrastructure. It uses [Locust](https://docs.locust.io/en/stable/index.html) under the hood.
 
 ## Project Details
 
 Chainbench lets you to easily define profiles for any EVM-compatible chain. 
 You can use not only hard-coded values but also real chain data to generate dynamic call parameters.
@@ -43,42 +62,51 @@
 - Python 3.10+
 - Poetry 1.2+ (installation instructions [here](https://python-poetry.org/docs/#installation))
 
 ## Installation
 
 ### Using pip
 
-> ⚠️ Installation using pip is not supported yet.
+```shell
+pip install chainbench
+```
+
+After installation, you can run the tool using the following command:
+```shell
+chainbench start --help
+```
 
 ### Using Poetry
 
 Clone the repository:
 ```shell
 git clone git@github.com:chainstacklabs/chainbench.git
 ```
 
 Install dependencies:
 ```shell
 cd chainbench && poetry install --without dev
 ```
 
-You might need to run the following command before running the tool:
+When installing using Poetry, you can run the tool using the following command:
 ```shell
-poetry shell
+poetry run chainbench start --help
 ```
 
 ## Example Usage
+All the examples below assume that you have installed the tool using `pip`. If you installed it using `poetry`, replace `chainbench` with `poetry run chainbench`.
+
 To learn about the parameters and flags, run the following command:
 ```shell
-python3 -m chainbench start --help
+chainbench start --help
 ```
 
 Basic usage is:
 ```shell
-python3 -m chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 This will run a load test for BSC with 2 workers, 50 users and 12 hours test time in headless mode.
 After the test is finished, the tool will automatically quit.
 
 ### Parameters and Flags
 - `--profile`: This flag specifies the profile to use for the benchmark. Available profiles are `ethereum`, `bsc`, `polygon`, `oasis`, and `avalanche`.
@@ -95,28 +123,28 @@
 
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
 Target is not required as you can specify it in the UI along with the number of users, spawn rate and test time.
 
 ```shell
-python3 -m chainbench start --profile bsc --workers 1
+chainbench start --profile bsc --workers 1
 ```
 
 ### Headless Mode
 
 If you want to run a load test for BSC in headless mode, run the following command:
 
 ```shell
-python3 -m chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
+chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
 ```
 
 It will run a load test for BSC with 4 workers, 100 users and 1 hour test time.
 
 In practice, you will probably want to run the benchmark on a remote server. Here's the example utilizing `nohup`:
 
 ```shell
-nohup python3 -m chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
+nohup chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
 ```
 
 ## License
-This project is licensed under the [Apache 2.0 License](LICENSE).
+This project is licensed under the [Apache 2.0 License](LICENSE).
```

### Comparing `chainbench-0.1.0/chainbench/main.py` & `chainbench-0.1.1/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/profile/avalanche.py` & `chainbench-0.1.1/chainbench/profile/avalanche.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/profile/bsc.py` & `chainbench-0.1.1/chainbench/profile/bsc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/profile/ethereum.py` & `chainbench-0.1.1/chainbench/profile/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/profile/oasis.py` & `chainbench-0.1.1/chainbench/profile/oasis.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/profile/polygon.py` & `chainbench-0.1.1/chainbench/profile/polygon.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/test_data/base.py` & `chainbench-0.1.1/chainbench/test_data/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/test_data/evm.py` & `chainbench-0.1.1/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/user/base.py` & `chainbench-0.1.1/chainbench/user/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/user/evm.py` & `chainbench-0.1.1/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/util/cli.py` & `chainbench-0.1.1/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/util/event.py` & `chainbench-0.1.1/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/chainbench/util/notify.py` & `chainbench-0.1.1/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.1.0/PKG-INFO` & `chainbench-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: chainbench
-Version: 0.1.0
-Summary: 
-Author: Egor Molodik
-Author-email: egor.molodik@chainstack.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: locust (>=2.15.0,<3.0.0)
-Description-Content-Type: text/markdown
-
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
  <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
 </p>
 
 <p align="center">
@@ -33,14 +18,18 @@
   <a target="_blank" href="https://chainstack.com/blog/">Chainstack blog</a> •
   <a target="_blank" href="https://docs.chainstack.com/quickstart/">Chainstack docs</a> •
   <a target="_blank" href="https://docs.chainstack.com/quickstart/">Blockchain API reference</a> • <br> 
   • <a target="_blank" href="https://console.chainstack.com/user/account/create">Start for free</a> •
 </p>
 
 # Chainbench
+![checks status](https://github.com/chainstacklabs/chainbench/actions/workflows/checks.yml/badge.svg) 
+![build status](https://github.com/chainstacklabs/chainbench/actions/workflows/python-publish.yml/badge.svg)
+![version](https://img.shields.io/pypi/v/chainbench)
+![license](https://img.shields.io/github/license/chainstacklabs/chainbench)
 
 This project allows you to benchmark your blockchain infrastructure. It uses [Locust](https://docs.locust.io/en/stable/index.html) under the hood.
 
 ## Project Details
 
 Chainbench lets you to easily define profiles for any EVM-compatible chain. 
 You can use not only hard-coded values but also real chain data to generate dynamic call parameters.
@@ -58,42 +47,51 @@
 - Python 3.10+
 - Poetry 1.2+ (installation instructions [here](https://python-poetry.org/docs/#installation))
 
 ## Installation
 
 ### Using pip
 
-> ⚠️ Installation using pip is not supported yet.
+```shell
+pip install chainbench
+```
+
+After installation, you can run the tool using the following command:
+```shell
+chainbench start --help
+```
 
 ### Using Poetry
 
 Clone the repository:
 ```shell
 git clone git@github.com:chainstacklabs/chainbench.git
 ```
 
 Install dependencies:
 ```shell
 cd chainbench && poetry install --without dev
 ```
 
-You might need to run the following command before running the tool:
+When installing using Poetry, you can run the tool using the following command:
 ```shell
-poetry shell
+poetry run chainbench start --help
 ```
 
 ## Example Usage
+All the examples below assume that you have installed the tool using `pip`. If you installed it using `poetry`, replace `chainbench` with `poetry run chainbench`.
+
 To learn about the parameters and flags, run the following command:
 ```shell
-python3 -m chainbench start --help
+chainbench start --help
 ```
 
 Basic usage is:
 ```shell
-python3 -m chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
+chainbench start --profile bsc --users 50 --workers 2 --test-time 12h --target https://node-url --headless --autoquit
 ```
 
 This will run a load test for BSC with 2 workers, 50 users and 12 hours test time in headless mode.
 After the test is finished, the tool will automatically quit.
 
 ### Parameters and Flags
 - `--profile`: This flag specifies the profile to use for the benchmark. Available profiles are `ethereum`, `bsc`, `polygon`, `oasis`, and `avalanche`.
@@ -110,28 +108,28 @@
 
 ### Web UI Mode
 
 Run the following command to run a load test for BSC in UI mode. It will start a web server on port 8089. 
 Target is not required as you can specify it in the UI along with the number of users, spawn rate and test time.
 
 ```shell
-python3 -m chainbench start --profile bsc --workers 1
+chainbench start --profile bsc --workers 1
 ```
 
 ### Headless Mode
 
 If you want to run a load test for BSC in headless mode, run the following command:
 
 ```shell
-python3 -m chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
+chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit
 ```
 
 It will run a load test for BSC with 4 workers, 100 users and 1 hour test time.
 
 In practice, you will probably want to run the benchmark on a remote server. Here's the example utilizing `nohup`:
 
 ```shell
-nohup python3 -m chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
+nohup chainbench start --profile bsc --workers 4 --users 100 --test-time 1h --target https://node-url --headless --autoquit &
 ```
 
 ## License
-This project is licensed under the [Apache 2.0 License](LICENSE).
+This project is licensed under the [Apache 2.0 License](LICENSE).
```

