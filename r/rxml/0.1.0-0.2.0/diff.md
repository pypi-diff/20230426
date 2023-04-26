# Comparing `tmp/rxml-0.1.0.tar.gz` & `tmp/rxml-0.2.0.tar.gz`

## Comparing `rxml-0.1.0.tar` & `rxml-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 rxml-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2708 2023-04-26 15:07:45.000000 rxml-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-26 15:07:45.000000 rxml-0.1.0/.gitignore
--rw-r--r--   0     1001      123     1071 2023-04-26 15:07:45.000000 rxml-0.1.0/LICENSE
--rw-r--r--   0     1001      123      980 2023-04-26 15:07:45.000000 rxml-0.1.0/README.md
--rw-r--r--   0     1001      123      367 2023-04-26 15:07:45.000000 rxml-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     3582 2023-04-26 15:07:45.000000 rxml-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123      150 2023-04-26 15:07:45.000000 rxml-0.1.0/xml_reader.pyi
--rw-r--r--   0     1001      123     8076 2023-04-26 15:07:45.000000 rxml-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 rxml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 rxml-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2708 2023-04-26 21:05:22.000000 rxml-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-26 21:05:22.000000 rxml-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1071 2023-04-26 21:05:22.000000 rxml-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1082 2023-04-26 21:05:22.000000 rxml-0.2.0/README.md
+-rw-r--r--   0     1001      123      423 2023-04-26 21:05:22.000000 rxml-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      340 2023-04-26 21:05:22.000000 rxml-0.2.0/rxml.pyi
+-rw-r--r--   0     1001      123     3933 2023-04-26 21:05:22.000000 rxml-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     8076 2023-04-26 21:05:22.000000 rxml-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 rxml-0.2.0/PKG-INFO
```

### Comparing `rxml-0.1.0/.github/workflows/CI.yml` & `rxml-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rxml-0.1.0/.gitignore` & `rxml-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rxml-0.1.0/LICENSE` & `rxml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxml-0.1.0/README.md` & `rxml-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # rxml
 
 ## What is rxml?
 
 `rxml` is a simple python library to read xml files up to 2 times faster than python's `xml(ElementTree)` library.
 
+## Installation
+
+To install `rxml` you can use `pip`:
+
+```bash
+pip install rxml
+```
+
+Simply as that!
+
 ## Example usage
 
 To a given xml with `test.xml` as name:
 
 ```xml
 <?xml version="1.0" encoding="UTF-8"?>
 <note example_attr="example value">
```

### Comparing `rxml-0.1.0/src/lib.rs` & `rxml-0.2.0/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use pyo3::prelude::*;
 use quick_xml::events::Event;
 use quick_xml::Reader;
 use std::collections::HashMap;
 use std::fs::File;
-use std::io::BufReader;
+use std::io::Read;
 
 macro_rules! f_str {
     ($e:expr) => {
         String::from($e)
     };
 }
 macro_rules! f_utf {
@@ -64,15 +64,15 @@
     }
 
     fn __repr__(&self) -> String {
         format!("Node({})", self.name)
     }
 }
 
-fn read_node(root_tag: String, reader: &mut Reader<BufReader<File>>) -> Node {
+fn read_node(root_tag: String, reader: &mut Reader<&[u8]>) -> Node {
     let mut buf = Vec::new();
     let mut root = Node {
         name: root_tag.clone(),
         attrs: HashMap::new(),
         children: Vec::new(),
         text: None,
         is_closed: false,
@@ -108,19 +108,29 @@
         buf.clear();
     }
     root
 }
 
 #[pyfunction]
 fn read_file(file_path: String, root_tag: String) -> Node {
-    let file_name = f_str!(file_path);
-    let mut reader = Reader::from_file(file_name).unwrap();
+    let mut file = File::open(file_path).unwrap();
+    let mut file_str = String::new();
+    file.read_to_string(&mut file_str).unwrap();
+    let mut reader = Reader::from_str(file_str.as_str());
+    reader.trim_text(true);
+    read_node(f_str!(root_tag), &mut reader)
+}
+
+#[pyfunction]
+fn read_string(xml_string: String, root_tag: String) -> Node {
+    let mut reader = Reader::from_str(xml_string.as_str());
     reader.trim_text(true);
     read_node(f_str!(root_tag), &mut reader)
 }
 
 #[pymodule]
 fn rxml(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<Node>()?;
     m.add_function(wrap_pyfunction!(read_file, m)?)?;
+    m.add_function(wrap_pyfunction!(read_string, m)?)?;
     Ok(())
 }
```

### Comparing `rxml-0.1.0/Cargo.lock` & `rxml-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rxml"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "quick-xml",
 ]
 
 [[package]]
 name = "scopeguard"
```

### Comparing `rxml-0.1.0/PKG-INFO` & `rxml-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 Metadata-Version: 2.1
 Name: rxml
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
+Summary: A XML parser for Python written in Rust
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rxml
 
 ## What is rxml?
 
 `rxml` is a simple python library to read xml files up to 2 times faster than python's `xml(ElementTree)` library.
 
+## Installation
+
+To install `rxml` you can use `pip`:
+
+```bash
+pip install rxml
+```
+
+Simply as that!
+
 ## Example usage
 
 To a given xml with `test.xml` as name:
 
 ```xml
 <?xml version="1.0" encoding="UTF-8"?>
 <note example_attr="example value">
```

