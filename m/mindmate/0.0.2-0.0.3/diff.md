# Comparing `tmp/mindmate-0.0.2.tar.gz` & `tmp/mindmate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindmate-0.0.2.tar", last modified: Wed Apr 26 01:20:10 2023, max compression
+gzip compressed data, was "mindmate-0.0.3.tar", last modified: Wed Apr 26 02:26:13 2023, max compression
```

## Comparing `mindmate-0.0.2.tar` & `mindmate-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 01:20:10.052497 mindmate-0.0.2/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1328 2023-04-26 01:20:10.048498 mindmate-0.0.2/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      244 2023-04-24 04:35:25.000000 mindmate-0.0.2/README.md
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 01:20:09.467919 mindmate-0.0.2/mindmate/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.2/mindmate/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-04-25 04:07:16.000000 mindmate-0.0.2/mindmate/cli.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 01:20:09.851966 mindmate-0.0.2/mindmate/commands/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.2/mindmate/commands/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3899 2023-04-25 23:30:04.000000 mindmate-0.0.2/mindmate/commands/ai.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-04-26 01:08:59.000000 mindmate-0.0.2/mindmate/commands/chat.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1343 2023-04-25 02:29:04.000000 mindmate-0.0.2/mindmate/commands/configure.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      381 2023-04-24 04:35:25.000000 mindmate-0.0.2/mindmate/commands/dropdb.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      301 2023-04-24 04:35:25.000000 mindmate-0.0.2/mindmate/commands/initdb.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 01:20:10.014497 mindmate-0.0.2/mindmate/utils/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.2/mindmate/utils/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1699 2023-04-26 01:06:56.000000 mindmate-0.0.2/mindmate/utils/conf.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.2/mindmate/utils/env.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-25 04:35:40.000000 mindmate-0.0.2/mindmate/utils/helper.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      897 2023-04-25 01:54:19.000000 mindmate-0.0.2/mindmate/utils/utils.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 01:20:09.631950 mindmate-0.0.2/mindmate.egg-info/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1328 2023-04-26 01:20:07.000000 mindmate-0.0.2/mindmate.egg-info/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      537 2023-04-26 01:20:07.000000 mindmate-0.0.2/mindmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-04-26 01:20:07.000000 mindmate-0.0.2/mindmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-04-26 01:20:07.000000 mindmate-0.0.2/mindmate.egg-info/entry_points.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       40 2023-04-26 01:20:07.000000 mindmate-0.0.2/mindmate.egg-info/requires.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-04-26 01:20:07.000000 mindmate-0.0.2/mindmate.egg-info/top_level.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-04-26 01:20:10.053497 mindmate-0.0.2/setup.cfg
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1793 2023-04-26 01:18:38.000000 mindmate-0.0.2/setup.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.738560 mindmate-0.0.3/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1328 2023-04-26 02:26:13.734371 mindmate-0.0.3/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      527 2023-04-26 02:15:41.000000 mindmate-0.0.3/README.md
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.199887 mindmate-0.0.3/mindmate/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/cli.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.571443 mindmate-0.0.3/mindmate/commands/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/commands/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3899 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/commands/ai.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/commands/chat.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.0.3/mindmate/commands/configure.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      381 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/commands/dropdb.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      301 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/commands/initdb.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.709369 mindmate-0.0.3/mindmate/utils/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/utils/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1699 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/utils/conf.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.3/mindmate/utils/env.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/utils/helper.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1679 2023-04-26 02:15:41.000000 mindmate-0.0.3/mindmate/utils/utils.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.382032 mindmate-0.0.3/mindmate.egg-info/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1328 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      537 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       40 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/requires.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/top_level.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-04-26 02:26:13.740563 mindmate-0.0.3/setup.cfg
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1793 2023-04-26 02:15:41.000000 mindmate-0.0.3/setup.py
```

### Comparing `mindmate-0.0.2/PKG-INFO` & `mindmate-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mindmate
-Version: 0.0.2
+Version: 0.0.3
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: MindMate is a powerful command-line tool that harnesses the capabilities of state-of-the-art artificial intelligence platforms to offer a wide range of use-cases to developers. With MindMate, developers can easily leverage advanced natural language processing (NLP) and machine learning (ML) functionalities to enable various applications
```

### Comparing `mindmate-0.0.2/mindmate/cli.py` & `mindmate-0.0.3/mindmate/cli.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.2/mindmate/commands/ai.py` & `mindmate-0.0.3/mindmate/commands/ai.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.2/mindmate/commands/chat.py` & `mindmate-0.0.3/mindmate/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.2/mindmate/commands/configure.py` & `mindmate-0.0.3/mindmate/commands/configure.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,16 @@
 import click
-import yaml
 import uuid
-import os
 from mindmate.utils.utils import utility
 from mindmate.utils.conf import constants
 
 @click.command()
 def configure():
     """collect keys from user and save it into state file as yaml"""
 
-    # PATH = '~/.mindmate'
-    # FILE_NAME = 'environment.yaml'
-
-    while not os.path.isfile(constants.FILE_PATH+'/'+constants.FILE_NAME):
-        try:
-            os.makedirs(constants.FILE_PATH)
-        except FileExistsError as f:
-            pass
-        data = {
-            'version':1,
-            'keys': {
-                'openai_token':'xxxx',
-                'openai_id':'xxxx',
-            }
-        }
-        with open(constants.FILE_PATH+'/'+constants.FILE_NAME, 'w') as outputfile:
-            yaml.dump(data, outputfile, default_flow_style=False)
-
     file = utility.set_yaml_state(constants.FILE_PATH+'/'+constants.FILE_NAME)
     #TODO: check environment variable first before setting values into yaml file. If exist, then skip yaml update
     openai_value = file['keys']['openai_token']
     openai_user_token = click.prompt(f'OPENAI TOKEN [****************{openai_value[-4:]}]', type=str)
     file['keys']['openai_token'] = openai_user_token
     file['keys']['openai_id'] = str(uuid.uuid4())
     utility.update_yaml_state(state=file, file_path=constants.FILE_PATH+'/'+constants.FILE_NAME)
```

### Comparing `mindmate-0.0.2/mindmate/utils/conf.py` & `mindmate-0.0.3/mindmate/utils/conf.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.2/mindmate/utils/env.py` & `mindmate-0.0.3/mindmate/utils/env.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.2/mindmate.egg-info/PKG-INFO` & `mindmate-0.0.3/mindmate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mindmate
-Version: 0.0.2
+Version: 0.0.3
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: MindMate is a powerful command-line tool that harnesses the capabilities of state-of-the-art artificial intelligence platforms to offer a wide range of use-cases to developers. With MindMate, developers can easily leverage advanced natural language processing (NLP) and machine learning (ML) functionalities to enable various applications
```

### Comparing `mindmate-0.0.2/mindmate.egg-info/SOURCES.txt` & `mindmate-0.0.3/mindmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.2/setup.py` & `mindmate-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 GITHUB_REPO = 'https://github.com/yalattas/mindmate'
 setup(
     name='mindmate',
-    version='0.0.2',
+    version='0.0.3',
     author='Yasser Alattas',
     author_email='y.alattas@gmail.com',
     description="MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers",
     long_description="MindMate is a powerful command-line tool that harnesses the capabilities of state-of-the-art artificial intelligence platforms to offer a wide range of use-cases to developers. With MindMate, developers can easily leverage advanced natural language processing (NLP) and machine learning (ML) functionalities to enable various applications",
     url=GITHUB_REPO,
     download_url=GITHUB_REPO,
     packages=find_packages(),
```

