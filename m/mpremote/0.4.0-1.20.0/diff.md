# Comparing `tmp/mpremote-0.4.0.tar.gz` & `tmp/mpremote-1.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpremote-0.4.0.tar", last modified: Wed Oct  5 14:03:05 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mpremote-0.4.0.tar` & `mpremote-1.20.0.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-10-05 14:03:05.768424 mpremote-0.4.0/
--rw-r--r--   0 damien    (1000) damien    (1000)     1088 2022-08-08 13:54:01.000000 mpremote-0.4.0/LICENSE
--rw-r--r--   0 damien    (1000) damien    (1000)     3917 2022-10-05 14:03:05.768424 mpremote-0.4.0/PKG-INFO
--rw-r--r--   0 damien    (1000) damien    (1000)     3388 2022-10-02 23:33:14.000000 mpremote-0.4.0/README.md
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-10-05 14:03:05.768424 mpremote-0.4.0/mpremote/
--rw-r--r--   0 damien    (1000) damien    (1000)       22 2022-10-05 14:02:30.000000 mpremote-0.4.0/mpremote/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)       84 2022-08-08 13:54:01.000000 mpremote-0.4.0/mpremote/__main__.py
--rw-r--r--   0 damien    (1000) damien    (1000)     7530 2022-10-05 13:58:12.000000 mpremote-0.4.0/mpremote/commands.py
--rw-r--r--   0 damien    (1000) damien    (1000)     5285 2022-08-08 13:54:01.000000 mpremote-0.4.0/mpremote/console.py
--rw-r--r--   0 damien    (1000) damien    (1000)    16258 2022-10-05 13:58:12.000000 mpremote-0.4.0/mpremote/main.py
--rw-r--r--   0 damien    (1000) damien    (1000)     6091 2022-10-02 23:33:14.000000 mpremote-0.4.0/mpremote/mip.py
--rwxr-xr-x   0 damien    (1000) damien    (1000)    28211 2022-10-05 14:03:02.000000 mpremote-0.4.0/mpremote/pyboard.py
--rw-r--r--   0 damien    (1000) damien    (1000)    20113 2022-08-08 13:54:01.000000 mpremote-0.4.0/mpremote/pyboardextended.py
--rw-r--r--   0 damien    (1000) damien    (1000)     3137 2022-10-05 13:58:12.000000 mpremote-0.4.0/mpremote/repl.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-10-05 14:03:05.768424 mpremote-0.4.0/mpremote.egg-info/
--rw-r--r--   0 damien    (1000) damien    (1000)     3917 2022-10-05 14:03:05.000000 mpremote-0.4.0/mpremote.egg-info/PKG-INFO
--rw-r--r--   0 damien    (1000) damien    (1000)      417 2022-10-05 14:03:05.000000 mpremote-0.4.0/mpremote.egg-info/SOURCES.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        1 2022-10-05 14:03:05.000000 mpremote-0.4.0/mpremote.egg-info/dependency_links.txt
--rw-r--r--   0 damien    (1000) damien    (1000)       48 2022-10-05 14:03:05.000000 mpremote-0.4.0/mpremote.egg-info/entry_points.txt
--rw-r--r--   0 damien    (1000) damien    (1000)       14 2022-10-05 14:03:05.000000 mpremote-0.4.0/mpremote.egg-info/requires.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        9 2022-10-05 14:03:05.000000 mpremote-0.4.0/mpremote.egg-info/top_level.txt
--rw-r--r--   0 damien    (1000) damien    (1000)      104 2022-08-08 13:54:01.000000 mpremote-0.4.0/pyproject.toml
--rw-r--r--   0 damien    (1000) damien    (1000)      710 2022-10-05 14:03:05.768424 mpremote-0.4.0/setup.cfg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/__main__.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/commands.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/console.py
+-rw-r--r--   0        0        0    16258 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/main.py
+-rw-r--r--   0        0        0     6091 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/mip.py
+-rw-r--r--   0        0        0    20264 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/pyboardextended.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/repl.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mpremote-1.20.0/requirements.txt
+-rwxr-xr-x   0        0        0    31437 2020-02-02 00:00:00.000000 mpremote-1.20.0/mpremote/pyboard.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 mpremote-1.20.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mpremote-1.20.0/LICENSE
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 mpremote-1.20.0/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 mpremote-1.20.0/pyproject.toml
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 mpremote-1.20.0/PKG-INFO
```

### Comparing `mpremote-0.4.0/LICENSE` & `mpremote-1.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpremote-0.4.0/PKG-INFO` & `mpremote-1.20.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: mpremote
-Version: 0.4.0
-Summary: Tool for interacting remotely with MicroPython
-Home-page: https://github.com/micropython/micropython
-Author: Damien George
-Author-email: damien@micropython.org
-Project-URL: Bug Tracker, https://github.com/micropython/micropython/issues
-Classifier: Programming Language :: Python :: 3
+Version: 1.20.0
+Summary: Tool for interacting remotely with MicroPython devices
+Project-URL: Homepage, https://github.com/micropython/micropython
+Author-email: Damien George <damien@micropython.org>
+License: MIT
+License-File: LICENSE
+Keywords: hardware,micropython
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.4
+Requires-Dist: importlib-metadata>=1.4
+Requires-Dist: pyserial>=3.3
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # mpremote -- MicroPython remote control
 
 This CLI tool provides an integrated set of utilities to remotely interact with
 and automate a MicroPython device over a serial connection.
 
 The simplest way to use this tool is:
 
     mpremote
 
-This will automatically connect to the device and provide an interactive REPL.
+This will automatically connect to a USB serial port and provide an interactive REPL.
 
 The full list of supported commands are:
 
     mpremote connect <device>         -- connect to given device
                                          device may be: list, auto, id:x, port:x
                                          or any valid device name/path
     mpremote disconnect               -- disconnect current device
```

### Comparing `mpremote-0.4.0/README.md` & `mpremote-1.20.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This CLI tool provides an integrated set of utilities to remotely interact with
 and automate a MicroPython device over a serial connection.
 
 The simplest way to use this tool is:
 
     mpremote
 
-This will automatically connect to the device and provide an interactive REPL.
+This will automatically connect to a USB serial port and provide an interactive REPL.
 
 The full list of supported commands are:
 
     mpremote connect <device>         -- connect to given device
                                          device may be: list, auto, id:x, port:x
                                          or any valid device name/path
     mpremote disconnect               -- disconnect current device
```

### Comparing `mpremote-0.4.0/mpremote/commands.py` & `mpremote-1.20.0/mpremote/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,22 +28,23 @@
                         p.manufacturer,
                         p.product,
                     )
                 )
             # Don't do implicit REPL command.
             state.did_action()
         elif dev == "auto":
-            # Auto-detect and auto-connect to the first available device.
+            # Auto-detect and auto-connect to the first available USB serial port.
             for p in sorted(serial.tools.list_ports.comports()):
-                try:
-                    state.pyb = pyboard.PyboardExtended(p.device, baudrate=115200)
-                    return
-                except pyboard.PyboardError as er:
-                    if not er.args[0].startswith("failed to access"):
-                        raise er
+                if p.vid is not None and p.pid is not None:
+                    try:
+                        state.pyb = pyboard.PyboardExtended(p.device, baudrate=115200)
+                        return
+                    except pyboard.PyboardError as er:
+                        if not er.args[0].startswith("failed to access"):
+                            raise er
             raise pyboard.PyboardError("no device found")
         elif dev.startswith("id:"):
             # Search for a device with the given serial number.
             serial_number = dev[len("id:") :]
             dev = None
             for p in serial.tools.list_ports.comports():
                 if p.serial_number == serial_number:
@@ -117,17 +118,17 @@
 
     command = args.command[0]
     paths = args.path
 
     if command == "cat":
         # Don't be verbose by default when using cat, so output can be
         # redirected to something.
-        verbose = args.verbose == True
+        verbose = args.verbose is True
     else:
-        verbose = args.verbose != False
+        verbose = args.verbose is not False
 
     if command == "cp" and args.recursive:
         if paths[-1] != ":":
             raise CommandError("'cp -r' destination must be ':'")
         paths.pop()
         src_files = []
         for path in paths:
@@ -170,15 +171,15 @@
         src = src.lstrip(":")
         dest_fd, dest = tempfile.mkstemp(suffix=os.path.basename(src))
         try:
             print("edit :%s" % (src,))
             os.close(dest_fd)
             state.pyb.fs_touch(src)
             state.pyb.fs_get(src, dest, progress_callback=show_progress_bar)
-            if os.system("$EDITOR '%s'" % (dest,)) == 0:
+            if os.system('%s "%s"' % (os.getenv("EDITOR"), dest)) == 0:
                 state.pyb.fs_put(dest, src, progress_callback=show_progress_bar)
         finally:
             os.unlink(dest)
 
 
 def _do_execbuffer(state, buf, follow):
     state.ensure_raw_repl()
```

### Comparing `mpremote-0.4.0/mpremote/console.py` & `mpremote-1.20.0/mpremote/console.py`

 * *Files identical despite different names*

### Comparing `mpremote-0.4.0/mpremote/main.py` & `mpremote-1.20.0/mpremote/main.py`

 * *Files identical despite different names*

### Comparing `mpremote-0.4.0/mpremote/mip.py` & `mpremote-1.20.0/mpremote/mip.py`

 * *Files identical despite different names*

### Comparing `mpremote-0.4.0/mpremote/pyboard.py` & `mpremote-1.20.0/mpremote/pyboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,18 +63,21 @@
 
 Or:
 
     python pyboard.py test.py
 
 """
 
+import ast
+import os
+import struct
 import sys
 import time
-import os
-import ast
+
+from collections import namedtuple
 
 try:
     stdout = sys.stdout.buffer
 except AttributeError:
     # Python2 doesn't have buffer attr
     stdout = sys.stdout
 
@@ -82,15 +85,23 @@
 def stdout_write_bytes(b):
     b = b.replace(b"\x04", b"")
     stdout.write(b)
     stdout.flush()
 
 
 class PyboardError(Exception):
-    pass
+    def convert(self, info):
+        if len(self.args) >= 3:
+            if b"OSError" in self.args[2] and b"ENOENT" in self.args[2]:
+                return OSError(errno.ENOENT, info)
+
+        return self
+
+
+listdir_result = namedtuple("dir_result", ["name", "st_mode", "st_ino", "st_size"])
 
 
 class TelnetToSerial:
     def __init__(self, ip, user, password, read_timeout=None):
         self.tn = None
         import telnetlib
 
@@ -271,15 +282,27 @@
             serial_kwargs = {"baudrate": baudrate, "interCharTimeout": 1}
             if serial.__version__ >= "3.3":
                 serial_kwargs["exclusive"] = exclusive
 
             delayed = False
             for attempt in range(wait + 1):
                 try:
-                    self.serial = serial.Serial(device, **serial_kwargs)
+                    if os.name == "nt":
+                        self.serial = serial.Serial(**serial_kwargs)
+                        self.serial.port = device
+                        portinfo = list(serial.tools.list_ports.grep(device))  # type: ignore
+                        if portinfo and portinfo[0].manufacturer != "Microsoft":
+                            # ESP8266/ESP32 boards use RTS/CTS for flashing and boot mode selection.
+                            # DTR False: to avoid using the reset button will hang the MCU in bootloader mode
+                            # RTS False: to prevent pulses on rts on serial.close() that would POWERON_RESET an ESPxx
+                            self.serial.dtr = False  # DTR False = gpio0 High = Normal boot
+                            self.serial.rts = False  # RTS False = EN High = MCU enabled
+                        self.serial.open()
+                    else:
+                        self.serial = serial.Serial(device, **serial_kwargs)
                     break
                 except (OSError, IOError):  # Py2 and Py3 have different errors
                     if wait == 0:
                         continue
                     if attempt == 0:
                         sys.stdout.write("Waiting {} seconds for pyboard ".format(wait))
                         delayed = True
@@ -375,15 +398,15 @@
 
         # return normal and error output
         return data, data_err
 
     def raw_paste_write(self, command_bytes):
         # Read initial header, with window size.
         data = self.serial.read(2)
-        window_size = data[0] | data[1] << 8
+        window_size = struct.unpack("<H", data)[0]
         window_remain = window_size
 
         # Write out the command_bytes data.
         i = 0
         while i < len(command_bytes):
             while window_remain == 0 or self.serial.inWaiting():
                 data = self.serial.read(1)
@@ -452,19 +475,25 @@
         if data != b"OK":
             raise PyboardError("could not exec command (response: %r)" % data)
 
     def exec_raw(self, command, timeout=10, data_consumer=None):
         self.exec_raw_no_follow(command)
         return self.follow(timeout, data_consumer)
 
-    def eval(self, expression):
-        ret = self.exec_("print({})".format(expression))
-        ret = ret.strip()
-        return ret
+    def eval(self, expression, parse=False):
+        if parse:
+            ret = self.exec_("print(repr({}))".format(expression))
+            ret = ret.strip()
+            return ast.literal_eval(ret.decode())
+        else:
+            ret = self.exec_("print({})".format(expression))
+            ret = ret.strip()
+            return ret
 
+    # In Python3, call as pyboard.exec(), see the setattr call below.
     def exec_(self, command, data_consumer=None):
         ret, ret_err = self.exec_raw(command, data_consumer=data_consumer)
         if ret_err:
             raise PyboardError("exception", ret, ret_err)
         return ret
 
     def execfile(self, filename):
@@ -487,38 +516,90 @@
         cmd = (
             "import uos\nfor f in uos.ilistdir(%s):\n"
             " print('{:12} {}{}'.format(f[3]if len(f)>3 else 0,f[0],'/'if f[1]&0x4000 else ''))"
             % (("'%s'" % src) if src else "")
         )
         self.exec_(cmd, data_consumer=stdout_write_bytes)
 
+    def fs_listdir(self, src=""):
+        buf = bytearray()
+
+        def repr_consumer(b):
+            buf.extend(b.replace(b"\x04", b""))
+
+        cmd = "import uos\nfor f in uos.ilistdir(%s):\n" " print(repr(f), end=',')" % (
+            ("'%s'" % src) if src else ""
+        )
+        try:
+            buf.extend(b"[")
+            self.exec_(cmd, data_consumer=repr_consumer)
+            buf.extend(b"]")
+        except PyboardError as e:
+            raise e.convert(src)
+
+        return [
+            listdir_result(*f) if len(f) == 4 else listdir_result(*(f + (0,)))
+            for f in ast.literal_eval(buf.decode())
+        ]
+
+    def fs_stat(self, src):
+        try:
+            self.exec_("import uos")
+            return os.stat_result(self.eval("uos.stat(%s)" % (("'%s'" % src)), parse=True))
+        except PyboardError as e:
+            raise e.convert(src)
+
     def fs_cat(self, src, chunk_size=256):
         cmd = (
             "with open('%s') as f:\n while 1:\n"
             "  b=f.read(%u)\n  if not b:break\n  print(b,end='')" % (src, chunk_size)
         )
         self.exec_(cmd, data_consumer=stdout_write_bytes)
 
+    def fs_readfile(self, src, chunk_size=256):
+        buf = bytearray()
+
+        def repr_consumer(b):
+            buf.extend(b.replace(b"\x04", b""))
+
+        cmd = (
+            "with open('%s', 'rb') as f:\n while 1:\n"
+            "  b=f.read(%u)\n  if not b:break\n  print(b,end='')" % (src, chunk_size)
+        )
+        try:
+            self.exec_(cmd, data_consumer=repr_consumer)
+        except PyboardError as e:
+            raise e.convert(src)
+        return ast.literal_eval(buf.decode())
+
+    def fs_writefile(self, dest, data, chunk_size=256):
+        self.exec_("f=open('%s','wb')\nw=f.write" % dest)
+        while data:
+            chunk = data[:chunk_size]
+            self.exec_("w(" + repr(chunk) + ")")
+            data = data[len(chunk) :]
+        self.exec_("f.close()")
+
     def fs_cp(self, src, dest, chunk_size=256, progress_callback=None):
         if progress_callback:
-            src_size = int(self.exec_("import os\nprint(os.stat('%s')[6])" % src))
+            src_size = self.fs_stat(src).st_size
             written = 0
         self.exec_("fr=open('%s','rb')\nr=fr.read\nfw=open('%s','wb')\nw=fw.write" % (src, dest))
         while True:
             data_len = int(self.exec_("d=r(%u)\nw(d)\nprint(len(d))" % chunk_size))
             if not data_len:
                 break
             if progress_callback:
                 written += data_len
                 progress_callback(written, src_size)
         self.exec_("fr.close()\nfw.close()")
 
     def fs_get(self, src, dest, chunk_size=256, progress_callback=None):
         if progress_callback:
-            src_size = int(self.exec_("import os\nprint(os.stat('%s')[6])" % src))
+            src_size = self.fs_stat(src).st_size
             written = 0
         self.exec_("f=open('%s','rb')\nr=f.read" % src)
         with open(dest, "wb") as f:
             while True:
                 data = bytearray()
                 self.exec_("print(r(%u))" % chunk_size, data_consumer=lambda d: data.extend(d))
                 assert data.endswith(b"\r\n\x04")
@@ -582,23 +663,24 @@
     pyb.close()
 
 
 def filesystem_command(pyb, args, progress_callback=None, verbose=False):
     def fname_remote(src):
         if src.startswith(":"):
             src = src[1:]
-        return src
+        # Convert all path separators to "/", because that's what a remote device uses.
+        return src.replace(os.path.sep, "/")
 
     def fname_cp_dest(src, dest):
         _, src = os.path.split(src)
         if dest is None or dest == "":
             dest = src
         elif dest == ".":
-            dest = os.path.join(".", src)
-        elif dest.endswith(os.path.sep):
+            dest = "./" + src
+        elif dest.endswith("/"):
             dest += src
         return dest
 
     cmd = args[0]
     args = args[1:]
     try:
         if cmd == "cp":
```

### Comparing `mpremote-0.4.0/mpremote/pyboardextended.py` & `mpremote-1.20.0/mpremote/pyboardextended.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,23 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, a, b, c):
         self.close()
 
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        l = self.readline()
+        if not l:
+            raise StopIteration
+        return l
+
     def ioctl(self, request, arg):
         if request == 1:  # FLUSH
             self.flush()
         elif request == 2:  # SEEK
             # This assumes a 32-bit bare-metal machine.
             import machine
             machine.mem32[arg] = self.seek(machine.mem32[arg], machine.mem32[arg + 4])
@@ -424,20 +433,19 @@
             self.wr_u32(int(stat.st_mtime))
             self.wr_u32(int(stat.st_ctime))
 
     def do_ilistdir_start(self):
         path = self.root + self.rd_str()
         try:
             self.path_check(path)
+            self.data_ilistdir[0] = path
+            self.data_ilistdir[1] = os.listdir(path)
             self.wr_s8(0)
         except OSError as er:
             self.wr_s8(-abs(er.errno))
-        else:
-            self.data_ilistdir[0] = path
-            self.data_ilistdir[1] = os.listdir(path)
 
     def do_ilistdir_next(self):
         if self.data_ilistdir[1]:
             entry = self.data_ilistdir[1].pop(0)
             try:
                 stat = os.lstat(self.data_ilistdir[0] + "/" + entry)
                 mode = stat.st_mode & 0xC000
```

### Comparing `mpremote-0.4.0/mpremote/repl.py` & `mpremote-1.20.0/mpremote/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def do_repl_main_loop(state, console_in, console_out_write, *, code_to_inject, file_to_inject):
     while True:
         console_in.waitchar(state.pyb.serial)
         c = console_in.readchar()
         if c:
-            if c == b"\x1d":  # ctrl-], quit
+            if c in (b"\x1d", b"\x18"):  # ctrl-] or ctrl-x, quit
                 break
             elif c == b"\x04":  # ctrl-D
                 # special handling needed for ctrl-D if filesystem is mounted
                 state.pyb.write_ctrl_d(console_out_write)
             elif c == b"\x0a" and code_to_inject is not None:  # ctrl-j, inject code
                 state.pyb.serial.write(code_to_inject)
             elif c == b"\x0b" and file_to_inject is not None:  # ctrl-k, inject script
@@ -52,15 +52,15 @@
     state.did_action()
 
     capture_file = args.capture
     code_to_inject = args.inject_code
     file_to_inject = args.inject_file
 
     print("Connected to MicroPython at %s" % state.pyb.device_name)
-    print("Use Ctrl-] to exit this shell")
+    print("Use Ctrl-] or Ctrl-x to exit this shell")
     if capture_file is not None:
         print('Capturing session to file "%s"' % capture_file)
         capture_file = open(capture_file, "wb")
     if code_to_inject is not None:
         code_to_inject = bytes(code_to_inject.replace("\\n", "\r\n"), "utf8")
         print("Use Ctrl-J to inject", code_to_inject)
     if file_to_inject is not None:
```

