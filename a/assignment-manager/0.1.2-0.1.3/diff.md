# Comparing `tmp/assignment-manager-0.1.2.tar.gz` & `tmp/assignment-manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assignment-manager-0.1.2.tar", last modified: Tue Apr 25 18:27:25 2023, max compression
+gzip compressed data, was "assignment-manager-0.1.3.tar", last modified: Wed Apr 26 06:47:06 2023, max compression
```

## Comparing `assignment-manager-0.1.2.tar` & `assignment-manager-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 18:27:25.353298 assignment-manager-0.1.2/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.2/LICENSE
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-25 18:27:25.353298 assignment-manager-0.1.2/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.2/README.md
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       98 2023-04-23 16:36:52.000000 assignment-manager-0.1.2/pyproject.toml
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-25 18:27:25.353298 assignment-manager-0.1.2/setup.cfg
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-25 18:27:02.000000 assignment-manager-0.1.2/setup.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 18:27:25.353298 assignment-manager-0.1.2/src/
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 18:27:25.353298 assignment-manager-0.1.2/src/assignment_manager/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.2/src/assignment_manager/__init__.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     3370 2023-04-25 18:23:45.000000 assignment-manager-0.1.2/src/assignment_manager/assignments.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     1811 2023-04-25 18:23:27.000000 assignment-manager-0.1.2/src/assignment_manager/data.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)     2210 2023-04-24 15:48:57.000000 assignment-manager-0.1.2/src/assignment_manager/io.py
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      922 2023-04-25 17:41:28.000000 assignment-manager-0.1.2/src/assignment_manager/main.py
-drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-25 18:27:25.353298 assignment-manager-0.1.2/src/assignment_manager.egg-info/
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-25 18:27:25.000000 assignment-manager-0.1.2/src/assignment_manager.egg-info/PKG-INFO
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-25 18:27:25.000000 assignment-manager-0.1.2/src/assignment_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-25 18:27:25.000000 assignment-manager-0.1.2/src/assignment_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-25 18:27:25.000000 assignment-manager-0.1.2/src/assignment_manager.egg-info/entry_points.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-25 18:27:25.000000 assignment-manager-0.1.2/src/assignment_manager.egg-info/requires.txt
--rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-25 18:27:25.000000 assignment-manager-0.1.2/src/assignment_manager.egg-info/top_level.txt
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1074 2023-04-23 16:17:44.000000 assignment-manager-0.1.3/LICENSE
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       21 2023-04-23 16:24:52.000000 assignment-manager-0.1.3/README.md
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       98 2023-04-23 16:36:52.000000 assignment-manager-0.1.3/pyproject.toml
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       74 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/setup.cfg
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2136 2023-04-25 18:46:18.000000 assignment-manager-0.1.3/setup.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.769841 assignment-manager-0.1.3/src/
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/src/assignment_manager/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        0 2023-04-23 16:35:05.000000 assignment-manager-0.1.3/src/assignment_manager/__init__.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     3684 2023-04-25 18:43:44.000000 assignment-manager-0.1.3/src/assignment_manager/assignments.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     1811 2023-04-25 18:23:27.000000 assignment-manager-0.1.3/src/assignment_manager/data.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)     2390 2023-04-25 18:39:29.000000 assignment-manager-0.1.3/src/assignment_manager/io.py
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      989 2023-04-25 18:44:19.000000 assignment-manager-0.1.3/src/assignment_manager/main.py
+drwxrwxr-x   0 rancic    (1000) rancic    (1000)        0 2023-04-26 06:47:06.773841 assignment-manager-0.1.3/src/assignment_manager.egg-info/
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      858 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      493 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)        1 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)      106 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       20 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/requires.txt
+-rw-rw-r--   0 rancic    (1000) rancic    (1000)       19 2023-04-26 06:47:06.000000 assignment-manager-0.1.3/src/assignment_manager.egg-info/top_level.txt
```

### Comparing `assignment-manager-0.1.2/LICENSE` & `assignment-manager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.2/PKG-INFO` & `assignment-manager-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `assignment-manager-0.1.2/setup.py` & `assignment-manager-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="assignment-manager",
-    version="0.1.2",
+    version="0.1.3",
     description=("Manage reoccuring assignments and tasks."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PraxTube/assignment-manager",
     author="Prax",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `assignment-manager-0.1.2/src/assignment_manager/assignments.py` & `assignment-manager-0.1.3/src/assignment_manager/assignments.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     params = io.add_assignment_response()
 
     if data_file_empty():
         data = {}
     else:
         data = load_data()
 
-    if params[0] in data.keys():
-        raise ValueError("Name already exists!", name)
+    if params[0] in data:
+        raise ValueError("Name already exists!", name, data.keys())
 
     progress = generate_dates(params[1], params[2], params[3], params[4])
     data[params[0]] = progress
     write_data(data)
 
 
 def update_assignment():
@@ -86,14 +86,26 @@
     progress_choices = [p.name for p in Progress]
     cycle, progress = io.update_assignment_response(cycle_choices, progress_choices)
 
     data[name][cycle][2] = progress
     write_data(data)
 
 
+def rename_assignment():
+    data = load_data()
+    old_name = io.course_response(data.keys())
+    new_name = io.rename_assignment_response()
+
+    if new_name in data:
+        raise ValueError("The name already exists!", new_name, data.keys())
+
+    data[new_name] = data.pop(old_name)
+    write_data(data)
+
+
 def remove_assignment():
     data = load_data()
     name = io.course_response(data.keys())
 
     confirmation_msg = "This will delete [bold]ALL[/bold] data for the course: [bold]{}[/bold]\n".format(
         name
     )
```

### Comparing `assignment-manager-0.1.2/src/assignment_manager/data.py` & `assignment-manager-0.1.3/src/assignment_manager/data.py`

 * *Files identical despite different names*

### Comparing `assignment-manager-0.1.2/src/assignment_manager/io.py` & `assignment-manager-0.1.3/src/assignment_manager/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,7 +73,14 @@
         ),
     ]
     answers = inquirer.prompt(questions)
     cycle = cycle_choices.index(answers["cycle"])
     progress = progress_choices.index(answers["progress"])
 
     return (cycle, progress)
+
+
+def rename_assignment_response():
+    question = [
+        inquirer.Text("name", message="What's the new name of the course?")
+    ]
+    return inquirer.prompt(question)["name"]
```

### Comparing `assignment-manager-0.1.2/src/assignment_manager/main.py` & `assignment-manager-0.1.3/src/assignment_manager/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 @app.command()
 def update():
     assignments.update_assignment()
 
 
 @app.command()
+def rename():
+    assignments.rename_assignment()
+
+
+@app.command()
 def remove():
     assignments.remove_assignment()
 
 
 @backup_app.command("copy")
 def copy_backup():
     """
```

### Comparing `assignment-manager-0.1.2/src/assignment_manager.egg-info/PKG-INFO` & `assignment-manager-0.1.3/src/assignment_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assignment-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Manage reoccuring assignments and tasks.
 Home-page: https://github.com/PraxTube/assignment-manager
 Author: Prax
 Project-URL: Bug Reports, https://github.com/PraxTube/assignment-manager/issues
 Project-URL: Source, https://github.com/PraxTube/assignment-manager
 Keywords: manager,task,assignment,task-manager,assignment-manager
 Classifier: Development Status :: 3 - Alpha
```

