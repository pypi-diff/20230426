# Comparing `tmp/terminally-0.1.5.tar.gz` & `tmp/terminally-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminally-0.1.5.tar", last modified: Tue Apr 25 11:15:19 2023, max compression
+gzip compressed data, was "terminally-0.1.6.tar", last modified: Tue Apr 25 18:29:36 2023, max compression
```

## Comparing `terminally-0.1.5.tar` & `terminally-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:15:19.693747 terminally-0.1.5/
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 11:15:19.693747 terminally-0.1.5/PKG-INFO
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)      601 2023-04-25 11:06:42.000000 terminally-0.1.5/README.md
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       38 2023-04-25 11:15:19.693747 terminally-0.1.5/setup.cfg
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)      300 2023-04-25 11:15:10.000000 terminally-0.1.5/setup.py
-drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:15:19.693747 terminally-0.1.5/terminally/
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       23 2023-04-25 11:12:41.000000 terminally-0.1.5/terminally/__init__.py
--rwxr-xr-x   0 moonsun   (1000) moonsun   (1000)     7413 2023-04-25 10:33:46.000000 terminally-0.1.5/terminally/ally.py
-drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:15:19.693747 terminally-0.1.5/terminally.egg-info/
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/PKG-INFO
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)      266 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/SOURCES.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)        1 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/dependency_links.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       46 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/entry_points.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       15 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/requires.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       11 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/top_level.txt
+drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 18:29:36.397460 terminally-0.1.6/
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 18:29:36.397460 terminally-0.1.6/PKG-INFO
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)      601 2023-04-25 11:06:42.000000 terminally-0.1.6/README.md
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       38 2023-04-25 18:29:36.397460 terminally-0.1.6/setup.cfg
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)      300 2023-04-25 18:29:32.000000 terminally-0.1.6/setup.py
+drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 18:29:36.397460 terminally-0.1.6/terminally/
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       23 2023-04-25 11:12:41.000000 terminally-0.1.6/terminally/__init__.py
+-rwxr-xr-x   0 moonsun   (1000) moonsun   (1000)     7838 2023-04-25 18:29:17.000000 terminally-0.1.6/terminally/ally.py
+drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 18:29:36.397460 terminally-0.1.6/terminally.egg-info/
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 18:29:36.000000 terminally-0.1.6/terminally.egg-info/PKG-INFO
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)      266 2023-04-25 18:29:36.000000 terminally-0.1.6/terminally.egg-info/SOURCES.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)        1 2023-04-25 18:29:36.000000 terminally-0.1.6/terminally.egg-info/dependency_links.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       46 2023-04-25 18:29:36.000000 terminally-0.1.6/terminally.egg-info/entry_points.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       15 2023-04-25 18:29:36.000000 terminally-0.1.6/terminally.egg-info/requires.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       11 2023-04-25 18:29:36.000000 terminally-0.1.6/terminally.egg-info/top_level.txt
```

### Comparing `terminally-0.1.5/README.md` & `terminally-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `terminally-0.1.5/terminally/ally.py` & `terminally-0.1.6/terminally/ally.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 
 from pprint import pprint
 DEFAULTING_MATCH = "I assume that's a NO then..."
 CONFIG_FILENAME = "config.json"
 DATASET_FILENAME = "dataset.json"
 
 FORBIDDEN_COMMANDS = ["eval"]
+
+def help():
+    print("Welcome to the TerminAlly beta test!")
+    print("You can find us on discord: https://discord.gg/DgNKk4WJ")
+    print("Usage:")
+    print("ally -> starts a prompt loop")
+    print("ally your prompt for a cli command")
+    print(f"Your prompt/reply data is stored in: {get_config_path(DATASET_FILENAME)}")
+    print("Sharing it with us would be so helpful in improving the algorithm!")
+
 def load_config():
     global USER_DATASET
     global USER_SHELL
 
     config = read_config()
 
     openai.api_key = config.get("OPENAI_API_KEY", "")
@@ -55,14 +65,15 @@
 
 def read_config():
     config_file = get_config_path(CONFIG_FILENAME)
     if os.path.exists(config_file):
         with open(config_file, "r") as f:
             config = json.load(f)
     else:
+        help()
         config = {}
     return config
 
 
 def explain_case(prompt, command):
     try:
         explanation = explain(prompt, command)
```

