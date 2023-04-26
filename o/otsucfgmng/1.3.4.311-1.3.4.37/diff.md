# Comparing `tmp/otsucfgmng-1.3.4.311.tar.gz` & `tmp/otsucfgmng-1.3.4.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otsucfgmng-1.3.4.311.tar", last modified: Wed Apr 26 00:06:40 2023, max compression
+gzip compressed data, was "otsucfgmng-1.3.4.37.tar", last modified: Wed Apr 26 00:05:37 2023, max compression
```

## Comparing `otsucfgmng-1.3.4.311.tar` & `otsucfgmng-1.3.4.37.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 00:06:40.503190 otsucfgmng-1.3.4.311/
--rw-rw-rw-   0        0        0     1087 2021-09-12 16:41:27.000000 otsucfgmng-1.3.4.311/LICENSE.txt
--rw-rw-rw-   0        0        0    20210 2023-04-26 00:06:40.501194 otsucfgmng-1.3.4.311/PKG-INFO
--rw-rw-rw-   0        0        0    18509 2023-04-26 00:06:23.000000 otsucfgmng-1.3.4.311/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 00:06:40.481383 otsucfgmng-1.3.4.311/otsucfgmng/
--rw-rw-rw-   0        0        0      282 2023-01-15 01:49:53.000000 otsucfgmng-1.3.4.311/otsucfgmng/__init__.py
--rw-rw-rw-   0        0        0    10546 2023-04-26 00:06:23.000000 otsucfgmng-1.3.4.311/otsucfgmng/configuration_manager.py
--rw-rw-rw-   0        0        0     2083 2023-04-26 00:06:23.000000 otsucfgmng-1.3.4.311/otsucfgmng/funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 00:06:40.500165 otsucfgmng-1.3.4.311/otsucfgmng.egg-info/
--rw-rw-rw-   0        0        0    20210 2023-04-26 00:06:40.000000 otsucfgmng-1.3.4.311/otsucfgmng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-26 00:06:40.000000 otsucfgmng-1.3.4.311/otsucfgmng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 00:06:40.000000 otsucfgmng-1.3.4.311/otsucfgmng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 00:06:40.000000 otsucfgmng-1.3.4.311/otsucfgmng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 00:06:40.000000 otsucfgmng-1.3.4.311/otsucfgmng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 00:06:40.503190 otsucfgmng-1.3.4.311/setup.cfg
--rw-rw-rw-   0        0        0      869 2023-04-26 00:06:23.000000 otsucfgmng-1.3.4.311/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 00:05:37.325952 otsucfgmng-1.3.4.37/
+-rw-rw-rw-   0        0        0     1087 2021-09-12 16:41:27.000000 otsucfgmng-1.3.4.37/LICENSE.txt
+-rw-rw-rw-   0        0        0    20207 2023-04-26 00:05:37.324952 otsucfgmng-1.3.4.37/PKG-INFO
+-rw-rw-rw-   0        0        0    18508 2023-04-26 00:02:22.000000 otsucfgmng-1.3.4.37/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 00:05:37.301114 otsucfgmng-1.3.4.37/otsucfgmng/
+-rw-rw-rw-   0        0        0      282 2023-01-15 01:49:53.000000 otsucfgmng-1.3.4.37/otsucfgmng/__init__.py
+-rw-rw-rw-   0        0        0    10629 2023-04-26 00:04:50.000000 otsucfgmng-1.3.4.37/otsucfgmng/configuration_manager.py
+-rw-rw-rw-   0        0        0     2110 2023-04-26 00:02:22.000000 otsucfgmng-1.3.4.37/otsucfgmng/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 00:05:37.323953 otsucfgmng-1.3.4.37/otsucfgmng.egg-info/
+-rw-rw-rw-   0        0        0    20207 2023-04-26 00:05:37.000000 otsucfgmng-1.3.4.37/otsucfgmng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-26 00:05:37.000000 otsucfgmng-1.3.4.37/otsucfgmng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 00:05:37.000000 otsucfgmng-1.3.4.37/otsucfgmng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 00:05:37.000000 otsucfgmng-1.3.4.37/otsucfgmng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 00:05:37.000000 otsucfgmng-1.3.4.37/otsucfgmng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 00:05:37.325952 otsucfgmng-1.3.4.37/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-04-26 00:02:27.000000 otsucfgmng-1.3.4.37/setup.py
```

### Comparing `otsucfgmng-1.3.4.311/LICENSE.txt` & `otsucfgmng-1.3.4.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otsucfgmng-1.3.4.311/PKG-INFO` & `otsucfgmng-1.3.4.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otsucfgmng
-Version: 1.3.4.311
+Version: 1.3.4.37
 Summary: 設定ファイルを扱うクラスを生成するライブラリです。
 Home-page: https://github.com/Otsuhachi/OtsuConfigurationManager.git
 Author: Otsuhachi
 Author-email: agequodagis.tufuiegoeris@gmail.com
 License: MIT License
         
         Copyright (c) 2021 Otsuhachi
@@ -24,15 +24,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: Python ConfigurationManager Configure json
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 - [概要](#概要)
   - [インストール](#インストール)
   - [使い方](#使い方)
   - [メソッド一覧](#メソッド一覧)
@@ -44,15 +44,15 @@
 このライブラリはjson形式の設定ファイルの読み書きを補助するための基底クラスです。  
 `BaseCM`クラスを継承し、`__defaults__`, `<attributes>`を定義するだけで必要な操作を行えるようになります。  
 
 ~~現在~~違うセクションに同じキーを持つような設定ファイルには対応していません。  
 **対応しないことに決定しました。**([理由はこちら](#なぜ異なるセクションで同名キーを持てないようにしましたか？))  
 
 このライブラリは以下の環境で作成されています。
-`Windows10(64bit)`, `Python3.11.1`
+`Windows10(64bit)`, `Python3.7.9`
 
 ```python
 # 違うセクションに同じキーを持つ例
 {
     'app': {'name': 'Hello'},
     'default': {'name': 'Python'}
 }
```

### Comparing `otsucfgmng-1.3.4.311/README.md` & `otsucfgmng-1.3.4.37/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 このライブラリはjson形式の設定ファイルの読み書きを補助するための基底クラスです。  
 `BaseCM`クラスを継承し、`__defaults__`, `<attributes>`を定義するだけで必要な操作を行えるようになります。  
 
 ~~現在~~違うセクションに同じキーを持つような設定ファイルには対応していません。  
 **対応しないことに決定しました。**([理由はこちら](#なぜ異なるセクションで同名キーを持てないようにしましたか？))  
 
 このライブラリは以下の環境で作成されています。
-`Windows10(64bit)`, `Python3.11.1`
+`Windows10(64bit)`, `Python3.7.9`
 
 ```python
 # 違うセクションに同じキーを持つ例
 {
     'app': {'name': 'Hello'},
     'default': {'name': 'Python'}
 }
```

### Comparing `otsucfgmng-1.3.4.311/otsucfgmng/configuration_manager.py` & `otsucfgmng-1.3.4.37/otsucfgmng/configuration_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,46 +4,48 @@
 __all__ = ("BaseCM",)
 
 
 import copy
 import json
 
 from pathlib import Path
-from typing import Any, NoReturn, Self, cast
+from typing import Any, List, NoReturn, cast
 
 from otsutil import OtsuNone, load_json, pathLike, save_json
 from otsuvalidator import CPath
 from otsuvalidator.validators import VBool, VTuple
 
 from .funcs import get_dict_keys_position, support_json_dump
 
 
 class __MetaCM(type):
-    def __new__(cls, name: str, bases: tuple, attrs: dict) -> Self:
+    def __new__(cls, name: str, bases: tuple, attrs: dict):
         excludes = {
             "__module__",
             "__qualname__",
             "__defaults__",
             "__hidden_options__",
             "__annotations__",
             "__doc__",
         }
         attr_keys = set(attrs.keys()) - excludes
-        if (dflt := attrs.get("__defaults__", OtsuNone)) is not OtsuNone:
+        dflt = attrs.get("__defaults__", OtsuNone)
+        if dflt is not OtsuNone:
             dflt = cast(dict, dflt)
             kp: dict = {}
             for k, v, position in get_dict_keys_position(dflt):
                 if k not in attr_keys:
                     msg = f'属性"{k}"は宣言されていません。'
                     raise AttributeError(msg)
                 if kp.get(k, OtsuNone) is not OtsuNone:
                     msg = f'属性"{k}"は異なるセクションに存在しています。'
                     raise AttributeError(msg)
                 kp[k] = position
-            if undefined := attr_keys - set(kp.keys()):
+            undefined = attr_keys - set(kp.keys())
+            if undefined:
                 msg = f"これらの属性の初期値が設定されていません。{undefined}"
                 raise AttributeError(msg)
             attrs["__attr_keys__"] = attr_keys
             attrs["__key_place__"] = kp
             attrs["__user__"] = {}
         return type.__new__(cls, name, bases, attrs)
 
@@ -56,15 +58,15 @@
     拡張子に制約はありませんが、読み込んだ際に辞書形式のjsonである必要があります。
     """
 
     __file__ = CPath(path_type=Path.is_file)
     __hidden_options__ = VTuple(str)
     __export_default_config__ = VBool()
 
-    def __enter__(self) -> Self:
+    def __enter__(self):
         return self
 
     def __exit__(self, *ex) -> bool:
         try:
             self.save_cm(self.__export_default_config__)
             if Any(ex):
                 return False
@@ -83,15 +85,16 @@
         self.__export_default_config__ = export_defautlt_config
         dflt = self.defaults_cm()
         cfu = cast(dict, self.__user__)
         kp = self.key_place_cm
         for k in self.attributes_cm:
             d = dflt
             u = cfu
-            if (place := kp[k]) is not None:
+            place = kp[k]
+            if place is not None:
                 for p in place:
                     d = d[p]
                     if u.get(p, OtsuNone) is OtsuNone:
                         u[p] = {}
                     u = u[p]
             setattr(self, k, d[k])
             setattr(self, f"default_{k}_cm", getattr(self, k))
@@ -127,23 +130,25 @@
 
         Returns:
             str: 設定の文字列。
         """
         if all:
             tmp = {"defaults": copy.deepcopy(self.defaults_cm()), "user": self.user_cm()}
             kp = cast(dict, self.key_place_cm)
-            if (ho := getattr(self, "__hidden_options__", OtsuNone)) is not OtsuNone:
+            ho = getattr(self, "__hidden_options__", OtsuNone)
+            if ho is not OtsuNone:
                 ho = set(cast(tuple, ho))
                 for key in ho:
-                    if (place := kp.get(key, OtsuNone)) is OtsuNone:
+                    place = kp.get(key, OtsuNone)
+                    if place is OtsuNone:
                         continue
                     dflt = tmp["defaults"]
                     user = tmp["user"]
                     if place is not None:
-                        place = cast(list[str], place)
+                        place = cast(List[str], place)
                         for p in place:
                             dflt = dflt[p]
                             user = user[p]
                     if user.get(key, OtsuNone) is OtsuNone:
                         del dflt[key]
         else:
             tmp = self.user_cm()
@@ -173,15 +178,16 @@
             if places is not None:
                 for p in places:
                     d = d.get(p, OtsuNone)  # type: ignore
                     if d is OtsuNone:
                         jsctn = "->".join(places)
                         msg = f"{jsctn}が発見できませんでした。{self.__file__}が正しい形式の設定ファイルか確認してください。"
                         raise KeyError(msg)
-            if (dk := d.get(key, OtsuNone)) is OtsuNone:  # type: ignore
+            dk = d.get(key, OtsuNone)  # type: ignore
+            if dk is OtsuNone:
                 continue
             setattr(self, key, dk)
 
     def save_cm(self, export_defautlt_config: bool = False, **kwargs) -> None:
         """設定ファイルを書き出します。
 
         書き出す項目はユーザが変更を行ったもののみになり、クラス既定の初期設定が書き出されることはありません。
```

### Comparing `otsucfgmng-1.3.4.311/otsucfgmng.egg-info/PKG-INFO` & `otsucfgmng-1.3.4.37/otsucfgmng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otsucfgmng
-Version: 1.3.4.311
+Version: 1.3.4.37
 Summary: 設定ファイルを扱うクラスを生成するライブラリです。
 Home-page: https://github.com/Otsuhachi/OtsuConfigurationManager.git
 Author: Otsuhachi
 Author-email: agequodagis.tufuiegoeris@gmail.com
 License: MIT License
         
         Copyright (c) 2021 Otsuhachi
@@ -24,15 +24,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: Python ConfigurationManager Configure json
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 - [概要](#概要)
   - [インストール](#インストール)
   - [使い方](#使い方)
   - [メソッド一覧](#メソッド一覧)
@@ -44,15 +44,15 @@
 このライブラリはjson形式の設定ファイルの読み書きを補助するための基底クラスです。  
 `BaseCM`クラスを継承し、`__defaults__`, `<attributes>`を定義するだけで必要な操作を行えるようになります。  
 
 ~~現在~~違うセクションに同じキーを持つような設定ファイルには対応していません。  
 **対応しないことに決定しました。**([理由はこちら](#なぜ異なるセクションで同名キーを持てないようにしましたか？))  
 
 このライブラリは以下の環境で作成されています。
-`Windows10(64bit)`, `Python3.11.1`
+`Windows10(64bit)`, `Python3.7.9`
 
 ```python
 # 違うセクションに同じキーを持つ例
 {
     'app': {'name': 'Hello'},
     'default': {'name': 'Python'}
 }
```

### Comparing `otsucfgmng-1.3.4.311/setup.py` & `otsucfgmng-1.3.4.37/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 with open("LICENSE.txt", "r", encoding="utf-8") as f:
     lcs = f.read()
 
-__VERSION__ = "1.3.4.311"
+__VERSION__ = "1.3.4.37"
 
 setup(
     name="otsucfgmng",
     version=__VERSION__,
     url="https://github.com/Otsuhachi/OtsuConfigurationManager.git",
     description="設定ファイルを扱うクラスを生成するライブラリです。",
     long_description_content_type="text/markdown",
@@ -20,9 +20,9 @@
     include_package_data=True,
     license=lcs,
     keywords="Python ConfigurationManager Configure json",
     install_requires=[
         "otsuvalidator",
         "otsutil",
     ],
-    python_requires=">=3.11",
+    python_requires=">=3.7",
 )
```

