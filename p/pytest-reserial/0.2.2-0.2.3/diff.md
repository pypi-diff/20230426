# Comparing `tmp/pytest-reserial-0.2.2.tar.gz` & `tmp/pytest-reserial-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reserial-0.2.2.tar", last modified: Tue Nov 29 13:15:36 2022, max compression
+gzip compressed data, was "pytest-reserial-0.2.3.tar", last modified: Wed Apr 26 10:55:20 2023, max compression
```

## Comparing `pytest-reserial-0.2.2.tar` & `pytest-reserial-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      701 2022-11-25 09:28:01.059725 pytest-reserial-0.2.2/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      565 2022-11-25 09:28:01.059725 pytest-reserial-0.2.2/.github/workflows/main.yml
--rw-r--r--   0        0        0      889 2022-10-13 12:05:42.754306 pytest-reserial-0.2.2/.gitignore
--rw-r--r--   0        0        0      517 2022-11-23 18:40:29.588865 pytest-reserial-0.2.2/.prospector.yaml
--rw-r--r--   0        0        0     1085 2022-10-13 12:05:42.750306 pytest-reserial-0.2.2/LICENSE
--rw-r--r--   0        0        0     4261 2022-11-25 09:28:01.059725 pytest-reserial-0.2.2/README.md
--rw-r--r--   0        0        0     1855 2022-11-25 09:28:01.059725 pytest-reserial-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       93 2022-11-29 13:13:59.468414 pytest-reserial-0.2.2/src/pytest_reserial/__init__.py
--rw-r--r--   0        0        0     9068 2022-11-29 13:11:52.356274 pytest-reserial-0.2.2/src/pytest_reserial/reserial.py
--rw-r--r--   0        0        0       28 2022-11-24 14:07:04.692702 pytest-reserial-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     2705 2022-11-24 15:20:19.896411 pytest-reserial-0.2.2/tests/test_reserial.py
--rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 pytest-reserial-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      701 2022-11-25 09:28:01.059725 pytest-reserial-0.2.3/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      565 2022-11-25 09:28:01.059725 pytest-reserial-0.2.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0      910 2023-04-26 10:42:13.829488 pytest-reserial-0.2.3/.gitignore
+-rw-r--r--   0        0        0      517 2022-11-23 18:40:29.588865 pytest-reserial-0.2.3/.prospector.yaml
+-rw-r--r--   0        0        0     1085 2022-10-13 12:05:42.750306 pytest-reserial-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4262 2023-04-26 10:40:51.426753 pytest-reserial-0.2.3/README.md
+-rw-r--r--   0        0        0     1855 2022-12-05 08:17:45.207736 pytest-reserial-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-26 10:40:51.438753 pytest-reserial-0.2.3/src/pytest_reserial/__init__.py
+-rw-r--r--   0        0        0     9498 2023-04-26 07:21:34.633769 pytest-reserial-0.2.3/src/pytest_reserial/reserial.py
+-rw-r--r--   0        0        0       28 2022-11-24 14:07:04.692702 pytest-reserial-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     3139 2023-04-26 07:20:50.160307 pytest-reserial-0.2.3/tests/test_reserial.py
+-rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 pytest-reserial-0.2.3/PKG-INFO
```

### Comparing `pytest-reserial-0.2.2/.github/workflows/codecov.yml` & `pytest-reserial-0.2.3/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `pytest-reserial-0.2.2/.github/workflows/main.yml` & `pytest-reserial-0.2.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest-reserial-0.2.2/.gitignore` & `pytest-reserial-0.2.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,9 @@
 
 # IPython Notebook
 .ipynb_checkpoints
 
 # pyenv
 .python-version
 
+# Spyder
+.spyproject
```

### Comparing `pytest-reserial-0.2.2/.prospector.yaml` & `pytest-reserial-0.2.3/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `pytest-reserial-0.2.2/LICENSE` & `pytest-reserial-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reserial-0.2.2/README.md` & `pytest-reserial-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     what tests are for, after all. Only, you can't figure out why the test is failing. You spend
     several hours trying to fix it, but eventually give up and revert your changes.
     But the test still fails.
     So you try another device, and sure enough, now it passes. Turns out, what you thought was a
     problem with your code was actually a hardware failure.
 
 -   Some of the tests depend on the device being in a certain state, and some of the tests depend on
-    the device being in *another* state. So you can't run the entire test suite all at once, instad
+    the device being in *another* state. So you can't run the entire test suite all at once, instead
     being forced to stop it halfway through and mess with a bunch of wires and buttons before you can
     run the rest of the tests.
    
 And then you asked yourself, 'How do I write my tests so that the device doesn't need to be connected?' You may have gone down the rabbit hole that is mocking, and then replaced large parts of pyserial with mock interfaces, and ultimately ended up with a test suite that was significantly more complex than the program it was meant to test.
 
 With pytest-reserial, you don't have to worry about any of that. Just write your tests as if the device is always connected. Then, simply use the `reserial` fixture to record the serial traffic from passing tests, and replay it when the device isn't connected.
```

### Comparing `pytest-reserial-0.2.2/pyproject.toml` & `pytest-reserial-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-reserial-0.2.2/src/pytest_reserial/reserial.py` & `pytest-reserial-0.2.3/src/pytest_reserial/reserial.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,25 @@
 
     DONT_PATCH = 0
     REPLAY = 1
     RECORD = 2
     INVALID = 3
 
 
+def reconfigure_port_patch(
+    self: Serial, force_update: bool = False  # pylint: disable=unused-argument
+) -> None:
+    """Don't try to set parameters on the mocked port.
+
+    When changing settings such as timeout, parity, stop bits, etc. the
+    _reconfigure_port method is called. It operates directly on the underlying operating
+    system resource, which doesn't exist in reserial. Therefore, this patch is required.
+    """
+
+
 @pytest.fixture
 def reserial(
     monkeypatch: pytest.MonkeyPatch,
     request: pytest.FixtureRequest,
 ) -> Generator[None, None, None]:
     """Record or replay serial traffic.
 
@@ -49,26 +60,27 @@
     log = get_traffic_log(mode, logpath, testname)
 
     read_patch, write_patch, open_patch, close_patch = get_patched_methods(mode, log)
     monkeypatch.setattr(Serial, "read", read_patch)
     monkeypatch.setattr(Serial, "write", write_patch)
     monkeypatch.setattr(Serial, "open", open_patch)
     monkeypatch.setattr(Serial, "close", close_patch)
+    monkeypatch.setattr(Serial, "_reconfigure_port", reconfigure_port_patch)
 
     yield
 
     if mode == Mode.RECORD:
         write_log(log, logpath, testname)
         return
 
     if log["rx"] or log["tx"]:
         raise ValueError("Not empty")
 
 
-def get_traffic_log(mode: Mode, logpath: str, testname: str) -> Dict[str, List[int]]:
+def get_traffic_log(mode: Mode, logpath: Path, testname: str) -> Dict[str, List[int]]:
     """Load recorded traffic (replay) or create an empty log (record).
 
     Parameters
     ----------
     mode : Mode
         The requested mode of operation, i.e. `REPLAY`, `RECORD`, or `DONT_PATCH`.
     logpath: str
@@ -175,16 +187,14 @@
         return values are identical to Serial.write.
 
         Raises
         ------
         ValueError
             If written data does not match recorded data.
         """
-        nonlocal log
-
         if list(data) == log["tx"][: len(data)]:
             log["tx"] = log["tx"][len(data) :]
         else:
             raise ValueError(
                 "Written data does not match recorded data: "
                 "f{data} != {traffic_log['tx'][: len(data)]}"
             )
@@ -196,23 +206,22 @@
         size: int = 1,
     ) -> bytes:
         """Replay RX data from recording instead of reading from the bus.
 
         Monkeypatch this method over Serial.read to replay traffic. Parameters and
         return values are identical to Serial.read.
         """
-        nonlocal log
         data = log["rx"][:size]
         log["rx"] = log["rx"][size:]
         return bytes(data)
 
     return replay_read, replay_write, replay_open, replay_close
 
 
-# The open/close method patches don't need any nonlocals, so they can stay down here.
+# The open/close method patches don't need access to logs, so they can stay down here.
 def replay_open(self: Serial) -> None:
     """Pretend that port was opened."""
     self.is_open = True
 
 
 def replay_close(self: Serial) -> None:
     """Pretend that port was closed."""
@@ -250,36 +259,34 @@
 
     def record_write(self: Serial, data: bytes) -> int:
         """Record TX data before writing to the bus.
 
         Monkeypatch this method over Serial.write to record traffic. Parameters and
         return values are identical to Serial.write.
         """
-        nonlocal log
         log["tx"] += list(data)
         written: int = real_write(self, data)
         return written
 
     def record_read(self: Serial, size: int = 1) -> bytes:
         """Record RX data after reading from the bus.
 
         Monkeypatch this method over Serial.read to record traffic. Parameters and
         return values are identical to Serial.read.
         """
         data: bytes = real_read(self, size)
-        nonlocal log
         log["rx"] += list(data)
         return data
 
     return record_read, record_write, Serial.open, Serial.close
 
 
 def write_log(
     log: Dict[str, List[int]],
-    logpath: str,
+    logpath: Path,
     testname: str,
 ) -> None:
     """Write recorded traffic to log file.
 
     Parameters
     ----------
     log: dict[str, list[int]]
```

### Comparing `pytest-reserial-0.2.2/tests/test_reserial.py` & `pytest-reserial-0.2.3/tests/test_reserial.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,7 +95,24 @@
         [
             "reserial:",
             "*--record * Record serial traffic.",
             "*--replay * Replay serial traffic.",
         ]
     )
     assert result.ret == 0
+
+
+def test_change_settings(pytester):
+    pytester.makefile(
+        ".json",
+        test_change_settings='{"test_reserial": {"tx": [], "rx": []}}',
+    )
+    pytester.makepyfile(
+        """
+            import serial
+            def test_reserial(reserial):
+                s = serial.Serial(port="/dev/ttyUSB0")
+                s.timeout = 1
+        """
+    )
+    result = pytester.runpytest("--replay")
+    assert result.ret == 0
```

### Comparing `pytest-reserial-0.2.2/PKG-INFO` & `pytest-reserial-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reserial
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pytest fixture for recording and replaying serial port traffic.
 Keywords: serial,testing,logging,mocking,patching,stubbing,record,replay
 Author-email: Alexander Bessman <alexander.bessman@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -88,15 +88,15 @@
     what tests are for, after all. Only, you can't figure out why the test is failing. You spend
     several hours trying to fix it, but eventually give up and revert your changes.
     But the test still fails.
     So you try another device, and sure enough, now it passes. Turns out, what you thought was a
     problem with your code was actually a hardware failure.
 
 -   Some of the tests depend on the device being in a certain state, and some of the tests depend on
-    the device being in *another* state. So you can't run the entire test suite all at once, instad
+    the device being in *another* state. So you can't run the entire test suite all at once, instead
     being forced to stop it halfway through and mess with a bunch of wires and buttons before you can
     run the rest of the tests.
    
 And then you asked yourself, 'How do I write my tests so that the device doesn't need to be connected?' You may have gone down the rabbit hole that is mocking, and then replaced large parts of pyserial with mock interfaces, and ultimately ended up with a test suite that was significantly more complex than the program it was meant to test.
 
 With pytest-reserial, you don't have to worry about any of that. Just write your tests as if the device is always connected. Then, simply use the `reserial` fixture to record the serial traffic from passing tests, and replay it when the device isn't connected.
```

