# Comparing `tmp/avplib-1.4.6.tar.gz` & `tmp/avplib-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avplib-1.4.6.tar", last modified: Fri Apr 21 07:17:24 2023, max compression
+gzip compressed data, was "avplib-1.4.7.tar", last modified: Tue Apr 25 17:30:34 2023, max compression
```

## Comparing `avplib-1.4.6.tar` & `avplib-1.4.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 07:17:24.816626 avplib-1.4.6/
--rw-rw-rw-   0        0        0     2295 2023-04-21 07:17:24.816626 avplib-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-03-27 16:06:22.000000 avplib-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 07:17:24.809627 avplib-1.4.6/avplib/
--rw-rw-rw-   0        0        0       97 2023-04-20 19:03:28.000000 avplib-1.4.6/avplib/__init__.py
--rw-rw-rw-   0        0        0    10154 2023-04-20 19:13:39.000000 avplib-1.4.6/avplib/__main__.py
--rw-rw-rw-   0        0        0     2359 2023-04-20 18:38:12.000000 avplib-1.4.6/avplib/avf.py
--rw-rw-rw-   0        0        0     8105 2023-04-20 12:53:03.000000 avplib-1.4.6/avplib/avplib.py
--rw-rw-rw-   0        0        0      275 2023-04-20 18:51:04.000000 avplib-1.4.6/avplib/units.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:17:24.814627 avplib-1.4.6/avplib.egg-info/
--rw-rw-rw-   0        0        0     2295 2023-04-21 07:17:24.000000 avplib-1.4.6/avplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-21 07:17:24.000000 avplib-1.4.6/avplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 07:17:24.000000 avplib-1.4.6/avplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-21 07:17:24.000000 avplib-1.4.6/avplib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 07:17:24.000000 avplib-1.4.6/avplib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 07:17:24.816626 avplib-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1441 2023-04-21 07:17:19.000000 avplib-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:30:34.083849 avplib-1.4.7/
+-rw-rw-rw-   0        0        0     1183 2023-04-25 17:30:34.083849 avplib-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-04-21 17:16:01.000000 avplib-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 17:30:34.076851 avplib-1.4.7/avplib/
+-rw-rw-rw-   0        0        0       97 2023-04-20 19:03:28.000000 avplib-1.4.7/avplib/__init__.py
+-rw-rw-rw-   0        0        0    10154 2023-04-20 19:13:39.000000 avplib-1.4.7/avplib/__main__.py
+-rw-rw-rw-   0        0        0     2359 2023-04-20 18:38:12.000000 avplib-1.4.7/avplib/avf.py
+-rw-rw-rw-   0        0        0     8330 2023-04-25 17:29:15.000000 avplib-1.4.7/avplib/avplib.py
+-rw-rw-rw-   0        0        0     3088 2023-04-22 18:03:58.000000 avplib-1.4.7/avplib/tui.py
+-rw-rw-rw-   0        0        0      275 2023-04-20 18:51:04.000000 avplib-1.4.7/avplib/units.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:30:34.082849 avplib-1.4.7/avplib.egg-info/
+-rw-rw-rw-   0        0        0     1183 2023-04-25 17:30:33.000000 avplib-1.4.7/avplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-04-25 17:30:33.000000 avplib-1.4.7/avplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:30:33.000000 avplib-1.4.7/avplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-25 17:30:33.000000 avplib-1.4.7/avplib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 17:30:33.000000 avplib-1.4.7/avplib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 17:30:34.083849 avplib-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2023-04-25 17:29:44.000000 avplib-1.4.7/setup.py
```

### Comparing `avplib-1.4.6/avplib/__main__.py` & `avplib-1.4.7/avplib/__main__.py`

 * *Files identical despite different names*

### Comparing `avplib-1.4.6/avplib/avf.py` & `avplib-1.4.7/avplib/avf.py`

 * *Files identical despite different names*

### Comparing `avplib-1.4.6/avplib/avplib.py` & `avplib-1.4.7/avplib/avplib.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 import time
 import moviepy.editor as mp
 import soundfile as sf
 from PIL import Image
 from io import BufferedReader, BytesIO
 from tempfile import NamedTemporaryFile
 from threading import Thread
-from multiprocessing import Process, Pipe
-from multiprocessing.connection import PipeConnection
+try: 
+    from multiprocessing import Process, Pipe
+    from multiprocessing.connection import PipeConnection
+    init_multiprocessing = True
+except:
+    init_multiprocessing = False
 # > Typing
 from typing import Literal, Any, Optional, Tuple, List
 # > Local Imports
 from .units import ASCII_CHARS_GRADIENTION, ASCII_CHARS
 
 # > Temp Detected
 class TempDetected:
@@ -89,41 +93,42 @@
             self.pl[idx] = generate_ascii_frame(image_frame, self.frame_size, self.ascii_chars_gradient)
         self.done += 1
         self.callback(self.done, self.frames_count)
     
     def get_acsii_frame(self, idx: int, data: Tuple[bool, Any]) -> None:
         Thread(target=self._gaf, args=(idx, data)).start()
 
-class MultiprocessingFrameHandler:
-    def __init__(self, frames_count: int, frame_size: Tuple[int, int], callback=_callback) -> None:
-        self.frames_count = frames_count
-        self.frame_size = frame_size
-        self.pl = ProgressiveList(frames_count)
-        self.done = 1
-        self.callback = callback
-        
-    @staticmethod
-    def _gaf(connection: PipeConnection) -> None:
-        self: MultiprocessingFrameHandler = connection.recv()
-        idx: int = connection.recv()
-        data: Tuple[bool, Any] = connection.recv()
+if init_multiprocessing:
+    class MultiprocessingFrameHandler:
+        def __init__(self, frames_count: int, frame_size: Tuple[int, int], callback=_callback) -> None:
+            self.frames_count = frames_count
+            self.frame_size = frame_size
+            self.pl = ProgressiveList(frames_count)
+            self.done = 1
+            self.callback = callback
+            
+        @staticmethod
+        def _gaf(connection: PipeConnection) -> None:
+            self: MultiprocessingFrameHandler = connection.recv()
+            idx: int = connection.recv()
+            data: Tuple[bool, Any] = connection.recv()
+            
+            ret, image_frame = data
+            if ret:
+                ac = "".join([ASCII_CHARS_GRADIENTION[pixel] for pixel in Image.fromarray(image_frame).convert("L").resize(self.frame_size).getdata()])
+                self.pl[idx] = "\n".join([ac[index:(index+self.frame_size[0])] for index in range(0, len(ac), self.frame_size[0])])
+            self.done += 1
+            self.callback(self.done, self.frames_count)
         
-        ret, image_frame = data
-        if ret:
-            ac = "".join([ASCII_CHARS_GRADIENTION[pixel] for pixel in Image.fromarray(image_frame).convert("L").resize(self.frame_size).getdata()])
-            self.pl[idx] = "\n".join([ac[index:(index+self.frame_size[0])] for index in range(0, len(ac), self.frame_size[0])])
-        self.done += 1
-        self.callback(self.done, self.frames_count)
-    
-    def get_acsii_frame(self, idx: int, data: Tuple[bool, Any]) -> None:
-        send_conn, recv_conn = Pipe()
-        Process(target=self._gaf, args=(recv_conn,)).start()
-        send_conn.send(self)
-        send_conn.send(idx)
-        send_conn.send(data)
+        def get_acsii_frame(self, idx: int, data: Tuple[bool, Any]) -> None:
+            send_conn, recv_conn = Pipe()
+            Process(target=self._gaf, args=(recv_conn,)).start()
+            send_conn.send(self)
+            send_conn.send(idx)
+            send_conn.send(data)
 
 # > Main Class
 class AVP:
     def __init__(self, fp, ascii_chars: List[str]=ASCII_CHARS) -> None:
         self.ascii_chars_gradient = generate_ascii_chars_gradient(ascii_chars)
         if isinstance(fp, str):
             self.path = os.path.abspath(fp)
```

### Comparing `avplib-1.4.6/setup.py` & `avplib-1.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             elif i.is_file(): files.append(i)
     elif path.is_file(): files.append(path)
     return files
 
 # * This setup
 setuptools.setup(
     name="avplib",
-    version="1.4.6",
+    version="1.4.7",
     description='AVP - ASCII Video Player. Allows you to play any video as ASCII-art.',
     keywords=["avplib"],
     packages=setuptools.find_packages(),
     author_email='semina054@gmail.com',
     url="https://github.com/romanin-rf/avplib",
     long_description=open(os.path.join(os.path.dirname(__file__), 'README.md')).read(),
     long_description_content_type="text/markdown",
```

