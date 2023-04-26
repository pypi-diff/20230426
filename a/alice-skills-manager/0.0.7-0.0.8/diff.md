# Comparing `tmp/alice-skills-manager-0.0.7.tar.gz` & `tmp/alice-skills-manager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alice-skills-manager-0.0.7.tar", last modified: Mon Apr 24 20:54:05 2023, max compression
+gzip compressed data, was "alice-skills-manager-0.0.8.tar", last modified: Tue Apr 25 16:00:12 2023, max compression
```

## Comparing `alice-skills-manager-0.0.7.tar` & `alice-skills-manager-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.152964 alice-skills-manager-0.0.7/
--rw-rw-rw-   0        0        0       61 2023-04-22 22:22:23.000000 alice-skills-manager-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      572 2023-04-24 20:54:05.152455 alice-skills-manager-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-manager-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.138179 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/
--rw-rw-rw-   0        0        0      572 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.146313 alice-skills-manager-0.0.7/asm/
--rw-rw-rw-   0        0        0      156 2023-04-22 21:56:13.000000 alice-skills-manager-0.0.7/asm/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-04-22 21:57:43.000000 alice-skills-manager-0.0.7/asm/__main__.py
--rw-rw-rw-   0        0        0    20216 2023-04-22 21:57:47.000000 alice-skills-manager-0.0.7/asm/alice_skills_manager.py
--rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-manager-0.0.7/asm/exceptions.py
--rw-rw-rw-   0        0        0    19210 2023-04-22 21:56:47.000000 alice-skills-manager-0.0.7/asm/skill_entry.py
--rw-rw-rw-   0        0        0     6598 2023-04-22 21:56:27.000000 alice-skills-manager-0.0.7/asm/skill_repo.py
--rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-manager-0.0.7/asm/skill_state.py
--rw-rw-rw-   0        0        0     2993 2023-04-22 21:56:45.000000 alice-skills-manager-0.0.7/asm/util.py
--rw-rw-rw-   0        0        0       42 2023-04-24 20:54:05.153474 alice-skills-manager-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1840 2023-04-24 05:16:49.000000 alice-skills-manager-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.151438 alice-skills-manager-0.0.7/tests/
--rw-rw-rw-   0        0        0    16155 2023-04-22 21:57:22.000000 alice-skills-manager-0.0.7/tests/test_alice_skills_manager.py
--rw-rw-rw-   0        0        0     1453 2023-04-22 21:57:14.000000 alice-skills-manager-0.0.7/tests/test_main.py
--rw-rw-rw-   0        0        0     2727 2023-04-22 21:56:58.000000 alice-skills-manager-0.0.7/tests/test_skill_entry.py
--rw-rw-rw-   0        0        0     1957 2023-04-22 21:56:53.000000 alice-skills-manager-0.0.7/tests/test_skill_repo.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:00:12.502509 alice-skills-manager-0.0.8/
+-rw-rw-rw-   0        0        0       61 2023-04-22 22:22:23.000000 alice-skills-manager-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      572 2023-04-25 16:00:12.501476 alice-skills-manager-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-manager-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 16:00:12.459746 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/
+-rw-rw-rw-   0        0        0      572 2023-04-25 16:00:12.000000 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-04-25 16:00:12.000000 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 16:00:12.000000 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 16:00:12.000000 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-04-25 16:00:12.000000 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-25 16:00:12.000000 alice-skills-manager-0.0.8/alice_skills_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 16:00:12.489128 alice-skills-manager-0.0.8/asm/
+-rw-rw-rw-   0        0        0      156 2023-04-22 21:56:13.000000 alice-skills-manager-0.0.8/asm/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-04-22 21:57:43.000000 alice-skills-manager-0.0.8/asm/__main__.py
+-rw-rw-rw-   0        0        0    20199 2023-04-25 15:56:28.000000 alice-skills-manager-0.0.8/asm/alice_skills_manager.py
+-rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-manager-0.0.8/asm/exceptions.py
+-rw-rw-rw-   0        0        0    19210 2023-04-22 21:56:47.000000 alice-skills-manager-0.0.8/asm/skill_entry.py
+-rw-rw-rw-   0        0        0     6598 2023-04-22 21:56:27.000000 alice-skills-manager-0.0.8/asm/skill_repo.py
+-rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-manager-0.0.8/asm/skill_state.py
+-rw-rw-rw-   0        0        0     2993 2023-04-22 21:56:45.000000 alice-skills-manager-0.0.8/asm/util.py
+-rw-rw-rw-   0        0        0       42 2023-04-25 16:00:12.503034 alice-skills-manager-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1840 2023-04-25 15:56:07.000000 alice-skills-manager-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:00:12.499419 alice-skills-manager-0.0.8/tests/
+-rw-rw-rw-   0        0        0    16155 2023-04-22 21:57:22.000000 alice-skills-manager-0.0.8/tests/test_alice_skills_manager.py
+-rw-rw-rw-   0        0        0     1453 2023-04-22 21:57:14.000000 alice-skills-manager-0.0.8/tests/test_main.py
+-rw-rw-rw-   0        0        0     2727 2023-04-22 21:56:58.000000 alice-skills-manager-0.0.8/tests/test_skill_entry.py
+-rw-rw-rw-   0        0        0     1957 2023-04-22 21:56:53.000000 alice-skills-manager-0.0.8/tests/test_skill_repo.py
```

### Comparing `alice-skills-manager-0.0.7/PKG-INFO` & `alice-skills-manager-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-skills-manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Alice Skills Manager
 Home-page: https://github.com/Alice-IA/alice-skills-manager
 Author: Alice-IA
 Author-email: yuiassistant@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `alice-skills-manager-0.0.7/README.md` & `alice-skills-manager-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/alice_skills_manager.egg-info/PKG-INFO` & `alice-skills-manager-0.0.8/alice_skills_manager.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-skills-manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Alice Skills Manager
 Home-page: https://github.com/Alice-IA/alice-skills-manager
 Author: Alice-IA
 Author-email: yuiassistant@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `alice-skills-manager-0.0.7/alice_skills_manager.egg-info/SOURCES.txt` & `alice-skills-manager-0.0.8/alice_skills_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/asm/__main__.py` & `alice-skills-manager-0.0.8/asm/__main__.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/asm/alice_skills_manager.py` & `alice-skills-manager-0.0.8/asm/alice_skills_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from functools import wraps
 from glob import glob
 from os import path
 from typing import Dict, List
 
 from xdg import BaseDirectory
 
-from alice_skills_manager import GitException
+from asm import GitException
 from asm.exceptions import (
     AlreadyInstalled,
     AlreadyRemoved,
     AsmException,
     MultipleSkillMatches,
     RemoveException,
     SkillNotFound
```

### Comparing `alice-skills-manager-0.0.7/asm/exceptions.py` & `alice-skills-manager-0.0.8/asm/exceptions.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/asm/skill_entry.py` & `alice-skills-manager-0.0.8/asm/skill_entry.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/asm/skill_repo.py` & `alice-skills-manager-0.0.8/asm/skill_repo.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/asm/skill_state.py` & `alice-skills-manager-0.0.8/asm/skill_state.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/asm/util.py` & `alice-skills-manager-0.0.8/asm/util.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/setup.py` & `alice-skills-manager-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #             print('USING LOOSE REQUIREMENTS!')
 #             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
 #         return [pkg for pkg in requirements
 #                 if pkg.strip() and not pkg.startswith("#")]
 
 setup(
     name='alice-skills-manager',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[line.strip() for line in open('requirements/requirements.txt')],
     package_data={'': package_files('asm')},
     # tests_require=required('requirements/tests.txt'),
     python_requires='>=3.6',
     url='https://github.com/Alice-IA/alice-skills-manager',
     license='Apache-2.0',
```

### Comparing `alice-skills-manager-0.0.7/tests/test_alice_skills_manager.py` & `alice-skills-manager-0.0.8/tests/test_alice_skills_manager.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/tests/test_main.py` & `alice-skills-manager-0.0.8/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/tests/test_skill_entry.py` & `alice-skills-manager-0.0.8/tests/test_skill_entry.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.7/tests/test_skill_repo.py` & `alice-skills-manager-0.0.8/tests/test_skill_repo.py`

 * *Files identical despite different names*

