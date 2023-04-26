# Comparing `tmp/CloudyDaze-1.3.tar.gz` & `tmp/CloudyDaze-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CloudyDaze-1.3.tar", last modified: Mon Nov 14 03:27:46 2022, max compression
+gzip compressed data, was "CloudyDaze-1.4.tar", last modified: Wed Apr 26 00:55:10 2023, max compression
```

## Comparing `CloudyDaze-1.3.tar` & `CloudyDaze-1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-11-14 03:27:46.711571 CloudyDaze-1.3/
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-11-14 03:27:46.703868 CloudyDaze-1.3/CloudyDaze/
--rw-r--r--   0 dave       (501) staff       (20)     1015 2021-08-08 23:42:06.000000 CloudyDaze-1.3/CloudyDaze/MyAWS.py
--rw-r--r--   0 dave       (501) staff       (20)     2940 2021-08-08 23:42:06.000000 CloudyDaze-1.3/CloudyDaze/MyEC2.py
--rw-r--r--   0 dave       (501) staff       (20)    16340 2021-08-08 23:42:06.000000 CloudyDaze-1.3/CloudyDaze/MySCP.py
--rw-r--r--   0 dave       (501) staff       (20)     4775 2022-11-14 02:59:45.000000 CloudyDaze-1.3/CloudyDaze/MySG.py
--rw-r--r--   0 dave       (501) staff       (20)     2697 2021-08-08 23:42:06.000000 CloudyDaze-1.3/CloudyDaze/MySSH.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-11-14 03:27:46.708109 CloudyDaze-1.3/CloudyDaze.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)     3520 2022-11-14 03:27:46.000000 CloudyDaze-1.3/CloudyDaze.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      347 2022-11-14 03:27:46.000000 CloudyDaze-1.3/CloudyDaze.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2022-11-14 03:27:46.000000 CloudyDaze-1.3/CloudyDaze.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)      100 2022-11-14 03:27:46.000000 CloudyDaze-1.3/CloudyDaze.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       11 2022-11-14 03:27:46.000000 CloudyDaze-1.3/CloudyDaze.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)     3520 2022-11-14 03:27:46.711739 CloudyDaze-1.3/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     3241 2021-08-08 23:42:06.000000 CloudyDaze-1.3/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2022-11-14 03:27:46.710919 CloudyDaze-1.3/bin/
--rwxr-xr-x   0 dave       (501) staff       (20)      143 2021-08-08 23:42:06.000000 CloudyDaze-1.3/bin/myEC2.py
--rwxr-xr-x   0 dave       (501) staff       (20)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.3/bin/mySCP.py
--rwxr-xr-x   0 dave       (501) staff       (20)      183 2022-11-14 03:01:14.000000 CloudyDaze-1.3/bin/mySG.py
--rwxr-xr-x   0 dave       (501) staff       (20)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.3/bin/mySSH.py
--rw-r--r--   0 dave       (501) staff       (20)       79 2022-11-14 03:27:46.713740 CloudyDaze-1.3/setup.cfg
--rwxr-xr-x   0 dave       (501) staff       (20)      892 2022-11-14 03:27:30.000000 CloudyDaze-1.3/setup.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.224612 CloudyDaze-1.4/
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.209612 CloudyDaze-1.4/CloudyDaze/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1015 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MyAWS.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     2940 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MyEC2.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)    16340 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MySCP.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     4834 2023-04-26 00:52:57.000000 CloudyDaze-1.4/CloudyDaze/MySG.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     2697 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MySSH.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.217612 CloudyDaze-1.4/CloudyDaze.egg-info/
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)     3557 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/PKG-INFO
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)      347 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/SOURCES.txt
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)        1 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/dependency_links.txt
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)      100 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/requires.txt
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)       11 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/top_level.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3557 2023-04-26 00:55:10.225612 CloudyDaze-1.4/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3241 2022-11-14 06:55:17.000000 CloudyDaze-1.4/README.md
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.223612 CloudyDaze-1.4/bin/
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)      143 2021-08-08 23:42:06.000000 CloudyDaze-1.4/bin/myEC2.py
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.4/bin/mySCP.py
+-rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)      183 2022-11-14 06:55:17.000000 CloudyDaze-1.4/bin/mySG.py
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.4/bin/mySSH.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-04-26 00:55:10.225612 CloudyDaze-1.4/setup.cfg
+-rwxrwx---   0 eddo8    (197610) eddo8    (197610)      892 2023-04-26 00:53:46.000000 CloudyDaze-1.4/setup.py
```

### Comparing `CloudyDaze-1.3/CloudyDaze/MyAWS.py` & `CloudyDaze-1.4/CloudyDaze/MyAWS.py`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.3/CloudyDaze/MyEC2.py` & `CloudyDaze-1.4/CloudyDaze/MyEC2.py`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.3/CloudyDaze/MySCP.py` & `CloudyDaze-1.4/CloudyDaze/MySCP.py`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.3/CloudyDaze/MySG.py` & `CloudyDaze-1.4/CloudyDaze/MySG.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 	ports = {
 		22: 'tcp',
 		1521: 'tcp',
 		1883: 'tcp',
 		3389: 'tcp',
 		8888: 'tcp',
+		9999: 'tcp',
 	}
 	
 	types=[
 		'tcp',
 		'udp',
 		'icmp',
 		-1
@@ -191,9 +192,11 @@
 	@args.parameter(name='ips', nargs='*', short='i')
 	@args.parameter(name='forall', short='a', flag=True, help='revoke all')
 	def replace(self, ips=[], forall=False):
 		result = dict()
 		result['revoked'] = self.revoke(ips, forall)
 		result['enabled'] = self.enable(ips)
 		return result
-		
-	
+
+				
+if __name__ == '__main__': args.execute()
+
```

### Comparing `CloudyDaze-1.3/CloudyDaze/MySSH.py` & `CloudyDaze-1.4/CloudyDaze/MySSH.py`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.3/CloudyDaze.egg-info/PKG-INFO` & `CloudyDaze-1.4/CloudyDaze.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: CloudyDaze
-Version: 1.3
+Version: 1.4
+Summary: UNKNOWN
 Home-page: https://github.com/eddo888/CloudyDaze
-Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.3.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
+Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.4.tar.gz
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # CloudyDaze
 
 bunch of usefull scripts for managing your cloud
 
 please note that these use the most excellent credstash library for python,
@@ -135,7 +137,9 @@
   -v, --verbose         verbose logging
 ```
 
 ---
 ## acknowledgements
 
 code graciously borrowed from [StaSh for Pythonista](https://github.com/ywangd/stash)
+
+
```

### Comparing `CloudyDaze-1.3/PKG-INFO` & `CloudyDaze-1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: CloudyDaze
-Version: 1.3
+Version: 1.4
+Summary: UNKNOWN
 Home-page: https://github.com/eddo888/CloudyDaze
-Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.3.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
+Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.4.tar.gz
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # CloudyDaze
 
 bunch of usefull scripts for managing your cloud
 
 please note that these use the most excellent credstash library for python,
@@ -135,7 +137,9 @@
   -v, --verbose         verbose logging
 ```
 
 ---
 ## acknowledgements
 
 code graciously borrowed from [StaSh for Pythonista](https://github.com/ywangd/stash)
+
+
```

### Comparing `CloudyDaze-1.3/README.md` & `CloudyDaze-1.4/README.md`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.3/setup.py` & `CloudyDaze-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
     long_description = input.read()
 
 name='CloudyDaze'
-version='1.3'
+version='1.4'
 
 setup(
 	name=name,
 	version=version,
 	license='MIT',
 	long_description=long_description,
 	long_description_content_type="text/markdown",
```

