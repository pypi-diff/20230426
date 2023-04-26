# Comparing `tmp/sroll-0.2.9.8.tar.gz` & `tmp/sroll-0.2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sroll-0.2.9.8.tar", last modified: Wed Apr 26 13:40:46 2023, max compression
+gzip compressed data, was "dist/sroll-0.2.9.9.tar", last modified: Wed Apr 26 13:44:19 2023, max compression
```

## Comparing `sroll-0.2.9.8.tar` & `sroll-0.2.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:40:46.000000 sroll-0.2.9.8/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       38 2023-04-26 13:40:46.000000 sroll-0.2.9.8/setup.cfg
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       46 2023-01-26 14:13:59.000000 sroll-0.2.9.8/MANIFEST.in
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      787 2023-04-26 13:40:42.000000 sroll-0.2.9.8/setup.py
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll.egg-info/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)        1 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll.egg-info/dependency_links.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      253 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll.egg-info/SOURCES.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       21 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll.egg-info/requires.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll.egg-info/PKG-INFO
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       14 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll.egg-info/top_level.txt
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll_package/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)     8359 2023-04-26 13:40:27.000000 sroll-0.2.9.8/sroll_package/set_env.py
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      142 2023-01-26 14:13:59.000000 sroll-0.2.9.8/sroll_package/__init__.py
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:40:46.000000 sroll-0.2.9.8/sroll_package/static/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      803 2023-04-26 10:25:01.000000 sroll-0.2.9.8/sroll_package/static/requirements.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-26 13:40:46.000000 sroll-0.2.9.8/PKG-INFO
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:44:19.000000 sroll-0.2.9.9/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       38 2023-04-26 13:44:19.000000 sroll-0.2.9.9/setup.cfg
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       46 2023-01-26 14:13:59.000000 sroll-0.2.9.9/MANIFEST.in
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      787 2023-04-26 13:44:15.000000 sroll-0.2.9.9/setup.py
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll.egg-info/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)        1 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll.egg-info/dependency_links.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      253 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll.egg-info/SOURCES.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       21 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll.egg-info/requires.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll.egg-info/PKG-INFO
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       14 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll.egg-info/top_level.txt
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll_package/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)     8357 2023-04-26 13:43:51.000000 sroll-0.2.9.9/sroll_package/set_env.py
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      142 2023-01-26 14:13:59.000000 sroll-0.2.9.9/sroll_package/__init__.py
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-26 13:44:19.000000 sroll-0.2.9.9/sroll_package/static/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      803 2023-04-26 10:25:01.000000 sroll-0.2.9.9/sroll_package/static/requirements.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-26 13:44:19.000000 sroll-0.2.9.9/PKG-INFO
```

### Comparing `sroll-0.2.9.8/setup.py` & `sroll-0.2.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 
 
 
 setuptools.setup(
     name='sroll',
-    version='0.2.9.8',    
+    version='0.2.9.9',    
     description='Python package for SRoll installation',    
     url='https://gitlab.ifremer.fr/iaocea/srollex.git',
     author='Theo Foulquier',
     author_email='tfoulqui@ifremer.fr',
     license='BSD 2-clause',
     include_package_data = True,
     packages=['sroll_package'],
```

### Comparing `sroll-0.2.9.8/sroll_package/set_env.py` & `sroll-0.2.9.9/sroll_package/set_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   os.system('mkdir -p '+str(vecout))
   
   # Read in the file
   with open(str(path)+"/srollex/sroll4/test"+str(name)+".py", 'r') as file :
     filedata = file.read()
 
   # Replace the target string
-  filedata = filedata.replace('CALL_FOSCAT = ','CALL_FOSCAT = "'str(path)+'"/srollex/sroll4/py_fct_foscat.py')
+  filedata = filedata.replace('CALLFOSCAT = ','CALLFOSCAT = "'str(path)+'"/srollex/sroll4/py_fct_foscat.py')
   filedata = filedata.replace('Out_MAP = ','Out_MAP = ["'+str(mapout)+'Nside%s_%s"%(Nside,i) for i in bolo_map]')
   filedata = filedata.replace('Out_VEC = ','Out_VEC = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_Offset = ','Out_Offset = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_Offset_corr = ','Out_Offset_corr = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_xi2 = ','Out_xi2 = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_xi2_corr = ','Out_xi2_corr = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
```

### Comparing `sroll-0.2.9.8/sroll_package/static/requirements.txt` & `sroll-0.2.9.9/sroll_package/static/requirements.txt`

 * *Files identical despite different names*

