# Comparing `tmp/hyperfetch-1.0.4.tar.gz` & `tmp/hyperfetch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.0.4.tar", last modified: Tue Apr 25 16:28:28 2023, max compression
+gzip compressed data, was "hyperfetch-1.0.5.tar", last modified: Tue Apr 25 19:22:16 2023, max compression
```

## Comparing `hyperfetch-1.0.4.tar` & `hyperfetch-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 16:28:28.973744 hyperfetch-1.0.4/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.4/LICENSE
--rw-rw-rw-   0        0        0    10321 2023-04-25 16:28:28.973744 hyperfetch-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7897 2023-04-25 07:24:16.000000 hyperfetch-1.0.4/README.md
--rw-rw-rw-   0        0        0     4785 2023-04-25 16:27:11.000000 hyperfetch-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 16:28:28.973744 hyperfetch-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 16:28:28.862697 hyperfetch-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 16:28:28.934870 hyperfetch-1.0.4/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-04-16 16:06:24.000000 hyperfetch-1.0.4/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-04-15 07:49:41.000000 hyperfetch-1.0.4/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-04-16 21:41:06.000000 hyperfetch-1.0.4/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     2118 2023-04-13 19:35:11.000000 hyperfetch-1.0.4/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    33318 2023-04-25 07:38:41.000000 hyperfetch-1.0.4/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4899 2023-04-24 13:08:27.000000 hyperfetch-1.0.4/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0      825 2023-04-16 16:50:23.000000 hyperfetch-1.0.4/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-04-25 16:28:28.972787 hyperfetch-1.0.4/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0    10321 2023-04-25 16:28:28.000000 hyperfetch-1.0.4/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-25 16:28:28.000000 hyperfetch-1.0.4/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 16:28:28.000000 hyperfetch-1.0.4/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-25 16:28:28.000000 hyperfetch-1.0.4/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     2238 2023-04-25 16:28:28.000000 hyperfetch-1.0.4/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 16:28:28.000000 hyperfetch-1.0.4/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.748423 hyperfetch-1.0.5/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    10367 2023-04-25 19:22:16.747423 hyperfetch-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.5/README.md
+-rw-rw-rw-   0        0        0     4794 2023-04-25 19:14:42.000000 hyperfetch-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 19:22:16.748423 hyperfetch-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.671912 hyperfetch-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.704422 hyperfetch-1.0.5/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-04-16 16:06:24.000000 hyperfetch-1.0.5/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-15 07:49:41.000000 hyperfetch-1.0.5/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-04-16 21:41:06.000000 hyperfetch-1.0.5/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     2118 2023-04-13 19:35:11.000000 hyperfetch-1.0.5/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    33572 2023-04-25 19:17:47.000000 hyperfetch-1.0.5/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4926 2023-04-25 19:17:51.000000 hyperfetch-1.0.5/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0      825 2023-04-16 16:50:23.000000 hyperfetch-1.0.5/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.745423 hyperfetch-1.0.5/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0    10367 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     2238 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.0.4/LICENSE` & `hyperfetch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.4/PKG-INFO` & `hyperfetch-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.4
+Version: 1.0.5
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
@@ -32,15 +32,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: FastAPI
-Requires-Python: >=3.9
+Requires-Python: <3.11.0,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HyperFetch
 #### HyperFetch is a tool consisting of:
 - [Website](https://github.com/karolisw/hyperFetch) for fetching hyperparameters that are tuned by others
 - Pip-module for tuning hyperparameters 
@@ -66,14 +66,19 @@
    * 1.1 [Examples](#example-1--tuning--posting-using-hyperfetch)
 * 2.0  [Using the Website](#getting-the-website-up-and-running)
    * 2.1 [Installation backend](#installation-backend)
    * 2.2 [Setup backend](#start-up-backend)
    * 2.3 [Setup frontend](#start-up-frontend)
    * 2.4 [Installation frontend](#installation-frontend)
 
+## Prerequisites
+Box2D-py
+swig
+
+
 ## Links
 Repository: [HyperFetch Github](https://github.com/karolisw/hyperFetch)\
 Documentation: [HyperFetch Website](https://github.com/karolisw/hyperFetch/tree/frontend)
 
 ## Using the pip module
 To use the pip model please do the following:
 1. Create a virtual environment in your favorite IDE. The virtual environment must be of the type virtualenv.
```

### Comparing `hyperfetch-1.0.4/README.md` & `hyperfetch-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,19 @@
    * 1.1 [Examples](#example-1--tuning--posting-using-hyperfetch)
 * 2.0  [Using the Website](#getting-the-website-up-and-running)
    * 2.1 [Installation backend](#installation-backend)
    * 2.2 [Setup backend](#start-up-backend)
    * 2.3 [Setup frontend](#start-up-frontend)
    * 2.4 [Installation frontend](#installation-frontend)
 
+## Prerequisites
+Box2D-py
+swig
+
+
 ## Links
 Repository: [HyperFetch Github](https://github.com/karolisw/hyperFetch)\
 Documentation: [HyperFetch Website](https://github.com/karolisw/hyperFetch/tree/frontend)
 
 ## Using the pip module
 To use the pip model please do the following:
 1. Create a virtual environment in your favorite IDE. The virtual environment must be of the type virtualenv.
```

### Comparing `hyperfetch-1.0.4/pyproject.toml` & `hyperfetch-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
-requires = ["setuptools>=64.0.3", "wheel"]
+requires = ["setuptools==64.0.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["hyperfetch"]
 
 [project]
 name = "hyperfetch"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Karoline Sund Wahl", email="karolines.wahl@gmail.com" },
 ]
 description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.9, <3.11.0"
 license = {file = "LICENSE"}
 keywords = ["reinforcement learning", "hyperparameters", "replication"]
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
```

### Comparing `hyperfetch-1.0.4/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.0.5/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.4/src/hyperfetch/auth_connection.py` & `hyperfetch-1.0.5/src/hyperfetch/auth_connection.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.4/src/hyperfetch/callbacks.py` & `hyperfetch-1.0.5/src/hyperfetch/callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.4/src/hyperfetch/manager.py` & `hyperfetch-1.0.5/src/hyperfetch/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         del model
 
         if is_pruned:
             raise optuna.exceptions.TrialPruned()
 
         return reward
 
-    def run(self) -> FrozenTrial:
+    def run(self) -> FrozenTrial | None:
 
         def check_threshold(study: optuna.study, trial):
             try:
                 if study.best_value > self.reward_threshold:
                     raise ThresholdExceeded()
             # ValueError in the start because there is no study.best value before any trials are run
             except ValueError:
@@ -160,41 +160,44 @@
                 study.optimize(self.objective, n_jobs=self.n_jobs, n_trials=self.n_trials,
                                callbacks=[check_threshold])
         except ThresholdExceeded:
             print('Threshold exceeded: {} > {}'.format(study.best_value, self.reward_threshold))
 
         print("Number of finished trials: ", len(study.trials))
 
-        trial = study.best_trial
-        print("Best trial: ", trial)
-
-        print("Value: ", trial.value)
-
-        print("Params: ")
-        for key, value in trial.params.items():
-            print("    {}: {}".format(key, value))
-
-        report_name = (
-            f"report_{self.env}_{self.n_trials}-trials-{self.n_timesteps}"
-            f"-{self.sampler}-{self.pruner}_{int(time())}"
-        )
-        # This is where the report will be written to
-        log_path = os.path.join(self.log_folder, self.alg, report_name)
-        print("Writing report to %s", log_path)
-        self.logger.info("Writing report to %s", log_path)
-
-        # Write report
-        os.makedirs(os.path.dirname(log_path), exist_ok=True)
-        study.trials_dataframe().to_csv(f"{log_path}.csv")
-
-        # Save the end time of the run
-        self.end_time = datetime.now()
-
-        # Return the best trial
-        return trial
+        try:
+            trial = study.best_trial
+            print("Best trial: ", trial)
+            print("Value: ", trial.value)
+            print("Params: ")
+            for key, value in trial.params.items():
+                print("    {}: {}".format(key, value))
+
+            # Write report
+            report_name = (
+                f"report_{self.env}_{self.n_trials}-trials-{self.n_timesteps}"
+                f"-{self.sampler}-{self.pruner}_{int(time())}"
+            )
+            # This is where the report will be written to
+            log_path = os.path.join(self.log_folder, self.alg, report_name)
+            print("Writing report to %s", log_path)
+            self.logger.info("Writing report to %s", log_path)
+
+            # Write report
+            os.makedirs(os.path.dirname(log_path), exist_ok=True)
+            study.trials_dataframe().to_csv(f"{log_path}.csv")
+
+            # Save the end time of the run
+            self.end_time = datetime.now()
+            # Return the best trial
+            return trial
+
+        except ValueError:
+            print("Study was completed, but all trials were pruned. ")
+            return None
 
     def _create_logger(self, logger_name) -> None:
         """
         :param logger_name: name of the logger
         :return: None, but sets the global logger object
         """
```

### Comparing `hyperfetch-1.0.4/src/hyperfetch/tuning.py` & `hyperfetch-1.0.5/src/hyperfetch/tuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     # Best performing trial is returned as FrozenTrial
     best_trial = manager.run()
 
     tracker.stop()
 
     # Post trial along with the tracking data unless user's config file states not to
-    if manager.post_run:
+    if manager.post_run and best_trial is not None:
         asyncio.run(manager.save_trial(
             trial=best_trial,
             client=MONGODB_URL,
             db=MONGO_DB,
             collection=MONGO_COLLECTION
         ))
```

### Comparing `hyperfetch-1.0.4/src/hyperfetch/util.py` & `hyperfetch-1.0.5/src/hyperfetch/util.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.4/src/hyperfetch.egg-info/PKG-INFO` & `hyperfetch-1.0.5/src/hyperfetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.4
+Version: 1.0.5
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
@@ -32,15 +32,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: FastAPI
-Requires-Python: >=3.9
+Requires-Python: <3.11.0,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HyperFetch
 #### HyperFetch is a tool consisting of:
 - [Website](https://github.com/karolisw/hyperFetch) for fetching hyperparameters that are tuned by others
 - Pip-module for tuning hyperparameters 
@@ -66,14 +66,19 @@
    * 1.1 [Examples](#example-1--tuning--posting-using-hyperfetch)
 * 2.0  [Using the Website](#getting-the-website-up-and-running)
    * 2.1 [Installation backend](#installation-backend)
    * 2.2 [Setup backend](#start-up-backend)
    * 2.3 [Setup frontend](#start-up-frontend)
    * 2.4 [Installation frontend](#installation-frontend)
 
+## Prerequisites
+Box2D-py
+swig
+
+
 ## Links
 Repository: [HyperFetch Github](https://github.com/karolisw/hyperFetch)\
 Documentation: [HyperFetch Website](https://github.com/karolisw/hyperFetch/tree/frontend)
 
 ## Using the pip module
 To use the pip model please do the following:
 1. Create a virtual environment in your favorite IDE. The virtual environment must be of the type virtualenv.
```

### Comparing `hyperfetch-1.0.4/src/hyperfetch.egg-info/requires.txt` & `hyperfetch-1.0.5/src/hyperfetch.egg-info/requires.txt`

 * *Files identical despite different names*

