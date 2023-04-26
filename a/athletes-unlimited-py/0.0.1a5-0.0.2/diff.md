# Comparing `tmp/athletes_unlimited_py-0.0.1a5.tar.gz` & `tmp/athletes_unlimited_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athletes_unlimited_py-0.0.1a5.tar", last modified: Wed Apr 12 23:11:28 2023, max compression
+gzip compressed data, was "athletes_unlimited_py-0.0.2.tar", last modified: Tue Apr 25 18:57:16 2023, max compression
```

## Comparing `athletes_unlimited_py-0.0.1a5.tar` & `athletes_unlimited_py-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:11:28.064222 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/aux_softball.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/basketball.py
--rw-r--r--   0 runner    (1001) docker     (123)    22245 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/lacrosse.py
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/softball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/volleyball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/athetes_unlimited_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25042 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/aux_softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/basketball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22245 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/lacrosse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47203 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/volleyball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/setup.cfg
```

### Comparing `athletes_unlimited_py-0.0.1a5/LICENSE` & `athletes_unlimited_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a5/PKG-INFO` & `athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: athletes_unlimited_py
-Version: 0.0.1a5
+Name: athletes-unlimited-py
+Version: 0.0.2
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
@@ -19,12 +19,42 @@
 
 # athletes-unlimited-py
 
 Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 
 ## How to install
 
-`athletes-unlimited-py` can be installed from this GitHub repository with the following command through pip:
+This package is is advalible through the `pip` package manager, and can be installed through one of the following commands in your terminal/shell:
+
+```
+pip install athletes_unlimited_py
+```
+
+OR
+
+```
+python -m pip install athletes_unlimited_py
+```
+
+If you are using a Linux/Mac instance, you may need to specify `python3` when installing.
+
+```
+python3 -m pip install athletes_unlimited_py
+```
+
+Alternatively, `athletes-unlimited-py` can be installed from this GitHub repository with the following command through pip:
 
 ```
 pip install git+https://github.com/armstjc/athletes-unlimited-py
 ```
+
+OR
+
+```
+python -m pip install git+https://github.com/armstjc/athletes-unlimited-py
+```
+
+OR
+
+```
+python3 -m pip install git+https://github.com/armstjc/athletes-unlimited-py
+```
```

### Comparing `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/basketball.py` & `athletes_unlimited_py-0.0.2/athetes_unlimited_py/basketball.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,23 +412,23 @@
     sport_json_data = json.loads(response.text)
     
     for i in tqdm(sport_json_data['data']):
         #print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
+            for j in tqdm(i['gameIds']):
                 print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_basketball_game_stats(season,j,get_team_stats=True)
+                game_df = get_au_basketball_pbp(season,j)
 
                 season_pbp_df = pd.concat([season_pbp_df,game_df],ignore_index=True)
                 del game_df
 
     return season_pbp_df
 
 def get_au_basketball_season_player_box(season:int) -> pd.DataFrame():
```

### Comparing `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/lacrosse.py` & `athletes_unlimited_py-0.0.2/athetes_unlimited_py/lacrosse.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/utils.py` & `athletes_unlimited_py-0.0.2/athetes_unlimited_py/utils.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/volleyball.py` & `athletes_unlimited_py-0.0.2/athetes_unlimited_py/volleyball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/PKG-INFO` & `athletes_unlimited_py-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: athletes-unlimited-py
-Version: 0.0.1a5
+Name: athletes_unlimited_py
+Version: 0.0.2
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
@@ -19,12 +19,42 @@
 
 # athletes-unlimited-py
 
 Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 
 ## How to install
 
-`athletes-unlimited-py` can be installed from this GitHub repository with the following command through pip:
+This package is is advalible through the `pip` package manager, and can be installed through one of the following commands in your terminal/shell:
+
+```
+pip install athletes_unlimited_py
+```
+
+OR
+
+```
+python -m pip install athletes_unlimited_py
+```
+
+If you are using a Linux/Mac instance, you may need to specify `python3` when installing.
+
+```
+python3 -m pip install athletes_unlimited_py
+```
+
+Alternatively, `athletes-unlimited-py` can be installed from this GitHub repository with the following command through pip:
 
 ```
 pip install git+https://github.com/armstjc/athletes-unlimited-py
 ```
+
+OR
+
+```
+python -m pip install git+https://github.com/armstjc/athletes-unlimited-py
+```
+
+OR
+
+```
+python3 -m pip install git+https://github.com/armstjc/athletes-unlimited-py
+```
```

### Comparing `athletes_unlimited_py-0.0.1a5/pyproject.toml` & `athletes_unlimited_py-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pyarrow","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "athletes_unlimited_py"
-version = "0.0.1a5"
+version = "0.0.2"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
```

