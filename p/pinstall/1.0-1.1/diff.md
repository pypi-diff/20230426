# Comparing `tmp/pinstall-1.0.tar.gz` & `tmp/pinstall-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinstall-1.0.tar", last modified: Mon Apr 24 03:13:16 2023, max compression
+gzip compressed data, was "pinstall-1.1.tar", last modified: Wed Apr 26 03:37:36 2023, max compression
```

## Comparing `pinstall-1.0.tar` & `pinstall-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 03:13:16.409518 pinstall-1.0/
--rw-r--r--   0 mark      (1000) mark      (1000)     6985 2023-04-24 03:13:16.409518 pinstall-1.0/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     6603 2023-04-24 03:05:45.000000 pinstall-1.0/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 03:13:16.406184 pinstall-1.0/pinstall/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pinstall-1.0/pinstall/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       70 2023-04-05 01:13:56.000000 pinstall-1.0/pinstall/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 03:13:16.409518 pinstall-1.0/pinstall/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     6047 2023-04-24 03:05:44.000000 pinstall-1.0/pinstall/commands/service.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1257 2023-04-21 01:09:48.000000 pinstall-1.0/pinstall/commands/status.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3549 2023-04-21 04:32:43.000000 pinstall-1.0/pinstall/commands/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1385 2023-04-16 04:09:21.000000 pinstall-1.0/pinstall/pinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      775 2023-04-13 07:15:57.000000 pinstall-1.0/pinstall/run.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 03:13:16.409518 pinstall-1.0/pinstall.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     6985 2023-04-24 03:13:16.000000 pinstall-1.0/pinstall.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2023-04-24 03:13:16.000000 pinstall-1.0/pinstall.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-24 03:13:16.000000 pinstall-1.0/pinstall.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-24 03:13:16.000000 pinstall-1.0/pinstall.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-04-24 03:13:16.000000 pinstall-1.0/pinstall.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       27 2023-04-24 03:13:16.000000 pinstall-1.0/pinstall.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-04-24 03:13:16.409518 pinstall-1.0/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1062 2023-04-24 02:39:23.000000 pinstall-1.0/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-26 03:37:36.639991 pinstall-1.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)     7011 2023-04-26 03:37:36.639991 pinstall-1.1/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     6629 2023-04-26 03:34:08.000000 pinstall-1.1/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-26 03:37:36.639991 pinstall-1.1/pinstall/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pinstall-1.1/pinstall/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       97 2023-04-26 03:19:54.000000 pinstall-1.1/pinstall/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-26 03:37:36.639991 pinstall-1.1/pinstall/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     6047 2023-04-24 03:05:44.000000 pinstall-1.1/pinstall/commands/service.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1257 2023-04-21 01:09:48.000000 pinstall-1.1/pinstall/commands/status.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3894 2023-04-26 03:33:34.000000 pinstall-1.1/pinstall/commands/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1385 2023-04-16 04:09:21.000000 pinstall-1.1/pinstall/pinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      775 2023-04-13 07:15:57.000000 pinstall-1.1/pinstall/run.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-26 03:37:36.639991 pinstall-1.1/pinstall.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     7011 2023-04-26 03:37:36.000000 pinstall-1.1/pinstall.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2023-04-26 03:37:36.000000 pinstall-1.1/pinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-26 03:37:36.000000 pinstall-1.1/pinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-26 03:37:36.000000 pinstall-1.1/pinstall.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-04-26 03:37:36.000000 pinstall-1.1/pinstall.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       27 2023-04-26 03:37:36.000000 pinstall-1.1/pinstall.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-04-26 03:37:36.639991 pinstall-1.1/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1062 2023-04-26 03:37:03.000000 pinstall-1.1/setup.py
```

### Comparing `pinstall-1.0/PKG-INFO` & `pinstall-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinstall
-Version: 1.0
+Version: 1.1
 Summary: Installer Tool for Python Programs
 Home-page: https://github.com/bulletmark/pinstall
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: venv virtualenv systemd service
 Classifier: Programming Language :: Python :: 3
@@ -192,15 +192,15 @@
 $ git pull
 $ sudo pip3 install -U --use-pep517 --root-user-action=ignore .
 ```
 
 ## Removal
 
 ```sh
-$ sudo pip3 uninstall pinstall
+$ sudo pip3 uninstall --root-user-action=ignore pinstall
 ```
 
 ## License
 
 Copyright (C) 2023 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License. This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU
```

### Comparing `pinstall-1.0/README.md` & `pinstall-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 $ git pull
 $ sudo pip3 install -U --use-pep517 --root-user-action=ignore .
 ```
 
 ## Removal
 
 ```sh
-$ sudo pip3 uninstall pinstall
+$ sudo pip3 uninstall --root-user-action=ignore pinstall
 ```
 
 ## License
 
 Copyright (C) 2023 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License. This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU
```

### Comparing `pinstall-1.0/pinstall/commands/service.py` & `pinstall-1.1/pinstall/commands/service.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.0/pinstall/commands/status.py` & `pinstall-1.1/pinstall/commands/status.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.0/pinstall/commands/venv.py` & `pinstall-1.1/pinstall/commands/venv.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 Runs `python -m venv` (optionally for the specified Python name or path
 or pyenv version) to create a venv; upgrades it with the latest pip +
 setuptools + wheel; then installs all packages from requirements.txt if
 present.
 '''
 import shutil
 from pathlib import Path
-from looseversion import LooseVersion as Version
 from ..run import run
 
 DEFDIR = 'venv'
 DEFEXE = 'python3'
 DEFREQ = 'requirements.txt'
 
 def init(parser):
@@ -44,20 +43,32 @@
 def main(args):
     'Called to action this command'
     if args.pyenv:
         pyenv_root = run('pyenv root', capture=True)
         if not pyenv_root:
             return 'Error: Can not find pyenv. Is it installed?'
 
-        versions = sorted(Path(pyenv_root, 'versions').glob(f'{args.pyenv}*'),
-                          key=lambda x: Version(x.name))
-        if not versions:
-            return f'Error: no pyenv version {args.pyenv} installed.'
+        basedir = Path(pyenv_root, 'versions')
+        pydir = basedir / args.pyenv
 
-        pyexe = str(versions[-1] / 'bin/python')
+        if not pydir.exists():
+            # Given specific version does not exist, get latest version
+            from looseversion import LooseVersion as Version
+            try:
+                versions = sorted(basedir.glob(f'{args.pyenv}[-.]*'),
+                                key=lambda x: Version(x.name))
+            except:
+                return f'Can not determine pyenv version for {args.pyenv}'
+
+            if not versions:
+                return f'Error: no pyenv version {args.pyenv} installed.'
+
+            pydir = versions[-1]
+
+        pyexe = str(pydir / 'bin/python')
     else:
         pyexe = args.python
 
     vdir = Path(args.dir)
     if '--upgrade' not in args.args and vdir.exists():
         print(f'### Removing existing {vdir}/ ..')
         shutil.rmtree(vdir)
```

### Comparing `pinstall-1.0/pinstall/pinstall.py` & `pinstall-1.1/pinstall/pinstall.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.0/pinstall/run.py` & `pinstall-1.1/pinstall/run.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.0/pinstall.egg-info/PKG-INFO` & `pinstall-1.1/pinstall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinstall
-Version: 1.0
+Version: 1.1
 Summary: Installer Tool for Python Programs
 Home-page: https://github.com/bulletmark/pinstall
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: venv virtualenv systemd service
 Classifier: Programming Language :: Python :: 3
@@ -192,15 +192,15 @@
 $ git pull
 $ sudo pip3 install -U --use-pep517 --root-user-action=ignore .
 ```
 
 ## Removal
 
 ```sh
-$ sudo pip3 uninstall pinstall
+$ sudo pip3 uninstall --root-user-action=ignore pinstall
 ```
 
 ## License
 
 Copyright (C) 2023 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License. This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU
```

### Comparing `pinstall-1.0/setup.py` & `pinstall-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 name = 'pinstall'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='1.0',
+    version='1.1',
     description='Installer Tool for Python Programs',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/bulletmark/{name}',
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
     keywords='venv virtualenv systemd service',
```

