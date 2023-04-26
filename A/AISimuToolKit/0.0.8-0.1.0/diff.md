# Comparing `tmp/AISimuToolKit-0.0.8.tar.gz` & `tmp/AISimuToolKit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AISimuToolKit-0.0.8.tar", last modified: Tue Apr 25 14:06:45 2023, max compression
+gzip compressed data, was "AISimuToolKit-0.1.0.tar", last modified: Tue Apr 25 14:24:00 2023, max compression
```

## Comparing `AISimuToolKit-0.0.8.tar` & `AISimuToolKit-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,52 @@
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/AISimuToolKit/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.0.8/AISimuToolKit/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/AISimuToolKit.egg-info/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      407 2023-04-25 14:06:45.000000 AISimuToolKit-0.0.8/AISimuToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      348 2023-04-25 14:06:45.000000 AISimuToolKit-0.0.8/AISimuToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        1 2023-04-25 14:06:45.000000 AISimuToolKit-0.0.8/AISimuToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      132 2023-04-25 14:06:45.000000 AISimuToolKit-0.0.8/AISimuToolKit.egg-info/requires.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       19 2023-04-25 14:06:45.000000 AISimuToolKit-0.0.8/AISimuToolKit.egg-info/top_level.txt
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      407 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/PKG-INFO
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     8780 2023-04-23 03:13:54.000000 AISimuToolKit-0.0.8/README.md
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       38 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/setup.cfg
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1125 2023-04-25 14:02:58.000000 AISimuToolKit-0.0.8/setup.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/test/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-23 03:13:55.000000 AISimuToolKit-0.0.8/test/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/test/exp/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.0.8/test/exp/__init__.py
-drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:06:45.063865 AISimuToolKit-0.0.8/test/exp/agents/
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.0.8/test/exp/agents/__init__.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      224 2023-04-24 18:44:21.000000 AISimuToolKit-0.0.8/test/exp/agents/test_agent.py
--rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1151 2023-04-23 15:54:29.000000 AISimuToolKit-0.0.8/test/test_experiment.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      450 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/base_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1512 2023-04-24 17:36:09.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/finetune_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1319 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/instruct_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1965 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/probe_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2524 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/reflect_action.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1866 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/actions/register.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)    13350 2023-04-25 11:27:15.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/agent.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9018 2023-04-25 10:46:01.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/agents/memory.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     5388 2023-04-25 11:38:16.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/experiment.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      158 2023-04-24 16:38:46.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/TimeStep.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      537 2023-04-22 12:03:37.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/register.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1309 2023-04-22 12:07:26.000000 AISimuToolKit-0.1.0/AISimuToolKit/exp/toolkit/toolkit.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/model/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1469 2023-04-25 04:36:11.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/embedding.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     9659 2023-04-24 19:29:48.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/model.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     2106 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/AISimuToolKit/model/register.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/store/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/store/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     6652 2023-04-22 11:34:15.000000 AISimuToolKit-0.1.0/AISimuToolKit/store/logger.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit/utils/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-22 12:44:44.000000 AISimuToolKit-0.1.0/AISimuToolKit/utils/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1559 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/AISimuToolKit/utils/utils.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1209 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        1 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      132 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/requires.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       19 2023-04-25 14:24:00.000000 AISimuToolKit-0.1.0/AISimuToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      439 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/PKG-INFO
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     8780 2023-04-23 03:13:54.000000 AISimuToolKit-0.1.0/README.md
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)       38 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/setup.cfg
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1157 2023-04-25 14:23:34.000000 AISimuToolKit-0.1.0/setup.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/test/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-23 03:13:55.000000 AISimuToolKit-0.1.0/test/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/test/exp/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.0/test/exp/__init__.py
+drwxrwxr-x   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-25 14:24:00.771638 AISimuToolKit-0.1.0/test/exp/agents/
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)        0 2023-04-24 18:42:26.000000 AISimuToolKit-0.1.0/test/exp/agents/__init__.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)      224 2023-04-24 18:44:21.000000 AISimuToolKit-0.1.0/test/exp/agents/test_agent.py
+-rw-rw-r--   0 guoshiguang2021  (1049) guoshiguang2021  (1049)     1151 2023-04-23 15:54:29.000000 AISimuToolKit-0.1.0/test/test_experiment.py
```

### Comparing `AISimuToolKit-0.0.8/README.md` & `AISimuToolKit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `AISimuToolKit-0.0.8/setup.py` & `AISimuToolKit-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
     name="AISimuToolKit",  # 这里是pip项目发布的名称
-    version="0.0.8",  # 版本号，数值大的会优先被pip
+    version="0.1.0",  # 版本号，数值大的会优先被pip
     keywords=["pip", "AISimuToolKit"],  # 关键字
     description="ICIP's private utils.",  # 描述
     long_description="ICIP's private utils. The development version will be released when it is sufficiently refined",
     license="MIT Licence",  # 许可证
     url="http://git.cipsup.cn/aisimulationplatform/toolkit/aisimulation",  # 项目相关文件地址，一般是github项目地址即可
     author="Ren & Guo",  # 作者
-    author_email="renmengjie22@mails.ucas.ac.cn",
+    author_email="renmengjie22@mails.ucas.ac.cn,guoshiguang22@mails.ucas.edu.cn",
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     python_requires='>=3.10',
     install_requires=["openai==0.27.4", "pandas==1.5.3", "PyYAML==6.0", "Requests==2.28.2", "scikit_learn==1.2.2",
                       "setuptools==65.6.3", "torch==1.13.1", "transformers==4.24.0", ]
     # 这个项目依赖的第三方库
```

### Comparing `AISimuToolKit-0.0.8/test/test_experiment.py` & `AISimuToolKit-0.1.0/test/test_experiment.py`

 * *Files identical despite different names*

