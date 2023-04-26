# Comparing `tmp/simple_spider_tool-0.0.18.tar.gz` & `tmp/simple_spider_tool-0.0.19.tar.gz`

## Comparing `simple_spider_tool-0.0.18.tar` & `simple_spider_tool-0.0.19.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/__init__.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/date.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/decorator.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/hash.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/jsons.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/re.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/simple_spider_tool/types.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/LICENSE
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/README.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/pyproject.toml
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/__init__.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/date.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/decorator.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/hash.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/jsons.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/re.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/simple_spider_tool/types.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/LICENSE
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 simple_spider_tool-0.0.19/PKG-INFO
```

### Comparing `simple_spider_tool-0.0.18/simple_spider_tool/date.py` & `simple_spider_tool-0.0.19/simple_spider_tool/date.py`

 * *Files identical despite different names*

### Comparing `simple_spider_tool-0.0.18/simple_spider_tool/decorator.py` & `simple_spider_tool-0.0.19/simple_spider_tool/decorator.py`

 * *Files identical despite different names*

### Comparing `simple_spider_tool-0.0.18/simple_spider_tool/jsons.py` & `simple_spider_tool-0.0.19/simple_spider_tool/jsons.py`

 * *Files identical despite different names*

### Comparing `simple_spider_tool-0.0.18/simple_spider_tool/re.py` & `simple_spider_tool-0.0.19/simple_spider_tool/re.py`

 * *Files identical despite different names*

### Comparing `simple_spider_tool-0.0.18/LICENSE` & `simple_spider_tool-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_spider_tool-0.0.18/pyproject.toml` & `simple_spider_tool-0.0.19/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [project]
 name = "simple-spider-tool"
-version = "0.0.18"
+version = "0.0.19"
 authors = [
     { name = "xingc", email = "xingcys@gmail.com" },
 ]
 description = "一些简易、好用的爬虫工具，减少代码与文件冗余，提升工作的效率和代码整洁度"
 readme = "README.md"
-# license = { file = "LICENSE" }
+license = "MIT"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 keywords = [
     "spider",
-    "json",
+    "tool",
     "jsonpath",
     "md5",
-    "encrypt",
     "datetime",
     "timestamp"
 ]
 dependencies = [
     "jsonpath>=0.82"
 ]
+
+[project.optional-dependencies]
+seventeen = [
+    "simple-spider-tool17"
+]
+
 [tool.hatch.build.targets.sdist]
 include = ["/simple_spider_tool", "/*.md"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
-
-#[build-system]
-#requires = ["setuptools"]
-#build-backend = "setuptools.build_meta"
```

### Comparing `simple_spider_tool-0.0.18/PKG-INFO` & `simple_spider_tool-0.0.19/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: simple-spider-tool
-Version: 0.0.18
+Version: 0.0.19
 Summary: 一些简易、好用的爬虫工具，减少代码与文件冗余，提升工作的效率和代码整洁度
 Author-email: xingc <xingcys@gmail.com>
+License-Expression: MIT
 License-File: LICENSE
-Keywords: datetime,encrypt,json,jsonpath,md5,spider,timestamp
+Keywords: datetime,jsonpath,md5,spider,timestamp,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.5
 Requires-Dist: jsonpath>=0.82
+Provides-Extra: seventeen
+Requires-Dist: simple-spider-tool17; extra == 'seventeen'
 Description-Content-Type: text/markdown
 
 # simple spider tool
 
-----
-
 在实际工作中，沉淀的一些简易、好用的爬虫工具，减少重复代码与文件冗余，希望一样能为使用者带来益处。如果您也想贡献好的代码片段，请将代码以及描述，通过邮箱（ [xingcys@gmail.com](mailto:xingc<xingcys@gmail.com>) ）发送给我。代码格式是遵循自我主观，如存在不足敬请指出！
 
+## 安装
+
+```shell
+pip install simple-spider-tool
+```
 ## 简单使用
 
 ```python
 from simple_spider_tool import format_json, jsonpath
 
 data = {
     "code": 200,
@@ -46,10 +52,17 @@
 
 boss_name = jsonpath(data, '$.data[?(@.level=="boss")].username', first=True)
 all_user_info = jsonpath(data, '$.data[*].username')
 
 print(boss_name)
 print(format_json(all_user_info))
 ```
+## 兼容使用
+在`0.0.18`对包目录发生改变，由`simple_spider_tools`更改为`simple_spider_tool`，如有使用过低于`0.0.18`版本，请通过安装兼容扩展包以达到兼容使用
+```shell
+pip install simple-spider-tool[seventeen]
+```
+
+## 链接
+Github：https://github.com/xingcweb/simple-spider-tool
 
-xingc-simple-spider-tool
-xst
+在线文档：https://simple-spider-tool.xingc.top/
```

