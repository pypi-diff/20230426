# Comparing `tmp/ats_case-0.6.6.tar.gz` & `tmp/ats_case-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.6.6.tar", last modified: Tue Apr 25 06:42:30 2023, max compression
+gzip compressed data, was "ats_case-0.6.7.tar", last modified: Wed Apr 26 05:45:02 2023, max compression
```

## Comparing `ats_case-0.6.6.tar` & `ats_case-0.6.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.515983 ats_case-0.6.6/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-25 06:42:30.513951 ats_case-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.116807 ats_case-0.6.6/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.6/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.339573 ats_case-0.6.6/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.6/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17451 2023-04-24 06:03:25.000000 ats_case-0.6.6/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.6/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.6.6/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5549 2023-04-24 01:14:40.000000 ats_case-0.6.6/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.401578 ats_case-0.6.6/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.6/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.6/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.6.6/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.463466 ats_case-0.6.6/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.6/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.6.6/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3624 2023-04-25 02:59:07.000000 ats_case-0.6.6/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.504943 ats_case-0.6.6/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.6/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.6/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-25 06:42:30.217542 ats_case-0.6.6/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-25 06:42:29.000000 ats_case-0.6.6/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-25 06:42:29.000000 ats_case-0.6.6/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:42:29.000000 ats_case-0.6.6/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-25 06:42:29.000000 ats_case-0.6.6/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 06:42:29.000000 ats_case-0.6.6/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:42:30.515983 ats_case-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-25 06:42:22.000000 ats_case-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:02.230628 ats_case-0.6.7/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-26 05:45:02.228633 ats_case-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:01.827506 ats_case-0.6.7/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.7/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:02.045282 ats_case-0.6.7/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.7/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17451 2023-04-24 06:03:25.000000 ats_case-0.6.7/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.7/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.6.7/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5549 2023-04-24 01:14:40.000000 ats_case-0.6.7/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:02.120084 ats_case-0.6.7/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.7/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.7/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.6.7/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:02.179923 ats_case-0.6.7/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.7/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.6.7/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.6.7/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:02.220654 ats_case-0.6.7/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.7/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.7/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-26 05:45:01.913398 ats_case-0.6.7/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-26 05:45:01.000000 ats_case-0.6.7/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-26 05:45:01.000000 ats_case-0.6.7/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 05:45:01.000000 ats_case-0.6.7/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-26 05:45:01.000000 ats_case-0.6.7/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 05:45:01.000000 ats_case-0.6.7/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 05:45:02.231625 ats_case-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-04-26 02:44:49.000000 ats_case-0.6.7/setup.py
```

### Comparing `ats_case-0.6.6/PKG-INFO` & `ats_case-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.6.6
+Version: 0.6.7
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.6/README.md` & `ats_case-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/ats_case/case/command.py` & `ats_case-0.6.7/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/ats_case/case/context.py` & `ats_case-0.6.7/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/ats_case/case/executor.py` & `ats_case-0.6.7/ats_case/case/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from importlib import import_module
 
+import gevent
 from ats_base.common import func
 from ats_base.log.logger import logger
 
 from ats_case.case import translator, command
 from ats_case.case.context import Context
 from ats_case.common.enum import *
 from ats_case.common.error import *
@@ -81,14 +82,17 @@
         if ifs is not None and type(ifs) is dict and len(ifs) > 0:
             for fc, values in ifs.items():
                 if command.ats().operation(fc).parameter(values).exec(self._context):
                     return False
         return True
 
     def step_exec(self):
+        if self._context.mode == WorkMode.FORMAL:   # 协程切换
+            gevent.sleep(0.05)
+
         logger.info('~ @TCC-STEP-> steps[#{}] execute'.format(self._context.runtime.step))
 
         self._flush()  # 缓存在断点续测时所需关键变量
         if self.is_exec():
             getattr(self._model, 'step_{}'.format(self._context.runtime.step))(self._context)
 
     def loop_meet(self):
```

### Comparing `ats_case-0.6.6/ats_case/case/translator.py` & `ats_case-0.6.7/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/ats_case/manage/core.py` & `ats_case-0.6.7/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/ats_case/manage/start.py` & `ats_case-0.6.7/ats_case/manage/start.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import threading
 
+import gevent
 import pytest
 
 from datetime import datetime
 
 from ats_base.common import func
 from ats_base.service import mm
 
@@ -27,18 +28,18 @@
     def __init__(self, data: dict):
         self._data = data
         self._username = self._data.get('tester').get('username', '')
         self._now = datetime.now().strftime('%y%m%d%H%M%S%f')
 
         self._init()
 
-    def run(self):
+    def _init(self):
         pass
 
-    def _init(self):
+    def run(self):
         pass
 
     def _build(self, work_mode: WorkMode, code: str = None):
         if code is None:
             code = 'case'
 
         user_dir = func.makeDir(func.project_dir(), 'testcase', work_mode.value.lower(), self._username)
@@ -61,54 +62,56 @@
             self._sn = self._username.upper() + self._now
             mm.Dict.put('test:log', self._sn, self._data)
             self._save()
         else:  # 断点续测
             self._data = mm.Dict.get('test:log', self._sn)
             self._data['renew'] = 1
 
-        self._cases = self._data.pop('cases')
-        self._meters = self._data.pop('meters')
+        self._cases = self._data.get('cases', [])
+        self.meters = self._data.get('meters', [])
 
-        self._test_sn = None
+    def _save(self):
+        pass  # 存数据库
 
     def run(self):
-        for case in self._cases:
-            test_task = self.TestTask(self, case, self._meters)
-            test_task.start()
-            test_task.join()
-
-    class TestTask(threading.Thread):
-        def __init__(self, parent, case, meters):
-            super(FormalMode.TestTask, self).__init__()
+        while self._cases:
+            case_task = self.CaseTask(self, self._cases.pop(0))
+            case_task.start()
+            case_task.join()
+
+            mm.Dict.put('test:log', self._sn, self._data)
+
+    class CaseTask(threading.Thread):
+        def __init__(self, parent, case):
+            super(FormalMode.CaseTask, self).__init__()
             self._parent = parent
             self._case = case
-            self._meters = meters
 
         def run(self):
-            for meter in self._meters:
-                self._parent.flush(case=self._case, meter=meter)
+            gs = []
+            for meter in self._parent.meters:
                 # i = 0 执行操作表台 传入参数index
-                th = threading.Thread(target=self._parent.exec, daemon=True)
-                th.start()
-
-    def exec(self):
-        pytest.main(
-            ["-sv", self._build(WorkMode.FORMAL), '--sn={}'.format(self._test_sn)])
+                gs.append(gevent.spawn(self._parent.exec, self._parent.flush(case=self._case, meter=meter)))
 
-    def _save(self):
-        pass  # 存数据库
+            gevent.joinall(gs)
 
     def flush(self, case, meter):
         self._data['usercase'] = case
         self._data['meter'] = meter
-        self._test_sn = '{}:{}:{}'.format(self._sn, case['id'], meter['pos'])
-        mm.Dict.put('test:log', '{}:{}:{}'.format(self._sn, case['id'], meter['pos']), self._data)
+
+        test_sn = '{}:{}:{}'.format(self._sn, case['id'], meter['pos'])
+        mm.Dict.put('test:log', test_sn, self._data)
+
+        return test_sn
+
+    def exec(self, test_sn):
+        pytest.main(["-sv", self._build(WorkMode.FORMAL), '--sn={}'.format(test_sn)])
 
 
 class DebugMode(ExecMode):
     def _init(self):
-        self._sn = '{}:{}:{}'.format(self._username.upper() + self._now,
-                                     self._data['usercase']['id'], self._data['meter']['pos'])
-        mm.Dict.put('test:log', self._sn, self._data)
+        self._test_sn = '{}:{}:{}'.format(self._username.upper() + self._now,
+                                          self._data['usercase']['id'], self._data['meter']['pos'])
+        mm.Dict.put('test:log', self._test_sn, self._data)
 
     def run(self):
-        pytest.main(["-sv", self._build(WorkMode.DEBUG), '--sn={}'.format(self._sn)])
+        pytest.main(["-sv", self._build(WorkMode.DEBUG), '--sn={}'.format(self._test_sn)])
```

### Comparing `ats_case-0.6.6/ats_case/template/testcase_v1.tmp` & `ats_case-0.6.7/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/ats_case.egg-info/PKG-INFO` & `ats_case-0.6.7/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.6.6
+Version: 0.6.7
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.6/ats_case.egg-info/SOURCES.txt` & `ats_case-0.6.7/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.6/setup.py` & `ats_case-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.6.6",
+    version="0.6.7",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
@@ -19,12 +19,12 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.9",
-    install_requires=["pytest", "pytest-ordering", "psutil", "ats-base"],
+    install_requires=["pytest", "pytest-ordering", "psutil", "gevent", "ats-base"],
     package_data={
         '': ['*.tmp'],
     },
 )
```

