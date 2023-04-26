# Comparing `tmp/easy-ernie-0.1.1.tar.gz` & `tmp/easy-ernie-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-ernie-0.1.1.tar", last modified: Wed Apr 26 08:45:40 2023, max compression
+gzip compressed data, was "easy-ernie-0.1.2.tar", last modified: Wed Apr 26 08:59:19 2023, max compression
```

## Comparing `easy-ernie-0.1.1.tar` & `easy-ernie-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:45:40.042473 easy-ernie-0.1.1/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1434 2023-04-26 08:45:40.042330 easy-ernie-0.1.1/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      843 2023-04-26 08:18:47.000000 easy-ernie-0.1.1/README.md
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-04-26 08:45:40.042509 easy-ernie-0.1.1/setup.cfg
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      934 2023-04-26 08:45:31.000000 easy-ernie-0.1.1/setup.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:45:40.039919 easy-ernie-0.1.1/src/
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:45:40.040970 easy-ernie-0.1.1/src/easy_ernie/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      124 2023-04-26 08:15:00.000000 easy-ernie-0.1.1/src/easy_ernie/__init__.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7106 2023-04-26 08:32:27.000000 easy-ernie-0.1.1/src/easy_ernie/ernie.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:14:13.000000 easy-ernie-0.1.1/src/easy_ernie/fast_ernie.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:45:40.042130 easy-ernie-0.1.1/src/easy_ernie.egg-info/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1434 2023-04-26 08:45:40.000000 easy-ernie-0.1.1/src/easy_ernie.egg-info/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      303 2023-04-26 08:45:40.000000 easy-ernie-0.1.1/src/easy_ernie.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-04-26 08:45:40.000000 easy-ernie-0.1.1/src/easy_ernie.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-04-26 08:45:40.000000 easy-ernie-0.1.1/src/easy_ernie.egg-info/requires.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-04-26 08:45:40.000000 easy-ernie-0.1.1/src/easy_ernie.egg-info/top_level.txt
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.606637 easy-ernie-0.1.2/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.2/LICENSE
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1590 2023-04-26 08:59:19.606487 easy-ernie-0.1.2/PKG-INFO
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      977 2023-04-26 08:55:17.000000 easy-ernie-0.1.2/README.md
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-04-26 08:59:19.606674 easy-ernie-0.1.2/setup.cfg
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      934 2023-04-26 08:56:41.000000 easy-ernie-0.1.2/setup.py
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.604332 easy-ernie-0.1.2/src/
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.605559 easy-ernie-0.1.2/src/easy_ernie/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      124 2023-04-26 08:15:00.000000 easy-ernie-0.1.2/src/easy_ernie/__init__.py
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7106 2023-04-26 08:32:27.000000 easy-ernie-0.1.2/src/easy_ernie/ernie.py
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:50:57.000000 easy-ernie-0.1.2/src/easy_ernie/fast_ernie.py
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-26 08:59:19.606308 easy-ernie-0.1.2/src/easy_ernie.egg-info/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1590 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      311 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/requires.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-04-26 08:59:19.000000 easy-ernie-0.1.2/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy-ernie-0.1.1/PKG-INFO` & `easy-ernie-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.1
+Version: 0.1.2
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
@@ -37,9 +38,11 @@
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BDUSS_BFESS', 'BAIDUID')
     print(fastErnie.ask('你好'))
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
+## Acs-Token
+由于文心一言的Acs-Token的时间戳参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.1/README.md` & `easy-ernie-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -20,9 +20,11 @@
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BDUSS_BFESS', 'BAIDUID')
     print(fastErnie.ask('你好'))
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
+## Acs-Token
+由于文心一言的Acs-Token的时间戳参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.1/setup.py` & `easy-ernie-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='easy-ernie',
-    version='0.1.1',
+    version='0.1.2',
     description='简洁的调用文心一言的WebAPI',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
```

### Comparing `easy-ernie-0.1.1/src/easy_ernie/ernie.py` & `easy-ernie-0.1.2/src/easy_ernie/ernie.py`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.1/src/easy_ernie/fast_ernie.py` & `easy-ernie-0.1.2/src/easy_ernie/fast_ernie.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,13 +20,13 @@
     def ask(self, question: str) -> dict:
         if not self.sessionId:
             self.sessionId = self.ernie.newConversation(question)
         data = self.ernie.ask(question, self.sessionId, self.parentChatId)
         self.parentChatId = data.get('chatId')
         return data
     
-    def reset(self) -> bool:
+    def close(self) -> bool:
         if self.ernie.deleteConversation(self.sessionId):
             self.sessionId = ''
             self.parentChatId = 0
             return True
         return False
```

### Comparing `easy-ernie-0.1.1/src/easy_ernie.egg-info/PKG-INFO` & `easy-ernie-0.1.2/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.1
+Version: 0.1.2
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
@@ -37,9 +38,11 @@
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BDUSS_BFESS', 'BAIDUID')
     print(fastErnie.ask('你好'))
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
+## Acs-Token
+由于文心一言的Acs-Token的时间戳参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

