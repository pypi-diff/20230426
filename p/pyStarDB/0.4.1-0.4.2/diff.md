# Comparing `tmp/pyStarDB-0.4.1.tar.gz` & `tmp/pyStarDB-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyStarDB-0.4.1.tar", last modified: Tue Aug 30 06:22:19 2022, max compression
+gzip compressed data, was "pyStarDB-0.4.2.tar", last modified: Wed Apr 26 07:38:35 2023, max compression
```

## Comparing `pyStarDB-0.4.1.tar` & `pyStarDB-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2022-08-30 06:22:19.664322 pyStarDB-0.4.1/
--rw-r--r--   0 twagner  (22293) domain users (32000)     1101 2020-09-15 10:59:24.000000 pyStarDB-0.4.1/LICENSE
--rw-r--r--   0 twagner  (22293) domain users (32000)      262 2022-08-30 06:22:19.664322 pyStarDB-0.4.1/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      986 2022-03-25 10:05:17.000000 pyStarDB-0.4.1/README.md
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2022-08-30 06:22:19.664322 pyStarDB-0.4.1/pyStarDB/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 10:59:24.000000 pyStarDB-0.4.1/pyStarDB/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    29130 2022-08-30 06:22:05.000000 pyStarDB-0.4.1/pyStarDB/sp_pystardb.py
--rwxr-xr-x   0 twagner  (22293) domain users (32000)     9354 2021-11-03 15:20:34.000000 pyStarDB-0.4.1/pyStarDB/star_viewer.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2022-08-30 06:22:19.664322 pyStarDB-0.4.1/pyStarDB.egg-info/
--rw-r--r--   0 twagner  (22293) domain users (32000)      262 2022-08-30 06:22:19.000000 pyStarDB-0.4.1/pyStarDB.egg-info/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      295 2022-08-30 06:22:19.000000 pyStarDB-0.4.1/pyStarDB.egg-info/SOURCES.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        1 2022-08-30 06:22:19.000000 pyStarDB-0.4.1/pyStarDB.egg-info/dependency_links.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       28 2022-08-30 06:22:19.000000 pyStarDB-0.4.1/pyStarDB.egg-info/requires.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       15 2022-08-30 06:22:19.000000 pyStarDB-0.4.1/pyStarDB.egg-info/top_level.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       38 2022-08-30 06:22:19.664322 pyStarDB-0.4.1/setup.cfg
--rw-r--r--   0 twagner  (22293) domain users (32000)      466 2022-08-30 06:22:16.000000 pyStarDB-0.4.1/setup.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2022-08-30 06:22:19.664322 pyStarDB-0.4.1/tests/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 11:49:36.000000 pyStarDB-0.4.1/tests/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    10291 2022-03-25 10:21:59.000000 pyStarDB-0.4.1/tests/test_pystardb.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1101 2020-09-15 10:59:24.000000 pyStarDB-0.4.2/LICENSE
+-rw-r--r--   0 twagner  (22293) domain users (32000)      234 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      986 2022-03-25 10:05:17.000000 pyStarDB-0.4.2/README.md
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/pyStarDB/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 10:59:24.000000 pyStarDB-0.4.2/pyStarDB/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    29159 2023-04-26 07:30:04.000000 pyStarDB-0.4.2/pyStarDB/sp_pystardb.py
+-rwxr-xr-x   0 twagner  (22293) domain users (32000)     9354 2021-11-03 15:20:34.000000 pyStarDB-0.4.2/pyStarDB/star_viewer.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/pyStarDB.egg-info/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      234 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      295 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/SOURCES.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/dependency_links.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       28 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/requires.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       15 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/top_level.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       38 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/setup.cfg
+-rw-r--r--   0 twagner  (22293) domain users (32000)      466 2023-04-26 07:35:48.000000 pyStarDB-0.4.2/setup.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/tests/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 11:49:36.000000 pyStarDB-0.4.2/tests/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    10527 2023-04-26 07:33:37.000000 pyStarDB-0.4.2/tests/test_pystardb.py
```

### Comparing `pyStarDB-0.4.1/LICENSE` & `pyStarDB-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyStarDB-0.4.1/README.md` & `pyStarDB-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyStarDB-0.4.1/pyStarDB/sp_pystardb.py` & `pyStarDB-0.4.2/pyStarDB/sp_pystardb.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,16 +242,16 @@
             self.star_content,
             usecols=[0],
             skiprows=line_dict['header'][0] - 1,
             nrows=line_dict['header'][1] - line_dict['header'][0] + 1,
             skip_blank_lines=False,
             header=None,
             delim_whitespace=True,
-            squeeze=True,
         )
+        header_names = header_names.squeeze("columns")
 
         self.star_content.seek(0)
         return pandas.read_csv(
             self.star_content,
             index_col=None,
             names=header_names,
             skiprows=line_dict['content'][0] - 1,
```

### Comparing `pyStarDB-0.4.1/pyStarDB/star_viewer.py` & `pyStarDB-0.4.2/pyStarDB/star_viewer.py`

 * *Files identical despite different names*

### Comparing `pyStarDB-0.4.1/tests/test_pystardb.py` & `pyStarDB-0.4.2/tests/test_pystardb.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,25 +37,32 @@
             b = pystar.StarFile(os.path.join(tmpdirname,"name.star"))
             b.update('', a, False)
             b.write_star_file()
             exists = os.path.exists(os.path.join(tmpdirname,"name.star"))
 
             self.assertTrue(exists,"File (no-loop) was not written")
 
+
+    def test_read_new_cbox(self):
+        starpath = os.path.join(os.path.dirname(__file__), '../resources/TcdA1-0155_frames_sum.cbox')
+        a = pystar.StarFile(starpath)
+        self.assertTrue('cryolo' in a)
+
     def test_create_and_read(self):
 
         with tempfile.TemporaryDirectory() as tmpdirname:
             fname = os.path.join(tmpdirname,'name.star')
 
             a = pd.DataFrame([[0, 1], [2, 3]], columns=['_col1', '_col2'])
             b = pystar.StarFile(fname)
             b.update('', a, True)
             b.write_star_file()
 
             c = pystar.StarFile(fname)
+            print(c)
 
             is_equal_col1 = a['_col1'].equals(c['']['_col1'])
             is_equal_col2 = a['_col2'].equals(c['']['_col2'])
 
             self.assertTrue(is_equal_col1 and is_equal_col2,"Write / Read test failed")
```

