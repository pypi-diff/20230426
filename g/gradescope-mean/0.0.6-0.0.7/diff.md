# Comparing `tmp/gradescope_mean-0.0.6.tar.gz` & `tmp/gradescope_mean-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradescope_mean-0.0.6.tar", last modified: Tue Apr 25 16:35:44 2023, max compression
+gzip compressed data, was "gradescope_mean-0.0.7.tar", last modified: Tue Apr 25 16:47:54 2023, max compression
```

## Comparing `gradescope_mean-0.0.6.tar` & `gradescope_mean-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1068 2022-05-09 19:38:36.000000 gradescope_mean-0.0.6/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)       40 2022-05-10 15:46:26.000000 gradescope_mean-0.0.6/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)     4313 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     2641 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/gradescope_mean/
--rw-rw-r--   0 matt      (1000) matt      (1000)       89 2022-12-15 17:55:21.000000 gradescope_mean-0.0.6/gradescope_mean/__init__.py
--rwxrwxr-x   0 matt      (1000) matt      (1000)     2486 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1667 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/assign_list.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/gradescope_mean/banner/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/banner/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1595 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/banner/__main__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/gradescope_mean/canvas/
--rw-rw-r--   0 matt      (1000) matt      (1000)       22 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/canvas/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1874 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/canvas/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2660 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/canvas/canvas.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4384 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      321 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/config.yaml
--rw-rw-r--   0 matt      (1000) matt      (1000)     1431 2022-05-09 19:40:21.000000 gradescope_mean-0.0.6/gradescope_mean/get_mean_drop_low.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    15791 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/gradescope_mean/gradebook.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1441 2022-12-15 17:55:21.000000 gradescope_mean-0.0.6/gradescope_mean/perc_to_letter.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1242 2022-12-15 17:55:21.000000 gradescope_mean-0.0.6/gradescope_mean/plot.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/gradescope_mean.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     4313 2023-04-25 16:35:44.000000 gradescope_mean-0.0.6/gradescope_mean.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      803 2023-04-25 16:35:44.000000 gradescope_mean-0.0.6/gradescope_mean.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-04-25 16:35:44.000000 gradescope_mean-0.0.6/gradescope_mean.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-04-25 16:35:44.000000 gradescope_mean-0.0.6/gradescope_mean.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       16 2023-04-25 16:35:44.000000 gradescope_mean-0.0.6/gradescope_mean.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)      704 2023-04-25 16:34:56.000000 gradescope_mean-0.0.6/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/setup.cfg
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:35:44.710909 gradescope_mean-0.0.6/test/
--rw-rw-r--   0 matt      (1000) matt      (1000)      846 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/test/test_assign_list.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      296 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/test/test_config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1311 2022-05-09 19:40:21.000000 gradescope_mean-0.0.6/test/test_get_mean_drop_low.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6225 2023-04-25 16:34:44.000000 gradescope_mean-0.0.6/test/test_gradebook.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      927 2022-12-15 17:55:21.000000 gradescope_mean-0.0.6/test/test_perc_to_letter.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:47:54.372385 gradescope_mean-0.0.7/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1068 2022-05-09 19:38:36.000000 gradescope_mean-0.0.7/LICENSE
+-rw-rw-r--   0 matt      (1000) matt      (1000)       40 2022-05-10 15:46:26.000000 gradescope_mean-0.0.7/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4313 2023-04-25 16:47:54.368385 gradescope_mean-0.0.7/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2641 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:47:54.368385 gradescope_mean-0.0.7/gradescope_mean/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       89 2022-12-15 17:55:21.000000 gradescope_mean-0.0.7/gradescope_mean/__init__.py
+-rwxrwxr-x   0 matt      (1000) matt      (1000)     2486 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1667 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/assign_list.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:47:54.368385 gradescope_mean-0.0.7/gradescope_mean/banner/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/banner/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1595 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/banner/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:47:54.368385 gradescope_mean-0.0.7/gradescope_mean/canvas/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       22 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/canvas/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1874 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/canvas/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2660 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/canvas/canvas.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4384 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      321 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/gradescope_mean/config.yaml
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1431 2022-05-09 19:40:21.000000 gradescope_mean-0.0.7/gradescope_mean/get_mean_drop_low.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    15777 2023-04-25 16:47:18.000000 gradescope_mean-0.0.7/gradescope_mean/gradebook.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1441 2022-12-15 17:55:21.000000 gradescope_mean-0.0.7/gradescope_mean/perc_to_letter.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1242 2022-12-15 17:55:21.000000 gradescope_mean-0.0.7/gradescope_mean/plot.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:47:54.368385 gradescope_mean-0.0.7/gradescope_mean.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     4313 2023-04-25 16:47:54.000000 gradescope_mean-0.0.7/gradescope_mean.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      803 2023-04-25 16:47:54.000000 gradescope_mean-0.0.7/gradescope_mean.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-04-25 16:47:54.000000 gradescope_mean-0.0.7/gradescope_mean.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-04-25 16:47:54.000000 gradescope_mean-0.0.7/gradescope_mean.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       16 2023-04-25 16:47:54.000000 gradescope_mean-0.0.7/gradescope_mean.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)      704 2023-04-25 16:47:34.000000 gradescope_mean-0.0.7/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-04-25 16:47:54.372385 gradescope_mean-0.0.7/setup.cfg
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-04-25 16:47:54.368385 gradescope_mean-0.0.7/test/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      846 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/test/test_assign_list.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      296 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/test/test_config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1311 2022-05-09 19:40:21.000000 gradescope_mean-0.0.7/test/test_get_mean_drop_low.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6225 2023-04-25 16:34:44.000000 gradescope_mean-0.0.7/test/test_gradebook.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      927 2022-12-15 17:55:21.000000 gradescope_mean-0.0.7/test/test_perc_to_letter.py
```

### Comparing `gradescope_mean-0.0.6/LICENSE` & `gradescope_mean-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/PKG-INFO` & `gradescope_mean-0.0.7/gradescope_mean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gradescope_mean
-Version: 0.0.6
+Name: gradescope-mean
+Version: 0.0.7
 Summary: utility to average gradescope csv output to final grades
 Author-email: Matt Higger <matt.higger@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 matt higger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gradescope_mean-0.0.6/README.md` & `gradescope_mean-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/__main__.py` & `gradescope_mean-0.0.7/gradescope_mean/__main__.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/assign_list.py` & `gradescope_mean-0.0.7/gradescope_mean/assign_list.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/banner/__main__.py` & `gradescope_mean-0.0.7/gradescope_mean/banner/__main__.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/canvas/__main__.py` & `gradescope_mean-0.0.7/gradescope_mean/canvas/__main__.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/canvas/canvas.py` & `gradescope_mean-0.0.7/gradescope_mean/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/config.py` & `gradescope_mean-0.0.7/gradescope_mean/config.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/get_mean_drop_low.py` & `gradescope_mean-0.0.7/gradescope_mean/get_mean_drop_low.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/gradebook.py` & `gradescope_mean-0.0.7/gradescope_mean/gradebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         """
         # find percent missing per assignment per ass, rm if above thresh
         s_complete_perc = 1 - (self.df_perc.fillna(0) == 0).mean(axis=0)
         for ass, comp_perc in s_complete_perc.sort_values().items():
             if comp_perc < min_complete_thresh:
                 msg = f'removed: {comp_perc * 100:.0f}% complete {ass}'
                 self.remove(ass, skip_match=True)
-            elif comp_perc < 1:
+            else:
                 msg = f'   kept: {comp_perc * 100:.0f}% complete {ass}'
             print(msg)
 
     def remove(self, ass, multi=False, skip_match=False):
         """ deletes an assignment
 
         Args:
```

### Comparing `gradescope_mean-0.0.6/gradescope_mean/perc_to_letter.py` & `gradescope_mean-0.0.7/gradescope_mean/perc_to_letter.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean/plot.py` & `gradescope_mean-0.0.7/gradescope_mean/plot.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/gradescope_mean.egg-info/PKG-INFO` & `gradescope_mean-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gradescope-mean
-Version: 0.0.6
+Name: gradescope_mean
+Version: 0.0.7
 Summary: utility to average gradescope csv output to final grades
 Author-email: Matt Higger <matt.higger@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 matt higger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gradescope_mean-0.0.6/gradescope_mean.egg-info/SOURCES.txt` & `gradescope_mean-0.0.7/gradescope_mean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/pyproject.toml` & `gradescope_mean-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gradescope_mean"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Matt Higger", email = "matt.higger@gmail.com" },
 ]
 description = "utility to average gradescope csv output to final grades"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `gradescope_mean-0.0.6/test/test_assign_list.py` & `gradescope_mean-0.0.7/test/test_assign_list.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/test/test_get_mean_drop_low.py` & `gradescope_mean-0.0.7/test/test_get_mean_drop_low.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/test/test_gradebook.py` & `gradescope_mean-0.0.7/test/test_gradebook.py`

 * *Files identical despite different names*

### Comparing `gradescope_mean-0.0.6/test/test_perc_to_letter.py` & `gradescope_mean-0.0.7/test/test_perc_to_letter.py`

 * *Files identical despite different names*

