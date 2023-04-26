# Comparing `tmp/casanova-1.8.0a1.tar.gz` & `tmp/casanova-1.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/casanova-1.8.0a1.tar", last modified: Mon Apr  3 08:40:58 2023, max compression
+gzip compressed data, was "dist/casanova-1.8.0a2.tar", last modified: Wed Apr  5 09:51:48 2023, max compression
```

## Comparing `casanova-1.8.0a1.tar` & `casanova-1.8.0a2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-03 08:40:58.000000 casanova-1.8.0a1/
--rw-r--r--   0 Yomgui     (501) staff       (20)    36933 2023-04-03 08:40:58.000000 casanova-1.8.0a1/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)    30111 2023-03-27 12:52:48.000000 casanova-1.8.0a1/README.md
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova/
--rw-r--r--   0 Yomgui     (501) staff       (20)     1211 2023-03-27 12:42:01.000000 casanova-1.8.0a1/casanova/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    12735 2023-04-01 19:51:02.000000 casanova-1.8.0a1/casanova/__main__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    13676 2023-04-01 20:09:13.000000 casanova-1.8.0a1/casanova/cli.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3298 2023-02-15 19:50:58.000000 casanova-1.8.0a1/casanova/contiguous_range_set.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     2090 2023-02-27 08:37:06.000000 casanova-1.8.0a1/casanova/defaults.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     8020 2023-03-24 15:04:16.000000 casanova-1.8.0a1/casanova/enricher.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1652 2023-02-27 12:19:46.000000 casanova-1.8.0a1/casanova/exceptions.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    16577 2023-03-27 12:47:25.000000 casanova-1.8.0a1/casanova/headers.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1227 2023-02-24 20:55:02.000000 casanova-1.8.0a1/casanova/http.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    10161 2023-03-09 09:58:36.000000 casanova-1.8.0a1/casanova/namedrecord.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      450 2023-02-27 11:54:09.000000 casanova-1.8.0a1/casanova/ndjson.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    14525 2023-03-03 18:58:41.000000 casanova-1.8.0a1/casanova/reader.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     7415 2023-02-24 20:55:02.000000 casanova-1.8.0a1/casanova/resumers.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3024 2023-02-16 09:15:22.000000 casanova-1.8.0a1/casanova/reverse_reader.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     2874 2023-03-06 10:27:39.000000 casanova-1.8.0a1/casanova/serialization.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     7430 2023-04-01 11:02:05.000000 casanova-1.8.0a1/casanova/utils.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     4168 2023-03-11 16:53:03.000000 casanova-1.8.0a1/casanova/writer.py
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/
--rw-r--r--   0 Yomgui     (501) staff       (20)    36933 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)      675 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/SOURCES.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/dependency_links.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       83 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/entry_points.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)      114 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/requires.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       17 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/top_level.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-04-03 08:40:58.000000 casanova-1.8.0a1/casanova.egg-info/zip-safe
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-04-03 08:40:58.000000 casanova-1.8.0a1/scripts/
--rw-r--r--   0 Yomgui     (501) staff       (20)        0 2023-02-24 20:55:02.000000 casanova-1.8.0a1/scripts/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      198 2023-02-24 20:55:02.000000 casanova-1.8.0a1/scripts/http.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      189 2023-02-15 19:50:58.000000 casanova-1.8.0a1/scripts/null_byte_writer_error.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-04-03 08:40:58.000000 casanova-1.8.0a1/setup.cfg
--rw-r--r--   0 Yomgui     (501) staff       (20)     1016 2023-04-03 08:40:31.000000 casanova-1.8.0a1/setup.py
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    36933 2023-04-05 09:51:48.000000 casanova-1.8.0a2/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    30111 2023-03-28 09:04:58.000000 casanova-1.8.0a2/README.md
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1211 2023-03-28 09:04:58.000000 casanova-1.8.0a2/casanova/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    12958 2023-04-05 09:22:51.000000 casanova-1.8.0a2/casanova/__main__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    14278 2023-04-05 09:27:15.000000 casanova-1.8.0a2/casanova/cli.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3298 2023-02-14 10:56:01.000000 casanova-1.8.0a2/casanova/contiguous_range_set.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2090 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/defaults.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     8020 2023-03-28 09:04:58.000000 casanova-1.8.0a2/casanova/enricher.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1652 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/exceptions.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    16577 2023-03-28 09:04:58.000000 casanova-1.8.0a2/casanova/headers.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1227 2023-02-24 13:49:12.000000 casanova-1.8.0a2/casanova/http.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    10161 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/namedrecord.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      450 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/ndjson.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    14525 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/reader.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7415 2023-02-24 12:30:01.000000 casanova-1.8.0a2/casanova/resumers.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3024 2023-02-17 09:45:23.000000 casanova-1.8.0a2/casanova/reverse_reader.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2874 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/serialization.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     7430 2023-03-31 13:21:46.000000 casanova-1.8.0a2/casanova/utils.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     4168 2023-03-15 09:15:31.000000 casanova-1.8.0a2/casanova/writer.py
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    36933 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/PKG-INFO
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      675 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/SOURCES.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/dependency_links.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       83 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/entry_points.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      114 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/requires.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       17 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/top_level.txt
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2023-04-05 09:51:48.000000 casanova-1.8.0a2/casanova.egg-info/zip-safe
+drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-04-05 09:51:48.000000 casanova-1.8.0a2/scripts/
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        0 2023-02-24 12:50:33.000000 casanova-1.8.0a2/scripts/__init__.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      198 2023-02-24 13:49:12.000000 casanova-1.8.0a2/scripts/http.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      189 2023-02-15 10:13:26.000000 casanova-1.8.0a2/scripts/null_byte_writer_error.py
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2023-04-05 09:51:48.000000 casanova-1.8.0a2/setup.cfg
+-rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1016 2023-04-05 09:51:28.000000 casanova-1.8.0a2/setup.py
```

### Comparing `casanova-1.8.0a1/PKG-INFO` & `casanova-1.8.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanova
-Version: 1.8.0a1
+Version: 1.8.0a2
 Summary: Specialized & performant CSV readers, writers and enrichers for python.
 Home-page: http://github.com/medialab/casanova
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/casanova/workflows/Tests/badge.svg)](https://github.com/medialab/casanova/actions)
```

### Comparing `casanova-1.8.0a1/README.md` & `casanova-1.8.0a2/README.md`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/__init__.py` & `casanova-1.8.0a2/casanova/__init__.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/__main__.py` & `casanova-1.8.0a2/casanova/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,35 +258,35 @@
     subparsers = parser.add_subparsers(dest="action", help="Command to execute.")
 
     map_parser = subparsers.add_parser("map", formatter_class=custom_formatter)
     add_common_arguments(map_parser)
     add_mp_arguments(map_parser)
     add_serialization_arguments(map_parser)
     map_parser.add_argument(
-        "new_column",
-        help="Name of the new column to create & containing the result of the evaluated code.",
+        "code", help="Python code to evaluate for each row of the CSV file."
     )
     map_parser.add_argument(
-        "code", help="Python code to evaluate for each row of the CSV file."
+        "new_column",
+        help="Name of the new column to create & containing the result of the evaluated code.",
     )
     map_parser.add_argument(
         "file",
         help="CSV file to map. Can be gzip-compressed, and can also be a URL. Will consider `-` as stdin.",
     )
 
     flatmap_parser = subparsers.add_parser("flatmap", formatter_class=custom_formatter)
     add_common_arguments(flatmap_parser)
     add_mp_arguments(flatmap_parser)
     add_serialization_arguments(flatmap_parser)
     flatmap_parser.add_argument(
-        "new_column",
-        help="Name of the new column to create & containing the result of the evaluated code.",
+        "code", help="Python code to evaluate for each row of the CSV file."
     )
     flatmap_parser.add_argument(
-        "code", help="Python code to evaluate for each row of the CSV file."
+        "new_column",
+        help="Name of the new column to create & containing the result of the evaluated code.",
     )
     flatmap_parser.add_argument(
         "file",
         help="CSV file to flatmap. Can be gzip-compressed, and can also be a URL. Will consider `-` as stdin.",
     )
 
     filter_parser = subparsers.add_parser("filter", formatter_class=custom_formatter)
@@ -319,14 +319,20 @@
         help="CSV file to map-reduce. Can be gzip-compressed, and can also be a URL. Will consider `-` as stdin.",
     )
     map_reduce_parser.add_argument(
         "-V",
         "--init-value",
         help="Python code to evaluate to initialize the accumulator's value. If not given, the initial value will be the first map result.",
     )
+    map_reduce_parser.add_argument(
+        "-f",
+        "--fieldnames",
+        help="Output CSV file fieldnames. Useful when emitting sequences without keys (e.g. lists, tuples etc.).",
+        type=SpliterType(),
+    )
 
     groupby_parser = subparsers.add_parser("groupby", formatter_class=custom_formatter)
     add_common_arguments(groupby_parser)
     add_mp_arguments(groupby_parser)
     add_serialization_arguments(groupby_parser)
     groupby_parser.add_argument(
         "code", help="Python code to evaluate to group each row of the CSV file."
```

### Comparing `casanova-1.8.0a1/casanova/cli.py` & `casanova-1.8.0a2/casanova/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -381,17 +381,26 @@
             if isinstance(final_result, Mapping):
                 fieldnames = list(final_result.keys())
                 writer.writerow(fieldnames)
                 writer.writerow(serializer.serialize_dict_row(final_result, fieldnames))
             elif isinstance(final_result, Iterable) and not isinstance(
                 final_result, (bytes, str)
             ):
-                writer.writerow(serializer.serialize_row(final_result))
+                serialized = serializer.serialize_row(final_result)
+                if cli_args.fieldnames:
+                    writer.writerow(cli_args.fieldnames)
+                else:
+                    writer.writerow(
+                        ["col%i" % i for i in range(1, len(serialized) + 1)]
+                    )
+                writer.writerow(serialized)
             else:
-                writer.writerow(fieldnames)
+                writer.writerow(
+                    fieldnames if cli_args.fieldnames is None else cli_args.fieldnames
+                )
                 writer.writerow(serializer(final_result))
 
         else:
             print(final_result, file=output_file)
 
 
 class GroupWrapper:
@@ -475,14 +484,19 @@
                     writer.writerow(fieldnames)
                     header_emitted = True
 
                 writer.writerow(
                     [name] + serializer.serialize_dict_row(result, mapping_fieldnames)
                 )
             elif isinstance(result, Iterable) and not isinstance(result, (bytes, str)):
+                if not header_emitted:
+                    fieldnames += ["col%i" % i for i in range(1, len(result) + 1)]
+                    writer.writerow(fieldnames)
+                    header_emitted = True
+
                 writer.writerow([name] + serializer.serialize_row(result))
             else:
                 if not header_emitted:
                     writer.writerow(fieldnames + ["value"])
                     header_emitted = True
                 writer.writerow([name, serializer(result)])
```

### Comparing `casanova-1.8.0a1/casanova/contiguous_range_set.py` & `casanova-1.8.0a2/casanova/contiguous_range_set.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/defaults.py` & `casanova-1.8.0a2/casanova/defaults.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/enricher.py` & `casanova-1.8.0a2/casanova/enricher.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/exceptions.py` & `casanova-1.8.0a2/casanova/exceptions.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/headers.py` & `casanova-1.8.0a2/casanova/headers.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/http.py` & `casanova-1.8.0a2/casanova/http.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/namedrecord.py` & `casanova-1.8.0a2/casanova/namedrecord.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/reader.py` & `casanova-1.8.0a2/casanova/reader.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/resumers.py` & `casanova-1.8.0a2/casanova/resumers.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/reverse_reader.py` & `casanova-1.8.0a2/casanova/reverse_reader.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/serialization.py` & `casanova-1.8.0a2/casanova/serialization.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/utils.py` & `casanova-1.8.0a2/casanova/utils.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova/writer.py` & `casanova-1.8.0a2/casanova/writer.py`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/casanova.egg-info/PKG-INFO` & `casanova-1.8.0a2/casanova.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casanova
-Version: 1.8.0a1
+Version: 1.8.0a2
 Summary: Specialized & performant CSV readers, writers and enrichers for python.
 Home-page: http://github.com/medialab/casanova
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/casanova/workflows/Tests/badge.svg)](https://github.com/medialab/casanova/actions)
```

### Comparing `casanova-1.8.0a1/casanova.egg-info/SOURCES.txt` & `casanova-1.8.0a2/casanova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casanova-1.8.0a1/setup.py` & `casanova-1.8.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="casanova",
-    version="1.8.0-a1",
+    version="1.8.0-a2",
     description="Specialized & performant CSV readers, writers and enrichers for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/casanova",
     license="MIT",
     author="Guillaume Plique",
     author_email="kropotkinepiotr@gmail.com",
```

