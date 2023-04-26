# Comparing `tmp/copydetect-0.4.4.tar.gz` & `tmp/copydetect-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copydetect-0.4.4.tar", last modified: Sat Feb  4 17:05:53 2023, max compression
+gzip compressed data, was "copydetect-0.4.5.tar", last modified: Wed Apr 26 03:30:22 2023, max compression
```

## Comparing `copydetect-0.4.4.tar` & `copydetect-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-02-04 17:05:53.283332 copydetect-0.4.4/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     1063 2020-10-17 00:41:54.000000 copydetect-0.4.4/LICENSE
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8631 2023-02-04 17:05:53.283332 copydetect-0.4.4/PKG-INFO
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     7839 2021-10-06 16:46:03.000000 copydetect-0.4.4/README.md
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-02-04 17:05:53.279332 copydetect-0.4.4/copydetect/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       90 2023-02-04 16:58:13.000000 copydetect-0.4.4/copydetect/__init__.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     6031 2022-11-05 17:08:31.000000 copydetect-0.4.4/copydetect/__main__.py
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-02-04 17:05:53.283332 copydetect-0.4.4/copydetect/data/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     2907 2021-10-06 17:02:55.000000 copydetect-0.4.4/copydetect/data/report.html
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       71 2022-05-29 22:08:04.000000 copydetect-0.4.4/copydetect/defaults.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)    28545 2023-02-04 16:56:25.000000 copydetect-0.4.4/copydetect/detector.py
--rw-r--r--   0 bryson    (1000) bryson    (1000)      928 2022-05-15 19:40:01.000000 copydetect-0.4.4/copydetect/pywinnow.py
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8342 2022-11-12 00:10:46.000000 copydetect-0.4.4/copydetect/utils.py
-drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-02-04 17:05:53.283332 copydetect-0.4.4/copydetect.egg-info/
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     8631 2023-02-04 17:05:53.000000 copydetect-0.4.4/copydetect.egg-info/PKG-INFO
--rw-rw-r--   0 bryson    (1000) bryson    (1000)      395 2023-02-04 17:05:53.000000 copydetect-0.4.4/copydetect.egg-info/SOURCES.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)        1 2023-02-04 17:05:53.000000 copydetect-0.4.4/copydetect.egg-info/dependency_links.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       56 2023-02-04 17:05:53.000000 copydetect-0.4.4/copydetect.egg-info/entry_points.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-02-04 17:05:53.000000 copydetect-0.4.4/copydetect.egg-info/requires.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       11 2023-02-04 17:05:53.000000 copydetect-0.4.4/copydetect.egg-info/top_level.txt
--rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-02-04 17:05:53.283332 copydetect-0.4.4/setup.cfg
--rw-rw-r--   0 bryson    (1000) bryson    (1000)     1588 2023-02-04 16:59:27.000000 copydetect-0.4.4/setup.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.280610 copydetect-0.4.5/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     1063 2020-10-17 00:41:54.000000 copydetect-0.4.5/LICENSE
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8631 2023-04-26 03:30:22.280610 copydetect-0.4.5/PKG-INFO
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     7839 2023-04-26 03:15:29.000000 copydetect-0.4.5/README.md
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       90 2023-04-26 03:20:41.000000 copydetect-0.4.5/copydetect/__init__.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     6031 2023-04-26 03:15:29.000000 copydetect-0.4.5/copydetect/__main__.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect/data/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     2907 2023-04-26 03:15:29.000000 copydetect-0.4.5/copydetect/data/report.html
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       71 2022-05-29 22:08:04.000000 copydetect-0.4.5/copydetect/defaults.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)    28649 2023-04-26 03:21:43.000000 copydetect-0.4.5/copydetect/detector.py
+-rw-r--r--   0 bryson    (1000) bryson    (1000)      928 2022-05-15 19:40:01.000000 copydetect-0.4.5/copydetect/pywinnow.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8342 2022-11-12 00:10:46.000000 copydetect-0.4.5/copydetect/utils.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect/winnow/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     3046 2020-10-17 00:41:54.000000 copydetect-0.4.5/copydetect/winnow/winnow.c
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/copydetect.egg-info/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8631 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/PKG-INFO
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)      543 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)        1 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       56 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/entry_points.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/requires.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       11 2023-04-26 03:30:22.000000 copydetect-0.4.5/copydetect.egg-info/top_level.txt
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)       38 2023-04-26 03:30:22.280610 copydetect-0.4.5/setup.cfg
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     1588 2023-04-26 03:29:32.000000 copydetect-0.4.5/setup.py
+drwxrwxr-x   0 bryson    (1000) bryson    (1000)        0 2023-04-26 03:30:22.276610 copydetect-0.4.5/tests/
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8689 2023-04-25 02:05:20.000000 copydetect-0.4.5/tests/test_detector.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     2252 2020-10-22 01:47:17.000000 copydetect-0.4.5/tests/test_pywinnowing.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     1069 2022-07-16 17:40:53.000000 copydetect-0.4.5/tests/test_sanity_checks.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     8314 2023-03-25 21:00:07.000000 copydetect-0.4.5/tests/test_utils.py
+-rw-rw-r--   0 bryson    (1000) bryson    (1000)     2718 2020-10-22 01:47:17.000000 copydetect-0.4.5/tests/test_winnowing.py
```

### Comparing `copydetect-0.4.4/LICENSE` & `copydetect-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.4/PKG-INFO` & `copydetect-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copydetect
-Version: 0.4.4
+Version: 0.4.5
 Summary: Code plagiarism detection tool
 Home-page: https://github.com/blingenf/copydetect
 Author: Bryson Lingenfelter
 Author-email: blingenfelter@nevada.unr.edu
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `copydetect-0.4.4/README.md` & `copydetect-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.4/copydetect/__main__.py` & `copydetect-0.4.5/copydetect/__main__.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.4/copydetect/data/report.html` & `copydetect-0.4.5/copydetect/data/report.html`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.4/copydetect/detector.py` & `copydetect-0.4.5/copydetect/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,24 +405,27 @@
     def _get_file_list(self, dirs, exts):
         """Recursively collects list of files from provided
         directories. Used to search test_dirs, ref_dirs, and
         boilerplate_dirs
         """
         file_list = []
         for dir in dirs:
+            print_warning = True
             for ext in exts:
                 if ext == "*":
                     matched_contents = Path(dir).rglob("*")
                 else:
                     matched_contents = Path(dir).rglob("*."+ext.lstrip("."))
                 files = [str(f) for f in matched_contents if f.is_file()]
 
-                if len(files) == 0:
-                    logging.warning("No files found in " + dir)
+                if len(files) > 0:
+                    print_warning = False
                 file_list.extend(files)
+            if print_warning:
+                logging.warning("No files found in " + dir)
 
         # convert to a set to remove duplicates, then back to a list
         return list(set(file_list))
 
     def add_file(self, filename, type="testref"):
         """Adds a file to the list of test files, reference files, or
         boilerplate files.
@@ -530,15 +533,15 @@
                     sim2, sim1 = self.similarity_matrix[ref_idx, test_idx]
                 else:
                     overlap, (sim1, sim2), (slices1, slices2) = compare_files(
                         self.file_data[test_f], self.file_data[ref_f]
                     )
                     comparisons[(test_f, ref_f)] = (i, j)
                     if slices1.shape[0] != 0:
-                        self.slice_matrix[(i, j)] = [slices1, slices2]
+                        self.slice_matrix[(test_f, ref_f)] = [slices1, slices2]
 
                 self.similarity_matrix[i, j] = np.array([sim1, sim2])
                 self.token_overlap_matrix[i, j] = overlap
 
         if not self.silent:
             print(f"{time.time()-start_time:6.2f}: Code comparison completed")
 
@@ -587,20 +590,20 @@
             if (ref_f, test_f) in file_pairs:
                 # if comparison is already in report, don't add it again
                 continue
             file_pairs.add((test_f, ref_f))
 
             test_sim = self.similarity_matrix[x[idx], y[idx], 0]
             ref_sim = self.similarity_matrix[x[idx], y[idx], 1]
-            if (x[idx], y[idx]) in self.slice_matrix:
-                slices_test = self.slice_matrix[(x[idx], y[idx])][0]
-                slices_ref = self.slice_matrix[(x[idx], y[idx])][1]
+            if (test_f, ref_f) in self.slice_matrix:
+                slices_test = self.slice_matrix[(test_f, ref_f)][0]
+                slices_ref = self.slice_matrix[(test_f, ref_f)][1]
             else:
-                slices_test = self.slice_matrix[(y[idx], x[idx])][1]
-                slices_ref = self.slice_matrix[(y[idx], x[idx])][0]
+                slices_test = self.slice_matrix[(ref_f, test_f)][1]
+                slices_ref = self.slice_matrix[(ref_f, test_f)][0]
 
             if self.truncate:
                 truncate = 10
             else:
                 truncate = -1
             hl_code_1, _ = highlight_overlap(
                 self.file_data[test_f].raw_code, slices_test,
```

### Comparing `copydetect-0.4.4/copydetect/pywinnow.py` & `copydetect-0.4.5/copydetect/pywinnow.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.4/copydetect/utils.py` & `copydetect-0.4.5/copydetect/utils.py`

 * *Files identical despite different names*

### Comparing `copydetect-0.4.4/copydetect.egg-info/PKG-INFO` & `copydetect-0.4.5/copydetect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copydetect
-Version: 0.4.4
+Version: 0.4.5
 Summary: Code plagiarism detection tool
 Home-page: https://github.com/blingenf/copydetect
 Author: Bryson Lingenfelter
 Author-email: blingenfelter@nevada.unr.edu
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `copydetect-0.4.4/setup.py` & `copydetect-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # the C extension is not currently built for versions uploaded to PyPI.
 # Speedup is not meaningful and it makes cross-platform support quite
 # a bit more painful
 
 setup(name="copydetect",
       author="Bryson Lingenfelter",
       author_email="blingenfelter@nevada.unr.edu",
-      version="0.4.4",
+      version="0.4.5",
       description="Code plagiarism detection tool",
       long_description=readme,
       long_description_content_type="text/markdown",
       url="https://github.com/blingenf/copydetect",
       packages=["copydetect"],
       #ext_modules=[Extension("copydetect.winnow",
       #                       sources=["copydetect/winnow/winnow.c"],
```

