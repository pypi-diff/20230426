# Comparing `tmp/pyshark-0.5.3.tar.gz` & `tmp/pyshark-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyshark-0.5.3.tar", last modified: Thu Jul 14 15:41:52 2022, max compression
+gzip compressed data, was "dist/pyshark-0.6.tar", last modified: Wed Apr 26 09:32:54 2023, max compression
```

## Comparing `pyshark-0.5.3.tar` & `pyshark-0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/
--rw-r--r--   0 dorg      (1000) dorg      (1000)       26 2020-05-27 13:39:51.000000 pyshark-0.5.3/MANIFEST.in
--rw-rw-r--   0 dorg      (1000) dorg      (1000)      850 2022-07-14 15:41:52.000000 pyshark-0.5.3/PKG-INFO
--rw-r--r--   0 dorg      (1000) dorg      (1000)      147 2020-05-27 13:39:51.000000 pyshark-0.5.3/README.txt
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)      716 2022-07-09 04:14:30.000000 pyshark-0.5.3/pyshark/__init__.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)      373 2022-06-28 13:02:32.000000 pyshark-0.5.3/pyshark/cache.py
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark/capture/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.5.3/pyshark/capture/__init__.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)    19757 2022-07-08 16:37:33.000000 pyshark-0.5.3/pyshark/capture/capture.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     5396 2022-06-28 07:03:30.000000 pyshark-0.5.3/pyshark/capture/file_capture.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     9188 2022-06-28 07:03:30.000000 pyshark-0.5.3/pyshark/capture/inmem_capture.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     6905 2022-07-09 05:31:23.000000 pyshark-0.5.3/pyshark/capture/live_capture.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     3879 2022-07-14 15:20:57.000000 pyshark-0.5.3/pyshark/capture/live_ring_capture.py
--rw-r--r--   0 dorg      (1000) dorg      (1000)     3090 2022-06-07 11:57:20.000000 pyshark-0.5.3/pyshark/capture/pipe_capture.py
--rw-r--r--   0 dorg      (1000) dorg      (1000)     2785 2022-06-07 10:51:59.000000 pyshark-0.5.3/pyshark/capture/remote_capture.py
--rw-r--r--   0 dorg      (1000) dorg      (1000)      471 2022-06-28 07:13:37.000000 pyshark-0.5.3/pyshark/config.ini
--rw-rw-r--   0 dorg      (1000) dorg      (1000)      517 2022-07-08 16:37:33.000000 pyshark-0.5.3/pyshark/config.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     3072 2022-07-12 15:49:43.000000 pyshark-0.5.3/pyshark/ek_field_mapping.py
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark/packet/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.5.3/pyshark/packet/__init__.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)      797 2022-07-09 05:39:55.000000 pyshark-0.5.3/pyshark/packet/common.py
--rw-r--r--   0 dorg      (1000) dorg      (1000)       34 2020-05-27 13:39:51.000000 pyshark-0.5.3/pyshark/packet/consts.py
--rw-r--r--   0 dorg      (1000) dorg      (1000)     3815 2022-06-07 10:46:28.000000 pyshark-0.5.3/pyshark/packet/fields.py
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark/packet/layers/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.5.3/pyshark/packet/layers/__init__.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     1916 2022-07-09 06:05:05.000000 pyshark-0.5.3/pyshark/packet/layers/base.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     7015 2022-07-09 06:03:26.000000 pyshark-0.5.3/pyshark/packet/layers/ek_layer.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     8386 2022-06-28 07:03:30.000000 pyshark-0.5.3/pyshark/packet/layers/json_layer.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     5186 2022-06-28 07:03:30.000000 pyshark-0.5.3/pyshark/packet/layers/xml_layer.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     4986 2022-06-27 14:17:01.000000 pyshark-0.5.3/pyshark/packet/packet.py
--rw-r--r--   0 dorg      (1000) dorg      (1000)      949 2022-06-07 10:48:06.000000 pyshark-0.5.3/pyshark/packet/packet_summary.py
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark/tshark/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.5.3/pyshark/tshark/__init__.py
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark/tshark/output_parser/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.5.3/pyshark/tshark/output_parser/__init__.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     1337 2022-06-27 14:28:24.000000 pyshark-0.5.3/pyshark/tshark/output_parser/base_parser.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     2127 2022-07-14 15:15:48.000000 pyshark-0.5.3/pyshark/tshark/output_parser/tshark_ek.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     4562 2022-06-27 14:28:24.000000 pyshark-0.5.3/pyshark/tshark/output_parser/tshark_json.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     5086 2022-06-27 14:28:24.000000 pyshark-0.5.3/pyshark/tshark/output_parser/tshark_xml.py
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     5807 2022-07-09 05:27:17.000000 pyshark-0.5.3/pyshark/tshark/tshark.py
-drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark.egg-info/
--rw-rw-r--   0 dorg      (1000) dorg      (1000)      850 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark.egg-info/PKG-INFO
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     1137 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark.egg-info/SOURCES.txt
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        1 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark.egg-info/dependency_links.txt
--rw-rw-r--   0 dorg      (1000) dorg      (1000)       26 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark.egg-info/requires.txt
--rw-rw-r--   0 dorg      (1000) dorg      (1000)        8 2022-07-14 15:41:52.000000 pyshark-0.5.3/pyshark.egg-info/top_level.txt
--rw-rw-r--   0 dorg      (1000) dorg      (1000)       38 2022-07-14 15:41:52.000000 pyshark-0.5.3/setup.cfg
--rw-rw-r--   0 dorg      (1000) dorg      (1000)     1036 2022-07-14 15:41:12.000000 pyshark-0.5.3/setup.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/
+-rw-r--r--   0 dorg      (1000) dorg      (1000)       26 2020-05-27 13:39:51.000000 pyshark-0.6/MANIFEST.in
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      748 2023-04-26 09:32:54.000000 pyshark-0.6/PKG-INFO
+-rw-r--r--   0 dorg      (1000) dorg      (1000)      147 2020-05-27 13:39:51.000000 pyshark-0.6/README.txt
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      716 2022-07-09 04:14:30.000000 pyshark-0.6/pyshark/__init__.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      373 2022-06-28 13:02:32.000000 pyshark-0.6/pyshark/cache.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark/capture/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.6/pyshark/capture/__init__.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)    19659 2023-04-26 09:26:05.000000 pyshark-0.6/pyshark/capture/capture.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     5335 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/capture/file_capture.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     9159 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/capture/inmem_capture.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     6983 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/capture/live_capture.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     4042 2023-04-26 09:26:05.000000 pyshark-0.6/pyshark/capture/live_ring_capture.py
+-rw-r--r--   0 dorg      (1000) dorg      (1000)     3090 2022-06-07 11:57:20.000000 pyshark-0.6/pyshark/capture/pipe_capture.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     2993 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/capture/remote_capture.py
+-rw-r--r--   0 dorg      (1000) dorg      (1000)      471 2022-06-28 07:13:37.000000 pyshark-0.6/pyshark/config.ini
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      517 2022-07-08 16:37:33.000000 pyshark-0.6/pyshark/config.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     3072 2022-07-12 15:49:43.000000 pyshark-0.6/pyshark/ek_field_mapping.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark/packet/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.6/pyshark/packet/__init__.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      941 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/common.py
+-rw-r--r--   0 dorg      (1000) dorg      (1000)       34 2020-05-27 13:39:51.000000 pyshark-0.6/pyshark/packet/consts.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     3809 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/fields.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark/packet/layers/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.6/pyshark/packet/layers/__init__.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     1941 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/layers/base.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     6969 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/layers/ek_layer.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     8374 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/layers/json_layer.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     5202 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/layers/xml_layer.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     4996 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/packet.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      939 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/packet/packet_summary.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark/tshark/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.6/pyshark/tshark/__init__.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark/tshark/output_parser/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        0 2022-07-09 04:06:14.000000 pyshark-0.6/pyshark/tshark/output_parser/__init__.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     1337 2022-06-27 14:28:24.000000 pyshark-0.6/pyshark/tshark/output_parser/base_parser.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     2127 2022-07-14 15:15:48.000000 pyshark-0.6/pyshark/tshark/output_parser/tshark_ek.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     4515 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/tshark/output_parser/tshark_json.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     5120 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/tshark/output_parser/tshark_xml.py
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     6051 2023-04-26 08:54:39.000000 pyshark-0.6/pyshark/tshark/tshark.py
+drwxrwxr-x   0 dorg      (1000) dorg      (1000)        0 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark.egg-info/
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      748 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark.egg-info/PKG-INFO
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)     1137 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        1 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)       33 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark.egg-info/requires.txt
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)        8 2023-04-26 09:32:54.000000 pyshark-0.6/pyshark.egg-info/top_level.txt
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)       38 2023-04-26 09:32:54.000000 pyshark-0.6/setup.cfg
+-rw-rw-r--   0 dorg      (1000) dorg      (1000)      943 2023-04-26 09:32:04.000000 pyshark-0.6/setup.py
```

### Comparing `pyshark-0.5.3/PKG-INFO` & `pyshark-0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 1.1
 Name: pyshark
-Version: 0.5.3
+Version: 0.6
 Summary: Python wrapper for tshark, allowing python packet parsing using wireshark dissectors
 Home-page: https://github.com/KimiNewt/pyshark
 Author: KimiNewt
 Author-email: UNKNOWN
 License: MIT
 Description: Python wrapper for tshark, allowing python packet parsing using wireshark dissectors.
         
         See https://github.com/KimiNewt/pyshark/ for documentation.
         
 Keywords: wireshark capture packets parsing packet
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyshark-0.5.3/pyshark/__init__.py` & `pyshark-0.6/pyshark/__init__.py`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/pyshark/capture/capture.py` & `pyshark-0.6/pyshark/capture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
         self.eventloop = eventloop
         if self.eventloop is None:
             self._setup_eventloop()
         if encryption_type and encryption_type.lower() in self.SUPPORTED_ENCRYPTION_STANDARDS:
             self.encryption = (decryption_key, encryption_type.lower())
         else:
-            raise UnknownEncyptionStandardException("Only the following standards are supported: %s."
-                                                    % ", ".join(self.SUPPORTED_ENCRYPTION_STANDARDS))
+            standards = ", ".join(self.SUPPORTED_ENCRYPTION_STANDARDS)
+            raise UnknownEncyptionStandardException(f"Only the following standards are supported: {standards}.")
 
     def __getitem__(self, item):
         """Gets the packet in the given index.
 
         :param item: packet index
         :return: Packet object.
         """
@@ -169,15 +169,15 @@
         if os.name == "nt":
             current_eventloop = asyncio.get_event_loop_policy().get_event_loop()
             if isinstance(current_eventloop, asyncio.ProactorEventLoop):
                 self.eventloop = current_eventloop
             else:
                 # On Python before 3.8, Proactor is not the default eventloop type, so we have to create a new one.
                 # If there was an existing eventloop this can create issues, since we effectively disable it here.
-                if asyncio.Task.all_tasks():
+                if asyncio.all_tasks():
                     warnings.warn("The running eventloop has tasks but pyshark must set a new eventloop to continue. "
                                   "Existing tasks may not run.")
                 self.eventloop = asyncio.ProactorEventLoop()
                 asyncio.set_event_loop(self.eventloop)
         else:
             try:
                 self.eventloop = asyncio.get_event_loop_policy().get_event_loop()
@@ -338,30 +338,29 @@
         else:
             output_type = "psml" if self._only_summaries else "pdml"
         parameters = [self._get_tshark_path(), "-l", "-n", "-T", output_type] + \
             self.get_parameters(packet_count=packet_count) + output_parameters
 
         self._log.debug(
             "Creating TShark subprocess with parameters: " + " ".join(parameters))
-        self._log.debug("Executable: %s" % parameters[0])
+        self._log.debug("Executable: %s", parameters[0])
         tshark_process = await asyncio.create_subprocess_exec(*parameters,
                                                               stdout=subprocess.PIPE,
                                                               stderr=subprocess.PIPE,
                                                               stdin=stdin)
         self._create_stderr_handling_task(tshark_process.stderr)
         self._created_new_process(parameters, tshark_process)
         return tshark_process
 
     def _created_new_process(self, parameters, process, process_name="TShark"):
         self._log.debug(
             process_name + f" subprocess (pid {process.pid}) created")
         if process.returncode is not None and process.returncode != 0:
             raise TSharkCrashException(
-                "%s seems to have crashed. Try updating it. (command ran: '%s')" % (
-                    process_name, " ".join(parameters)))
+                f"{process_name} seems to have crashed. Try updating it. (command ran: '{' '.join(parameters)}')")
         self._running_processes.add(process)
 
     async def _cleanup_subprocess(self, process):
         """Kill the given process and properly closes any pipes connected to it."""
         self._log.debug(f"Cleanup Subprocess (pid {process.pid})")
         if process.returncode is None:
             try:
@@ -438,16 +437,15 @@
         if all(self.encryption):
             params += ["-o", "wlan.enable_decryption:TRUE", "-o", 'uat:80211_keys:"' + self.encryption[1] + '","' +
                                                                   self.encryption[0] + '"']
         if self._override_prefs:
             for preference_name, preference_value in self._override_prefs.items():
                 if all(self.encryption) and preference_name in ("wlan.enable_decryption", "uat:80211_keys"):
                     continue  # skip if override preferences also given via --encryption options
-                params += ["-o",
-                           "{0}:{1}".format(preference_name, preference_value)]
+                params += ["-o", f"{preference_name}:{preference_value}"]
 
         if self._output_file:
             params += ["-w", self._output_file]
 
         if self._decode_as:
             for criterion, decode_as_proto in self._decode_as.items():
                 params += ["-d",
@@ -461,8 +459,8 @@
     def __iter__(self):
         if self.loaded:
             return iter(self._packets)
         else:
             return self._packets_from_tshark_sync()
 
     def __repr__(self):
-        return "<%s (%d packets)>" % (self.__class__.__name__, len(self._packets))
+        return f"<{self.__class__.__name__} ({len(self._packets)} packets)>"
```

### Comparing `pyshark-0.5.3/pyshark/capture/file_capture.py` & `pyshark-0.6/pyshark/capture/file_capture.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             raise NotImplementedError("Cannot use getitem if packets are not kept")
             # We may not yet have this packet
         while packet_index >= len(self._packets):
             try:
                 self.next()
             except StopIteration:
                 # We read the whole file, and there's still not such packet.
-                raise KeyError("Packet of index %d does not exist in capture" % packet_index)
+                raise KeyError(f"Packet of index {packet_index} does not exist in capture")
         return super(FileCapture, self).__getitem__(packet_index)
 
     def get_parameters(self, packet_count=None):
         return super(FileCapture, self).get_parameters(packet_count=packet_count) + [
             "-r", self.input_filepath.as_posix()]
 
     def _verify_capture_parameters(self):
@@ -84,11 +84,10 @@
             with self.input_filepath.open("rb"):
                 pass
         except PermissionError:
             raise PermissionError(f"Permission denied for file {self.input_filepath}")
 
     def __repr__(self):
         if self.keep_packets:
-            return "<%s %s>" % (self.__class__.__name__, self.input_filepath.as_posix())
+            return f"<{self.__class__.__name__} {self.input_filepath.as_posix()}>"
         else:
-            return "<%s %s (%d packets)>" % (self.__class__.__name__, self.input_filepath.as_posix(),
-                                             len(self._packets))
+            return f"<{self.__class__.__name__} {self.input_filepath.as_posix()} ({len(self._packets)} packets)>"
```

### Comparing `pyshark-0.5.3/pyshark/capture/inmem_capture.py` & `pyshark-0.6/pyshark/capture/inmem_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         """"Returns the separators between packets in a JSON output
 
         Returns a tuple of (packet_separator, end_of_file_separator, characters_to_disregard).
         The latter variable being the number of characters to ignore in order to pass the packet (i.e. extra newlines,
         commas, parenthesis).
         """
         if self._get_tshark_version() >= version.parse("2.6.7"):
-            return ("%s  }" % os.linesep).encode(), ("}%s]" % os.linesep).encode(), 0
+            return f"{os.linesep}  }}".encode(), f"}}{os.linesep}]".encode(), 0
         else:
-            return ("}%s%s" % (os.linesep, os.linesep)).encode(), ("}%s%s]" % (os.linesep, os.linesep)).encode(), 1
+            return f'}}{os.linesep}{os.linesep}'.encode(), f"}}{os.linesep}{os.linesep}]", 1
 
     def _write_packet(self, packet, sniff_time):
         if sniff_time is None:
             now = time.time()
         elif isinstance(sniff_time, datetime.datetime):
             now = sniff_time.timestamp()
         else:
```

### Comparing `pyshark-0.5.3/pyshark/capture/live_capture.py` & `pyshark-0.6/pyshark/capture/live_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         params += ["-i", "-"]
         return params
 
     def _verify_capture_parameters(self):
         all_interfaces_names = tshark.get_all_tshark_interfaces_names(self.tshark_path)
         all_interfaces_lowercase = [interface.lower() for interface in all_interfaces_names]
         for each_interface in self.interfaces:
+            if each_interface.startswith("rpcap://"):
+                continue
             if each_interface.isnumeric():
                 continue
             if each_interface.lower() not in all_interfaces_lowercase:
                 raise UnknownInterfaceException(
                     f"Interface '{each_interface}' does not exist, unable to initiate capture. "
                     f"Perhaps permissions are missing?\n"
                     f"Possible interfaces: {os.linesep.join(all_interfaces_names)}")
@@ -99,15 +101,15 @@
         return params
 
     async def _get_tshark_process(self, packet_count=None, stdin=None):
         read, write = os.pipe()
 
         dumpcap_params = [get_process_path(process_name="dumpcap", tshark_path=self.tshark_path)] + self._get_dumpcap_parameters()
 
-        self._log.debug("Creating Dumpcap subprocess with parameters: %s" % " ".join(dumpcap_params))
+        self._log.debug("Creating Dumpcap subprocess with parameters: %s", " ".join(dumpcap_params))
         dumpcap_process = await asyncio.create_subprocess_exec(*dumpcap_params, stdout=write,
                                                                stderr=subprocess.PIPE)
         self._create_stderr_handling_task(dumpcap_process.stderr)
         self._created_new_process(dumpcap_params, dumpcap_process, process_name="Dumpcap")
 
         tshark = await super(LiveCapture, self)._get_tshark_process(packet_count=packet_count, stdin=read)
         return tshark
```

### Comparing `pyshark-0.5.3/pyshark/capture/live_ring_capture.py` & `pyshark-0.6/pyshark/capture/live_ring_capture.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,7 +46,12 @@
         self.ring_file_name = ring_file_name
 
     def get_parameters(self, packet_count=None):
         params = super(LiveRingCapture, self).get_parameters(packet_count=packet_count)
         params += ['-b', 'filesize:' + str(self.ring_file_size), '-b', 'files:' + str(self.num_ring_files),
                    '-w', self.ring_file_name, '-P', '-V']
         return params
+    
+    def _get_dumpcap_parameters(self):
+        params = super(LiveRingCapture, self)._get_dumpcap_parameters()
+        params += ['-P']
+        return params
```

### Comparing `pyshark-0.5.3/pyshark/capture/pipe_capture.py` & `pyshark-0.6/pyshark/capture/pipe_capture.py`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/pyshark/capture/remote_capture.py` & `pyshark-0.6/pyshark/capture/remote_capture.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 from pyshark import LiveCapture
 
 
 class RemoteCapture(LiveCapture):
     """A capture which is performed on a remote machine which has an rpcapd service running."""
 
-    def __init__(self, remote_host, remote_interface, remote_port=2002, bpf_filter=None, only_summaries=False,
-                 decryption_key=None, encryption_type='wpa-pwk', decode_as=None,
-                 disable_protocol=None,tshark_path=None, override_prefs=None, eventloop=None, debug=False):
+    def __init__(
+        self,
+        remote_host,
+        remote_interface,
+        *args,
+        remote_port=2002,
+        bpf_filter=None,
+        only_summaries=False,
+        decryption_key=None,
+        encryption_type="wpa-pwk",
+        decode_as=None,
+        disable_protocol=None,
+        tshark_path=None,
+        override_prefs=None,
+        eventloop=None,
+        debug=False,
+        **kwargs
+    ):
         """
         Creates a new remote capture which will connect to a remote machine which is running rpcapd. Use the sniff()
         method to get packets.
         Note: The remote machine should have rpcapd running in null authentication mode (-n). Be warned that the traffic
         is unencrypted!
 
+        Note:
+            *args and **kwargs are passed to LiveCature's __init__ method.
+
+
         :param remote_host: The remote host to capture on (IP or hostname). Should be running rpcapd.
         :param remote_interface: The remote interface on the remote machine to capture on. Note that on windows it is
         not the device display name but the true interface name (i.e. \\Device\\NPF_..).
         :param remote_port: The remote port the rpcapd service is listening on
         :param bpf_filter: A BPF (tcpdump) filter to apply on the cap before reading.
         :param only_summaries: Only produce packet summaries, much faster but includes very little information
         :param decryption_key: Key used to encrypt and decrypt captured traffic.
@@ -25,13 +44,23 @@
         :param decode_as: A dictionary of {decode_criterion_string: decode_as_protocol} that are used to tell tshark
         to decode protocols in situations it wouldn't usually, for instance {'tcp.port==8888': 'http'} would make
         it attempt to decode any port 8888 traffic as HTTP. See tshark documentation for details.
         :param tshark_path: Path of the tshark binary
         :param override_prefs: A dictionary of tshark preferences to override, {PREFERENCE_NAME: PREFERENCE_VALUE, ...}.
         :param disable_protocol: Tells tshark to remove a dissector for a specifc protocol.
         """
-        interface = 'rpcap://%s:%d/%s' % (remote_host, remote_port, remote_interface)
-        super(RemoteCapture, self).__init__(interface, bpf_filter=bpf_filter, only_summaries=only_summaries,
-                                            decryption_key=decryption_key, encryption_type=encryption_type,
-                                            tshark_path=tshark_path, decode_as=decode_as,  disable_protocol=disable_protocol,
-                                            override_prefs=override_prefs, eventloop=eventloop,
-                                            debug=debug)
+        interface =  f'rpcap://{remote_host}:{remote_port}/{remote_interface}'
+        super(RemoteCapture, self).__init__(
+            interface,
+            *args,
+            bpf_filter=bpf_filter,
+            only_summaries=only_summaries,
+            decryption_key=decryption_key,
+            encryption_type=encryption_type,
+            tshark_path=tshark_path,
+            decode_as=decode_as,
+            disable_protocol=disable_protocol,
+            override_prefs=override_prefs,
+            eventloop=eventloop,
+            debug=debug,
+            **kwargs
+        )
```

### Comparing `pyshark-0.5.3/pyshark/config.py` & `pyshark-0.6/pyshark/config.py`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/pyshark/ek_field_mapping.py` & `pyshark-0.6/pyshark/ek_field_mapping.py`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/pyshark/packet/common.py` & `pyshark-0.6/pyshark/packet/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+import sys
+import functools
+
+import termcolor
+
+
 class Pickleable(object):
     """
     Base class that implements getstate/setstate, since most of the classes are overriding getattr.
     """
 
     def __getstate__(self):
         return self.__dict__
@@ -20,15 +26,16 @@
         return ret
 
     def __setstate__(self, data):
         for key, val in data.items():
             setattr(self, key, val)
 
 
-class StrWriter:
-    """A class which mocks the py.io.TerminalWriter to write to an internal buffer"""
-
-    def __init__(self):
-        self.buffer = ""
-
-    def write(self, text, *_, **__):
-        self.buffer += text
+@functools.wraps(termcolor.colored)
+def colored(text, *args, **kwargs):
+    try:
+        enable_color = sys.stdout.isatty()
+    except (AttributeError, NotImplementedError, FileNotFoundError):
+        enable_color = False
+    if enable_color:
+        return termcolor.colored(text, *args, **kwargs)
+    return text
```

### Comparing `pyshark-0.5.3/pyshark/packet/fields.py` & `pyshark-0.6/pyshark/packet/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         if hide and hide == 'yes':
             self.hide = True
         else:
             self.hide = False
 
     def __repr__(self):
-        return '<LayerField %s: %s>' % (self.name, self.get_default_value())
+        return f'<LayerField {self.name}: {self.get_default_value()}>'
 
     def get_default_value(self) -> str:
         """Gets the best 'value' string this field has."""
         val = self.show
         if not val:
             val = self.raw_value
         if not val:
```

### Comparing `pyshark-0.5.3/pyshark/packet/layers/base.py` & `pyshark-0.6/pyshark/packet/layers/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import typing
-
-import py
+import io
+import sys
 
 from pyshark.packet import common
 
 DATA_LAYER_NAME = "DATA"
 
 
 class BaseLayer(common.SlotsPickleable):
@@ -46,25 +46,26 @@
         val = self.get_field(item)
         if val is None:
             raise AttributeError(f"{item} does not exist in Layer")
         return val
 
     def pretty_print(self, writer=None):
         if not writer:
-            writer = py.io.TerminalWriter()
+            writer = sys.stdout
         if self.layer_name == DATA_LAYER_NAME:
             writer.write('DATA')
             return
 
-        writer.write('Layer %s:' % self.layer_name.upper() + os.linesep, yellow=True, bold=True)
+        text = f'Layer {self.layer_name.upper()}{os.linesep}:'
+        writer.write(common.colored(text, color="yellow", attrs=["bold"]))
         self._pretty_print_layer_fields(writer)
 
-    def _pretty_print_layer_fields(self, terminal_writer: py.io.TerminalWriter):
+    def _pretty_print_layer_fields(self, terminal_writer: io.IOBase):
         raise NotImplementedError()
 
     def __repr__(self):
-        return '<%s Layer>' % self.layer_name.upper()
+        return f'<{self.layer_name.upper()} Layer>'
 
     def __str__(self):
-        writer = common.StrWriter()
+        writer = io.StringIO()
         self.pretty_print(writer=writer)
-        return writer.buffer
+        return writer.getvalue()
```

### Comparing `pyshark-0.5.3/pyshark/packet/layers/ek_layer.py` & `pyshark-0.6/pyshark/packet/layers/ek_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import os
+import io
 
-import py
 import typing
 
+from pyshark.packet.common import colored
 from pyshark import ek_field_mapping
 from pyshark.packet.layers.base import BaseLayer
 
 
 class _EkLayerHelperFuncsMixin(abc.ABC):
     """For methods shared between the EK layer and sublayers"""
 
@@ -102,32 +103,32 @@
     def _field_has_subfields(self, field_ek_name):
         field_ek_name_with_ext = f"{field_ek_name}_"
         for field_name in self._fields_dict:
             if field_name.startswith(field_ek_name_with_ext):
                 return True
         return False
 
-    def _pretty_print_layer_fields(self, terminal_writer: py.io.TerminalWriter):
+    def _pretty_print_layer_fields(self, file: io.IOBase):
         for field_name in self.field_names:
             field = self.get_field(field_name)
-            self._pretty_print_field(field_name, field, terminal_writer, indent=1)
+            self._pretty_print_field(field_name, field, file, indent=1)
 
-    def _pretty_print_field(self, field_name, field, terminal_writer, indent=0):
+    def _pretty_print_field(self, field_name, field, file, indent=0):
         prefix = "\t" * indent
         if isinstance(field, EkMultiField):
-            terminal_writer.write(f"{prefix}{field_name}: ", green=True, bold=True)
+            file.write(colored(f"{prefix}{field_name}: ", "green", attrs=["bold"]))
             if field.value is not None:
-                terminal_writer.write(str(field.value))
-            terminal_writer.write(os.linesep)
+                file.write(str(field.value))
+            file.write(os.linesep)
             for subfield in field.subfields:
-                self._pretty_print_field(subfield, field.get_field(subfield), terminal_writer,
+                self._pretty_print_field(subfield, field.get_field(subfield), file,
                                          indent=indent + 1)
         else:
-            terminal_writer.write(f"{prefix}{field_name}: ", green=True, bold=True)
-            terminal_writer.write(f"{field}{os.linesep}")
+            file.write(colored(f"{prefix}{field_name}: ", "green", attrs=["bold"]))
+            file.write(f"{field}{os.linesep}")
 
     def _get_possible_layer_prefixes(self):
         """Gets the possible prefixes for a field under this layer.
 
         The order matters, longest must be first
         """
         return [f"{self._layer_name}_{self._layer_name}", self._layer_name]
```

### Comparing `pyshark-0.5.3/pyshark/packet/layers/json_layer.py` & `pyshark-0.6/pyshark/packet/layers/json_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+import io
 
-import py
-
+from pyshark.packet.common import colored
 from pyshark.packet.fields import LayerField
 from pyshark.packet.fields import LayerFieldsContainer
 from pyshark.packet.layers.base import BaseLayer
 
 
 class JsonLayer(BaseLayer):
     __slots__ = [
@@ -49,15 +49,15 @@
         if field is None:
             is_fake = False
             field = self._get_internal_field_by_name(name)
             if field is None:
                 # Might be a "fake" field in JSON
                 is_fake = self._is_fake_field(name)
                 if not is_fake:
-                    raise AttributeError("No such field %s" % name)
+                    raise AttributeError(f"No such field {name}")
             field = self._make_wrapped_field(name, field, is_fake=is_fake)
             self._wrapped_fields[name] = field
         return field
 
     @property
     def field_names(self):
         self._convert_showname_field_names_to_field_names()
@@ -75,20 +75,20 @@
         for part in parts:
             if part in cur_layer.field_names:
                 cur_layer = cur_layer.get_field(part)
             else:
                 return False
         return True
 
-    def _pretty_print_layer_fields(self, terminal_writer: py.io.TerminalWriter):
+    def _pretty_print_layer_fields(self, file: io.IOBase):
         for field_line in self._get_all_field_lines():
             if ':' in field_line:
                 field_name, field_line = field_line.split(':', 1)
-                terminal_writer.write(field_name + ':', green=True, bold=True)
-            terminal_writer.write(field_line, bold=True)
+                file.write(colored(field_name + ':', "green", ["bold"]))
+            file.write(colored(field_line, attrs=["bold"]))
 
     def _get_all_field_lines(self):
         """Returns all lines that represent the fields of the layer (both their names and values)."""
         for field in self._get_all_fields_with_alternates():
             yield from self._get_field_or_layer_repr(field)
 
     def _get_field_or_layer_repr(self, field):
@@ -143,57 +143,57 @@
                 self._all_fields[
                     self._field_name_from_showname(field_name)] = field_value
 
         self._showname_fields_converted_to_regular = True
 
     def _get_internal_field_by_name(self, name):
         """Gets the field by name, or None if not found."""
-        field = self._all_fields.get(name, self._all_fields.get('%s.%s' % (self._full_name, name)))
+        field = self._all_fields.get(name, self._all_fields.get(f"{self._full_name}.{name}"))
         if field is not None:
             return field
         for field_name in self._all_fields:
             # Specific name
-            if field_name.endswith('.%s' % name):
+            if field_name.endswith(f'.{name}'):
                 return self._all_fields[field_name]
 
     def _is_fake_field(self, name):
         # Some fields include parts that are not reflected in the JSON dictionary
         # i.e. a possible json is:
         # {
         #   foo: {
         #           foo.bar.baz: {
         #                   foo.baz: 3
         #               }
         # }
         # So in this case we must create a fake layer for "bar".
-        field_full_name = '%s.%s.' % (self._full_name, name)
+        field_full_name = f"{self._full_name}.{name}."
         for name, field in self._all_fields.items():
             if name.startswith(field_full_name):
                 return True
         return False
 
     def _make_wrapped_field(self, name, field, is_fake=False, full_name=None):
         """Creates the field lazily.
 
         If it's a simple field, wraps it in a container that adds extra features.
         If it's a nested layer, creates a layer for it.
         If it's an intermediate layer, copies over the relevant fields and creates a new layer for
         it.
         """
         if not full_name:
-            full_name = '%s.%s' % (self._full_name, name)
+            full_name = f"{self._full_name}.{name}"
 
         if is_fake:
             # Populate with all fields that are supposed to be inside of it
             field = {key: value for key, value in self._all_fields.items()
                      if key.startswith(full_name)}
         if isinstance(field, dict):
             if name.endswith('_tree'):
                 name = name.replace('_tree', '')
-                full_name = '%s.%s' % (self._full_name, name)
+                full_name = f'{self._full_name}.{name}'
             return JsonLayer(name, field, full_name=full_name, is_intermediate=is_fake)
         elif isinstance(field, list):
             # For whatever reason in list-type object it goes back to using the original parent name
             return [self._make_wrapped_field(name, field_part,
                                              full_name=self._full_name.split('.')[0])
                     for field_part in field]
```

### Comparing `pyshark-0.5.3/pyshark/packet/layers/xml_layer.py` & `pyshark-0.6/pyshark/packet/layers/xml_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import typing
+import io
 
-import py
-
+from pyshark.packet.common import colored
 from pyshark.packet.fields import LayerField, LayerFieldsContainer
 from pyshark.packet.layers import base
 
 
 class XmlLayer(base.BaseLayer):
     __slots__ = [
         "raw_mode",
@@ -92,20 +92,20 @@
         """Sanitizes an XML field name
 
         An xml field might have characters which would make it inaccessible as a python attribute).
         """
         field_name = field_name.replace(self._field_prefix, '')
         return field_name.replace('.', '_').replace('-', '_').lower()
 
-    def _pretty_print_layer_fields(self, terminal_writer: py.io.TerminalWriter):
+    def _pretty_print_layer_fields(self, file: io.IOBase):
         for field_line in self._get_all_field_lines():
             if ':' in field_line:
                 field_name, field_line = field_line.split(':', 1)
-                terminal_writer.write(field_name + ':', green=True, bold=True)
-            terminal_writer.write(field_line, bold=True)
+                file.write(colored(field_name + ':', "green", attrs=["bold"]))
+            file.write(colored(field_line, attrs=["bold"]))
 
     def _get_all_fields_with_alternates(self):
         all_fields = list(self._all_fields.values())
         all_fields += sum([field.alternate_fields for field in all_fields
                            if isinstance(field, LayerFieldsContainer)], [])
         return all_fields
 
@@ -123,15 +123,15 @@
         if field.hide:
             return
         if field.showname:
             return field.showname
         elif field.show:
             return field.show
         elif field.raw_value:
-            return "%s: %s" % (self._sanitize_field_name(field.name), field.raw_value)
+            return f"{self._sanitize_field_name(field.name)}: {field.raw_value}"
 
     def get_field_by_showname(self, showname) -> typing.Union[LayerFieldsContainer, None]:
         """Gets a field by its "showname"
         This is the name that appears in Wireshark's detailed display i.e. in 'User-Agent: Mozilla...',
         'User-Agent' is the .showname
         Returns None if not found.
         """
```

### Comparing `pyshark-0.5.3/pyshark/packet/packet.py` & `pyshark-0.6/pyshark/packet/packet.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         :param item: layer index or name
         :return: BaseLayer object.
         """
         if isinstance(item, int):
             return self.layers[item]
         for layer in self.layers:
-            if layer.layer_name == item.lower():
+            if layer.layer_name.lower() == item.lower():
                 return layer
         raise KeyError('Layer does not exist in packet')
 
     def __contains__(self, item):
         """Checks if the layer is inside the packet.
 
         :param item: name of the layer
@@ -92,41 +92,41 @@
         return datetime.datetime.fromtimestamp(timestamp)
 
     def __repr__(self):
         transport_protocol = ''
         if self.transport_layer != self.highest_layer and self.transport_layer is not None:
             transport_protocol = self.transport_layer + '/'
 
-        return '<%s%s Packet>' % (transport_protocol, self.highest_layer)
+        return f'<{transport_protocol}{self.highest_layer} Packet>'
 
     def __str__(self):
         s = self._packet_string
         for layer in self.layers:
             s += str(layer)
         return s
 
     @property
     def _packet_string(self):
         """A simple pretty string that represents the packet."""
-        return 'Packet (Length: %s)%s' % (self.length, os.linesep)
+        return f'Packet (Length: {self.length}){os.linesep}'
 
     def pretty_print(self):
         for layer in self.layers:
             layer.pretty_print()
     # Alias
     show = pretty_print
 
     def __getattr__(self, item):
         """
         Allows layers to be retrieved via get attr. For instance: pkt.ip
         """
         for layer in self.layers:
-            if layer.layer_name == item:
+            if layer.layer_name.lower() == item.lower():
                 return layer
-        raise AttributeError("No attribute named %s" % item)
+        raise AttributeError(f"No attribute named {item}")
 
     @property
     def highest_layer(self) -> BaseLayer:
         return self.layers[-1].layer_name.upper()
 
     @property
     def transport_layer(self) -> BaseLayer:
```

### Comparing `pyshark-0.5.3/pyshark/packet/packet_summary.py` & `pyshark-0.6/pyshark/packet/packet_summary.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             self._fields[key] = val
             self._field_order.append(key)
             setattr(self, key.lower().replace('.', '').replace(',', ''), val)
 
     def __repr__(self):
         protocol, src, dst = self._fields.get('Protocol', '?'), self._fields.get('Source', '?'),\
                              self._fields.get('Destination', '?')
-        return '<%s %s: %s to %s>' % (self.__class__.__name__, protocol, src, dst)
+        return f'<{self.__class__.__name__} {protocol}: {src} to {dst}>'
 
     def __str__(self):
         return self.summary_line
 
     @property
     def summary_line(self) -> str:
         return ' '.join([self._fields[key] for key in self._field_order])
```

### Comparing `pyshark-0.5.3/pyshark/tshark/output_parser/base_parser.py` & `pyshark-0.6/pyshark/tshark/output_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/pyshark/tshark/output_parser/tshark_ek.py` & `pyshark-0.6/pyshark/tshark/output_parser/tshark_ek.py`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/pyshark/tshark/output_parser/tshark_json.py` & `pyshark-0.6/pyshark/tshark/output_parser/tshark_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,18 +54,17 @@
         """"Returns the separators between packets in a JSON output
 
         Returns a tuple of (packet_separator, end_of_file_separator, characters_to_disregard).
         The latter variable being the number of characters to ignore in order to pass the packet (i.e. extra newlines,
         commas, parenthesis).
         """
         if not self._tshark_version or self._tshark_version >= version.parse("3.0.0"):
-            return ("%s  },%s" % (os.linesep, os.linesep)).encode(), ("}%s]" % os.linesep).encode(), (
-                    1 + len(os.linesep))
+            return f"{os.linesep}  }},{os.linesep}".encode(), f"}}{os.linesep}]".encode(), 1 + len(os.linesep)
         else:
-            return ("}%s%s  ," % (os.linesep, os.linesep)).encode(), ("}%s%s]" % (os.linesep, os.linesep)).encode(), 1
+            return f"}}{os.linesep}{os.linesep}  ,".encode(), f"}}{os.linesep}{os.linesep}]".encode(), 1
 
 
 def duplicate_object_hook(ordered_pairs):
     """Make lists out of duplicate keys."""
     json_dict = {}
     for key, val in ordered_pairs:
         existing_val = json_dict.get(key)
```

### Comparing `pyshark-0.5.3/pyshark/tshark/output_parser/tshark_xml.py` & `pyshark-0.6/pyshark/tshark/output_parser/tshark_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
 
     :param xml_pkt: str or xml object.
     :param psml_structure: a list of the fields in each packet summary in the psml data. If given, packets will
     be returned as a PacketSummary object.
     :return: Packet object.
     """
     if not isinstance(xml_pkt, lxml.objectify.ObjectifiedElement):
-        parser = lxml.objectify.makeparser(huge_tree=True, recover=True)
+        parser = lxml.objectify.makeparser(huge_tree=True, recover=True, encoding='utf-8')
         xml_pkt = xml_pkt.decode(errors='ignore').translate(DEL_BAD_XML_CHARS)
-        xml_pkt = lxml.objectify.fromstring(xml_pkt, parser)
+        xml_pkt = lxml.objectify.fromstring(xml_pkt.encode('utf-8'), parser)
     if psml_structure:
         return _packet_from_psml_packet(xml_pkt, psml_structure)
     return _packet_from_pdml_packet(xml_pkt)
 
 
 def _packet_from_psml_packet(psml_packet, structure):
     return PacketSummary(structure, psml_packet.findall('section'))
```

### Comparing `pyshark-0.5.3/pyshark/tshark/tshark.py` & `pyshark-0.6/pyshark/tshark/tshark.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,29 +31,29 @@
     :param tshark_path: Path of the tshark binary
     :raises TSharkNotFoundException in case TShark is not found in any location.
     """
     possible_paths = []
     # Check if `config.ini` exists in the current directory or the pyshark directory
     config = get_config()
     if config:
-        possible_paths.append(config.get(process_name, "%s_path" % process_name))
+        possible_paths.append(config.get(process_name, f"{process_name}_path"))
 
     # Add the user provided path to the search list
     if tshark_path is not None:
         user_tshark_path = os.path.join(os.path.dirname(tshark_path),
-                                        "%s.exe" % process_name if sys.platform.startswith("win") else process_name)
+                                        f"{process_name}.exe" if sys.platform.startswith("win") else process_name)
         possible_paths.insert(0, user_tshark_path)
 
     # Windows search order: configuration file"s path, common paths.
     if sys.platform.startswith("win"):
         for env in ("ProgramFiles(x86)", "ProgramFiles"):
             program_files = os.getenv(env)
             if program_files is not None:
                 possible_paths.append(
-                    os.path.join(program_files, "Wireshark", "%s.exe" % process_name)
+                    os.path.join(program_files, "Wireshark", f"{process_name}.exe")
                 )
     # Linux, etc. search order: configuration file's path, the system's path
     else:
         os_path = os.getenv(
             "PATH",
             "/usr/bin:/usr/sbin:/usr/lib/tshark:/usr/local/bin"
         )
@@ -65,15 +65,15 @@
     for path in possible_paths:
         if os.path.exists(path):
             if sys.platform.startswith("win"):
                 path = path.replace("\\", "/")
             return path
     raise TSharkNotFoundException(
         "TShark not found. Try adding its location to the configuration file. "
-        "Searched these paths: {}".format(possible_paths)
+        f"Searched these paths: {possible_paths}"
     )
 
 
 def get_tshark_version(tshark_path=None):
     parameters = [get_process_path(tshark_path), "-v"]
     with open(os.devnull, "w") as null:
         version_output = subprocess.check_output(parameters, stderr=null).decode("ascii")
@@ -134,16 +134,21 @@
     parameters = [get_process_path(tshark_path), "-G", "elastic-mapping"]
     with open(os.devnull, "w") as null:
         mapping = subprocess.check_output(parameters, stderr=null).decode("ascii")
 
     mapping = json.loads(
         mapping,
         object_pairs_hook=_duplicate_object_hook)["mappings"]
-    if "doc" in mapping:
+    # If using wireshark 4, the key "mapping" contains what we want,
+    if "dynamic" in mapping and "properties" in mapping:
+        pass
+    # if using wireshark 3.5 to < 4 the data in "mapping.doc",
+    elif "doc" in mapping:
         mapping = mapping["doc"]
+    # or "mapping.pcap_file" if using wireshark < 3.5
     elif "pcap_file" in mapping:
         mapping = mapping["pcap_file"]
     else:
         raise TSharkVersionException(f"Your tshark version does not support elastic-mapping. Please upgrade.")
 
     return mapping["properties"]["layers"]["properties"]
```

### Comparing `pyshark-0.5.3/pyshark.egg-info/PKG-INFO` & `pyshark-0.6/pyshark.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 1.1
 Name: pyshark
-Version: 0.5.3
+Version: 0.6
 Summary: Python wrapper for tshark, allowing python packet parsing using wireshark dissectors
 Home-page: https://github.com/KimiNewt/pyshark
 Author: KimiNewt
 Author-email: UNKNOWN
 License: MIT
 Description: Python wrapper for tshark, allowing python packet parsing using wireshark dissectors.
         
         See https://github.com/KimiNewt/pyshark/ for documentation.
         
 Keywords: wireshark capture packets parsing packet
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyshark-0.5.3/pyshark.egg-info/SOURCES.txt` & `pyshark-0.6/pyshark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyshark-0.5.3/setup.py` & `pyshark-0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.txt')) as f:
     long_description = f.read()
 
 setup(
     name="pyshark",
-    version="0.5.3",
+    version="0.6",
     packages=find_packages(),
     package_data={'': ['*.ini', '*.pcapng']},
-    install_requires=['lxml', 'py', 'packaging', 'appdirs'],
+    install_requires=['lxml', 'termcolor', 'packaging', 'appdirs'],
     tests_require=['pytest'],
     url="https://github.com/KimiNewt/pyshark",
     license="MIT",
     long_description=long_description,
     author="KimiNewt",
     description="Python wrapper for tshark, allowing python packet parsing using wireshark dissectors",
     keywords="wireshark capture packets parsing packet",
 
     classifiers=[
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

