# Comparing `tmp/zigpy-cli-1.0.3.tar.gz` & `tmp/zigpy-cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-cli-1.0.3.tar", last modified: Fri Mar 31 19:12:10 2023, max compression
+gzip compressed data, was "zigpy-cli-1.0.4.tar", last modified: Wed Apr 26 20:48:03 2023, max compression
```

## Comparing `zigpy-cli-1.0.3.tar` & `zigpy-cli-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:12:10.853282 zigpy-cli-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-03-31 19:12:10.853282 zigpy-cli-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-31 19:11:58.000000 zigpy-cli-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:12:10.853282 zigpy-cli-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:12:10.853282 zigpy-cli-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/tests/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:12:10.853282 zigpy-cli-1.0.3/zigpy_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/ota.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-03-31 19:11:57.000000 zigpy-cli-1.0.3/zigpy_cli/radio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:12:10.853282 zigpy-cli-1.0.3/zigpy_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-03-31 19:12:10.000000 zigpy-cli-1.0.3/zigpy_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-31 19:12:10.000000 zigpy-cli-1.0.3/zigpy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:12:10.000000 zigpy-cli-1.0.3/zigpy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-31 19:12:10.000000 zigpy-cli-1.0.3/zigpy_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-31 19:12:10.000000 zigpy-cli-1.0.3/zigpy_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 19:12:10.000000 zigpy-cli-1.0.3/zigpy_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:48:03.008741 zigpy-cli-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-04-26 20:48:03.008741 zigpy-cli-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:48:03.008741 zigpy-cli-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:48:03.008741 zigpy-cli-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/tests/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:48:03.008741 zigpy-cli-1.0.4/zigpy_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/ota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-26 20:47:53.000000 zigpy-cli-1.0.4/zigpy_cli/radio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:48:03.008741 zigpy-cli-1.0.4/zigpy_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-04-26 20:48:02.000000 zigpy-cli-1.0.4/zigpy_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 20:48:03.000000 zigpy-cli-1.0.4/zigpy_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:48:03.000000 zigpy-cli-1.0.4/zigpy_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 20:48:03.000000 zigpy-cli-1.0.4/zigpy_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-26 20:48:03.000000 zigpy-cli-1.0.4/zigpy_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 20:48:03.000000 zigpy-cli-1.0.4/zigpy_cli.egg-info/top_level.txt
```

### Comparing `zigpy-cli-1.0.3/LICENSE` & `zigpy-cli-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-cli-1.0.3/PKG-INFO` & `zigpy-cli-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unified command line interface for zigpy radios
 Author-email: puddly <puddly3@gmail.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zigpy-cli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `zigpy-cli-1.0.3/README.md` & `zigpy-cli-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-cli-1.0.3/pyproject.toml` & `zigpy-cli-1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 [build-system]
-requires = ["setuptools>=61.0.0"]
+requires = ["setuptools>=61.0.0", "wheel", "setuptools-git-versioning<2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zigpy-cli"
-version = "1.0.3"
+dynamic = ["version"]
 description = "Unified command line interface for zigpy radios"
 urls = {repository = "https://github.com/zigpy/zigpy-cli"}
 authors = [
     {name = "puddly", email = "puddly3@gmail.com"}
 ]
 readme = "README.md"
 license = {text = "GPL-3.0"}
 requires-python = ">=3.8"
 dependencies = [
     "click",
     "coloredlogs",
     "scapy",
-    "zigpy>=0.54.0",
-    "bellows>=0.35.0",
-    "zigpy-deconz>=0.12.0",
-    "zigpy-znp>=0.10.0",
-    "zigpy-xbee>=0.17.0",
+    "zigpy>=0.55.0",
+    "bellows>=0.35.1",
+    "zigpy-deconz>=0.21.0",
+    "zigpy-xbee>=0.18.0",
+    "zigpy-zigate>=0.11.0",
+    "zigpy-znp>=0.11.1"
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*"]
 
 [project.optional-dependencies]
 testing = [
     "pytest>=7.1.2",
     "pytest-asyncio>=0.19.0",
     "pytest-timeout>=2.1.0",
     "pytest-mock>=3.8.2",
     "pytest-cov>=3.0.0",
 ]
 
+[tool.setuptools-git-versioning]
+enabled = true
+
 [project.scripts]
 zigpy = "zigpy_cli.__main__:cli"
 
 
 [tool.ruff]
 select = [
     # Pyflakes
```

### Comparing `zigpy-cli-1.0.3/zigpy_cli/cli.py` & `zigpy-cli-1.0.4/zigpy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `zigpy-cli-1.0.3/zigpy_cli/const.py` & `zigpy-cli-1.0.4/zigpy_cli/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-cli-1.0.3/zigpy_cli/database.py` & `zigpy-cli-1.0.4/zigpy_cli/database.py`

 * *Files identical despite different names*

### Comparing `zigpy-cli-1.0.3/zigpy_cli/ota.py` & `zigpy-cli-1.0.4/zigpy_cli/ota.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,14 +228,26 @@
                 offset = int(zcl["zbee_zcl_general.ota.file.offset"])
                 data = bytes.fromhex(
                     zcl["zbee_zcl_general.ota.image.data"].replace(":", "")
                 )
 
                 ota_chunks[image_key].add((offset, data))
 
+    unknown_sizes = set()
+
+    for key in ota_chunks:
+        if key in ota_sizes:
+            continue
+
+        unknown_sizes.add(key)
+        ota_sizes[key] = max(offset + len(data) for offset, data in ota_chunks[key])
+        LOGGER.error(
+            "Image size for %s not captured, assuming size %s", key, ota_sizes[key]
+        )
+
     for image_key, image_size in ota_sizes.items():
         image_version, image_type, image_manuf_code = image_key
         print(
             f"Constructing image type={image_type}, version={image_version}"
             f", manuf_code={image_manuf_code}: {image_size} bytes"
         )
 
@@ -279,14 +291,15 @@
                 f"Missing {count} bytes starting at offset 0x{start:08X}:"
                 f" filling with 0x{fill_byte:02X}"
             )
             buffer[start : start + count] = [fill_byte] * count
 
         filename = output_root / (
             f"ota_t{image_type}_m{image_manuf_code}_v{image_version}"
+            f"{'_unk_size' if image_key in unknown_sizes else ''}"
             f"{'_partial' if missing_ranges else ''}.ota"
         )
 
         output_root.mkdir(exist_ok=True)
         filename.write_bytes(bytes(buffer))
 
         info.callback([filename])
```

### Comparing `zigpy-cli-1.0.3/zigpy_cli/pcap.py` & `zigpy-cli-1.0.4/zigpy_cli/pcap.py`

 * *Files identical despite different names*

### Comparing `zigpy-cli-1.0.3/zigpy_cli/radio.py` & `zigpy-cli-1.0.4/zigpy_cli/radio.py`

 * *Files 18% similar despite different names*

```diff
@@ -232,41 +232,8 @@
 @click.option("-c", "--channel", type=int)
 @click_coroutine
 async def change_channel(app, channel):
     await app.startup()
 
     LOGGER.info("Current channel is %s", app.state.network_info.channel)
 
-    await zigpy.zdo.broadcast(
-        app=app,
-        command=zigpy.zdo.types.ZDOCmd.Mgmt_NWK_Update_req,
-        grpid=None,
-        radius=0,
-        broadcast_address=zigpy.types.BroadcastAddress.ALL_DEVICES,
-        NwkUpdate=zigpy.zdo.types.NwkUpdate(
-            ScanChannels=zigpy.types.Channels.from_channel_list([channel]),
-            ScanDuration=zigpy.zdo.types.NwkUpdate.CHANNEL_CHANGE_REQ,
-            nwkUpdateId=app.state.network_info.nwk_update_id + 1,
-        ),
-    )
-
-    try:
-        await app.get_device(nwk=0x0000).zdo.Mgmt_NWK_Update_req(
-            zigpy.zdo.types.NwkUpdate(
-                ScanChannels=zigpy.types.Channels.from_channel_list([channel]),
-                ScanDuration=zigpy.zdo.types.NwkUpdate.CHANNEL_CHANGE_REQ,
-                nwkUpdateId=app.state.network_info.nwk_update_id + 1,
-            ),
-        )
-    except asyncio.TimeoutError:
-        pass
-
-    while True:
-        await app.load_network_info()
-
-        LOGGER.info("Channel is currently %s", app.state.network_info.channel)
-
-        if app.state.network_info.channel == channel:
-            break
-
-        LOGGER.info("Waiting...")
-        await asyncio.sleep(3)
+    await app.move_network_to_channel(channel)
```

### Comparing `zigpy-cli-1.0.3/zigpy_cli.egg-info/PKG-INFO` & `zigpy-cli-1.0.4/zigpy_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unified command line interface for zigpy radios
 Author-email: puddly <puddly3@gmail.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zigpy-cli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

