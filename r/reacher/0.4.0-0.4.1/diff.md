# Comparing `tmp/reacher-0.4.0-py2.py3-none-any.whl.zip` & `tmp/reacher-0.4.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8459 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    21950 b- defN 23-Apr-17 17:10 reacher/reacher.py
--rw-rw-r--  2.0 unx     7010 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      374 b- defN 23-Apr-17 17:13 reacher-0.4.0.dist-info/RECORD
-5 files, 29452 bytes uncompressed, 7765 bytes compressed:  73.6%
+Zip file size: 8471 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx    21991 b- defN 23-Apr-24 19:07 reacher/reacher.py
+-rw-rw-r--  2.0 unx     7010 b- defN 23-Apr-26 17:20 reacher-0.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-26 17:20 reacher-0.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-26 17:20 reacher-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      374 b- defN 23-Apr-26 17:20 reacher-0.4.1.dist-info/RECORD
+5 files, 29493 bytes uncompressed, 7777 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.4.0.dist-info/METADATA
+Filename: reacher-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.4.0.dist-info/WHEEL
+Filename: reacher-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.4.0.dist-info/top_level.txt
+Filename: reacher-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.4.0.dist-info/RECORD
+Filename: reacher-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -486,15 +486,15 @@
         )
 
         self._image_name = image_name
         self._build_context = build_context 
 
     def _setup_remote(self):
 
-        super()._setup_remote()
+        super().setup()
 
         self._client.upload(
             self._build_context,
             self.build_path,
         )
 
     def clear(self):
@@ -524,14 +524,16 @@
 
         return r
 
     def build(self):
 
         self.clear()
 
+        self._setup_remote()
+
         self._client.execute_command(
             f"docker build -t {self._build_name} {os.path.join(self.build_path, self._build_context)}",
             stream=True,
         )
 
     def execute_command(
         self,
@@ -662,15 +664,14 @@
                 self.request.send(data)
 
         peername = self.request.getpeername()
         chan.close()
         self.request.close()
         print("Tunnel closed from %r" % (peername,))
 
-
 def forward_tunnel(local_port, remote_host, remote_port, transport):
 
     class SubHander(Handler):
         chain_host = remote_host
         chain_port = remote_port
         ssh_transport = transport
 
@@ -741,28 +742,31 @@
         
         self._threads[-1].start()
 
 
 ## Some helper functions for creating notebooks and tensorboards
 
 def create_notebook(
-        reacher: Reacher,
-        remote_port: int,
-        local_port: int,
-        paramiko: bool = False
-    ):
+    reacher: Reacher,
+    remote_port: int,
+    local_port: int,
+    paramiko: bool = False
+):
+
+    import time 
 
     reacher.execute_command(
         f"jupyter notebook --ip 0.0.0.0 --allow-root --port {remote_port}",
         wrap_in_screen=True,
         named_session="notebook",
         ignore_output=True,
-        timeout=1,
     )
 
+    time.sleep(1)
+
     reacher.add_port_forward(remote_port=remote_port, local_port=local_port, paramiko=paramiko)
 
     r = reacher.execute_command("jupyter notebook list", stream=False, suppress=True)
 
     r = r.replace(str(remote_port), str(local_port))
 
     print(r)
@@ -771,20 +775,23 @@
     reacher: Reacher,
     remote_port: int,
     local_port: int,
     paramiko: bool = False,
     logdir: str = "artifacts"
 ):
     
+    import time 
+    
     reacher.execute_command(f"mkdir -p {logdir}")
 
     reacher.execute_command(
         f"tensorboard --host 0.0.0.0 --port {remote_port} --logdir {logdir}",
         wrap_in_screen=True,
         named_session="tensorboard",
         ignore_output=True,
-        timeout=1,
     )
 
+    time.sleep(1)
+
     reacher.add_port_forward(remote_port=remote_port, local_port=local_port, paramiko=paramiko)
 
     print(f"tensorboard running on\nhttp://0.0.0.0:{local_port}/")
```

## Comparing `reacher-0.4.0.dist-info/METADATA` & `reacher-0.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

