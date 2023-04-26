# Comparing `tmp/SocketWrapper-0.2.2.tar.gz` & `tmp/SocketWrapper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SocketWrapper-0.2.2.tar", last modified: Tue Apr 25 00:20:55 2023, max compression
+gzip compressed data, was "SocketWrapper-0.2.3.tar", last modified: Tue Apr 25 16:06:35 2023, max compression
```

## Comparing `SocketWrapper-0.2.2.tar` & `SocketWrapper-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 00:20:55.056917 SocketWrapper-0.2.2/
--rw-r--r--   0 jarredtd   (501) staff       (20)     1073 2023-04-20 23:18:46.000000 SocketWrapper-0.2.2/LICENSE
--rw-r--r--   0 jarredtd   (501) staff       (20)     2092 2023-04-25 00:20:55.057156 SocketWrapper-0.2.2/PKG-INFO
--rw-r--r--   0 jarredtd   (501) staff       (20)     1516 2023-04-25 00:12:39.000000 SocketWrapper-0.2.2/README.md
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 00:20:55.053839 SocketWrapper-0.2.2/SocketWrapper/
--rw-r--r--   0 jarredtd   (501) staff       (20)     1357 2023-04-25 00:10:43.000000 SocketWrapper-0.2.2/SocketWrapper/Client.py
--rw-r--r--   0 jarredtd   (501) staff       (20)     1329 2023-04-25 00:10:51.000000 SocketWrapper-0.2.2/SocketWrapper/Server.py
--rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 22:24:19.000000 SocketWrapper-0.2.2/SocketWrapper/__init__.py
-drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 00:20:55.056036 SocketWrapper-0.2.2/SocketWrapper.egg-info/
--rw-r--r--   0 jarredtd   (501) staff       (20)     2092 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/PKG-INFO
--rw-r--r--   0 jarredtd   (501) staff       (20)      258 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)        1 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)       14 2023-04-25 00:20:55.000000 SocketWrapper-0.2.2/SocketWrapper.egg-info/top_level.txt
--rw-r--r--   0 jarredtd   (501) staff       (20)       79 2023-04-25 00:20:55.058133 SocketWrapper-0.2.2/setup.cfg
--rw-r--r--   0 jarredtd   (501) staff       (20)     1645 2023-04-25 00:17:23.000000 SocketWrapper-0.2.2/setup.py
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 16:06:35.815349 SocketWrapper-0.2.3/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1073 2023-04-20 23:18:46.000000 SocketWrapper-0.2.3/LICENSE
+-rw-r--r--   0 jarredtd   (501) staff       (20)     2092 2023-04-25 16:06:35.815438 SocketWrapper-0.2.3/PKG-INFO
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1516 2023-04-25 00:12:39.000000 SocketWrapper-0.2.3/README.md
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 16:06:35.814631 SocketWrapper-0.2.3/SocketWrapper/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1357 2023-04-25 00:10:43.000000 SocketWrapper-0.2.3/SocketWrapper/Client.py
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1329 2023-04-25 00:10:51.000000 SocketWrapper-0.2.3/SocketWrapper/Server.py
+-rw-r--r--   0 jarredtd   (501) staff       (20)        0 2023-04-20 22:24:19.000000 SocketWrapper-0.2.3/SocketWrapper/__init__.py
+drwxr-xr-x   0 jarredtd   (501) staff       (20)        0 2023-04-25 16:06:35.815219 SocketWrapper-0.2.3/SocketWrapper.egg-info/
+-rw-r--r--   0 jarredtd   (501) staff       (20)     2092 2023-04-25 16:06:35.000000 SocketWrapper-0.2.3/SocketWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 jarredtd   (501) staff       (20)      258 2023-04-25 16:06:35.000000 SocketWrapper-0.2.3/SocketWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)        1 2023-04-25 16:06:35.000000 SocketWrapper-0.2.3/SocketWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)       14 2023-04-25 16:06:35.000000 SocketWrapper-0.2.3/SocketWrapper.egg-info/top_level.txt
+-rw-r--r--   0 jarredtd   (501) staff       (20)       79 2023-04-25 16:06:35.815794 SocketWrapper-0.2.3/setup.cfg
+-rw-r--r--   0 jarredtd   (501) staff       (20)     1645 2023-04-25 16:06:26.000000 SocketWrapper-0.2.3/setup.py
```

### Comparing `SocketWrapper-0.2.2/LICENSE` & `SocketWrapper-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SocketWrapper-0.2.2/PKG-INFO` & `SocketWrapper-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SocketWrapper
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/JarredTD/Socket_Wrapper
-Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.3.tar.gz
 Author: Jarred
 Author-email: jarredtdesrosiers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SocketWrapper-0.2.2/README.md` & `SocketWrapper-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `SocketWrapper-0.2.2/SocketWrapper/Client.py` & `SocketWrapper-0.2.3/SocketWrapper/Client.py`

 * *Files identical despite different names*

### Comparing `SocketWrapper-0.2.2/SocketWrapper/Server.py` & `SocketWrapper-0.2.3/SocketWrapper/Server.py`

 * *Files identical despite different names*

### Comparing `SocketWrapper-0.2.2/SocketWrapper.egg-info/PKG-INFO` & `SocketWrapper-0.2.3/SocketWrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SocketWrapper
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/JarredTD/Socket_Wrapper
-Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.3.tar.gz
 Author: Jarred
 Author-email: jarredtdesrosiers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SocketWrapper-0.2.2/setup.py` & `SocketWrapper-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'SocketWrapper',         # How you named your package folder (MyLib)
   packages = ['SocketWrapper'],   # Chose the same as "name"
-  version = '0.2.2',      # Start with a small number and increase it with every change you make
+  version = '0.2.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Jarred',                   # Type in your name
   author_email = 'jarredtdesrosiers@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/JarredTD/Socket_Wrapper',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.2.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/JarredTD/Socket_Wrapper/archive/refs/tags/0.2.3.tar.gz',    # I explain this later on
   keywords = [],   # Keywords that define your package best
   install_requires=[],        # I get to this in a second,
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

