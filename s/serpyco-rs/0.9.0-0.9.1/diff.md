# Comparing `tmp/serpyco_rs-0.9.0.tar.gz` & `tmp/serpyco_rs-0.9.1.tar.gz`

## Comparing `serpyco_rs-0.9.0.tar` & `serpyco_rs-0.9.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 serpyco_rs-0.9.0/Cargo.toml
--rw-r--r--   0     1001      123       25 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/.envrc.example
--rw-r--r--   0     1001      123     3931 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/.gitignore
--rw-r--r--   0     1001      123     1069 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/LICENSE
--rw-r--r--   0     1001      123       34 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/MANIFEST.in
--rw-r--r--   0     1001      123     8943 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/README.md
--rw-r--r--   0     1001      123        0 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/__init__.py
--rw-r--r--   0     1001      123     1832 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/graph.py
--rw-r--r--   0     1001      123        0 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/__init__.py
--rw-r--r--   0     1001      123      645 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/base.py
--rw-r--r--   0     1001      123      356 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/marshmallow.py
--rw-r--r--   0     1001      123      704 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/mashumaro.py
--rw-r--r--   0     1001      123      521 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/pydantic.py
--rw-r--r--   0     1001      123      355 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/serpyco.py
--rw-r--r--   0     1001      123      361 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/libs/serpyco_rs.py
--rw-r--r--   0     1001      123     1642 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/compare/test_benchmarks.py
--rw-r--r--   0     1001      123     6092 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/test_encoders.py
--rw-r--r--   0     1001      123      803 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/test_full.py
--rw-r--r--   0     1001      123      197 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/bench/utils.py
--rw-r--r--   0     1001      123     2272 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/noxfile.py
--rw-r--r--   0     1001      123      948 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/pyproject.toml
--rw-r--r--   0     1001      123      152 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/__init__.py
--rw-r--r--   0     1001      123    16707 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_describe.py
--rw-r--r--   0     1001      123       72 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_impl.py
--rw-r--r--   0     1001      123      320 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_impl.pyi
--rw-r--r--   0     1001      123      199 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/__init__.py
--rw-r--r--   0     1001      123     6010 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/_convert.py
--rw-r--r--   0     1001      123     5094 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/_entities.py
--rw-r--r--   0     1001      123     1035 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/_validate.py
--rw-r--r--   0     1001      123     1234 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_main.py
--rw-r--r--   0     1001      123      166 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/_utils.py
--rw-r--r--   0     1001      123      364 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/exceptions.py
--rw-r--r--   0     1001      123     1464 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/metadata.py
--rw-r--r--   0     1001      123        0 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/python/serpyco_rs/py.typed
--rw-r--r--   0     1001      123      110 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/requirements/bench.txt
--rw-r--r--   0     1001      123       72 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/requirements/dev.txt
--rw-r--r--   0     1001      123       29 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/requirements/lint.txt
--rw-r--r--   0     1001      123       47 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/requirements/type_check.txt
--rwxr-xr-x   0     1001      123      832 2023-04-03 07:22:09.000000 serpyco_rs-0.9.0/run-maturin-action.sh
--rw-r--r--   0     1001      123       54 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/build.rs
--rw-r--r--   0     1001      123      297 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/lib.rs
--rw-r--r--   0     1001      123     4436 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer/dateutil.rs
--rw-r--r--   0     1001      123    13404 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer/encoders.rs
--rw-r--r--   0     1001      123     2252 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer/macros.rs
--rw-r--r--   0     1001      123     8828 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer/main.rs
--rw-r--r--   0     1001      123     5126 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer/py.rs
--rw-r--r--   0     1001      123     7134 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer/types.rs
--rw-r--r--   0     1001      123      152 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/src/serializer.rs
--rw-r--r--   0     1001      123        0 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/json_schema/__init__.py
--rw-r--r--   0     1001      123    11743 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/json_schema/test_convert.py
--rw-r--r--   0     1001      123     6944 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/json_schema/test_validator.py
--rw-r--r--   0     1001      123    20723 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test__describe.py
--rw-r--r--   0     1001      123     1234 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test_custom_encoder.py
--rw-r--r--   0     1001      123     5798 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test_encoders.py
--rw-r--r--   0     1001      123     1496 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test_metadata.py
--rw-r--r--   0     1001      123     2567 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test_recursive.py
--rw-r--r--   0     1001      123     6100 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test_simple.py
--rw-r--r--   0     1001      123     3392 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/tests/test_union.py
--rw-r--r--   0     1001      123    15160 2023-04-03 07:21:35.000000 serpyco_rs-0.9.0/Cargo.lock
--rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 serpyco_rs-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 serpyco_rs-0.9.1/Cargo.toml
+-rw-r--r--   0     1001      123       25 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.envrc.example
+-rw-r--r--   0     1001      123      196 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.github/dependabot.yml
+-rw-r--r--   0     1001      123     4009 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.gitignore
+-rw-r--r--   0     1001      123     1069 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/LICENSE
+-rw-r--r--   0     1001      123       34 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/MANIFEST.in
+-rw-r--r--   0     1001      123     8943 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/README.md
+-rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/__init__.py
+-rw-r--r--   0     1001      123     1832 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/graph.py
+-rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/__init__.py
+-rw-r--r--   0     1001      123      645 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/base.py
+-rw-r--r--   0     1001      123      356 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/marshmallow.py
+-rw-r--r--   0     1001      123      704 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/mashumaro.py
+-rw-r--r--   0     1001      123      521 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/pydantic.py
+-rw-r--r--   0     1001      123      355 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/serpyco.py
+-rw-r--r--   0     1001      123      361 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/serpyco_rs.py
+-rw-r--r--   0     1001      123     1642 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/test_benchmarks.py
+-rw-r--r--   0     1001      123     6092 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/test_encoders.py
+-rw-r--r--   0     1001      123      803 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/test_full.py
+-rw-r--r--   0     1001      123      197 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/utils.py
+-rw-r--r--   0     1001      123     2271 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/noxfile.py
+-rw-r--r--   0     1001      123      948 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      123      152 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/__init__.py
+-rw-r--r--   0     1001      123    16736 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_describe.py
+-rw-r--r--   0     1001      123       72 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_impl.py
+-rw-r--r--   0     1001      123      320 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_impl.pyi
+-rw-r--r--   0     1001      123      199 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/__init__.py
+-rw-r--r--   0     1001      123     6010 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_convert.py
+-rw-r--r--   0     1001      123     5094 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_entities.py
+-rw-r--r--   0     1001      123     1035 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_validate.py
+-rw-r--r--   0     1001      123     1234 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_main.py
+-rw-r--r--   0     1001      123      166 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_utils.py
+-rw-r--r--   0     1001      123      364 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/exceptions.py
+-rw-r--r--   0     1001      123     1464 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/metadata.py
+-rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/py.typed
+-rw-r--r--   0     1001      123      110 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/bench.txt
+-rw-r--r--   0     1001      123       78 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/dev.txt
+-rw-r--r--   0     1001      123       29 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/lint.txt
+-rw-r--r--   0     1001      123       47 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/type_check.txt
+-rwxr-xr-x   0     1001      123     1010 2023-04-26 13:54:41.000000 serpyco_rs-0.9.1/run-maturin-action.sh
+-rw-r--r--   0     1001      123       54 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/build.rs
+-rw-r--r--   0     1001      123      297 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/lib.rs
+-rw-r--r--   0     1001      123     4430 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/dateutil.rs
+-rw-r--r--   0     1001      123    13404 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/encoders.rs
+-rw-r--r--   0     1001      123     2252 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/macros.rs
+-rw-r--r--   0     1001      123     8828 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/main.rs
+-rw-r--r--   0     1001      123     5126 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/py.rs
+-rw-r--r--   0     1001      123     7134 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/types.rs
+-rw-r--r--   0     1001      123      152 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer.rs
+-rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/json_schema/__init__.py
+-rw-r--r--   0     1001      123    11743 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/json_schema/test_convert.py
+-rw-r--r--   0     1001      123     6944 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/json_schema/test_validator.py
+-rw-r--r--   0     1001      123    20723 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test__describe.py
+-rw-r--r--   0     1001      123     1234 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_custom_encoder.py
+-rw-r--r--   0     1001      123     5798 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_encoders.py
+-rw-r--r--   0     1001      123     1496 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_metadata.py
+-rw-r--r--   0     1001      123     2567 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_recursive.py
+-rw-r--r--   0     1001      123     6100 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_simple.py
+-rw-r--r--   0     1001      123     3981 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_union.py
+-rw-r--r--   0     1001      123    14885 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/Cargo.lock
+-rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 serpyco_rs-0.9.1/PKG-INFO
```

### Comparing `serpyco_rs-0.9.0/Cargo.toml` & `serpyco_rs-0.9.1/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [package]
 name = "serpyco-rs"
-version = "0.9.0"
+version = "0.9.1"
 edition = "2021"
 homepage = "https://github.com/ermakov-oleg/serpyco-rs"
 repository = "https://github.com/ermakov-oleg/serpyco-rs"
 
 [package.metadata.maturin]
 python-source = "python"
 name = "serpyco_rs._serpyco_rs"
 
 [lib]
 name = "serpyco_rs"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.18.2", features = ["extension-module"] }
+pyo3 = { version = "0.18.3", features = ["extension-module"] }
 pyo3-ffi = "*"
 cfg-if = "*"
 chrono = { version = "*"}
 
 dyn-clone = "1.0"
 atomic_refcell = "0.1.9"
 
 [build-dependencies]
-pyo3-build-config = { version = "0.17.2", features = ["resolve-config"] }
+pyo3-build-config = { version = "0.18.3", features = ["resolve-config"] }
```

### Comparing `serpyco_rs-0.9.0/.github/workflows/CI.yml` & `serpyco_rs-0.9.1/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     steps:
       - uses: actions/checkout@v3
       - uses: messense/maturin-action@v1
         with:
           manylinux: auto
           command: build
           args: --release --sdist -o dist --find-interpreter
+          sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   windows:
@@ -33,14 +34,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
       - uses: messense/maturin-action@v1
         with:
           command: build
           args: --release -o dist --find-interpreter
+          sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   macos:
@@ -53,14 +55,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
       - uses: messense/maturin-action@v1
         with:
           command: build
           args: --release -o dist --universal2 --find-interpreter
+          sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   test:
```

### Comparing `serpyco_rs-0.9.0/.gitignore` & `serpyco_rs-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/LICENSE` & `serpyco_rs-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/README.md` & `serpyco_rs-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/compare/graph.py` & `serpyco_rs-0.9.1/bench/compare/graph.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/compare/libs/base.py` & `serpyco_rs-0.9.1/bench/compare/libs/base.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/compare/libs/mashumaro.py` & `serpyco_rs-0.9.1/bench/compare/libs/mashumaro.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/compare/libs/pydantic.py` & `serpyco_rs-0.9.1/bench/compare/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/compare/test_benchmarks.py` & `serpyco_rs-0.9.1/bench/compare/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/test_encoders.py` & `serpyco_rs-0.9.1/bench/test_encoders.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/bench/test_full.py` & `serpyco_rs-0.9.1/bench/test_full.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/noxfile.py` & `serpyco_rs-0.9.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 def bench(session):
     build(session)
     session.install("-r", "requirements/bench.txt")
 
     session.run(
         "pytest",
         "--verbose",
-        "--benchmark-min-time=0.5",
-        "--benchmark-max-time=2.5",
+        "--benchmark-min-time=0.25",
+        "--benchmark-max-time=1",
         "--benchmark-disable-gc",
         "--benchmark-autosave",
         "--benchmark-save-data",
         "--benchmark-compare",
         "--ignore=bench/test_full.py",
         *(session.posargs if session.posargs else ["bench"]),
     )
```

### Comparing `serpyco_rs-0.9.0/pyproject.toml` & `serpyco_rs-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/python/serpyco_rs/_describe.py` & `serpyco_rs-0.9.1/python/serpyco_rs/_describe.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 
         meta = dataclasses.replace(meta, discriminator_field=discriminator.name)
         return UnionType(
             item_types={
                 _get_discriminator_value(arg, discriminator.name): describe_type(annotation_wrapper(arg), meta)
                 for arg in args
             },
-            discriminator=discriminator.name,
+            discriminator=_apply_format(filed_format, discriminator.name),
             custom_encoder=custom_encoder,
         )
 
     if isinstance(t, TypeVar):
         raise RuntimeError(f"Unfilled TypeVar: {t}")
 
     raise RuntimeError(f"Unknown type {t!r}")
```

### Comparing `serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/_convert.py` & `serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_convert.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/_entities.py` & `serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_entities.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/python/serpyco_rs/_json_schema/_validate.py` & `serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_validate.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/python/serpyco_rs/_main.py` & `serpyco_rs-0.9.1/python/serpyco_rs/_main.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/python/serpyco_rs/metadata.py` & `serpyco_rs-0.9.1/python/serpyco_rs/metadata.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/run-maturin-action.sh` & `serpyco_rs-0.9.1/run-maturin-action.sh`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,15 @@
 export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
 curl -L https://github.com/PyO3/maturin/releases/download/v0.13.7/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
 python3 -m pip install cffi || true
 echo "::endgroup::"
-maturin build --release --sdist -o dist --find-interpreter
+echo "::group::Install sccache"
+python3 -m pip install --pre sccache
+sccache --version
+echo "::endgroup::"
+maturin build --release --sdist -o dist --find-interpreter
+echo "::group::sccache stats"
+sccache --show-stats
+echo "::endgroup::"
```

### Comparing `serpyco_rs-0.9.0/src/serializer/dateutil.rs` & `serpyco_rs-0.9.1/src/serializer/dateutil.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 pub fn parse_time(value: &str) -> PyResult<*mut PyObject> {
     #[allow(clippy::redundant_closure)]
     let (time, tz) = NaiveTime::parse_from_str(value, "%H:%M:%S%.f")
         .or_else(|_| NaiveTime::parse_from_str(value, "%H:%M"))
         .map(|v| (v, None))
         .or_else(|_| {
-            let mut datetime_raw = Utc::now().date().naive_utc().to_string();
+            let mut datetime_raw = Utc::now().date_naive().to_string();
             datetime_raw.push('T');
             datetime_raw.push_str(value);
             let datetime = DateTime::parse_from_rfc3339(&datetime_raw)?;
             let tz = datetime.offset().fix();
             Ok((datetime.time(), Some(tz)))
         })
         .map_err(|e: ParseError| InnerParseError::from(e))?;
```

### Comparing `serpyco_rs-0.9.0/src/serializer/encoders.rs` & `serpyco_rs-0.9.1/src/serializer/encoders.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/src/serializer/macros.rs` & `serpyco_rs-0.9.1/src/serializer/macros.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/src/serializer/main.rs` & `serpyco_rs-0.9.1/src/serializer/main.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/src/serializer/py.rs` & `serpyco_rs-0.9.1/src/serializer/py.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/src/serializer/types.rs` & `serpyco_rs-0.9.1/src/serializer/types.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/json_schema/test_convert.py` & `serpyco_rs-0.9.1/tests/json_schema/test_convert.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/json_schema/test_validator.py` & `serpyco_rs-0.9.1/tests/json_schema/test_validator.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test__describe.py` & `serpyco_rs-0.9.1/tests/test__describe.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test_custom_encoder.py` & `serpyco_rs-0.9.1/tests/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test_encoders.py` & `serpyco_rs-0.9.1/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test_metadata.py` & `serpyco_rs-0.9.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test_recursive.py` & `serpyco_rs-0.9.1/tests/test_recursive.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test_simple.py` & `serpyco_rs-0.9.1/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.0/tests/test_union.py` & `serpyco_rs-0.9.1/tests/test_union.py`

 * *Files 14% similar despite different names*

```diff
@@ -135,7 +135,34 @@
         "children": [
             {"params": 1234, "type": "A"},
             {"children": [{"params": "bar", "type": "B"}], "params": "foo", "type": "B"},
         ],
     }
     assert serializer.dump(data) == raw_data
     assert serializer.load(raw_data) == data
+
+
+def test_tagged_union__camel_case_filed_format():
+    @dataclass
+    class A:
+        discriminator_with_multiple_words: Literal["A"]
+        a: int
+
+    @dataclass
+    class B:
+        discriminator_with_multiple_words: Literal["B"]
+        b: str
+
+    a = {
+        "discriminatorWithMultipleWords": "A",
+        "a": 128,
+    }
+
+    serializer = Serializer(
+        Annotated[Union[A, B], Discriminator("discriminator_with_multiple_words")],
+        camelcase_fields=True,
+    )
+
+    assert serializer.load(a) == A(
+        discriminator_with_multiple_words="A",
+        a=128,
+    )
```

### Comparing `serpyco_rs-0.9.0/Cargo.lock` & `serpyco_rs-0.9.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.11.0"
+version = "3.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1ad822118d20d2c234f427000d5acc36eabe1e29a348c89b63dd60b13f28e5d"
+checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
 
 [[package]]
 name = "cc"
 version = "1.0.73"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fff2a6927b3bb87f9595d67196a70493f627687a71d87a0d692242c33f58c11"
 
@@ -45,17 +45,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.22"
+version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfd4d1b31faaa3a89d7934dbded3111da0d2ef28e3ebccdb4f0179f5929d1ef1"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "iana-time-zone",
  "js-sys",
  "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
@@ -120,17 +120,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9b0705efd4599c15a38151f4721f7bc388306f61084d3bfd50bd07fbca5cb60"
+checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.51"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5a6ef98976b22b3b7f2f3a806f858cb862044cfa66805aa3ad84cb3d3b785ed"
 dependencies = [
@@ -265,76 +265,66 @@
 checksum = "0a2ca2c61bc9f3d74d2886294ab7b9853abd9c1ad903a3ac7815c58989bb7bab"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
- "pyo3-build-config 0.18.2",
+ "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf0708c9ed01692635cbf056e286008e5a2927ab1a5e48cdd3aeb1ba5a6fef47"
-dependencies = [
- "once_cell",
- "target-lexicon",
-]
-
-[[package]]
-name = "pyo3-build-config"
-version = "0.18.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
- "pyo3-build-config 0.18.2",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -365,22 +355,22 @@
 name = "scratch"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8132065adcfd6e02db789d9285a0deb2f3fcb04002865ab67d5fb103533898"
 
 [[package]]
 name = "serpyco-rs"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "atomic_refcell",
  "cfg-if",
  "chrono",
  "dyn-clone",
  "pyo3",
- "pyo3-build-config 0.17.2",
+ "pyo3-build-config",
  "pyo3-ffi",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

### Comparing `serpyco_rs-0.9.0/PKG-INFO` & `serpyco_rs-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serpyco-rs
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

