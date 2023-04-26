# Comparing `tmp/falra_run_github-0.1.1.tar.gz` & `tmp/falra_run_github-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/falra_run_github-0.1.1.tar", last modified: Wed Apr 26 15:02:59 2023, max compression
+gzip compressed data, was "dist/falra_run_github-0.1.3.tar", last modified: Wed Apr 26 15:18:49 2023, max compression
```

## Comparing `falra_run_github-0.1.1.tar` & `falra_run_github-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:02:59.902256 falra_run_github-0.1.1/
--rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:02:59.901967 falra_run_github-0.1.1/PKG-INFO
--rw-r--r--   0 wengroy    (501) staff       (20)      984 2023-04-13 18:39:23.000000 falra_run_github-0.1.1/README.md
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:02:59.897884 falra_run_github-0.1.1/falra_run_github/
--rw-r--r--   0 wengroy    (501) staff       (20)        0 2023-03-09 00:23:54.000000 falra_run_github-0.1.1/falra_run_github/__init__.py
--rw-r--r--   0 wengroy    (501) staff       (20)       78 2023-04-13 18:03:18.000000 falra_run_github-0.1.1/falra_run_github/__main__.py
--rwxr-xr-x   0 wengroy    (501) staff       (20)     8790 2023-04-26 14:56:03.000000 falra_run_github-0.1.1/falra_run_github/main.py
-drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:02:59.901517 falra_run_github-0.1.1/falra_run_github.egg-info/
--rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/PKG-INFO
--rw-r--r--   0 wengroy    (501) staff       (20)      343 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/SOURCES.txt
--rw-r--r--   0 wengroy    (501) staff       (20)        1 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/dependency_links.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       62 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/entry_points.txt
--rw-r--r--   0 wengroy    (501) staff       (20)      600 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/requires.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       17 2023-04-26 15:02:59.000000 falra_run_github-0.1.1/falra_run_github.egg-info/top_level.txt
--rw-r--r--   0 wengroy    (501) staff       (20)       38 2023-04-26 15:02:59.902355 falra_run_github-0.1.1/setup.cfg
--rwxr-xr-x   0 wengroy    (501) staff       (20)      439 2023-04-26 14:57:49.000000 falra_run_github-0.1.1/setup.py
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:18:49.820818 falra_run_github-0.1.3/
+-rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:18:49.820528 falra_run_github-0.1.3/PKG-INFO
+-rw-r--r--   0 wengroy    (501) staff       (20)      984 2023-04-13 18:39:23.000000 falra_run_github-0.1.3/README.md
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:18:49.816282 falra_run_github-0.1.3/falra_run_github/
+-rw-r--r--   0 wengroy    (501) staff       (20)        0 2023-03-09 00:23:54.000000 falra_run_github-0.1.3/falra_run_github/__init__.py
+-rw-r--r--   0 wengroy    (501) staff       (20)       78 2023-04-13 18:03:18.000000 falra_run_github-0.1.3/falra_run_github/__main__.py
+-rwxr-xr-x   0 wengroy    (501) staff       (20)     8896 2023-04-26 15:18:41.000000 falra_run_github-0.1.3/falra_run_github/main.py
+drwxr-xr-x   0 wengroy    (501) staff       (20)        0 2023-04-26 15:18:49.820055 falra_run_github-0.1.3/falra_run_github.egg-info/
+-rw-r--r--   0 wengroy    (501) staff       (20)      190 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/PKG-INFO
+-rw-r--r--   0 wengroy    (501) staff       (20)      343 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/SOURCES.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)        1 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/dependency_links.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       62 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/entry_points.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)      600 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/requires.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       17 2023-04-26 15:18:49.000000 falra_run_github-0.1.3/falra_run_github.egg-info/top_level.txt
+-rw-r--r--   0 wengroy    (501) staff       (20)       38 2023-04-26 15:18:49.820911 falra_run_github-0.1.3/setup.cfg
+-rwxr-xr-x   0 wengroy    (501) staff       (20)      439 2023-04-26 15:18:46.000000 falra_run_github-0.1.3/setup.py
```

### Comparing `falra_run_github-0.1.1/README.md` & `falra_run_github-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `falra_run_github-0.1.1/falra_run_github/main.py` & `falra_run_github-0.1.3/falra_run_github/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     execution_result = query_output(repo_name=repo_name)
     print(execution_result)
     print("004 run_main_py done.")
 
 
 def main():
     parser = argparse.ArgumentParser(description='GitHub Executor')
-    parser.add_argument('--action', type=str, required=True, choices=['start', 'output', 'clean'], help="The actions to execute")
+    parser.add_argument('--action', type=str, required=True, choices=['start', 'output', 'clean', 'version'], help="The actions to execute")
     parser.add_argument('--repo_url', metavar='repo_url', type=str, help='URL of the GitHub repository')
     parser.add_argument('--access_token', metavar='access_token', type=str, help='Access token for the GitHub API')
     parser.add_argument('--user_id', metavar='user_id', type=str, help='user_id as string')
     parser.add_argument('--repo_name', metavar='repo_name', type=str, help='Name of the repository')
     parser.add_argument('--py_name', metavar='py_name', type=str, help='Name of the Python file to execute')
     parser.add_argument('--argument', metavar='argument', type=str, help='Arguments of the Python to execute as string')
 
@@ -239,9 +239,13 @@
         if not args.repo_name:
             parser.error("Executing output query requires --repo_name parameter")
         query_output(args.repo_name)
 
     elif args.action == "clean":
         clean_user_repo()
 
+    elif args.action == "version":
+        print("This package is: falra-run-github v0.1.3")
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `falra_run_github-0.1.1/falra_run_github.egg-info/requires.txt` & `falra_run_github-0.1.3/falra_run_github.egg-info/requires.txt`

 * *Files identical despite different names*

