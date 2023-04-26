# Comparing `tmp/rubpy-6.1.2.tar.gz` & `tmp/rubpy-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.1.2.tar", last modified: Mon Apr 24 21:00:50 2023, max compression
+gzip compressed data, was "rubpy-6.1.4.tar", last modified: Tue Apr 25 22:06:43 2023, max compression
```

## Comparing `rubpy-6.1.2.tar` & `rubpy-6.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.953629 rubpy-6.1.2/
--rw-rw-rw-   0        0        0     3347 2023-04-24 21:00:50.953629 rubpy-6.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2207 2023-04-24 00:06:56.000000 rubpy-6.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.875064 rubpy-6.1.2/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-24 20:58:12.000000 rubpy-6.1.2/rubpy/__init__.py
--rw-rw-rw-   0        0        0    32368 2023-04-24 20:56:07.000000 rubpy-6.1.2/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.890685 rubpy-6.1.2/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.906332 rubpy-6.1.2/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.2/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.2/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 rubpy-6.1.2/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.937967 rubpy-6.1.2/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.1.2/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.937967 rubpy-6.1.2/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.953629 rubpy-6.1.2/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.2/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.2/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:00:50.890685 rubpy-6.1.2/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3347 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 21:00:50.000000 rubpy-6.1.2/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 21:00:50.953629 rubpy-6.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-04-24 20:58:39.000000 rubpy-6.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.134875 rubpy-6.1.4/
+-rw-rw-rw-   0        0        0     3347 2023-04-25 22:06:43.134875 rubpy-6.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2207 2023-04-24 00:06:56.000000 rubpy-6.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.102124 rubpy-6.1.4/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-25 22:06:08.000000 rubpy-6.1.4/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    41245 2023-04-25 22:02:49.000000 rubpy-6.1.4/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.117780 rubpy-6.1.4/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.134875 rubpy-6.1.4/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.4/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.4/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 rubpy-6.1.4/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.134875 rubpy-6.1.4/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.1.4/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.134875 rubpy-6.1.4/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.134875 rubpy-6.1.4/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.4/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.4/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:06:43.117780 rubpy-6.1.4/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-04-25 22:06:42.000000 rubpy-6.1.4/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-25 22:06:42.000000 rubpy-6.1.4/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:06:42.000000 rubpy-6.1.4/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-25 22:06:42.000000 rubpy-6.1.4/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-25 22:06:42.000000 rubpy-6.1.4/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 22:06:43.134875 rubpy-6.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-25 22:05:39.000000 rubpy-6.1.4/setup.py
```

### Comparing `rubpy-6.1.2/PKG-INFO` & `rubpy-6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.2
+Version: 6.1.4
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.2 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.4 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.2/README.md` & `rubpy-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/client.py` & `rubpy-6.1.4/rubpy/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import io
+import aiofiles
 import logging
 from .crypto import Crypto
 from .structs import Struct
 from . import __name__ as logger_name
 from .network import Connection, Proxies
 from .gadgets import exceptions, methods, thumbnail
 from .sessions import StringSession, SQLiteSession
@@ -474,14 +476,268 @@
         return await self(
             methods.messages.SendMessage(
                 object_guid,
                 message=message,
                 file_inline=file_inline,
                 reply_to_message_id=reply_to_message_id))
 
+    async def send_photo(self,
+        object_guid: str,
+        photo: bytes,
+        caption: str = None,
+        file_name: str = None,
+        width: int = None,
+        height: int = None,
+        thumb: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(photo) != bytes:
+            async with aiofiles.open(photo, 'rb') as file:
+                file_name = os.path.basename(photo)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                photo = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        thumb = thumbnail.MakeThumbnail(photo)
+
+        file_inline = await self.upload(photo, *args, **kwargs)
+        file_inline['type'] = 'Image'
+
+        if thumb and width and height != None:
+            file_inline['width'] = width
+            file_inline['height'] = height
+            file_inline['thumb_inline'] = thumb
+        else:
+            if isinstance(thumb, thumbnail.Thumbnail):
+                file_inline['width'] = thumb.width
+                file_inline['height'] = thumb.height
+                file_inline['thumb_inline'] = thumb.to_base64()
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_file(self,
+        object_guid: str,
+        file: bytes,
+        caption: str = None,
+        file_name: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(file) != bytes:
+            async with aiofiles.open(file, 'rb') as ofile:
+                file_name = os.path.basename(file)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await ofile.read()
+                await ofile.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(file, *args, **kwargs)
+        file_inline['type'] = 'File'
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_gif(self,
+        object_guid: str,
+        gif: bytes,
+        caption: str = None,
+        file_name: str = None,
+        thumb: str = None,
+        time: str = None,
+        width: int = None,
+        height: int = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(gif) != bytes:
+            async with aiofiles.open(gif, 'rb') as file:
+                file_name = os.path.basename(gif)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(gif, *args, **kwargs)
+        file_inline['type'] = 'Gif'
+
+        thumb = thumbnail.MakeThumbnail.from_video(gif)
+
+        if thumb and width and height and time != None:
+            file_inline['width'] = width
+            file_inline['height'] = height
+            file_inline['thumb_inline'] = thumb
+            file_inline['time'] = time
+        else:
+            if isinstance(thumb, thumbnail.Thumbnail):
+                file_inline['time'] = thumb.seconds
+                file_inline['width'] = thumb.width
+                file_inline['height'] = thumb.height
+                file_inline['thumb_inline'] = thumb.to_base64()
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_video(self,
+        object_guid: str,
+        video: bytes,
+        caption: str = None,
+        file_name: str = None,
+        thumb: str = None,
+        time: str = None,
+        width: int = None,
+        height: int = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(video) != bytes:
+            async with aiofiles.open(video, 'rb') as file:
+                file_name = os.path.basename(video)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(video, *args, **kwargs)
+        file_inline['type'] = 'Video'
+
+        thumb = thumbnail.MakeThumbnail.from_video(video)
+
+        if thumb and width and height and time != None:
+            file_inline['width'] = width
+            file_inline['height'] = height
+            file_inline['thumb_inline'] = thumb
+            file_inline['time'] = time
+        else:
+            if isinstance(thumb, thumbnail.Thumbnail):
+                file_inline['time'] = thumb.seconds
+                file_inline['width'] = thumb.width
+                file_inline['height'] = thumb.height
+                file_inline['thumb_inline'] = thumb.to_base64()
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_music(self,
+        object_guid: str,
+        music: bytes,
+        caption: str = None,
+        file_name: str = None,
+        time: str = None,
+        music_performer: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(music) != bytes:
+            async with aiofiles.open(music, 'rb') as file:
+                file_name = os.path.basename(music)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(music, *args, **kwargs)
+        file_inline['type'] = 'Music'
+        file_inline['auto_play'] = False
+        file_inline['music_performer'] = kwargs.get('performer', music_performer or '')
+
+        if time != None:
+            file_inline['time'] = time
+        else:
+            file_inline['time'] = '60'
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_voice(self,
+        object_guid: str,
+        music: bytes,
+        caption: str = None,
+        file_name: str = None,
+        time: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(music) != bytes:
+            async with aiofiles.open(music, 'rb') as file:
+                file_name = os.path.basename(music)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(music, *args, **kwargs)
+        file_inline['type'] = 'Voice'
+        file_inline['mime'] = 'ogg'
+        file_inline['auto_play'] = False
+
+        if time != None:
+            file_inline['time'] = time
+        else:
+            file_inline['time'] = '60'
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
     async def edit_message(self, object_guid: str, message_id: str, text: str):
         return await self(methods.messages.EditMessage(object_guid, message_id, text))
 
     async def delete_messages(self, object_guid: str, message_ids: list, type: str = 'Global'):
         return await self(methods.messages.DeleteMessages(object_guid, message_ids, type))
 
     async def request_send_file(self, file_name: str, size: int, mime: str):
```

### Comparing `rubpy-6.1.2/rubpy/crypto/crypto.py` & `rubpy-6.1.4/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/gadgets/classino.py` & `rubpy-6.1.4/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/gadgets/exceptions.py` & `rubpy-6.1.4/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/gadgets/grouping.py` & `rubpy-6.1.4/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/gadgets/methods.py` & `rubpy-6.1.4/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/gadgets/thumbnail.py` & `rubpy-6.1.4/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/network/connection.py` & `rubpy-6.1.4/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/network/proxies.py` & `rubpy-6.1.4/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/sessions/sqliteSession.py` & `rubpy-6.1.4/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/sessions/stringSession.py` & `rubpy-6.1.4/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/structs/handlers.py` & `rubpy-6.1.4/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/structs/models.py` & `rubpy-6.1.4/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/structs/results.py` & `rubpy-6.1.4/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy/structs/struct.py` & `rubpy-6.1.4/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/rubpy.egg-info/PKG-INFO` & `rubpy-6.1.4/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.2
+Version: 6.1.4
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.2 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.4 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.1.2/rubpy.egg-info/SOURCES.txt` & `rubpy-6.1.4/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.2/setup.py` & `rubpy-6.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-requirements = ['aiohttp', 'pycryptodome']
+requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.1.2',
+    version = '6.1.4',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

