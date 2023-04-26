# Comparing `tmp/zoomaker-0.1.0.tar.gz` & `tmp/zoomaker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.1.0.tar", max compression
+gzip compressed data, was "zoomaker-0.1.1.tar", max compression
```

## Comparing `zoomaker-0.1.0.tar` & `zoomaker-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2516 2023-04-25 10:26:51.821798 zoomaker-0.1.0/README.md
--rw-r--r--   0        0        0      346 2023-04-25 09:40:21.148193 zoomaker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5387 2023-04-25 10:10:44.361691 zoomaker-0.1.0/zoomaker.py
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 zoomaker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2516 2023-04-25 10:26:51.821798 zoomaker-0.1.1/README.md
+-rw-r--r--   0        0        0      346 2023-04-25 12:37:05.238936 zoomaker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5410 2023-04-25 12:36:59.947188 zoomaker-0.1.1/zoomaker.py
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 zoomaker-0.1.1/PKG-INFO
```

### Comparing `zoomaker-0.1.0/README.md` & `zoomaker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zoomaker-0.1.0/zoomaker.py` & `zoomaker-0.1.1/zoomaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,22 @@
                 file.write(data)
         progress_bar.close()
         if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
             print("Error: Failed to download the complete file.")
             return None
         return filename
 
-
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file")
     parser.add_argument("command", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.1.0")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.1.1")
     args = parser.parse_args()
 
     zoomaker = Zoomaker("zoo.yaml")
     if args.command == "install":
         zoomaker.install()
     elif args.command == "run":
         zoomaker.run(args.script)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `zoomaker-0.1.0/PKG-INFO` & `zoomaker-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_x5wywf97_/tmp8msvtlna_TarContainer/0/3", line 116, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_x5wywf97_/tmp8msvtlna_TarContainer/0/3", line 116, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zoomaker Version: 0.1.0 Summary: Author: Benedikt
+Metadata-Version: 2.1 Name: zoomaker Version: 0.1.1 Summary: Author: Benedikt
 GroÃ Requires-Python: >=3.9,<4.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0) Requires-Dist: huggingface-hub
 (>=0.14.0,<0.15.0) Description-Content-Type: text/markdown # Work in progress.
 Please ignore. zoomaker ======== Zoomaker is a command-line tool that helps
 install models, git repositories and run scripts. The information about the
```

