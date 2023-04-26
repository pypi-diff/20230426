# Comparing `tmp/remyxai-0.1.0.tar.gz` & `tmp/remyxai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remyxai-0.1.0.tar", last modified: Tue Apr 25 04:44:34 2023, max compression
+gzip compressed data, was "remyxai-0.1.1.tar", last modified: Tue Apr 25 14:41:46 2023, max compression
```

## Comparing `remyxai-0.1.0.tar` & `remyxai-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 04:44:34.776373 remyxai-0.1.0/
--rw-rw-r--   0 funk      (1000) funk      (1000)     2176 2023-04-25 04:44:34.776373 remyxai-0.1.0/PKG-INFO
--rw-rw-r--   0 funk      (1000) funk      (1000)     2084 2023-04-25 04:27:08.000000 remyxai-0.1.0/README.md
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 04:44:34.776373 remyxai-0.1.0/remyxai/
--rw-rw-r--   0 funk      (1000) funk      (1000)        0 2023-04-24 16:17:23.000000 remyxai-0.1.0/remyxai/__init__.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     1472 2023-04-25 04:03:15.000000 remyxai-0.1.0/remyxai/api.py
--rw-rw-r--   0 funk      (1000) funk      (1000)     3190 2023-04-25 03:49:52.000000 remyxai-0.1.0/remyxai/cli.py
-drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 04:44:34.776373 remyxai-0.1.0/remyxai.egg-info/
--rw-rw-r--   0 funk      (1000) funk      (1000)     2176 2023-04-25 04:44:34.000000 remyxai-0.1.0/remyxai.egg-info/PKG-INFO
--rw-rw-r--   0 funk      (1000) funk      (1000)      256 2023-04-25 04:44:34.000000 remyxai-0.1.0/remyxai.egg-info/SOURCES.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        1 2023-04-25 04:44:34.000000 remyxai-0.1.0/remyxai.egg-info/dependency_links.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       45 2023-04-25 04:44:34.000000 remyxai-0.1.0/remyxai.egg-info/entry_points.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        9 2023-04-25 04:44:34.000000 remyxai-0.1.0/remyxai.egg-info/requires.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)        8 2023-04-25 04:44:34.000000 remyxai-0.1.0/remyxai.egg-info/top_level.txt
--rw-rw-r--   0 funk      (1000) funk      (1000)       38 2023-04-25 04:44:34.776373 remyxai-0.1.0/setup.cfg
--rw-rw-r--   0 funk      (1000) funk      (1000)      522 2023-04-25 04:44:28.000000 remyxai-0.1.0/setup.py
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 14:41:46.511942 remyxai-0.1.1/
+-rw-rw-r--   0 funk      (1000) funk      (1000)     1065 2023-04-25 04:59:23.000000 remyxai-0.1.1/LICENSE
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2200 2023-04-25 14:41:46.511942 remyxai-0.1.1/PKG-INFO
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2086 2023-04-25 14:19:52.000000 remyxai-0.1.1/README.md
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 14:41:46.511942 remyxai-0.1.1/remyxai/
+-rw-rw-r--   0 funk      (1000) funk      (1000)        0 2023-04-24 16:17:23.000000 remyxai-0.1.1/remyxai/__init__.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     1490 2023-04-25 14:41:30.000000 remyxai-0.1.1/remyxai/api.py
+-rw-rw-r--   0 funk      (1000) funk      (1000)     3222 2023-04-25 14:41:30.000000 remyxai-0.1.1/remyxai/cli.py
+drwxrwxr-x   0 funk      (1000) funk      (1000)        0 2023-04-25 14:41:46.511942 remyxai-0.1.1/remyxai.egg-info/
+-rw-rw-r--   0 funk      (1000) funk      (1000)     2200 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/PKG-INFO
+-rw-rw-r--   0 funk      (1000) funk      (1000)      264 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        1 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       45 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/entry_points.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        9 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/requires.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)        8 2023-04-25 14:41:46.000000 remyxai-0.1.1/remyxai.egg-info/top_level.txt
+-rw-rw-r--   0 funk      (1000) funk      (1000)       38 2023-04-25 14:41:46.511942 remyxai-0.1.1/setup.cfg
+-rw-rw-r--   0 funk      (1000) funk      (1000)      522 2023-04-25 14:41:30.000000 remyxai-0.1.1/setup.py
```

### Comparing `remyxai-0.1.0/PKG-INFO` & `remyxai-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: remyxai
-Version: 0.1.0
+Version: 0.1.1
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
 ```
 
 ## Token authentication
-OpenAI API requires authentication token, which can be obtained on this page: https://engine.remyx.ai/account
+Remyx AI API requires authentication token, which can be obtained on this page: https://engine.remyx.ai/account
 
 Provide api key to the CLI through an environment variable `REMYXAI_API_KEY`.
 ```
 export REMYXAI_API_KEY=<your-key-here>
 ```
 
 ## Usage
```

### Comparing `remyxai-0.1.0/README.md` & `remyxai-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
 ```
 
 ## Token authentication
-OpenAI API requires authentication token, which can be obtained on this page: https://engine.remyx.ai/account
+Remyx AI API requires authentication token, which can be obtained on this page: https://engine.remyx.ai/account
 
 Provide api key to the CLI through an environment variable `REMYXAI_API_KEY`.
 ```
 export REMYXAI_API_KEY=<your-key-here>
 ```
 
 ## Usage
```

### Comparing `remyxai-0.1.0/remyxai/api.py` & `remyxai-0.1.1/remyxai/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     return response.json()
 
 def download_model(model_name, model_format):
     url = f"{BASE_URL}model/download/{model_name}/{model_format}"
     response = requests.post(url, headers=HEADERS, stream=True)
     with open(f"{model_name}.zip", "wb") as out_file:
         shutil.copyfileobj(response.raw, out_file)
-    return 'The file was saved successfully'
+    return f"The file {model_name}.zip was saved successfully"
 
 # Engines
 def train_classifier(model_name, labels, model_selector):
     url = f"{BASE_URL}task/classify/{model_name}/{','.join(labels)}/{model_selector}"
     response = requests.post(url, headers=HEADERS)
     return response.json()
```

### Comparing `remyxai-0.1.0/remyxai/cli.py` & `remyxai-0.1.1/remyxai/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .api import *
 import argparse
+from pprint import pprint
 
 def main():
     parser = argparse.ArgumentParser(description="Model management script")
 
     # Define top-level actions
     subparsers_action = parser.add_subparsers(dest="action", help="Top-level actions")
 
@@ -40,34 +41,34 @@
     credits_parser = subparsers_user.add_parser("credits", help="Get user credits and subscription info if it exists")
 
     args = parser.parse_args()
 
     if args.action == "model":
         if args.subaction == "list":
             models = list_models()
-            return models
+            pprint(models)
         elif args.subaction == "delete":
             deleted_model = delete_model(args.model_name)
-            return deleted_model
+            pprint(deleted_model)
         elif args.subaction == "download":
             downloaded_model = download_model(args.model_name, args.model_format)
-            return downloaded_model
+            print(downloaded_model)
         else:
             print("Invalid argument for 'model'")
     elif args.action == "classify":
         labels = args.labels.split(",")
         training_classifier = train_classifier(args.model_name, labels, args.model_size)
-        return training_classifier
+        pprint(training_classifier) 
     elif args.action == "user":
         if args.subaction == "profile":
             profile = get_user_profile()
-            return profile
+            pprint(profile)
         elif args.subaction == "credits":
             user_credits = get_user_credits()
-            return user_credits
+            pprint(user_credits)
         else:
             print("Invalid argument for 'user'")
     else:
         print("Invalid action")
 
 if __name__ == "__main__":
     main()
```

### Comparing `remyxai-0.1.0/remyxai.egg-info/PKG-INFO` & `remyxai-0.1.1/remyxai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: remyxai
-Version: 0.1.0
+Version: 0.1.1
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Remyx AI command-line client
 
 ## Installation
 To install the Remyx AI CLI in Python virtual environment, run:
 
 ```
 pip install remyxai
 ```
 
 ## Token authentication
-OpenAI API requires authentication token, which can be obtained on this page: https://engine.remyx.ai/account
+Remyx AI API requires authentication token, which can be obtained on this page: https://engine.remyx.ai/account
 
 Provide api key to the CLI through an environment variable `REMYXAI_API_KEY`.
 ```
 export REMYXAI_API_KEY=<your-key-here>
 ```
 
 ## Usage
```

### Comparing `remyxai-0.1.0/setup.py` & `remyxai-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="remyxai",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=["requests"],
     entry_points={
         "console_scripts": [
             "remyxai=remyxai.cli:main",
         ],
     },
```

