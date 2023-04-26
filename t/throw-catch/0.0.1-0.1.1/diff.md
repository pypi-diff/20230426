# Comparing `tmp/throw_catch-0.0.1-py3-none-any.whl.zip` & `tmp/throw_catch-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4714 bytes, number of entries: 9
+Zip file size: 4703 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-13 05:29 test/__init__.py
 -rw-rw-r--  2.0 unx      766 b- defN 23-Mar-13 05:31 test/test_throw_catch.py
 -rw-rw-r--  2.0 unx       36 b- defN 23-Mar-10 09:15 throw_catch/__init__.py
--rw-rw-r--  2.0 unx     4286 b- defN 23-Mar-13 05:26 throw_catch/src.py
--rwxrwxr-x  2.0 unx     1094 b- defN 23-Mar-13 05:31 throw_catch-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1629 b- defN 23-Mar-13 05:31 throw_catch-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-13 05:31 throw_catch-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Mar-13 05:31 throw_catch-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      709 b- defN 23-Mar-13 05:31 throw_catch-0.0.1.dist-info/RECORD
-9 files, 8629 bytes uncompressed, 3488 bytes compressed:  59.6%
+-rw-rw-r--  2.0 unx     4242 b- defN 23-Apr-26 16:26 throw_catch/src.py
+-rwxrwxr-x  2.0 unx     1094 b- defN 23-Apr-26 16:27 throw_catch-0.1.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1629 b- defN 23-Apr-26 16:27 throw_catch-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-26 16:27 throw_catch-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Apr-26 16:27 throw_catch-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      709 b- defN 23-Apr-26 16:27 throw_catch-0.1.1.dist-info/RECORD
+9 files, 8585 bytes uncompressed, 3477 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: throw_catch/__init__.py
 Comment: 
 
 Filename: throw_catch/src.py
 Comment: 
 
-Filename: throw_catch-0.0.1.dist-info/LICENSE
+Filename: throw_catch-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: throw_catch-0.0.1.dist-info/METADATA
+Filename: throw_catch-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: throw_catch-0.0.1.dist-info/WHEEL
+Filename: throw_catch-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: throw_catch-0.0.1.dist-info/top_level.txt
+Filename: throw_catch-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: throw_catch-0.0.1.dist-info/RECORD
+Filename: throw_catch-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## throw_catch/src.py

```diff
@@ -2,28 +2,29 @@
 import logging
 import orjson
 import traceback
 import datetime
 from typing import Union
 
 
-def throw(payload:dict={}, tag: str="throwed", uri:str=None, routing_key: str="throw_catch", ttl :int=180, **kwargs) -> Union[None, str]:
+def throw(payload:dict={}, tag: str=None, uri: str=None, routing_key: str="throw_catch", ttl :int=180, **kwargs) -> Union[None, str]:
     """ 
     throw [send message to rabbitmq]:
     payload: dict ~ payload data 
     tag: str ~ message tag  
     uri: str ~ rabbitmq uri 
     routing_key: str ~ routing key name   
     ttl: int ~ message time to live (in minutes)
     """
 
     assert bool(payload), "Payload dictionary required" 
     assert isinstance(uri, str) and len(uri) > 0 and len(uri) < 256, "AMQP uri required and must be string" 
-    assert isinstance(routing_key, str) and routing_key.isascii() and len(routing_key) < 256, "Invalid routing key name"  
-    assert isinstance(tag, str) and tag.isascii() and len(tag) > 0 and len(tag) < 256, "Invalid tag name or tag is empty" 
+    assert isinstance(routing_key, str) and routing_key.isascii() and len(routing_key) < 256, "Invalid routing key name" 
+    if tag: 
+        assert isinstance(tag, str) and tag.isascii() and len(tag) < 256, "Invalid tag name" 
     assert isinstance(ttl, int) and ttl >= 0, "TTL message must be positive integer" 
 
     stack = traceback.extract_stack()
     filename, lineno, function_name, code = stack[-2]
 
     connection = None
     channel = None
@@ -60,29 +61,29 @@
     else:
         logging.exception(f"pika channel opening failed connection={connection} channel={channel}")  
 
     if connection:
         connection.close()
 
 
-def catch(tag: str="throwed", uri: str=None, queue: str="throw_catch", count: int=1, **kwargs) -> list[dict]:
+def catch(tag: str=None, uri: str=None, queue: str="throw_catch", count: int=1, **kwargs) -> list[dict]:
     """ 
     catch [get message from rabbitmq]:
     tag:str ~ message tag
     uri: str ~ rabbitmq uri 
     queue:str ~ message queue
     count:int ~ messages num
     """
 
     assert isinstance(uri, str) and len(uri) > 0 and len(uri) < 256, "AMQP uri required and must be string" 
     assert isinstance(queue, str) and queue.isascii() and len(queue) < 256, "Invalid queue name"
-    assert isinstance(tag, str) and tag.isascii() and len(tag) > 0 and len(tag) < 256, "Invalid tag name or tag is empty" 
+    if tag:
+        assert isinstance(tag, str) and tag.isascii() and len(tag) < 256, "Invalid tag name" 
 
     messages = []
-
     connection = pika.BlockingConnection(pika.URLParameters(uri))
     channel = connection.channel()
     channel.queue_declare(queue=queue, durable=False)  
 
     for _ in range(count):
         method_frame, header_frame, body = channel.basic_get(queue)
         if method_frame:
```

## Comparing `throw_catch-0.0.1.dist-info/LICENSE` & `throw_catch-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `throw_catch-0.0.1.dist-info/METADATA` & `throw_catch-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: throw-catch
-Version: 0.0.1
+Version: 0.1.1
 Summary: RabbitMQ throw & catch messages
 Home-page: https://github.com/Sobolev5/throw-catch/
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `throw_catch-0.0.1.dist-info/RECORD` & `throw_catch-0.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_throw_catch.py,sha256=O-RhuC3ArrWOJocbvJsGYN2KcbBoqfTd7VoQU36UUBE,766
 throw_catch/__init__.py,sha256=ENSwYoLTjzkOCeSk72zHeeWvDesglRfuhE2LaENU-XQ,36
-throw_catch/src.py,sha256=JcPMZkw8VFtLqv26yfKhL73SFueq8tyURjKRxhgFrjE,4286
-throw_catch-0.0.1.dist-info/LICENSE,sha256=aMACVoCcmACM4isctBUg72tg_tmTDUiRuN9W2NUS_iU,1094
-throw_catch-0.0.1.dist-info/METADATA,sha256=IkOjSwKts-x6ATycnEGWu78osEE-4Kc5XVlGJfhCo3I,1629
-throw_catch-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-throw_catch-0.0.1.dist-info/top_level.txt,sha256=_LlrG5HXSVklHWM2Hj39pu3CnDhvEuIvcETJ6Ni8B0A,17
-throw_catch-0.0.1.dist-info/RECORD,,
+throw_catch/src.py,sha256=8wXyge1Wti7R3x3QWXTu8nPtSZdJetSd2fJtrBkPFOg,4242
+throw_catch-0.1.1.dist-info/LICENSE,sha256=aMACVoCcmACM4isctBUg72tg_tmTDUiRuN9W2NUS_iU,1094
+throw_catch-0.1.1.dist-info/METADATA,sha256=vIsCGO2rKMd2_BuAiyuz1tRsKJCoPRmvKUtmV_393SU,1629
+throw_catch-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+throw_catch-0.1.1.dist-info/top_level.txt,sha256=_LlrG5HXSVklHWM2Hj39pu3CnDhvEuIvcETJ6Ni8B0A,17
+throw_catch-0.1.1.dist-info/RECORD,,
```

