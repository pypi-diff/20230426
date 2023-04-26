# Comparing `tmp/vk_maria-3.0.7.tar.gz` & `tmp/vk-maria-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk_maria-3.0.7.tar", last modified: Mon Feb 13 11:37:43 2023, max compression
+gzip compressed data, was "vk-maria-3.0.8.tar", max compression
```

## Comparing `vk_maria-3.0.7.tar` & `vk-maria-3.0.8.tar`

### file list

```diff
@@ -1,64 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:43.017215 vk_maria-3.0.7/
--rw-rw-rw-   0        0        0    35823 2023-02-12 23:36:01.000000 vk_maria-3.0.7/LICENSE
--rw-rw-rw-   0        0        0       38 2023-02-13 01:11:00.000000 vk_maria-3.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2617 2023-02-13 11:37:43.016216 vk_maria-3.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-02-12 23:36:01.000000 vk_maria-3.0.7/README.md
--rw-rw-rw-   0        0        0     2014 2023-02-12 23:36:01.000000 vk_maria-3.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-02-13 11:37:43.017215 vk_maria-3.0.7/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-02-13 11:37:40.000000 vk_maria-3.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.939212 vk_maria-3.0.7/tests/
--rw-rw-rw-   0        0        0     1653 2023-02-12 23:36:01.000000 vk_maria-3.0.7/tests/test_api_method.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.950213 vk_maria-3.0.7/vk_maria/
--rw-rw-rw-   0        0        0       65 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/__init__.py
--rw-rw-rw-   0        0        0    78923 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/api.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.970212 vk_maria-3.0.7/vk_maria/dispatcher/
--rw-rw-rw-   0        0        0       36 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/__init__.py
--rw-rw-rw-   0        0        0     4899 2023-02-12 23:47:37.000000 vk_maria-3.0.7/vk_maria/dispatcher/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.974214 vk_maria-3.0.7/vk_maria/dispatcher/filters/
--rw-rw-rw-   0        0        0       24 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/filters/__init__.py
--rw-rw-rw-   0        0        0     6207 2023-02-12 23:45:00.000000 vk_maria-3.0.7/vk_maria/dispatcher/filters/filters.py
--rw-rw-rw-   0        0        0     1320 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/filters/handler.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.977213 vk_maria-3.0.7/vk_maria/dispatcher/fsm/
--rw-rw-rw-   0        0        0      198 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/state.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.980212 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/
--rw-rw-rw-   0        0        0      154 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/__init__.py
--rw-rw-rw-   0        0        0     5835 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/core.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.986213 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/
--rw-rw-rw-   0        0        0       97 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/__init__.py
--rw-rw-rw-   0        0        0      623 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/base.py
--rw-rw-rw-   0        0        0      794 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/json.py
--rw-rw-rw-   0        0        0      624 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/pickle.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.989212 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/memory/
--rw-rw-rw-   0        0        0       35 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/memory/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/memory/memory.py
--rw-rw-rw-   0        0        0     1054 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.992213 vk_maria-3.0.7/vk_maria/longpoll/
--rw-rw-rw-   0        0        0       32 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/longpoll/__init__.py
--rw-rw-rw-   0        0        0     1851 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/longpoll/longpoll.py
--rw-rw-rw-   0        0        0      373 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/mixins.py
--rw-rw-rw-   0        0        0     5670 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/responses.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:43.007214 vk_maria-3.0.7/vk_maria/types/
--rw-rw-rw-   0        0        0      372 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/__init__.py
--rw-rw-rw-   0        0        0      348 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/callback_query_event.py
--rw-rw-rw-   0        0        0      949 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/chat.py
--rw-rw-rw-   0        0        0      696 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/event.py
--rw-rw-rw-   0        0        0     1824 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/event_type.py
--rw-rw-rw-   0        0        0     4224 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/keyboard.py
--rw-rw-rw-   0        0        0     2000 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/message.py
--rw-rw-rw-   0        0        0     1194 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/message_event.py
--rw-rw-rw-   0        0        0       97 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/types/state.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:43.014214 vk_maria-3.0.7/vk_maria/upload/
--rw-rw-rw-   0        0        0       26 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/upload/__init__.py
--rw-rw-rw-   0        0        0       52 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/upload/exceptions.py
--rw-rw-rw-   0        0        0     3250 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/upload/upload.py
--rw-rw-rw-   0        0        0      739 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/upload/utils.py
--rw-rw-rw-   0        0        0     4200 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/utils.py
--rw-rw-rw-   0        0        0     7268 2023-02-12 23:36:01.000000 vk_maria-3.0.7/vk_maria/vk_types.py
-drwxrwxrwx   0        0        0        0 2023-02-13 11:37:42.967212 vk_maria-3.0.7/vk_maria.egg-info/
--rw-rw-rw-   0        0        0     2617 2023-02-13 11:37:42.000000 vk_maria-3.0.7/vk_maria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1447 2023-02-13 11:37:42.000000 vk_maria-3.0.7/vk_maria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 11:37:42.000000 vk_maria-3.0.7/vk_maria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-13 00:36:33.000000 vk_maria-3.0.7/vk_maria.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2023-02-13 11:37:42.000000 vk_maria-3.0.7/vk_maria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-13 11:37:42.000000 vk_maria-3.0.7/vk_maria.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35823 2023-02-12 23:36:01.445096 vk-maria-3.0.8/LICENSE
+-rw-r--r--   0        0        0     1080 2023-04-25 19:58:03.440394 vk-maria-3.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2014 2023-02-12 23:36:01.446095 vk-maria-3.0.8/README.rst
+-rw-r--r--   0        0        0       65 2023-02-12 23:36:01.466103 vk-maria-3.0.8/vk_maria/__init__.py
+-rw-r--r--   0        0        0    78923 2023-02-12 23:36:01.468098 vk-maria-3.0.8/vk_maria/api.py
+-rw-r--r--   0        0        0       36 2023-02-12 23:36:01.469105 vk-maria-3.0.8/vk_maria/dispatcher/__init__.py
+-rw-r--r--   0        0        0     4899 2023-02-12 23:47:37.696831 vk-maria-3.0.8/vk_maria/dispatcher/dispatcher.py
+-rw-r--r--   0        0        0       24 2023-02-12 23:36:01.470096 vk-maria-3.0.8/vk_maria/dispatcher/filters/__init__.py
+-rw-r--r--   0        0        0     6207 2023-02-12 23:45:00.152169 vk-maria-3.0.8/vk_maria/dispatcher/filters/filters.py
+-rw-r--r--   0        0        0     1320 2023-02-12 23:36:01.471098 vk-maria-3.0.8/vk_maria/dispatcher/filters/handler.py
+-rw-r--r--   0        0        0      198 2023-02-12 23:36:01.471098 vk-maria-3.0.8/vk_maria/dispatcher/fsm/__init__.py
+-rw-r--r--   0        0        0     2612 2023-02-12 23:36:01.472098 vk-maria-3.0.8/vk_maria/dispatcher/fsm/state.py
+-rw-r--r--   0        0        0      154 2023-02-12 23:36:01.472098 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/__init__.py
+-rw-r--r--   0        0        0     5835 2023-02-12 23:36:01.473098 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/core.py
+-rw-r--r--   0        0        0       97 2023-02-12 23:36:01.474096 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/__init__.py
+-rw-r--r--   0        0        0      623 2023-02-12 23:36:01.474096 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/base.py
+-rw-r--r--   0        0        0      794 2023-02-12 23:36:01.475105 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/json.py
+-rw-r--r--   0        0        0      624 2023-02-12 23:36:01.475105 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/pickle.py
+-rw-r--r--   0        0        0       35 2023-02-12 23:36:01.476097 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/memory/__init__.py
+-rw-r--r--   0        0        0     3072 2023-02-12 23:36:01.476097 vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/memory/memory.py
+-rw-r--r--   0        0        0     1054 2023-02-12 23:36:01.477105 vk-maria-3.0.8/vk_maria/exceptions.py
+-rw-r--r--   0        0        0       32 2023-02-12 23:36:01.477105 vk-maria-3.0.8/vk_maria/longpoll/__init__.py
+-rw-r--r--   0        0        0     1851 2023-02-12 23:36:01.478106 vk-maria-3.0.8/vk_maria/longpoll/longpoll.py
+-rw-r--r--   0        0        0      373 2023-02-12 23:36:01.479097 vk-maria-3.0.8/vk_maria/mixins.py
+-rw-r--r--   0        0        0     5670 2023-02-12 23:36:01.479097 vk-maria-3.0.8/vk_maria/responses.py
+-rw-r--r--   0        0        0      436 2023-04-25 12:08:20.275600 vk-maria-3.0.8/vk_maria/types/__init__.py
+-rw-r--r--   0        0        0      348 2023-02-12 23:36:01.480097 vk-maria-3.0.8/vk_maria/types/callback_query_event.py
+-rw-r--r--   0        0        0      949 2023-02-12 23:36:01.481095 vk-maria-3.0.8/vk_maria/types/chat.py
+-rw-r--r--   0        0        0      696 2023-02-12 23:36:01.481095 vk-maria-3.0.8/vk_maria/types/event.py
+-rw-r--r--   0        0        0     1824 2023-02-12 23:36:01.482105 vk-maria-3.0.8/vk_maria/types/event_type.py
+-rw-r--r--   0        0        0      813 2023-04-25 11:27:30.802933 vk-maria-3.0.8/vk_maria/types/input_file.py
+-rw-r--r--   0        0        0     4224 2023-02-12 23:36:01.483096 vk-maria-3.0.8/vk_maria/types/keyboard.py
+-rw-r--r--   0        0        0     2000 2023-02-12 23:36:01.483096 vk-maria-3.0.8/vk_maria/types/message.py
+-rw-r--r--   0        0        0     1196 2023-04-24 22:39:47.775407 vk-maria-3.0.8/vk_maria/types/message_event.py
+-rw-r--r--   0        0        0       97 2023-02-12 23:36:01.484095 vk-maria-3.0.8/vk_maria/types/state.py
+-rw-r--r--   0        0        0       26 2023-02-12 23:36:01.484095 vk-maria-3.0.8/vk_maria/upload/__init__.py
+-rw-r--r--   0        0        0       52 2023-02-12 23:36:01.485096 vk-maria-3.0.8/vk_maria/upload/exceptions.py
+-rw-r--r--   0        0        0     3125 2023-04-25 19:19:18.007641 vk-maria-3.0.8/vk_maria/upload/upload.py
+-rw-r--r--   0        0        0      264 2023-04-25 19:12:48.112798 vk-maria-3.0.8/vk_maria/upload/utils.py
+-rw-r--r--   0        0        0     4200 2023-02-12 23:36:01.486096 vk-maria-3.0.8/vk_maria/utils.py
+-rw-r--r--   0        0        0     7268 2023-02-12 23:36:01.487096 vk-maria-3.0.8/vk_maria/vk_types.py
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 vk-maria-3.0.8/setup.py
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 vk-maria-3.0.8/PKG-INFO
```

### Comparing `vk_maria-3.0.7/LICENSE` & `vk-maria-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/README.rst` & `vk-maria-3.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/api.py` & `vk-maria-3.0.8/vk_maria/api.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/dispatcher.py` & `vk-maria-3.0.8/vk_maria/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/filters/filters.py` & `vk-maria-3.0.8/vk_maria/dispatcher/filters/filters.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/filters/handler.py` & `vk-maria-3.0.8/vk_maria/dispatcher/filters/handler.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/fsm/state.py` & `vk-maria-3.0.8/vk_maria/dispatcher/fsm/state.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/core.py` & `vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/core.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/base.py` & `vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/base.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/json.py` & `vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/json.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/file/pickle.py` & `vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/file/pickle.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/dispatcher/fsm/storage/memory/memory.py` & `vk-maria-3.0.8/vk_maria/dispatcher/fsm/storage/memory/memory.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/exceptions.py` & `vk-maria-3.0.8/vk_maria/exceptions.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/longpoll/longpoll.py` & `vk-maria-3.0.8/vk_maria/longpoll/longpoll.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/responses.py` & `vk-maria-3.0.8/vk_maria/responses.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/types/chat.py` & `vk-maria-3.0.8/vk_maria/types/chat.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/types/event.py` & `vk-maria-3.0.8/vk_maria/types/event.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/types/event_type.py` & `vk-maria-3.0.8/vk_maria/types/event_type.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/types/keyboard.py` & `vk-maria-3.0.8/vk_maria/types/keyboard.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/types/message.py` & `vk-maria-3.0.8/vk_maria/types/message.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/types/message_event.py` & `vk-maria-3.0.8/vk_maria/types/message_event.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         elif self.from_group:
             kwargs.update(peer_id=self.message.from_id)
 
         return self.vk.messages_send(message=message, **kwargs)
 
     def reply(self, message: str = None, **kwargs):
         kwargs.update(reply_to=self.message.id)
-        return self.answer(message=message, **kwargs)
+        return self.answer(message=message, **kwargs)
```

### Comparing `vk_maria-3.0.7/vk_maria/upload/upload.py` & `vk-maria-3.0.8/vk_maria/upload/upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from os import PathLike
-from typing import Union, List, BinaryIO
+from typing import List
 
-from .utils import open_files
+from .utils import prepare_files
 from ..api import Vk
+from ..types.input_file import InputFile
 
 
 class Upload:
     """
     Класс реализующий загрузку файлов на сервер вк.
     """
+
     def __init__(self, vk: Vk):
         self.vk = vk
         self.method = self.vk.method
 
-    def photo(self, photo: Union[str, bytes, PathLike]):
+    def photo(self, photo: InputFile):
         """Загрузка фотографии, возвращает объект для вставки в сообщение"""
 
-        data = open_files(photo, 'photo')
-
+        files = prepare_files(photo)
         upload = self.vk.photos_get_messages_upload_server()
-        response = self.method(server=upload.upload_url, group_id=upload.group_id, files=data)
+        response = self.method(server=upload.upload_url, group_id=upload.group_id, files=files)
         p = self.vk.photos_save_messages_photo(**response)[0]
 
         return f'photo{p.owner_id}_{p.id}_{p.access_key}'
 
     def set_chat_photo(self,
-                       photo: Union[str, bytes, PathLike],
+                       photo: InputFile,
                        chat_id: int,
                        crop_x: int = None,
                        crop_y: int = None,
                        crop_width: int = None):
         """Установка обложки чата"""
 
-        data = open_files(photo, 'photo')
+        files = prepare_files(photo)
 
         upload_url = self.vk.photos_get_chat_upload_server(
             chat_id=chat_id,
             crop_x=crop_x,
             crop_y=crop_y,
             crop_width=crop_width
         )
 
-        response = self.method(server=upload_url, files=data)
+        response = self.method(server=upload_url, files=files)
 
         return self.vk.messages_set_chat_photo(file=response['response'])
 
     def set_group_cover_photo(self,
-                              photo: Union[str, bytes, PathLike],
+                              photo: InputFile,
                               crop_x: int = None,
                               crop_y: int = None,
                               crop_x2: int = None,
                               crop_y2: int = None):
         """Загрузка и установка обложки сообщества"""
 
-        data = open_files(photo, 'photo')
+        files = prepare_files(photo)
 
         upload_url = self.vk.photos_get_owner_cover_photo_upload_server(
             crop_x=crop_x,
             crop_y=crop_y,
             crop_x2=crop_x2,
             crop_y2=crop_y2
         )
 
-        response = self.method(server=upload_url, files=data)
+        response = self.method(server=upload_url, files=files)
 
         return self.vk.photos_save_owner_cover_photo(response['hash'], response['photo'])
 
     def document(self,
-                 document: Union[str, BinaryIO, PathLike, List[Union[str, BinaryIO, PathLike]]],
+                 document: InputFile,
                  peer_id: int,
                  title: str = None,
                  tags: List[str] = None,
                  return_tags: int = None,
                  type: str = 'doc'):
         """Загрузка документа, возвращает объект для вставки в сообщение"""
 
         if tags:
             tags = ','.join(tags)
 
-        data = open_files(document, 'file')
+        files = prepare_files(document)
 
         upload_url = self.vk.docs_get_messages_upload_server(peer_id=peer_id, type=type)
-        response = self.method(server=upload_url, files=data)
+        response = self.method(server=upload_url, files=files)
         d = self.vk.docs_save(file=response['file'], title=title, tags=tags, return_tags=return_tags)
 
         return f'{d.type}{d.doc["owner_id"]}_{d.doc["id"]}'
```

### Comparing `vk_maria-3.0.7/vk_maria/utils.py` & `vk-maria-3.0.8/vk_maria/utils.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria/vk_types.py` & `vk-maria-3.0.8/vk_maria/vk_types.py`

 * *Files identical despite different names*

### Comparing `vk_maria-3.0.7/vk_maria.egg-info/PKG-INFO` & `vk-maria-3.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-Metadata-Version: 2.1
-Name: vk-maria
-Version: 3.0.7
-Summary: vk bot api framework
-Home-page: https://github.com/lxstvayne/vk_maria
-Author: lxstvayne
-Author-email: lxstv4yne@gmail.com
-License: UNKNOWN
-Keywords: vk bot tools
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-License-File: LICENSE
-
-.. vk_maria documentation master file, created by
-   sphinx-quickstart on Mon Apr  4 14:48:43 2022.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Welcome to vk_maria's documentation!
-====================================
-
-   .. image:: https://img.shields.io/badge/telegram-vk_maria-blue.svg?style=flat-square
-      :target: https://t.me/vk_maria_ru
-      :alt: [Telegram] vk_maria live
-
-   .. image:: https://img.shields.io/pypi/v/vk_maria.svg?style=flat-square
-      :target: https://pypi.python.org/pypi/vk_maria
-      :alt: PyPi Package Version
-
-   .. image:: https://img.shields.io/pypi/dm/vk_maria.svg?style=flat-square
-      :target: https://pypi.python.org/pypi/vk_maria
-      :alt: PyPi Month Downloads
-
-   .. image:: https://pepy.tech/badge/vk-maria
-      :target: https://pepy.tech/project/vk-maria
-      :alt: PyPi Total Downloads
-
-   .. image:: https://img.shields.io/pypi/pyversions/vk_maria.svg?style=flat-square
-      :target: https://pypi.python.org/pypi/vk_maria
-      :alt: Supported python versions
-
-**vk_maria** очень простой фреймворк для создания ботов сообществ `Vk <https://dev.vk.com/reference>`_, написанный на Python 3.8.
-
-Официальные ресурсы vk_maria
-----------------------------
-- Новости: `@vk_maria <https://t.me/vk_maria_ru>`_
-- Чат комьюнити: `@vk_maria_ru <https://t.me/vk_maria_ru_chat>`_
-- Pip: `vk_maria <https://pypi.org/project/vk-maria/>`_
-- Docs: `ReadTheDocs <https://vk-maria.readthedocs.io/ru/latest/>`_
-- Source: `Github репозиторий <https://github.com/lxstvayne/vk_maria>`_
-- Issues/Bug tracker: `Github issues tracker <https://github.com/lxstvayne/vk_maria/issues>`_
-
-Сильные стороны
-----------------
-- Простота и удобство
-- Наличие конечных автоматов (FSM)
-- Типизированная
-
-
+Metadata-Version: 2.1
+Name: vk-maria
+Version: 3.0.8
+Summary: Simple Vk Bot synchronous framework
+License: GPL-3.0
+Keywords: vk,bot,api,framework,wrapper,sync
+Author: lxstvayne
+Requires-Python: >=3.8
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: loguru (>=0.5.3)
+Requires-Dist: pydotdict (>=3.3.11)
+Requires-Dist: requests (>=2.20.1)
+Project-URL: Documentation, https://vk-maria.readthedocs.io/ru/latest/
+Project-URL: Repository, https://github.com/lxstvayne/vk_maria
+Description-Content-Type: text/x-rst
+
+.. vk_maria documentation master file, created by
+   sphinx-quickstart on Mon Apr  4 14:48:43 2022.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+Welcome to vk_maria's documentation!
+====================================
+
+   .. image:: https://img.shields.io/badge/telegram-vk_maria-blue.svg?style=flat-square
+      :target: https://t.me/vk_maria_ru
+      :alt: [Telegram] vk_maria live
+
+   .. image:: https://img.shields.io/pypi/v/vk_maria.svg?style=flat-square
+      :target: https://pypi.python.org/pypi/vk_maria
+      :alt: PyPi Package Version
+
+   .. image:: https://img.shields.io/pypi/dm/vk_maria.svg?style=flat-square
+      :target: https://pypi.python.org/pypi/vk_maria
+      :alt: PyPi Month Downloads
+
+   .. image:: https://pepy.tech/badge/vk-maria
+      :target: https://pepy.tech/project/vk-maria
+      :alt: PyPi Total Downloads
+
+   .. image:: https://img.shields.io/pypi/pyversions/vk_maria.svg?style=flat-square
+      :target: https://pypi.python.org/pypi/vk_maria
+      :alt: Supported python versions
+
+**vk_maria** очень простой фреймворк для создания ботов сообществ `Vk <https://dev.vk.com/reference>`_, написанный на Python 3.8.
+
+Официальные ресурсы vk_maria
+----------------------------
+- Новости: `@vk_maria <https://t.me/vk_maria_ru>`_
+- Чат комьюнити: `@vk_maria_ru <https://t.me/vk_maria_ru_chat>`_
+- Pip: `vk_maria <https://pypi.org/project/vk-maria/>`_
+- Docs: `ReadTheDocs <https://vk-maria.readthedocs.io/ru/latest/>`_
+- Source: `Github репозиторий <https://github.com/lxstvayne/vk_maria>`_
+- Issues/Bug tracker: `Github issues tracker <https://github.com/lxstvayne/vk_maria/issues>`_
+
+Сильные стороны
+----------------
+- Простота и удобство
+- Наличие конечных автоматов (FSM)
+- Типизированная
+
```

