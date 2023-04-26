# Comparing `tmp/fchroot-1.0.1.tar.gz` & `tmp/fchroot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fchroot-1.0.1.tar", last modified: Wed Mar  8 22:53:26 2023, max compression
+gzip compressed data, was "dist/fchroot-1.0.2.tar", last modified: Wed Apr 26 20:47:38 2023, max compression
```

## Comparing `fchroot-1.0.1.tar` & `fchroot-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-03-08 22:53:26.000000 fchroot-1.0.1/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       66 2022-04-21 19:42:55.000000 fchroot-1.0.1/.gitattributes
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2022-05-20 02:07:28.000000 fchroot-1.0.1/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       20 2022-07-26 22:11:05.000000 fchroot-1.0.1/CODENAME
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      579 2022-04-21 20:05:54.000000 fchroot-1.0.1/COPYRIGHT.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6435 2023-03-08 22:53:26.000000 fchroot-1.0.1/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5987 2022-04-21 19:42:55.000000 fchroot-1.0.1/README.md
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-03-08 22:52:40.000000 fchroot-1.0.1/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-03-08 22:53:26.000000 fchroot-1.0.1/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1145 2022-04-21 19:42:55.000000 fchroot-1.0.1/bin/binfmt-helper
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     7017 2022-07-26 22:11:05.000000 fchroot-1.0.1/bin/fchroot
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      404 2022-05-19 21:44:29.000000 fchroot-1.0.1/bin/magic-reader
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      670 2022-04-21 19:42:55.000000 fchroot-1.0.1/bin/wrapper-builder
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-03-08 22:53:26.000000 fchroot-1.0.1/fchroot/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-22 04:27:05.000000 fchroot-1.0.1/fchroot/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7187 2022-07-26 22:11:05.000000 fchroot-1.0.1/fchroot/binfmt.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4540 2023-03-08 22:52:56.000000 fchroot-1.0.1/fchroot/common.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       59 2023-03-08 22:53:22.000000 fchroot-1.0.1/fchroot/version.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-03-08 22:53:26.000000 fchroot-1.0.1/fchroot.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6435 2023-03-08 22:53:26.000000 fchroot-1.0.1/fchroot.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      382 2023-03-08 22:53:26.000000 fchroot-1.0.1/fchroot.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-03-08 22:53:26.000000 fchroot-1.0.1/fchroot.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        8 2023-03-08 22:53:26.000000 fchroot-1.0.1/fchroot.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      692 2022-07-26 22:11:05.000000 fchroot-1.0.1/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-03-08 22:53:26.000000 fchroot-1.0.1/man/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1371 2022-04-22 04:27:05.000000 fchroot-1.0.1/man/fchroot.1.rst.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-03-08 22:53:26.000000 fchroot-1.0.1/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      714 2023-03-08 22:53:22.000000 fchroot-1.0.1/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      720 2022-07-26 22:11:05.000000 fchroot-1.0.1/setup.py.in
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-26 20:47:38.000000 fchroot-1.0.2/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       66 2022-04-21 19:42:55.000000 fchroot-1.0.2/.gitattributes
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2022-05-20 02:07:28.000000 fchroot-1.0.2/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       20 2022-07-26 22:11:05.000000 fchroot-1.0.2/CODENAME
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      579 2022-04-21 20:05:54.000000 fchroot-1.0.2/COPYRIGHT.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6435 2023-04-26 20:47:38.000000 fchroot-1.0.2/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5987 2022-04-21 19:42:55.000000 fchroot-1.0.2/README.md
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-04-26 20:47:20.000000 fchroot-1.0.2/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-26 20:47:38.000000 fchroot-1.0.2/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1145 2022-04-21 19:42:55.000000 fchroot-1.0.2/bin/binfmt-helper
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     7017 2022-07-26 22:11:05.000000 fchroot-1.0.2/bin/fchroot
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      404 2022-05-19 21:44:29.000000 fchroot-1.0.2/bin/magic-reader
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      670 2022-04-21 19:42:55.000000 fchroot-1.0.2/bin/wrapper-builder
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-26 20:47:38.000000 fchroot-1.0.2/fchroot/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-22 04:27:05.000000 fchroot-1.0.2/fchroot/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7187 2022-07-26 22:11:05.000000 fchroot-1.0.2/fchroot/binfmt.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4805 2023-04-25 17:02:55.000000 fchroot-1.0.2/fchroot/common.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       59 2023-04-26 20:47:33.000000 fchroot-1.0.2/fchroot/version.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-26 20:47:38.000000 fchroot-1.0.2/fchroot.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6435 2023-04-26 20:47:37.000000 fchroot-1.0.2/fchroot.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      382 2023-04-26 20:47:37.000000 fchroot-1.0.2/fchroot.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-04-26 20:47:37.000000 fchroot-1.0.2/fchroot.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        8 2023-04-26 20:47:37.000000 fchroot-1.0.2/fchroot.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      692 2022-07-26 22:11:05.000000 fchroot-1.0.2/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-26 20:47:38.000000 fchroot-1.0.2/man/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1371 2022-04-22 04:27:05.000000 fchroot-1.0.2/man/fchroot.1.rst.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-04-26 20:47:38.000000 fchroot-1.0.2/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      714 2023-04-26 20:47:33.000000 fchroot-1.0.2/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      720 2022-07-26 22:11:05.000000 fchroot-1.0.2/setup.py.in
```

### Comparing `fchroot-1.0.1/COPYRIGHT.txt` & `fchroot-1.0.2/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/PKG-INFO` & `fchroot-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fchroot
-Version: 1.0.1
+Version: 1.0.2
 Summary: Funtoo franken-chroot tool.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/fchroot/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `fchroot-1.0.1/README.md` & `fchroot-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/bin/binfmt-helper` & `fchroot-1.0.2/bin/binfmt-helper`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/bin/fchroot` & `fchroot-1.0.2/bin/fchroot`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/bin/wrapper-builder` & `fchroot-1.0.2/bin/wrapper-builder`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/fchroot/binfmt.py` & `fchroot-1.0.2/fchroot/binfmt.py`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/fchroot/common.py` & `fchroot-1.0.2/fchroot/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     for recurse, bind_groups in (True, global_binds), (False, local_binds):
         for dest, src in bind_groups.items():
             dest = dest.lstrip("/")
             dest_abs = os.path.join(chroot_path, dest)
             if umount:
                 action = "umount"
-                mount_cmd = ["/bin/umount", "-R", dest_abs]
+                mount_cmd = ["/bin/umount", "-R", "--lazy", dest_abs]
                 badval = 10
             else:
                 action = "mount"
                 if not os.path.isdir(dest_abs):
                     die(f"Required chroot directory '{dest_abs}' does not exist. Exiting.")
                 if recurse:
                     bindopt = "--rbind"
@@ -117,8 +117,14 @@
                     bindopt = "--bind"
                 mount_cmd = ["/bin/mount", bindopt, f"/{src}", dest_abs]
                 badval = None
             if action == "mount" and os.path.ismount(dest_abs):
                 sys.stderr.write(GREEN + f" {action}: /{dest} (already mounted)\n")
             else:
                 run_verbose(action, mount_cmd, badval=badval)
+                if not umount:
+                    if recurse:
+                        opt = "--make-rprivate"
+                    else:
+                        opt = "--make-private"
+                    run_verbose(action, ["/bin/mount", opt, dest_abs])
```

### Comparing `fchroot-1.0.1/fchroot.egg-info/PKG-INFO` & `fchroot-1.0.2/fchroot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fchroot
-Version: 1.0.1
+Version: 1.0.2
 Summary: Funtoo franken-chroot tool.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/fchroot/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `fchroot-1.0.1/make.sh` & `fchroot-1.0.2/make.sh`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/man/fchroot.1.rst.in` & `fchroot-1.0.2/man/fchroot.1.rst.in`

 * *Files identical despite different names*

### Comparing `fchroot-1.0.1/setup.py` & `fchroot-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fchroot",
-    version="1.0.1",
+    version="1.0.2",
     author="Daniel Robbins",
     author_email="drobbins@funtoo.org",
     description="Funtoo franken-chroot tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://code.funtoo.org/bitbucket/users/drobbins/repos/fchroot/browse",
     scripts=['bin/fchroot'],
```

### Comparing `fchroot-1.0.1/setup.py.in` & `fchroot-1.0.2/setup.py.in`

 * *Files identical despite different names*

