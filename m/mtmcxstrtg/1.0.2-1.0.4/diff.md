# Comparing `tmp/mtmcxstrtg-1.0.2.tar.gz` & `tmp/mtmcxstrtg-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmcxstrtg-1.0.2.tar", last modified: Tue Apr 25 14:55:40 2023, max compression
+gzip compressed data, was "mtmcxstrtg-1.0.4.tar", last modified: Tue Apr 25 15:59:49 2023, max compression
```

## Comparing `mtmcxstrtg-1.0.2.tar` & `mtmcxstrtg-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:40.623001 mtmcxstrtg-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-25 14:55:40.623001 mtmcxstrtg-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 14:55:40.623001 mtmcxstrtg-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:40.619001 mtmcxstrtg-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:40.619001 mtmcxstrtg-1.0.2/src/mtmcxstrtg/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:40.623001 mtmcxstrtg-1.0.2/src/mtmcxstrtg/strategy/
--rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-04-25 14:55:32.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:55:40.623001 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-25 14:55:40.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-25 14:55:40.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:55:40.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:55:40.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-25 14:55:40.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 14:55:40.000000 mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.395214 mtmcxstrtg-1.0.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.391214 mtmcxstrtg-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.395214 mtmcxstrtg-1.0.4/src/mtmcxstrtg/
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.395214 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/top_level.txt
```

### Comparing `mtmcxstrtg-1.0.2/PKG-INFO` & `mtmcxstrtg-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmcxstrtg
-Version: 1.0.2
+Version: 1.0.4
 Summary: imutum_cryptocurrency_strategy
 Home-page: https://github.com/imutum/imutum_cryptocurrency_strategy
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmcxstrtg-1.0.2/setup.py` & `mtmcxstrtg-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_cryptocurrency_strategy"
 abbreviation_name = "mtmcxstrtg"  # 缩写
 description = ""
-version = "1.0.2"
+version = "1.0.4"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
@@ -56,14 +56,15 @@
         "numpy",
         "requests",
         "pandas",
         "ccxt",
         "mtmtool",
     ],
     python_requires='>=3.6',
+    scripts=['scripts/run.py'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.6",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
```

### Comparing `mtmcxstrtg-1.0.2/src/mtmcxstrtg/account.py` & `mtmcxstrtg-1.0.4/src/mtmcxstrtg/account.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.2/src/mtmcxstrtg/config.py` & `mtmcxstrtg-1.0.4/src/mtmcxstrtg/config.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.2/src/mtmcxstrtg/flow.py` & `mtmcxstrtg-1.0.4/src/mtmcxstrtg/flow.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.2/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py` & `mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,25 +42,26 @@
     # 准备工作, 从yaml中的流配置中创建需要的部分参数
     clients = {account_info["userId"]: Account(account_info) for account_info in accounts_info}
     envs["ccxt"] = clients
     for flow_item in config_dict["strategy"]["flow"]:
         envs[flow_item["var"]] = action(action_info=flow_item["action"], envs=envs)
 
     # 以下是策略逻辑
+    next_quantity = 0
+    next_amount = envs["base_coins"]
     for trigger_item in strategy_info["trigger"]:
         if envs[trigger_item["condition"]]:
             # 交易
             action(action_info=trigger_item["action"], envs=envs)
 
             # 记录本次交易信息
             messages = strategy_info["sendtemplate"].copy()
             messages["side"] = "↑buy↑" if trigger_item["action"]["params"]["side"].lower() == "buy" else "↓sell↓"
             messages["coin"] = envs["amount"]
             messages["price"] = envs["price_current"]
-            next_amount = envs["base_coins"]
             next_quantity = float(envs["amount"])
             if trigger_item["status"] == "close" and last_price:
                 expect_profit = get_profit(envs["price_current"], last_price, 0.001, trigger_item["side"] == "long")
                 expect_earn_usd = get_earn(expect_profit, float(envs["amount"]), last_price)
                 messages["profit"] = float(expect_profit)
                 messages["earnValue"] = float(expect_earn_usd)
                 next_amount = envs["base_coins"] + expect_earn_usd
```

### Comparing `mtmcxstrtg-1.0.2/src/mtmcxstrtg/util.py` & `mtmcxstrtg-1.0.4/src/mtmcxstrtg/util.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.2/src/mtmcxstrtg.egg-info/PKG-INFO` & `mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmcxstrtg
-Version: 1.0.2
+Version: 1.0.4
 Summary: imutum_cryptocurrency_strategy
 Home-page: https://github.com/imutum/imutum_cryptocurrency_strategy
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

