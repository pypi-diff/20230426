# Comparing `tmp/HtmlPageParser-0.0.2.tar.gz` & `tmp/HtmlPageParser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HtmlPageParser-0.0.2.tar", last modified: Wed Apr 26 07:03:07 2023, max compression
+gzip compressed data, was "HtmlPageParser-0.0.3.tar", last modified: Wed Apr 26 09:02:08 2023, max compression
```

## Comparing `HtmlPageParser-0.0.2.tar` & `HtmlPageParser-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 07:03:07.628390 HtmlPageParser-0.0.2/
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     1069 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.2/LICENSE
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7363 2023-04-26 07:03:07.628390 HtmlPageParser-0.0.2/PKG-INFO
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      515 2023-04-26 06:54:35.000000 HtmlPageParser-0.0.2/pyproject.toml
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     6929 2023-04-26 07:00:50.000000 HtmlPageParser-0.0.2/readme.md
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       38 2023-04-26 07:03:07.628390 HtmlPageParser-0.0.2/setup.cfg
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 07:03:07.628390 HtmlPageParser-0.0.2/src/
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 07:03:07.628390 HtmlPageParser-0.0.2/src/HtmlPageParser.egg-info/
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7363 2023-04-26 07:03:07.000000 HtmlPageParser-0.0.2/src/HtmlPageParser.egg-info/PKG-INFO
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      317 2023-04-26 07:03:07.000000 HtmlPageParser-0.0.2/src/HtmlPageParser.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        1 2023-04-26 07:03:07.000000 HtmlPageParser-0.0.2/src/HtmlPageParser.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       40 2023-04-26 07:03:07.000000 HtmlPageParser-0.0.2/src/HtmlPageParser.egg-info/top_level.txt
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.2/src/__init__.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     8726 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.2/src/htmllabel.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3636 2023-04-26 06:54:35.000000 HtmlPageParser-0.0.2/src/json2markdown.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3435 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.2/src/parser.py
-drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 07:03:07.628390 HtmlPageParser-0.0.2/tests/
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      466 2023-04-26 06:49:33.000000 HtmlPageParser-0.0.2/tests/test_json2markdown.py
--rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      918 2023-04-26 06:50:28.000000 HtmlPageParser-0.0.2/tests/test_parser.py
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     1069 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/LICENSE
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7371 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/PKG-INFO
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      515 2023-04-26 09:01:01.000000 HtmlPageParser-0.0.3/pyproject.toml
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     6937 2023-04-26 09:00:30.000000 HtmlPageParser-0.0.3/readme.md
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       38 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/setup.cfg
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/src/
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     7371 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      317 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        1 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)       40 2023-04-26 09:02:08.000000 HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/top_level.txt
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/src/__init__.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     8726 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/src/htmllabel.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3636 2023-04-26 06:54:35.000000 HtmlPageParser-0.0.3/src/json2markdown.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)     3435 2023-04-26 06:32:27.000000 HtmlPageParser-0.0.3/src/parser.py
+drwxrwxr-x   0 jeffrey   (1000) jeffrey   (1000)        0 2023-04-26 09:02:08.842992 HtmlPageParser-0.0.3/tests/
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      466 2023-04-26 06:49:33.000000 HtmlPageParser-0.0.3/tests/test_json2markdown.py
+-rw-rw-r--   0 jeffrey   (1000) jeffrey   (1000)      918 2023-04-26 06:50:28.000000 HtmlPageParser-0.0.3/tests/test_parser.py
```

### Comparing `HtmlPageParser-0.0.2/LICENSE` & `HtmlPageParser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.2/PKG-INFO` & `HtmlPageParser-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HtmlPageParser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A generic HTML page parser
 Author-email: Jeffrey Yang <snjyor@163.com>
 Project-URL: Homepage, https://github.com/snjyor/HtmlPageParser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -18,15 +18,15 @@
 ```shell
 pip install HtmlPageParser
 ```
 
 ## 使用示例
 ```python
 # 爬取页面内容
-from HtmlParser.src.parser import Parser
+from HtmlPageParser.src.parser import Parser
 with open("test.html", "r", encoding="utf-8") as f:
     html = f.read()
 client = Parser(base_url="https://www.163.com/")
 xpath_css = [
     {".//p[@class='f_center']": ".f_center"},
     {".//p[@class='f_center']": ".f_center"},
     {".//p[@class='f_center']": ".f_center"},
@@ -34,15 +34,15 @@
     {".//p[@class='f_center']": ".f_center"}
 ]
 data = client.parser(html, css_selector="#content > div.post_body", xpath_css=xpath_css)
 print(data)
 
 # json结构数据转为markdown格式
 import json
-from HtmlParser.src.json2markdown import Json2Markdown
+from HtmlPageParser.src.json2markdown import Json2Markdown
 with open("json_data.json", 'r', encoding='utf-8') as f:
     json_data = json.load(f)
 J2M = Json2Markdown()
 markdown_data = J2M.json2markdown(json_data)
 print(markdown_data)
 
 ```
```

### Comparing `HtmlPageParser-0.0.2/pyproject.toml` & `HtmlPageParser-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "HtmlPageParser"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jeffrey Yang", email="snjyor@163.com" },
 ]
 description = "A generic HTML page parser"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HtmlPageParser-0.0.2/readme.md` & `HtmlPageParser-0.0.3/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ```shell
 pip install HtmlPageParser
 ```
 
 ## 使用示例
 ```python
 # 爬取页面内容
-from HtmlParser.src.parser import Parser
+from HtmlPageParser.src.parser import Parser
 with open("test.html", "r", encoding="utf-8") as f:
     html = f.read()
 client = Parser(base_url="https://www.163.com/")
 xpath_css = [
     {".//p[@class='f_center']": ".f_center"},
     {".//p[@class='f_center']": ".f_center"},
     {".//p[@class='f_center']": ".f_center"},
@@ -21,15 +21,15 @@
     {".//p[@class='f_center']": ".f_center"}
 ]
 data = client.parser(html, css_selector="#content > div.post_body", xpath_css=xpath_css)
 print(data)
 
 # json结构数据转为markdown格式
 import json
-from HtmlParser.src.json2markdown import Json2Markdown
+from HtmlPageParser.src.json2markdown import Json2Markdown
 with open("json_data.json", 'r', encoding='utf-8') as f:
     json_data = json.load(f)
 J2M = Json2Markdown()
 markdown_data = J2M.json2markdown(json_data)
 print(markdown_data)
 
 ```
```

### Comparing `HtmlPageParser-0.0.2/src/HtmlPageParser.egg-info/PKG-INFO` & `HtmlPageParser-0.0.3/src/HtmlPageParser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HtmlPageParser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A generic HTML page parser
 Author-email: Jeffrey Yang <snjyor@163.com>
 Project-URL: Homepage, https://github.com/snjyor/HtmlPageParser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -18,15 +18,15 @@
 ```shell
 pip install HtmlPageParser
 ```
 
 ## 使用示例
 ```python
 # 爬取页面内容
-from HtmlParser.src.parser import Parser
+from HtmlPageParser.src.parser import Parser
 with open("test.html", "r", encoding="utf-8") as f:
     html = f.read()
 client = Parser(base_url="https://www.163.com/")
 xpath_css = [
     {".//p[@class='f_center']": ".f_center"},
     {".//p[@class='f_center']": ".f_center"},
     {".//p[@class='f_center']": ".f_center"},
@@ -34,15 +34,15 @@
     {".//p[@class='f_center']": ".f_center"}
 ]
 data = client.parser(html, css_selector="#content > div.post_body", xpath_css=xpath_css)
 print(data)
 
 # json结构数据转为markdown格式
 import json
-from HtmlParser.src.json2markdown import Json2Markdown
+from HtmlPageParser.src.json2markdown import Json2Markdown
 with open("json_data.json", 'r', encoding='utf-8') as f:
     json_data = json.load(f)
 J2M = Json2Markdown()
 markdown_data = J2M.json2markdown(json_data)
 print(markdown_data)
 
 ```
```

### Comparing `HtmlPageParser-0.0.2/src/htmllabel.py` & `HtmlPageParser-0.0.3/src/htmllabel.py`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.2/src/json2markdown.py` & `HtmlPageParser-0.0.3/src/json2markdown.py`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.2/src/parser.py` & `HtmlPageParser-0.0.3/src/parser.py`

 * *Files identical despite different names*

### Comparing `HtmlPageParser-0.0.2/tests/test_parser.py` & `HtmlPageParser-0.0.3/tests/test_parser.py`

 * *Files identical despite different names*

