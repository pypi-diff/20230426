# Comparing `tmp/xhs-0.1.4.tar.gz` & `tmp/xhs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.4.tar", last modified: Sat Apr 22 15:40:18 2023, max compression
+gzip compressed data, was "xhs-0.1.5.tar", last modified: Tue Apr 25 14:08:23 2023, max compression
```

## Comparing `xhs-0.1.4.tar` & `xhs-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-22 15:40:06.000000 xhs-0.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-22 15:40:06.000000 xhs-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-22 15:40:06.000000 xhs-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-22 15:40:18.186189 xhs-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-22 15:40:06.000000 xhs-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 15:40:06.000000 xhs-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-22 15:40:18.186189 xhs-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-22 15:40:06.000000 xhs-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 15:40:06.000000 xhs-0.1.4/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-22 15:40:06.000000 xhs-0.1.4/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:18.186189 xhs-0.1.4/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 15:40:18.000000 xhs-0.1.4/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.763887 xhs-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-25 14:08:10.000000 xhs-0.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 14:08:10.000000 xhs-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 14:08:10.000000 xhs-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-25 14:08:23.763887 xhs-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 14:08:10.000000 xhs-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 14:08:10.000000 xhs-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-25 14:08:23.763887 xhs-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-25 14:08:10.000000 xhs-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.759887 xhs-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.763887 xhs-0.1.5/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.763887 xhs-0.1.5/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.4/CHANGELOG.md` & `xhs-0.1.5/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.5
+
+### Fixed
+
+- fix get_user_all_notes lose note time and last_update_time
+
 ## 0.1.4
 
-### ADD
+### Added
 
 - add get user like notes
 - add get user collect notes
 
 ## 0.1.3
 
-### ADD
+### Added
 
 - add get note comments
 - add get note sub comments
 - add get note all comments
 
 ## 0.1.2
 
-### ADD
+### Added
 
 - add get user all notes
 
 ### Changed
 
 - change properties setter getter
 
 ## 0.1.1
 
-### ADD
+### Added
 
 - add search sort and note_type args
 
-### FIX
+### Fixed
 
 - fix save file error when invalid title
 
 ## 0.1.0
 
-### ADD
+### Added
 
 - add comment note api
 - add delete note comment api
 - add comment user api
 - add follow user api
 - add unfollow user api
 - add collect note api
@@ -57,34 +63,34 @@
 - add dislike comment api
 - add get qrcode api
 - add check qrcode api
 - add save files from note id api
 
 ## 0.0.4
 
-### ADD
+### Added
 
 - add x-s 、search_id signature
 - add get note by id api
 - add get self info api
 - add get user info api
 - add get home feed api
 - add get note by keyword api
 - add get user notes api
 
 ## 0.0.3
 
-### ADD
+### Added
 
 - add pypi, doc, test ci actions
 
 ## 0.0.2
 
-### ADD
+### Added
 
 - add Sphinx Doc
 
 ## 0.0.1
 
-### ADD
+### Added
 
 - Structuring project (base on [Structuring Your Project](https://docs.python-guide.org/writing/structure/))
```

### Comparing `xhs-0.1.4/LICENSE` & `xhs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.4/PKG-INFO` & `xhs-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.4
+Version: 0.1.5
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xhs-0.1.4/README.md` & `xhs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.1.4/setup.py` & `xhs-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.4/tests/__init__.py` & `xhs-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.4/tests/test_help.py` & `xhs-0.1.5/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.4/tests/test_xhs.py` & `xhs-0.1.5/tests/test_xhs.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     data = xhs_client.get_user_notes(user_id)
     beauty_print(data)
     assert len(data["notes"]) > 0
 
 
 @pytest.mark.skip(reason="it take much request and time")
 def test_get_user_all_notes(xhs_client: XhsClient):
-    user_id = "5c2766b500000000050283f1"
+    user_id = "63273a77000000002303cc9b"
     notes = xhs_client.get_user_all_notes(user_id, 0)
     beauty_print(notes)
 
 
 def test_get_note_comments(xhs_client: XhsClient):
     note_id = "63db8819000000001a01ead1"
     comments = xhs_client.get_note_comments(note_id)
```

### Comparing `xhs-0.1.4/xhs/core.py` & `xhs-0.1.5/xhs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     video_url: str
     tag_list: list
     at_user_list: list
     collected_count: str
     comment_count: str
     liked_count: str
     share_count: str
+    time: int
+    last_update_time: int
 
 
 def download_file(url: str, filename: str):
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(filename, 'wb') as f:
             for chunk in r.iter_content(chunk_size=8192):
@@ -346,14 +348,16 @@
                     video_url=self._get_video_url_from_note(note),
                     tag_list=note["tag_list"],
                     at_user_list=note["at_user_list"],
                     collected_count=interact_info["collected_count"],
                     comment_count=interact_info["comment_count"],
                     liked_count=interact_info["liked_count"],
                     share_count=interact_info["share_count"],
+                    time=note["time"],
+                    last_update_time=note["last_update_time"],
                 )
                 result.append(note_info)
                 time.sleep(crawl_interval)
         return result
 
     def get_note_comments(self, note_id: str, cursor: str = ""):
         """get note comments
```

### Comparing `xhs-0.1.4/xhs/help.py` & `xhs-0.1.5/xhs/help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.4/xhs.egg-info/PKG-INFO` & `xhs-0.1.5/xhs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.4
+Version: 0.1.5
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

