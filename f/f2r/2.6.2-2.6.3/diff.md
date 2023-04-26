# Comparing `tmp/f2r-2.6.2.tar.gz` & `tmp/f2r-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f2r-2.6.2.tar", last modified: Wed Apr  5 13:01:37 2023, max compression
+gzip compressed data, was "f2r-2.6.3.tar", last modified: Wed Apr 26 13:07:03 2023, max compression
```

## Comparing `f2r-2.6.2.tar` & `f2r-2.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)        0 2023-04-05 13:01:37.128030 f2r-2.6.2/
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)    35141 2021-06-11 10:11:11.000000 f2r-2.6.2/COPYING
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     2813 2023-04-05 13:01:37.128030 f2r-2.6.2/PKG-INFO
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     2214 2021-06-11 10:11:11.000000 f2r-2.6.2/README.md
--rwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)     7469 2022-03-24 13:17:21.000000 f2r-2.6.2/f2r
-drwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)        0 2023-04-05 13:01:37.123030 f2r-2.6.2/f2r.egg-info/
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     2813 2023-04-05 13:01:36.000000 f2r-2.6.2/f2r.egg-info/PKG-INFO
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      490 2023-04-05 13:01:37.000000 f2r-2.6.2/f2r.egg-info/SOURCES.txt
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)        1 2023-04-05 13:01:36.000000 f2r-2.6.2/f2r.egg-info/dependency_links.txt
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)       34 2023-04-05 13:01:36.000000 f2r-2.6.2/f2r.egg-info/requires.txt
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)        8 2023-04-05 13:01:36.000000 f2r-2.6.2/f2r.egg-info/top_level.txt
-drwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)        0 2023-04-05 13:01:37.128030 f2r-2.6.2/flp2rpm/
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      361 2021-06-11 10:11:11.000000 f2r-2.6.2/flp2rpm/Defaults.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     8759 2022-12-09 13:56:22.000000 f2r-2.6.2/flp2rpm/Fpm.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1548 2021-06-11 10:11:11.000000 f2r-2.6.2/flp2rpm/Module.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     3043 2021-06-25 16:32:51.000000 f2r-2.6.2/flp2rpm/Package.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      558 2021-06-11 10:11:11.000000 f2r-2.6.2/flp2rpm/Repo.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1609 2021-09-15 10:29:30.000000 f2r-2.6.2/flp2rpm/S3.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)       24 2021-06-11 10:11:11.000000 f2r-2.6.2/flp2rpm/__init__.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1577 2023-04-05 13:01:03.000000 f2r-2.6.2/flp2rpm/after_install_template.sh
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      603 2021-06-11 10:11:11.000000 f2r-2.6.2/flp2rpm/after_remove_template.sh
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      314 2023-01-13 10:02:47.000000 f2r-2.6.2/flp2rpm/config.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      731 2021-06-25 16:32:51.000000 f2r-2.6.2/flp2rpm/devel.slc7.yaml
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1040 2023-02-08 13:59:41.000000 f2r-2.6.2/flp2rpm/devel.slc8.yaml
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1728 2021-06-11 10:11:11.000000 f2r-2.6.2/flp2rpm/helpers.py
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      407 2021-06-25 16:32:51.000000 f2r-2.6.2/flp2rpm/runtime.slc7.yaml
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      716 2023-02-08 13:59:41.000000 f2r-2.6.2/flp2rpm/runtime.slc8.yaml
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)       38 2023-04-05 13:01:37.129030 f2r-2.6.2/setup.cfg
--rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1124 2023-04-05 13:01:11.000000 f2r-2.6.2/setup.py
+drwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)        0 2023-04-26 13:07:03.670204 f2r-2.6.3/
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)    35141 2021-06-11 10:11:11.000000 f2r-2.6.3/COPYING
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     2813 2023-04-26 13:07:03.669204 f2r-2.6.3/PKG-INFO
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     2214 2021-06-11 10:11:11.000000 f2r-2.6.3/README.md
+-rwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)     7469 2022-03-24 13:17:21.000000 f2r-2.6.3/f2r
+drwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)        0 2023-04-26 13:07:03.664204 f2r-2.6.3/f2r.egg-info/
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     2813 2023-04-26 13:07:03.000000 f2r-2.6.3/f2r.egg-info/PKG-INFO
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      490 2023-04-26 13:07:03.000000 f2r-2.6.3/f2r.egg-info/SOURCES.txt
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)        1 2023-04-26 13:07:03.000000 f2r-2.6.3/f2r.egg-info/dependency_links.txt
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)       34 2023-04-26 13:07:03.000000 f2r-2.6.3/f2r.egg-info/requires.txt
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)        8 2023-04-26 13:07:03.000000 f2r-2.6.3/f2r.egg-info/top_level.txt
+drwxrwxr-x   0 awegrzyn  (1000) awegrzyn  (1000)        0 2023-04-26 13:07:03.669204 f2r-2.6.3/flp2rpm/
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      361 2021-06-11 10:11:11.000000 f2r-2.6.3/flp2rpm/Defaults.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     8771 2023-04-26 13:06:51.000000 f2r-2.6.3/flp2rpm/Fpm.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1548 2021-06-11 10:11:11.000000 f2r-2.6.3/flp2rpm/Module.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     3043 2021-06-25 16:32:51.000000 f2r-2.6.3/flp2rpm/Package.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      558 2021-06-11 10:11:11.000000 f2r-2.6.3/flp2rpm/Repo.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1609 2021-09-15 10:29:30.000000 f2r-2.6.3/flp2rpm/S3.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)       24 2021-06-11 10:11:11.000000 f2r-2.6.3/flp2rpm/__init__.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1647 2023-04-26 13:06:51.000000 f2r-2.6.3/flp2rpm/after_install_template.sh
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      603 2021-06-11 10:11:11.000000 f2r-2.6.3/flp2rpm/after_remove_template.sh
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      314 2023-01-13 10:02:47.000000 f2r-2.6.3/flp2rpm/config.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      731 2021-06-25 16:32:51.000000 f2r-2.6.3/flp2rpm/devel.slc7.yaml
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1040 2023-02-08 13:59:41.000000 f2r-2.6.3/flp2rpm/devel.slc8.yaml
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1728 2021-06-11 10:11:11.000000 f2r-2.6.3/flp2rpm/helpers.py
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      407 2021-06-25 16:32:51.000000 f2r-2.6.3/flp2rpm/runtime.slc7.yaml
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)      716 2023-02-08 13:59:41.000000 f2r-2.6.3/flp2rpm/runtime.slc8.yaml
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)       38 2023-04-26 13:07:03.670204 f2r-2.6.3/setup.cfg
+-rw-rw-r--   0 awegrzyn  (1000) awegrzyn  (1000)     1124 2023-04-26 13:06:51.000000 f2r-2.6.3/setup.py
```

### Comparing `f2r-2.6.2/COPYING` & `f2r-2.6.3/COPYING`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/PKG-INFO` & `f2r-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f2r
-Version: 2.6.2
+Version: 2.6.3
 Summary: Produces RPMs for FLP packages out of aliBuild ouput
 Home-page: https://gitlab.cern.ch/AliceO2Group/flp-to-rpm
 Author: Adam Wegrzynek
 Author-email: adam.wegrzynek@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `f2r-2.6.2/README.md` & `f2r-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/f2r` & `f2r-2.6.3/f2r`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/f2r.egg-info/PKG-INFO` & `f2r-2.6.3/f2r.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f2r
-Version: 2.6.2
+Version: 2.6.3
 Summary: Produces RPMs for FLP packages out of aliBuild ouput
 Home-page: https://gitlab.cern.ch/AliceO2Group/flp-to-rpm
 Author: Adam Wegrzynek
 Author-email: adam.wegrzynek@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `f2r-2.6.2/flp2rpm/Fpm.py` & `f2r-2.6.3/flp2rpm/Fpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     rpmType = 'dir'
     # prep dir arguments
     # `=.` is necessary so that the complete source dir path
     # is not replicated and the target dir consists of only
     # prefix + package name + dir
     package_dir = self.buildDir + "/" + name + "/" + fullVersion + "/"
-    subdirs = ['bin', 'lib', 'lib64', 'etc', 'include', 'bin-safe', 'libexec', 'WebDID', 'share', 'plugins', 'cmake', 'sbin', 'icons', 'fonts']
+    subdirs = ['bin', 'lib', 'lib64', 'etc', 'include', 'bin-safe', 'libexec', 'WebDID', 'share', 'plugins', 'cmake', 'sbin', 'icons', 'fonts', 'response']
     paths = []
     for subdir in subdirs:
         if os.path.exists(package_dir + subdir):
             if subdir == 'etc' and os.listdir(package_dir + subdir) == ['modulefiles', 'profile.d']:
                 continue
             paths.append(package_dir + subdir + '=.')
```

### Comparing `f2r-2.6.2/flp2rpm/Module.py` & `f2r-2.6.3/flp2rpm/Module.py`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/Package.py` & `f2r-2.6.3/flp2rpm/Package.py`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/Repo.py` & `f2r-2.6.3/flp2rpm/Repo.py`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/S3.py` & `f2r-2.6.3/flp2rpm/S3.py`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/after_install_template.sh` & `f2r-2.6.3/flp2rpm/after_install_template.sh`

 * *Files 3% similar despite different names*

```diff
@@ -33,9 +33,10 @@
 
 devel_suffix="devel"
 if [[ "$package" == *"$devel_suffix"* ]]; then
   if [ ! -f $devel_file ]; then
     echo "export LIBRARY_PATH=/opt/o2/lib/" >> $devel_file
     echo "export CPLUS_INCLUDE_PATH=/opt/o2/include/" >> $devel_file
     echo "source /opt/rh/gcc-toolset-12/enable" >> $devel_file
+    echo "export PATH=${package_root}/bin-safe:\$PATH" >> $devel_file
   fi
 fi
```

### Comparing `f2r-2.6.2/flp2rpm/after_remove_template.sh` & `f2r-2.6.3/flp2rpm/after_remove_template.sh`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/devel.slc7.yaml` & `f2r-2.6.3/flp2rpm/devel.slc7.yaml`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/devel.slc8.yaml` & `f2r-2.6.3/flp2rpm/devel.slc8.yaml`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/helpers.py` & `f2r-2.6.3/flp2rpm/helpers.py`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/flp2rpm/runtime.slc8.yaml` & `f2r-2.6.3/flp2rpm/runtime.slc8.yaml`

 * *Files identical despite different names*

### Comparing `f2r-2.6.2/setup.py` & `f2r-2.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='f2r',
-    version='2.6.2',
+    version='2.6.3',
     author='Adam Wegrzynek',
     author_email='adam.wegrzynek@cern.ch',
     url='https://gitlab.cern.ch/AliceO2Group/flp-to-rpm',
     license='GPLv3',
     description='Produces RPMs for FLP packages out of aliBuild ouput',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

