# Comparing `tmp/rpart-0.1.0.tar.gz` & `tmp/rpart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpart-0.1.0.tar", max compression
+gzip compressed data, was "rpart-0.1.1.tar", max compression
```

## Comparing `rpart-0.1.0.tar` & `rpart-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      392 2023-04-25 15:34:34.564266 rpart-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5739 2023-04-22 00:44:59.262064 rpart-0.1.0/rpart/DecisionTree-trythis/DecisionTree.py
--rw-r--r--   0        0        0      452 2023-04-22 00:44:59.262189 rpart-0.1.0/rpart/DecisionTree-trythis/Node.py
--rw-r--r--   0        0        0     1320 2023-04-22 00:44:59.262310 rpart-0.1.0/rpart/DecisionTree-trythis/RandomForestClassifier.py
--rw-r--r--   0        0        0      791 2023-04-22 00:44:59.262424 rpart-0.1.0/rpart/DecisionTree-trythis/train.py
--rw-r--r--   0        0        0      722 2023-04-22 00:44:59.262536 rpart-0.1.0/rpart/DecisionTree-trythis/utils.py
--rw-r--r--   0        0        0     1042 2023-04-22 00:44:59.262657 rpart-0.1.0/rpart/DecisionTree-trythis/visualize_tree.py
--rw-r--r--   0        0        0     8118 2023-04-23 23:32:43.656126 rpart-0.1.0/rpart/DecisionTreeClassifier.py
--rw-r--r--   0        0        0      426 2023-04-23 06:28:56.620450 rpart-0.1.0/rpart/Node.py
--rw-r--r--   0        0        0     4369 2023-04-23 05:45:25.762723 rpart-0.1.0/rpart/RandomForestClassifier.py
--rw-r--r--   0        0        0       82 2023-03-06 20:39:40.203453 rpart-0.1.0/rpart/__init__.py
--rw-r--r--   0        0        0      217 2023-04-03 19:08:25.703343 rpart-0.1.0/rpart/dataset.py
--rw-r--r--   0        0        0     6213 2023-04-23 06:07:05.101058 rpart-0.1.0/rpart/entropy.py
--rw-r--r--   0        0        0     2845 2023-04-23 22:49:20.206878 rpart-0.1.0/rpart/utils.py
--rw-r--r--   0        0        0      609 2023-04-25 15:35:00.402959 rpart-0.1.0/setup.py
--rw-r--r--   0        0        0      380 2023-04-25 15:35:00.403096 rpart-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-04-25 15:39:07.436884 rpart-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5739 2023-04-22 00:44:59.262064 rpart-0.1.1/rpart/DecisionTree-trythis/DecisionTree.py
+-rw-r--r--   0        0        0      452 2023-04-22 00:44:59.262189 rpart-0.1.1/rpart/DecisionTree-trythis/Node.py
+-rw-r--r--   0        0        0     1320 2023-04-22 00:44:59.262310 rpart-0.1.1/rpart/DecisionTree-trythis/RandomForestClassifier.py
+-rw-r--r--   0        0        0      791 2023-04-22 00:44:59.262424 rpart-0.1.1/rpart/DecisionTree-trythis/train.py
+-rw-r--r--   0        0        0      722 2023-04-22 00:44:59.262536 rpart-0.1.1/rpart/DecisionTree-trythis/utils.py
+-rw-r--r--   0        0        0     1042 2023-04-22 00:44:59.262657 rpart-0.1.1/rpart/DecisionTree-trythis/visualize_tree.py
+-rw-r--r--   0        0        0     8118 2023-04-23 23:32:43.656126 rpart-0.1.1/rpart/DecisionTreeClassifier.py
+-rw-r--r--   0        0        0      426 2023-04-23 06:28:56.620450 rpart-0.1.1/rpart/Node.py
+-rw-r--r--   0        0        0     4369 2023-04-23 05:45:25.762723 rpart-0.1.1/rpart/RandomForestClassifier.py
+-rw-r--r--   0        0        0      141 2023-04-25 15:38:42.262907 rpart-0.1.1/rpart/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-03 19:08:25.703343 rpart-0.1.1/rpart/dataset.py
+-rw-r--r--   0        0        0     6213 2023-04-23 06:07:05.101058 rpart-0.1.1/rpart/entropy.py
+-rw-r--r--   0        0        0     2845 2023-04-23 22:49:20.206878 rpart-0.1.1/rpart/utils.py
+-rw-r--r--   0        0        0      609 2023-04-25 15:39:24.671374 rpart-0.1.1/setup.py
+-rw-r--r--   0        0        0      380 2023-04-25 15:39:24.671530 rpart-0.1.1/PKG-INFO
```

### Comparing `rpart-0.1.0/rpart/DecisionTree-trythis/DecisionTree.py` & `rpart-0.1.1/rpart/DecisionTree-trythis/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/DecisionTree-trythis/RandomForestClassifier.py` & `rpart-0.1.1/rpart/DecisionTree-trythis/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/DecisionTree-trythis/train.py` & `rpart-0.1.1/rpart/DecisionTree-trythis/train.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/DecisionTree-trythis/utils.py` & `rpart-0.1.1/rpart/DecisionTree-trythis/utils.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/DecisionTree-trythis/visualize_tree.py` & `rpart-0.1.1/rpart/DecisionTree-trythis/visualize_tree.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/DecisionTreeClassifier.py` & `rpart-0.1.1/rpart/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/RandomForestClassifier.py` & `rpart-0.1.1/rpart/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/entropy.py` & `rpart-0.1.1/rpart/entropy.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/rpart/utils.py` & `rpart-0.1.1/rpart/utils.py`

 * *Files identical despite different names*

### Comparing `rpart-0.1.0/setup.py` & `rpart-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.5.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'rpart',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': None,
     'author': 'Qiushi Yan',
     'author_email': 'qiushi.yann@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

