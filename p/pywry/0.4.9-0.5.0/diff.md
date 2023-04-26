# Comparing `tmp/pywry-0.4.9.tar.gz` & `tmp/pywry-0.5.0.tar.gz`

## Comparing `pywry-0.4.9.tar` & `pywry-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 pywry-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 pywry-0.4.9/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     2678 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/src/websocket.rs
--rw-r--r--   0     1001      123    20668 2023-04-25 21:07:29.000000 pywry-0.4.9/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    61106 2023-04-25 21:07:29.000000 pywry-0.4.9/Cargo.lock
--rw-r--r--   0     1001      123    11138 2023-04-25 21:07:29.000000 pywry-0.4.9/python/pywry/core.py
--rw-r--r--   0     1001      123      985 2023-04-25 21:07:29.000000 pywry-0.4.9/python/pywry/backend.py
--rw-r--r--   0     1001      123      370 2023-04-25 21:07:29.000000 pywry-0.4.9/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      180 2023-04-25 21:07:29.000000 pywry-0.4.9/python/pywry/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-25 21:07:29.000000 pywry-0.4.9/python/pywry/py.typed
--rw-r--r--   0     1001      123      792 2023-04-25 21:07:29.000000 pywry-0.4.9/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-04-25 21:07:29.000000 pywry-0.4.9/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-25 21:07:29.000000 pywry-0.4.9/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-25 21:07:29.000000 pywry-0.4.9/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-25 21:07:29.000000 pywry-0.4.9/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-25 21:07:29.000000 pywry-0.4.9/src/websocket.rs
--rw-r--r--   0     1001      123    20668 2023-04-25 21:07:29.000000 pywry-0.4.9/src/window.rs
--rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 pywry-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 pywry-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 pywry-0.5.0/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     2678 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     2149 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/websocket.rs
+-rw-r--r--   0     1001      123    20668 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    61106 2023-04-26 14:02:46.000000 pywry-0.5.0/Cargo.lock
+-rw-r--r--   0     1001      123    11147 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/core.py
+-rw-r--r--   0     1001      123      985 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/backend.py
+-rw-r--r--   0     1001      123      370 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      180 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/py.typed
+-rw-r--r--   0     1001      123      792 2023-04-26 14:02:46.000000 pywry-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      123     2149 2023-04-26 14:02:46.000000 pywry-0.5.0/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-04-26 14:02:46.000000 pywry-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-04-26 14:02:46.000000 pywry-0.5.0/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-04-26 14:02:46.000000 pywry-0.5.0/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-04-26 14:02:46.000000 pywry-0.5.0/src/websocket.rs
+-rw-r--r--   0     1001      123    20668 2023-04-26 14:02:46.000000 pywry-0.5.0/src/window.rs
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 pywry-0.5.0/PKG-INFO
```

### Comparing `pywry-0.4.9/pyproject.toml` & `pywry-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "pywry"
-version = "0.4.9"
+version = "0.5.0"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
 ]
 
-dependencies = ['websockets>=11.0.1', 'psutil>=5.8.0,<5.9.4', "setproctitle"]
+dependencies = ["websockets", "psutil>=5.8.0,<5.9.4", "setproctitle"]
 
 [build-system]
 requires = [
     "setuptools>=58.0.0",
     "wheel",
     "maturin>=0.14,<0.15",
     "toml"
```

### Comparing `pywry-0.4.9/rust_src/pywry/Cargo.toml` & `pywry-0.5.0/rust_src/pywry/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.4.9"
+version = "0.5.0"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.4.9/rust_src/pywry/LICENSE` & `pywry-0.5.0/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/rust_src/pywry/README.md` & `pywry-0.5.0/rust_src/pywry/README.md`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/rust_src/pywry/src/constants.rs` & `pywry-0.5.0/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/rust_src/pywry/src/lib.rs` & `pywry-0.5.0/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/rust_src/pywry/src/structs.rs` & `pywry-0.5.0/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/rust_src/pywry/src/websocket.rs` & `pywry-0.5.0/rust_src/pywry/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/rust_src/pywry/src/window.rs` & `pywry-0.5.0/rust_src/pywry/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/Cargo.lock` & `pywry-0.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1494,15 +1494,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.4.9"
+version = "0.5.0"
 dependencies = [
  "futures-util",
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
```

### Comparing `pywry-0.4.9/python/pywry/core.py` & `pywry-0.5.0/python/pywry/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,23 +207,23 @@
                 cmd = [sys.executable, "-m", "pywry.backend", "--start"]
                 if self.debug:
                     cmd.append("--debug")
                 kwargs = {"stderr": subprocess.PIPE}
             else:
                 # pylint: disable=E1101,W0212
                 pywrypath = (Path(sys._MEIPASS) / "OpenBBPlotsBackend").resolve()
-                if sys.platform == "win32":
-                    cmd = f"{pywrypath} --start{' --debug' if self.debug else ''}"
+                cmd = f"OpenBBPlotsBackend --start{' --debug' if self.debug else ''}"
                 if sys.platform == "darwin":
                     cmd = f"'{pywrypath}'"
 
                 kwargs = {
                     "stdout": subprocess.PIPE,
                     "stderr": subprocess.STDOUT,
                     "stdin": subprocess.PIPE,
+                    "cwd": str(pywrypath.parent),
                 }
                 self.shell = True
 
             env = os.environ.copy()
             env["PYWRY_PROCESS_NAME"] = self.proc_name
 
             self.runner = psutil.Popen(
```

### Comparing `pywry-0.4.9/python/pywry/backend.py` & `pywry-0.5.0/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/Cargo.toml` & `pywry-0.5.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.4.9"
+version = "0.5.0"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.4.9/src/constants.rs` & `pywry-0.5.0/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/src/lib.rs` & `pywry-0.5.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/src/structs.rs` & `pywry-0.5.0/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/src/websocket.rs` & `pywry-0.5.0/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/src/window.rs` & `pywry-0.5.0/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.9/PKG-INFO` & `pywry-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.4.9
+Version: 0.5.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: websockets>=11.0.1
+Requires-Dist: websockets
 Requires-Dist: psutil>=5.8.0,<5.9.4
 Requires-Dist: setproctitle
 Requires-Dist: auditwheel; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Requires-Python: >=3.8
```

