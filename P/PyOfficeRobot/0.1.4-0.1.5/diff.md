# Comparing `tmp/PyOfficeRobot-0.1.4.tar.gz` & `tmp/PyOfficeRobot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.4.tar", last modified: Tue Apr 18 13:25:54 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.5.tar", last modified: Wed Apr 26 14:22:46 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.4.tar` & `PyOfficeRobot-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.735327 PyOfficeRobot-0.1.4/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     7869 2023-04-18 13:25:54.736329 PyOfficeRobot-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.648998 PyOfficeRobot-0.1.4/PyOfficeRobot/
--rw-rw-rw-   0        0        0      120 2023-04-16 15:36:09.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.697810 PyOfficeRobot-0.1.4/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/file.py
--rw-rw-rw-   0        0        0     1625 2023-04-16 15:41:21.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/test.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.703805 PyOfficeRobot-0.1.4/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    13543 2023-04-18 13:17:17.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.708804 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.719827 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.723812 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.681773 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     7869 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      728 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 13:36:22.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7289 2023-04-02 05:09:27.000000 PyOfficeRobot-0.1.4/README.md
--rw-rw-rw-   0        0        0      785 2023-04-18 13:25:54.738327 PyOfficeRobot-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.734341 PyOfficeRobot-0.1.4/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.4/tests/chat.py
--rw-rw-rw-   0        0        0     1230 2023-04-18 13:15:33.000000 PyOfficeRobot-0.1.4/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.685162 PyOfficeRobot-0.1.5/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     7869 2023-04-26 14:22:46.686158 PyOfficeRobot-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.563447 PyOfficeRobot-0.1.5/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      158 2023-04-23 15:01:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.635623 PyOfficeRobot-0.1.5/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     9290 2023-04-26 14:07:27.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/friend.py
+-rw-rw-rw-   0        0        0     1625 2023-04-16 15:41:21.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/api/test.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.640628 PyOfficeRobot-0.1.5/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13543 2023-04-18 13:17:17.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.652621 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.658623 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.670629 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.605654 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     7869 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      756 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 14:08:10.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       52 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-26 14:22:46.000000 PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7289 2023-04-02 05:09:27.000000 PyOfficeRobot-0.1.5/README.md
+-rw-rw-rw-   0        0        0      807 2023-04-26 14:22:46.689164 PyOfficeRobot-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:22:46.683161 PyOfficeRobot-0.1.5/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.5/tests/chat.py
+-rw-rw-rw-   0        0        0     1230 2023-04-18 13:15:33.000000 PyOfficeRobot-0.1.5/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.4/LICENSE` & `PyOfficeRobot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/PKG-INFO` & `PyOfficeRobot-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.4 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.5 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.5/PyOfficeRobot/api/chat.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.5/PyOfficeRobot/api/file.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot/api/test.py` & `PyOfficeRobot-0.1.5/PyOfficeRobot/api/test.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.5/PyOfficeRobot/core/WeChatType.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.5/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.4 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.5 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.5/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 PyOfficeRobot.egg-info/dependency_links.txt
 PyOfficeRobot.egg-info/not-zip-safe
 PyOfficeRobot.egg-info/requires.txt
 PyOfficeRobot.egg-info/top_level.txt
 PyOfficeRobot/api/__init__.py
 PyOfficeRobot/api/chat.py
 PyOfficeRobot/api/file.py
+PyOfficeRobot/api/friend.py
 PyOfficeRobot/api/test.py
 PyOfficeRobot/core/WeChatType.py
 PyOfficeRobot/core/__init__.py
 PyOfficeRobot/lib/CONST.py
 PyOfficeRobot/lib/__init__.py
 PyOfficeRobot/lib/dec/__init__.py
 PyOfficeRobot/lib/dec/act_dec.py
```

### Comparing `PyOfficeRobot-0.1.4/README.md` & `PyOfficeRobot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.4/setup.cfg` & `PyOfficeRobot-0.1.5/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
+00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -35,16 +35,17 @@
 00000220: 6f6d 2f43 6f64 6572 5761 6e46 656e 672f  om/CoderWanFeng/
 00000230: 5079 4f66 6669 6365 526f 626f 740d 0a0d  PyOfficeRobot...
 00000240: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 00000250: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
 00000260: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
 00000270: 200d 0a09 7569 6175 746f 6d61 7469 6f6e   ...uiautomation
 00000280: 0d0a 0973 6368 6564 756c 650d 0a09 7061  ...schedule...pa
-00000290: 6e64 6173 0d0a 0970 6f61 690d 0a70 7974  ndas...poai..pyt
-000002a0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002b0: 3d33 2e36 0d0a 696e 636c 7564 655f 7061  =3.6..include_pa
-000002c0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-000002d0: 650d 0a7a 6970 5f73 6166 6520 3d20 4661  e..zip_safe = Fa
-000002e0: 6c73 650d 0a0d 0a5b 6567 675f 696e 666f  lse....[egg_info
-000002f0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000300: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000310: 0a                                       .
+00000290: 6e64 6173 0d0a 0970 6f61 690d 0a09 7079  ndas...poai...py
+000002a0: 7769 6e33 320d 0a09 7079 7769 6e61 7574  win32...pywinaut
+000002b0: 6f0d 0a70 7974 686f 6e5f 7265 7175 6972  o..python_requir
+000002c0: 6573 203d 203e 3d33 2e36 0d0a 696e 636c  es = >=3.6..incl
+000002d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+000002e0: 203d 2054 7275 650d 0a7a 6970 5f73 6166   = True..zip_saf
+000002f0: 6520 3d20 4661 6c73 650d 0a0d 0a5b 6567  e = False....[eg
+00000300: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000310: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000320: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `PyOfficeRobot-0.1.4/tests/test_file.py` & `PyOfficeRobot-0.1.5/tests/test_file.py`

 * *Files identical despite different names*

