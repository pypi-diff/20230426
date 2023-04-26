# Comparing `tmp/gggifcheck-0.0.2.tar.gz` & `tmp/gggifcheck-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggifcheck-0.0.2.tar", last modified: Wed Apr 19 07:37:07 2023, max compression
+gzip compressed data, was "gggifcheck-0.0.3.tar", last modified: Wed Apr 26 11:05:12 2023, max compression
```

## Comparing `gggifcheck-0.0.2.tar` & `gggifcheck-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:37:07.334746 gggifcheck-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggifcheck-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4783 2023-04-19 07:37:07.335745 gggifcheck-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4073 2023-04-19 07:32:34.000000 gggifcheck-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 07:37:07.330924 gggifcheck-0.0.2/gggifcheck/
--rw-rw-rw-   0        0        0       86 2023-04-13 04:29:58.000000 gggifcheck-0.0.2/gggifcheck/__init__.py
--rw-rw-rw-   0        0        0    11500 2023-04-18 09:27:13.000000 gggifcheck-0.0.2/gggifcheck/fields.py
--rw-rw-rw-   0        0        0     6948 2023-04-19 07:19:30.000000 gggifcheck-0.0.2/gggifcheck/items.py
--rw-rw-rw-   0        0        0     2838 2023-04-19 07:32:34.000000 gggifcheck-0.0.2/gggifcheck/scrapy_ifcheck.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:37:07.334746 gggifcheck-0.0.2/gggifcheck.egg-info/
--rw-rw-rw-   0        0        0     4783 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-19 07:37:07.000000 gggifcheck-0.0.2/gggifcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      770 2023-04-19 07:37:07.340675 gggifcheck-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      164 2023-04-13 03:43:33.000000 gggifcheck-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:05:12.592520 gggifcheck-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggifcheck-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5394 2023-04-26 11:05:12.593519 gggifcheck-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4684 2023-04-26 10:42:11.000000 gggifcheck-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 11:05:12.587380 gggifcheck-0.0.3/gggifcheck/
+-rw-rw-rw-   0        0        0       86 2023-04-13 04:29:58.000000 gggifcheck-0.0.3/gggifcheck/__init__.py
+-rw-rw-rw-   0        0        0    11566 2023-04-25 02:42:29.000000 gggifcheck-0.0.3/gggifcheck/fields.py
+-rw-rw-rw-   0        0        0     7101 2023-04-26 10:39:56.000000 gggifcheck-0.0.3/gggifcheck/items.py
+-rw-rw-rw-   0        0        0     3331 2023-04-24 11:22:06.000000 gggifcheck-0.0.3/gggifcheck/scrapy_ifcheck.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:05:12.592520 gggifcheck-0.0.3/gggifcheck.egg-info/
+-rw-rw-rw-   0        0        0     5394 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      770 2023-04-26 11:05:12.598405 gggifcheck-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      164 2023-04-13 03:43:33.000000 gggifcheck-0.0.3/setup.py
```

### Comparing `gggifcheck-0.0.2/LICENSE` & `gggifcheck-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gggifcheck-0.0.2/PKG-INFO` & `gggifcheck-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggifcheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggifcheck
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggifcheck/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggifcheck/blob/master/README.md
@@ -41,23 +41,24 @@
 s.input('s', 'aa')
 print(s.value)
 ```
     
 ### 使用CheckItem
 
 ```python
-from gggifcheck.fields import StringCheckField
-from gggifcheck.items import CheckItem
+from gggifcheck import fields, items
 
 
-class TestCheckItem(CheckItem):
-    a = StringCheckField(min_length=1, max_length=2, contains=['a'],
-                         excludes=['b'])
-    b = StringCheckField(min_length=1, max_length=2, contains=['a'],
-                         excludes=['c'])
+class TestCheckItem(items.CheckItem):
+    a = items.BuildCheckField(
+        check_field_class=fields.StringCheckField, min_length=1, 
+        max_length=2, contains=['a'], excludes=['b'])
+    b = items.BuildCheckField(
+        check_field_class=fields.StringCheckField, min_length=1, 
+        max_length=2, contains=['a'], excludes=['c'])
 
 
 item = TestCheckItem()
 item['a'] = 'aa'
 item['b'] = 'ab'
 print(dict(item))
 ```
@@ -66,15 +67,15 @@
 
 ### 结合scrapy
 
 ```python
 # 对scrapy Item进行改写
 import scrapy
 from gggifcheck import fields
-from gggifcheck.items import CheckItem
+from gggifcheck.items import CheckItem, BuildCheckField
 
 
 class ScrapyCheckItem(scrapy.Item, CheckItem):
 
     def __init__(self, *args, **kwargs):
         self._values = {}
         self.check_fields = {}
@@ -108,17 +109,28 @@
     def __setattr__(self, name, value):
         if name.startswith('_') or name in ['check_fields']:
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
-    def keys(self):
+    def check_all(self):
+        """
+        进行所有字段检查
+        :return:
+        """
         self._process_and_check()
-        _ = [self[field] for field in self.fields]  # 进行所有字段检查
+        _ = [self[field] for field in self.fields]
+
+    def keys(self):
+        # 不能放在此处验证的原因是scrapy item进入pipeline前有日志打印等操作导致进行
+        # 此处验证，导致如果在pipeline里进行透传时验证不生效，提前检查报错，此处验证放
+        # 在check_all方法中，因此需要手动调用
+        # self._process_and_check()
+        # _ = [self[field] for field in self.fields]  # 进行所有字段检查
         return self._values.keys()
 
     def get_base_value(self, key):
         if key in self.check_fields:
             return self.check_fields[key].base_value
         elif key in self.fields:
             field = self.fields[key]
@@ -131,19 +143,20 @@
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
 
 # 示例
 class PostItem(ScrapyCheckItem):
     id = scrapy.Field(
-        check_field=fields.MD5CheckField(
-            nullable=False))
+        build_check_field=BuildCheckField(
+            check_field_class=fields.MD5CheckField, nullable=False))
     channel = scrapy.Field(
-        check_field=fields.IntegerCheckField(nullable=False, min_value=1,
-                                             max_value=6))
+        build_check_field=BuildCheckField(
+            check_field_class=fields.IntegerCheckField,
+            nullable=False, min_value=1, max_value=6))
 
 
 item = PostItem()
 item['id'] = '81dc9bdb52d04dc20036dbd8313ed055'
 item['channel'] = 1
 print(dict(item))
 ```
```

### Comparing `gggifcheck-0.0.2/README.md` & `gggifcheck-0.0.3/gggifcheck.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: gggifcheck
+Version: 0.0.3
+Summary: 通用、便捷、准确的字符串时间解析工具
+Home-page: https://github.com/kusen-alpha/gggifcheck
+Author: kusen
+Author-email: hu1194542196@qq.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggifcheck/issues
+Project-URL: Documentation, https://github.com/kusen-alpha/gggifcheck/blob/master/README.md
+Project-URL: Source Code, https://github.com/kusen-alpha/gggifcheck
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gggifcheck
 
 通用条目字段检查(General General General Item Field Check)
 ，是基于Python编写通用检查工具，适应于各种场景的使用，只需要略微进行适配。
 
 ## 使用方法
 
@@ -23,23 +41,24 @@
 s.input('s', 'aa')
 print(s.value)
 ```
     
 ### 使用CheckItem
 
 ```python
-from gggifcheck.fields import StringCheckField
-from gggifcheck.items import CheckItem
+from gggifcheck import fields, items
 
 
-class TestCheckItem(CheckItem):
-    a = StringCheckField(min_length=1, max_length=2, contains=['a'],
-                         excludes=['b'])
-    b = StringCheckField(min_length=1, max_length=2, contains=['a'],
-                         excludes=['c'])
+class TestCheckItem(items.CheckItem):
+    a = items.BuildCheckField(
+        check_field_class=fields.StringCheckField, min_length=1, 
+        max_length=2, contains=['a'], excludes=['b'])
+    b = items.BuildCheckField(
+        check_field_class=fields.StringCheckField, min_length=1, 
+        max_length=2, contains=['a'], excludes=['c'])
 
 
 item = TestCheckItem()
 item['a'] = 'aa'
 item['b'] = 'ab'
 print(dict(item))
 ```
@@ -48,15 +67,15 @@
 
 ### 结合scrapy
 
 ```python
 # 对scrapy Item进行改写
 import scrapy
 from gggifcheck import fields
-from gggifcheck.items import CheckItem
+from gggifcheck.items import CheckItem, BuildCheckField
 
 
 class ScrapyCheckItem(scrapy.Item, CheckItem):
 
     def __init__(self, *args, **kwargs):
         self._values = {}
         self.check_fields = {}
@@ -90,17 +109,28 @@
     def __setattr__(self, name, value):
         if name.startswith('_') or name in ['check_fields']:
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
-    def keys(self):
+    def check_all(self):
+        """
+        进行所有字段检查
+        :return:
+        """
         self._process_and_check()
-        _ = [self[field] for field in self.fields]  # 进行所有字段检查
+        _ = [self[field] for field in self.fields]
+
+    def keys(self):
+        # 不能放在此处验证的原因是scrapy item进入pipeline前有日志打印等操作导致进行
+        # 此处验证，导致如果在pipeline里进行透传时验证不生效，提前检查报错，此处验证放
+        # 在check_all方法中，因此需要手动调用
+        # self._process_and_check()
+        # _ = [self[field] for field in self.fields]  # 进行所有字段检查
         return self._values.keys()
 
     def get_base_value(self, key):
         if key in self.check_fields:
             return self.check_fields[key].base_value
         elif key in self.fields:
             field = self.fields[key]
@@ -113,25 +143,26 @@
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
 
 # 示例
 class PostItem(ScrapyCheckItem):
     id = scrapy.Field(
-        check_field=fields.MD5CheckField(
-            nullable=False))
+        build_check_field=BuildCheckField(
+            check_field_class=fields.MD5CheckField, nullable=False))
     channel = scrapy.Field(
-        check_field=fields.IntegerCheckField(nullable=False, min_value=1,
-                                             max_value=6))
+        build_check_field=BuildCheckField(
+            check_field_class=fields.IntegerCheckField,
+            nullable=False, min_value=1, max_value=6))
 
 
 item = PostItem()
 item['id'] = '81dc9bdb52d04dc20036dbd8313ed055'
 item['channel'] = 1
 print(dict(item))
 ```
 
 ## 关于作者
 
 1. 邮箱：1194542196@qq.com
 2. 微信：hu1194542196
-3. 目前还需要很多需要改进的地方，可以私信作者，你们的提供越多，本库才能更完善。
+3. 目前还需要很多需要改进的地方，可以私信作者，你们的提供越多，本库才能更完善。
```

### Comparing `gggifcheck-0.0.2/gggifcheck/fields.py` & `gggifcheck-0.0.3/gggifcheck/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,17 @@
         ]
 
     def _check_types(self):
         if self._value is None:
             return []
         if not isinstance(self._value, self.types):
             self._type_checked = False
-            error_msg = 'Field %s input: %s, is not types: %s' % (
-                self.key, self._value, self.types)
+            error_msg = ('Field %s input: %s, the type is %s, is not '
+                         'types: %s') % (
+                self.key, self._value, type(self._value), self.types)
             return [Exception(error_msg)]
         return []
 
     def _check_choices(self):
         if self.choices and self._value not in self.choices:
             error_msg = 'Field %s intput: %s, is not in choices: %s' % (
                 self.key, self._value, self.choices)
```

### Comparing `gggifcheck-0.0.2/gggifcheck/items.py` & `gggifcheck-0.0.3/gggifcheck/items.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,56 +3,55 @@
 # email: 1194542196@qq.com
 # date: 2023/4/13
 
 
 import itertools
 from collections.abc import MutableMapping
 
-from .fields import CheckField
-
 
 class ItemMeta(object):
     def __new__(cls, *args, **kwargs):
-        fields = {}
+        build_fields = {}
         for n in dir(cls):
             v = getattr(cls, n)
-            if isinstance(v, CheckField):
-                fields[n] = v
-        cls.fields = fields
+            if isinstance(v, BuildCheckField):
+                build_fields[n] = v
+        cls.build_fields = build_fields
         return super().__new__(cls)
 
 
 class CheckItem(MutableMapping, ItemMeta):
     relate_process_default = []  # 关联处理字段间互相取默认值
     relate_check_null = []  # 关联检查字段间互相是否为None
     relate_check_sequence_length = []  # 关联检查序列字段间互相长度判断
     relate_check_startswith = []  # 关联检查字符串字段间互相startswith关系
     relate_check_endswith = []  # 关联检查字符串字段间互相endswith关系
     relate_check_contains = []  # 关联检查字符串字段间互相包含关系
     bundle_errors = []  # 是否一次性返回所有错误，暂时没有使用该字段
 
     def __init__(self, *args, **kwargs):
+        self.check_fields = {}
         if args or kwargs:
             for k, v in dict(*args, **kwargs).items():
-                self.fields[k].input(k, v)
+                self[k] = v
 
     def process(self):
         for key in itertools.chain(self._get_config_attr_names(),
-                                   self.fields.keys()):
+                                   self.build_fields.keys()):
             field_name = key
             if not key.startswith('_'):
                 field_name = '_' + field_name
             process_method_name = '_process' + field_name
             if not hasattr(self, process_method_name):
                 continue
             getattr(self, process_method_name)()
 
     def check(self):
         for key in itertools.chain(self._get_config_attr_names(),
-                                   self.fields.keys()):
+                                   self.build_fields.keys()):
             field_name = key
             if not key.startswith('_'):
                 field_name = '_' + field_name
             check_method_name = '_check' + field_name
             if not hasattr(self, check_method_name):
                 continue
             getattr(self, check_method_name)()
@@ -118,61 +117,62 @@
         for k in dir(self.__class__):
             if k.startswith('relate_process_') or k.startswith(
                     'relate_check_') or k == 'bundle_errors':
                 attr_names.append(k)
         return attr_names
 
     def __setitem__(self, key, value):
-        if key in self.fields:
-            self.fields[key].input(key, value)
+        if key in self.build_fields:
+            self.check_fields[key] = self.build_fields[key].build(
+                key=key, value=value)
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
     def __getitem__(self, key):
-        if key in self.fields:
-            field = self.fields[key]
+        if key in self.check_fields:
+            field = self.check_fields[key]
             if not field.key:
                 field.key = key
-            return self.fields[key].value
+            return self.check_fields[key].value
         elif key in self.__dict__:
             return self.__dict__[key]
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not have field: {key}")
 
     def __delitem__(self, key):
-        del self.fields[key]
+        del self.check_fields[key]
 
     def __len__(self):
         return len(self.__dict__.keys())
 
     def __iter__(self):
         self._process_and_check()
-        return iter(self.fields)
+        return iter(self.build_fields)
 
     def _process_and_check(self):
         self.process()
         self.check()
 
     def __getattr__(self, name):
         if name in self.__dict__:
             return self.__dict__[name]
         raise AttributeError(f"Use item[{name!r}] to get field value")
 
     def __setattr__(self, name, value):
-        if name in self.__dict__:
+        if name in self.__dict__ or name in ['check_fields']:
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
     def keys(self):  # to dict时优先调用，不会调用__iter__和__len__，但必须实现
         self._process_and_check()
-        return self.fields.keys()
+        return self.build_fields.keys()
 
 
 class BuildCheckField(object):
     def __init__(self, check_field_class, **kwargs):
         self.check_field_class = check_field_class
         self.kwargs = kwargs
```

### Comparing `gggifcheck-0.0.2/gggifcheck/scrapy_ifcheck.py` & `gggifcheck-0.0.3/gggifcheck/scrapy_ifcheck.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,17 +45,28 @@
     def __setattr__(self, name, value):
         if name.startswith('_') or name in ['check_fields']:
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
-    def keys(self):
+    def check_all(self):
+        """
+        进行所有字段检查
+        :return:
+        """
         self._process_and_check()
-        _ = [self[field] for field in self.fields]  # 进行所有字段检查
+        _ = [self[field] for field in self.fields]
+
+    def keys(self):
+        # 不能放在此处验证的原因是scrapy item进入pipeline前有日志打印等操作导致进行
+        # 此处验证，导致如果在pipeline里进行透传时验证不生效，提前检查报错，此处验证放
+        # 在check_all方法中，因此需要手动调用
+        # self._process_and_check()
+        # _ = [self[field] for field in self.fields]  # 进行所有字段检查
         return self._values.keys()
 
     def get_base_value(self, key):
         if key in self.check_fields:
             return self.check_fields[key].base_value
         elif key in self.fields:
             field = self.fields[key]
@@ -64,14 +75,15 @@
                 return build_check_field.build_default(
                     key=key, value=None).base_value
             return self.fields[key] or None
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
+
 if __name__ == '__main__':
     class PostItem(ScrapyCheckItem):
         id = scrapy.Field(
             check_field=fields.MD5CheckField(
                 nullable=False))
         channel = scrapy.Field(
             check_field=fields.IntegerCheckField(nullable=False, min_value=1,
```

### Comparing `gggifcheck-0.0.2/setup.cfg` & `gggifcheck-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6966 6368 6563 6b0d 0a76   = gggifcheck..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
 00000030: 6175 7468 6f72 203d 206b 7573 656e 0d0a  author = kusen..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2068  author_email = h
 00000050: 7531 3139 3435 3432 3139 3640 7171 2e63  u1194542196@qq.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 cda8 d3c3 a1a2 b1e3 bddd a1a2 d7bc  = ..............
 00000080: c8b7 b5c4 d7d6 b7fb b4ae cab1 bce4 bde2  ................
 00000090: cef6 b9a4 bedf 0d0a 6c6f 6e67 5f64 6573  ........long_des
```

