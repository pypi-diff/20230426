# Comparing `tmp/serpyco_rs-0.9.1.tar.gz` & `tmp/serpyco_rs-0.9.2.tar.gz`

## Comparing `serpyco_rs-0.9.1.tar` & `serpyco_rs-0.9.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 serpyco_rs-0.9.1/Cargo.toml
--rw-r--r--   0     1001      123       25 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.envrc.example
--rw-r--r--   0     1001      123      196 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.github/dependabot.yml
--rw-r--r--   0     1001      123     4009 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/.gitignore
--rw-r--r--   0     1001      123     1069 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/LICENSE
--rw-r--r--   0     1001      123       34 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/MANIFEST.in
--rw-r--r--   0     1001      123     8943 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/README.md
--rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/__init__.py
--rw-r--r--   0     1001      123     1832 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/graph.py
--rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/__init__.py
--rw-r--r--   0     1001      123      645 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/base.py
--rw-r--r--   0     1001      123      356 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/marshmallow.py
--rw-r--r--   0     1001      123      704 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/mashumaro.py
--rw-r--r--   0     1001      123      521 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/pydantic.py
--rw-r--r--   0     1001      123      355 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/serpyco.py
--rw-r--r--   0     1001      123      361 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/libs/serpyco_rs.py
--rw-r--r--   0     1001      123     1642 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/compare/test_benchmarks.py
--rw-r--r--   0     1001      123     6092 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/test_encoders.py
--rw-r--r--   0     1001      123      803 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/test_full.py
--rw-r--r--   0     1001      123      197 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/bench/utils.py
--rw-r--r--   0     1001      123     2271 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/noxfile.py
--rw-r--r--   0     1001      123      948 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/pyproject.toml
--rw-r--r--   0     1001      123      152 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/__init__.py
--rw-r--r--   0     1001      123    16736 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_describe.py
--rw-r--r--   0     1001      123       72 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_impl.py
--rw-r--r--   0     1001      123      320 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_impl.pyi
--rw-r--r--   0     1001      123      199 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/__init__.py
--rw-r--r--   0     1001      123     6010 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_convert.py
--rw-r--r--   0     1001      123     5094 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_entities.py
--rw-r--r--   0     1001      123     1035 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_validate.py
--rw-r--r--   0     1001      123     1234 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_main.py
--rw-r--r--   0     1001      123      166 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/_utils.py
--rw-r--r--   0     1001      123      364 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/exceptions.py
--rw-r--r--   0     1001      123     1464 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/metadata.py
--rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/python/serpyco_rs/py.typed
--rw-r--r--   0     1001      123      110 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/bench.txt
--rw-r--r--   0     1001      123       78 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/dev.txt
--rw-r--r--   0     1001      123       29 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/lint.txt
--rw-r--r--   0     1001      123       47 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/requirements/type_check.txt
--rwxr-xr-x   0     1001      123     1010 2023-04-26 13:54:41.000000 serpyco_rs-0.9.1/run-maturin-action.sh
--rw-r--r--   0     1001      123       54 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/build.rs
--rw-r--r--   0     1001      123      297 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/lib.rs
--rw-r--r--   0     1001      123     4430 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/dateutil.rs
--rw-r--r--   0     1001      123    13404 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/encoders.rs
--rw-r--r--   0     1001      123     2252 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/macros.rs
--rw-r--r--   0     1001      123     8828 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/main.rs
--rw-r--r--   0     1001      123     5126 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/py.rs
--rw-r--r--   0     1001      123     7134 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer/types.rs
--rw-r--r--   0     1001      123      152 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/src/serializer.rs
--rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/json_schema/__init__.py
--rw-r--r--   0     1001      123    11743 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/json_schema/test_convert.py
--rw-r--r--   0     1001      123     6944 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/json_schema/test_validator.py
--rw-r--r--   0     1001      123    20723 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test__describe.py
--rw-r--r--   0     1001      123     1234 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_custom_encoder.py
--rw-r--r--   0     1001      123     5798 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_encoders.py
--rw-r--r--   0     1001      123     1496 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_metadata.py
--rw-r--r--   0     1001      123     2567 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_recursive.py
--rw-r--r--   0     1001      123     6100 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_simple.py
--rw-r--r--   0     1001      123     3981 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/tests/test_union.py
--rw-r--r--   0     1001      123    14885 2023-04-26 13:54:08.000000 serpyco_rs-0.9.1/Cargo.lock
--rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 serpyco_rs-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 serpyco_rs-0.9.2/Cargo.toml
+-rw-r--r--   0     1001      123       25 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.envrc.example
+-rw-r--r--   0     1001      123      196 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.github/dependabot.yml
+-rw-r--r--   0     1001      123     4009 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.gitignore
+-rw-r--r--   0     1001      123     1069 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/LICENSE
+-rw-r--r--   0     1001      123       34 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/MANIFEST.in
+-rw-r--r--   0     1001      123     8943 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/README.md
+-rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/__init__.py
+-rw-r--r--   0     1001      123     1832 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/graph.py
+-rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/__init__.py
+-rw-r--r--   0     1001      123      645 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/base.py
+-rw-r--r--   0     1001      123      356 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/marshmallow.py
+-rw-r--r--   0     1001      123      704 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/mashumaro.py
+-rw-r--r--   0     1001      123      521 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/pydantic.py
+-rw-r--r--   0     1001      123      355 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/serpyco.py
+-rw-r--r--   0     1001      123      361 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/serpyco_rs.py
+-rw-r--r--   0     1001      123     1642 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/test_benchmarks.py
+-rw-r--r--   0     1001      123     6092 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/test_encoders.py
+-rw-r--r--   0     1001      123      803 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/test_full.py
+-rw-r--r--   0     1001      123      197 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/utils.py
+-rw-r--r--   0     1001      123     2289 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/noxfile.py
+-rw-r--r--   0     1001      123      948 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/pyproject.toml
+-rw-r--r--   0     1001      123      152 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/__init__.py
+-rw-r--r--   0     1001      123    16825 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_describe.py
+-rw-r--r--   0     1001      123       72 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_impl.py
+-rw-r--r--   0     1001      123      320 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_impl.pyi
+-rw-r--r--   0     1001      123      199 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/__init__.py
+-rw-r--r--   0     1001      123     6015 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_convert.py
+-rw-r--r--   0     1001      123     5094 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_entities.py
+-rw-r--r--   0     1001      123     1035 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_validate.py
+-rw-r--r--   0     1001      123     1234 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_main.py
+-rw-r--r--   0     1001      123      166 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_utils.py
+-rw-r--r--   0     1001      123      364 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/exceptions.py
+-rw-r--r--   0     1001      123     1464 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/metadata.py
+-rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/py.typed
+-rw-r--r--   0     1001      123      110 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/bench.txt
+-rw-r--r--   0     1001      123       78 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/dev.txt
+-rw-r--r--   0     1001      123       29 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/lint.txt
+-rw-r--r--   0     1001      123       47 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/type_check.txt
+-rwxr-xr-x   0     1001      123     1013 2023-04-26 18:01:37.000000 serpyco_rs-0.9.2/run-maturin-action.sh
+-rw-r--r--   0     1001      123       54 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/build.rs
+-rw-r--r--   0     1001      123      297 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/lib.rs
+-rw-r--r--   0     1001      123     4430 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/dateutil.rs
+-rw-r--r--   0     1001      123    13465 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/encoders.rs
+-rw-r--r--   0     1001      123     2252 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/macros.rs
+-rw-r--r--   0     1001      123     9108 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/main.rs
+-rw-r--r--   0     1001      123     5126 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/py.rs
+-rw-r--r--   0     1001      123     7134 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/types.rs
+-rw-r--r--   0     1001      123      152 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer.rs
+-rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/json_schema/__init__.py
+-rw-r--r--   0     1001      123    11743 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/json_schema/test_convert.py
+-rw-r--r--   0     1001      123     6944 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/json_schema/test_validator.py
+-rw-r--r--   0     1001      123    20837 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test__describe.py
+-rw-r--r--   0     1001      123     1234 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_custom_encoder.py
+-rw-r--r--   0     1001      123     5798 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_encoders.py
+-rw-r--r--   0     1001      123     1496 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_metadata.py
+-rw-r--r--   0     1001      123     2567 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_recursive.py
+-rw-r--r--   0     1001      123     6100 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_simple.py
+-rw-r--r--   0     1001      123     4304 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_union.py
+-rw-r--r--   0     1001      123    14885 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/Cargo.lock
+-rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 serpyco_rs-0.9.2/PKG-INFO
```

### Comparing `serpyco_rs-0.9.1/Cargo.toml` & `serpyco_rs-0.9.2/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "serpyco-rs"
-version = "0.9.1"
+version = "0.9.2"
 edition = "2021"
 homepage = "https://github.com/ermakov-oleg/serpyco-rs"
 repository = "https://github.com/ermakov-oleg/serpyco-rs"
 
 [package.metadata.maturin]
 python-source = "python"
 name = "serpyco_rs._serpyco_rs"
```

### Comparing `serpyco_rs-0.9.1/.github/workflows/CI.yml` & `serpyco_rs-0.9.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/.gitignore` & `serpyco_rs-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/LICENSE` & `serpyco_rs-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/README.md` & `serpyco_rs-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/compare/graph.py` & `serpyco_rs-0.9.2/bench/compare/graph.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/compare/libs/base.py` & `serpyco_rs-0.9.2/bench/compare/libs/base.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/compare/libs/mashumaro.py` & `serpyco_rs-0.9.2/bench/compare/libs/mashumaro.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/compare/libs/pydantic.py` & `serpyco_rs-0.9.2/bench/compare/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/compare/test_benchmarks.py` & `serpyco_rs-0.9.2/bench/compare/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/test_encoders.py` & `serpyco_rs-0.9.2/bench/test_encoders.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/bench/test_full.py` & `serpyco_rs-0.9.2/bench/test_full.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/noxfile.py` & `serpyco_rs-0.9.2/noxfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     session.run_always("maturin", "develop", "-r")
 
 
 @nox.session
 def test(session):
     build(session)
     session.install("-r", "requirements/dev.txt")
-    session.run("pytest", "-vss", "tests/")
+    session.run("pytest", "-vss", "tests/", *session.posargs)
 
 
 @nox.session
 def lint(session):
     build(session)
     session.install("-r", "requirements/lint.txt")
```

### Comparing `serpyco_rs-0.9.1/pyproject.toml` & `serpyco_rs-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/python/serpyco_rs/_describe.py` & `serpyco_rs-0.9.2/python/serpyco_rs/_describe.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,16 @@
 class TupleType(Type):
     item_types: Sequence[Type]
 
 
 @dataclasses.dataclass
 class UnionType(Type):
     item_types: Mapping[str, Type]
-    discriminator: str
+    dump_discriminator: str
+    load_discriminator: str
 
 
 @dataclasses.dataclass
 class AnyType(Type):
     pass
 
 
@@ -371,15 +372,16 @@
 
         meta = dataclasses.replace(meta, discriminator_field=discriminator.name)
         return UnionType(
             item_types={
                 _get_discriminator_value(arg, discriminator.name): describe_type(annotation_wrapper(arg), meta)
                 for arg in args
             },
-            discriminator=_apply_format(filed_format, discriminator.name),
+            dump_discriminator=discriminator.name,
+            load_discriminator=_apply_format(filed_format, discriminator.name),
             custom_encoder=custom_encoder,
         )
 
     if isinstance(t, TypeVar):
         raise RuntimeError(f"Unfilled TypeVar: {t}")
 
     raise RuntimeError(f"Unknown type {t!r}")
```

### Comparing `serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_convert.py` & `serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         for name, t in arg.item_types.items()
         if (schema := to_json_schema(t)) and _check_unions_schema_types(schema)
     }
 
     return UnionType(
         oneOf=list(objects.values()),
         discriminator=Discriminator(
-            property_name=arg.discriminator,
+            property_name=arg.load_discriminator,
             mapping={name: cast(str, val.ref) for name, val in objects.items()},
         ),
         description=doc,
     )
 
 
 def _check_unions_schema_types(schema: Schema) -> TypeGuard[Union[ObjectType, RefType]]:
```

### Comparing `serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_entities.py` & `serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_entities.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/python/serpyco_rs/_json_schema/_validate.py` & `serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_validate.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/python/serpyco_rs/_main.py` & `serpyco_rs-0.9.2/python/serpyco_rs/_main.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/python/serpyco_rs/metadata.py` & `serpyco_rs-0.9.2/python/serpyco_rs/metadata.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/run-maturin-action.sh` & `serpyco_rs-0.9.2/run-maturin-action.sh`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 echo "::group::Install maturin"
 curl -L https://github.com/PyO3/maturin/releases/download/v0.13.7/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
 python3 -m pip install cffi || true
 echo "::endgroup::"
 echo "::group::Install sccache"
-python3 -m pip install --pre sccache
+python3 -m pip install "sccache>=0.4.0"
 sccache --version
 echo "::endgroup::"
 maturin build --release --sdist -o dist --find-interpreter
 echo "::group::sccache stats"
 sccache --show-stats
 echo "::endgroup::"
```

### Comparing `serpyco_rs-0.9.1/src/serializer/dateutil.rs` & `serpyco_rs-0.9.2/src/serializer/dateutil.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/src/serializer/encoders.rs` & `serpyco_rs-0.9.2/src/serializer/encoders.rs`

 * *Files 2% similar despite different names*

```diff
@@ -313,35 +313,36 @@
         Ok(tuple)
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct UnionEncoder {
     pub(crate) encoders: HashMap<String, Box<TEncoder>>,
-    pub(crate) discriminator: Py<PyString>,
+    pub(crate) dump_discriminator: Py<PyString>,
+    pub(crate) load_discriminator: Py<PyString>,
 }
 
 impl Encoder for UnionEncoder {
     #[inline]
     fn dump(&self, value: *mut PyObject) -> PyResult<*mut PyObject> {
-        let discriminator = ffi!(PyObject_GetAttr(value, self.discriminator.as_ptr())); // val RC +1
+        let discriminator = py_object_get_attr(value, self.dump_discriminator.as_ptr())?; // val RC +1
         let key = py_str_to_str(discriminator)?;
         let encoder = self
             .encoders
             .get(key)
             .ok_or(ValidationError::new_err(format!(
                 "No encoder for '{key}' discriminator"
             )))?;
         ffi!(Py_DECREF(discriminator));
         encoder.dump(value)
     }
 
     #[inline]
     fn load(&self, value: *mut PyObject) -> PyResult<*mut PyObject> {
-        let discriminator = py_object_get_item(value, self.discriminator.as_ptr())?; // val RC +1
+        let discriminator = py_object_get_item(value, self.load_discriminator.as_ptr())?; // val RC +1
         let key = py_str_to_str(discriminator)?;
         let encoder = self
             .encoders
             .get(key)
             .ok_or(ValidationError::new_err(format!(
                 "No encoder for '{key}' discriminator"
             )))?;
```

### Comparing `serpyco_rs-0.9.1/src/serializer/macros.rs` & `serpyco_rs-0.9.2/src/serializer/macros.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/src/serializer/main.rs` & `serpyco_rs-0.9.2/src/serializer/main.rs`

 * *Files 6% similar despite different names*

```diff
@@ -110,16 +110,19 @@
                 let item_type = item_type?;
                 let encoder = get_encoder(py, get_object_type(item_type)?, encoder_state)?;
                 encoders.push(encoder);
             }
             wrap_with_custom_encoder(py, type_info, Box::new(TupleEncoder { encoders }))?
         }
         Type::UnionType(type_info) => {
-            let discriminator_raw = type_info.getattr(py, "discriminator")?;
-            let discriminator: &PyString = discriminator_raw.as_ref(py).downcast()?;
+            let dump_discriminator_raw = type_info.getattr(py, "dump_discriminator")?;
+            let dump_discriminator: &PyString = dump_discriminator_raw.as_ref(py).downcast()?;
+
+            let load_discriminator_raw = type_info.getattr(py, "load_discriminator")?;
+            let load_discriminator: &PyString = load_discriminator_raw.as_ref(py).downcast()?;
 
             let item_types_raw = type_info.getattr(py, "item_types")?;
             let item_types: &PyDict = item_types_raw.as_ref(py).downcast()?;
 
             let mut encoders = HashMap::new();
 
             for (key, value) in item_types.iter() {
@@ -129,15 +132,16 @@
             }
 
             wrap_with_custom_encoder(
                 py,
                 type_info,
                 Box::new(UnionEncoder {
                     encoders,
-                    discriminator: discriminator.into(),
+                    dump_discriminator: dump_discriminator.into(),
+                    load_discriminator: load_discriminator.into(),
                 }),
             )?
         }
         Type::Entity(type_info) => {
             let py_type = type_info.getattr(py, "cls")?;
             let class_fields = type_info.getattr(py, "fields")?;
             let omit_none = type_info.getattr(py, "omit_none")?.is_true(py)?;
```

### Comparing `serpyco_rs-0.9.1/src/serializer/py.rs` & `serpyco_rs-0.9.2/src/serializer/py.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/src/serializer/types.rs` & `serpyco_rs-0.9.2/src/serializer/types.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/json_schema/test_convert.py` & `serpyco_rs-0.9.2/tests/json_schema/test_convert.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/json_schema/test_validator.py` & `serpyco_rs-0.9.2/tests/json_schema/test_validator.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/test__describe.py` & `serpyco_rs-0.9.2/tests/test__describe.py`

 * *Files 3% similar despite different names*

```diff
@@ -620,24 +620,24 @@
     assert describe_type(Literal["foo", "bar"]) == LiteralType(args=("foo", "bar"), custom_encoder=None)
 
 
 def test_describe__tagged_union():
     @dataclass
     class Foo:
         val: int
-        type: Literal["foo"]
+        filed_type: Literal["foo"]
 
     @dataclass
     class Bar:
         val: str
-        type: Literal["bar"]
+        filed_type: Literal["bar"]
 
     @dataclass
     class Base:
-        field: Annotated[Union[Foo, Bar], Discriminator("type")]
+        field: Annotated[Union[Foo, Bar], Discriminator("filed_type"), CamelCase]
 
     assert describe_type(Base) == EntityType(
         cls=Base,
         name=mock.ANY,
         fields=[
             EntityField(
                 name="field",
@@ -650,16 +650,16 @@
                             fields=[
                                 EntityField(
                                     name="val",
                                     dict_key="val",
                                     type=IntegerType(min=None, max=None, custom_encoder=None),
                                 ),
                                 EntityField(
-                                    name="type",
-                                    dict_key="type",
+                                    name="filed_type",
+                                    dict_key="filedType",
                                     type=LiteralType(args=("foo",), custom_encoder=None),
                                     is_discriminator_field=True,
                                 ),
                             ],
                             doc=mock.ANY,
                             custom_encoder=None,
                         ),
@@ -669,25 +669,26 @@
                             fields=[
                                 EntityField(
                                     name="val",
                                     dict_key="val",
                                     type=StringType(min_length=None, max_length=None, custom_encoder=None),
                                 ),
                                 EntityField(
-                                    name="type",
-                                    dict_key="type",
+                                    name="filed_type",
+                                    dict_key="filedType",
                                     type=LiteralType(args=("bar",), custom_encoder=None),
                                     is_discriminator_field=True,
                                 ),
                             ],
                             doc=mock.ANY,
                             custom_encoder=None,
                         ),
                     },
-                    discriminator="type",
+                    load_discriminator="filedType",
+                    dump_discriminator="filed_type",
                     custom_encoder=None,
                 ),
             )
         ],
         doc=mock.ANY,
         custom_encoder=None,
     )
```

### Comparing `serpyco_rs-0.9.1/tests/test_custom_encoder.py` & `serpyco_rs-0.9.2/tests/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/test_encoders.py` & `serpyco_rs-0.9.2/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/test_metadata.py` & `serpyco_rs-0.9.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/test_recursive.py` & `serpyco_rs-0.9.2/tests/test_recursive.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/test_simple.py` & `serpyco_rs-0.9.2/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.1/tests/test_union.py` & `serpyco_rs-0.9.2/tests/test_union.py`

 * *Files 15% similar despite different names*

```diff
@@ -148,21 +148,35 @@
         a: int
 
     @dataclass
     class B:
         discriminator_with_multiple_words: Literal["B"]
         b: str
 
-    a = {
-        "discriminatorWithMultipleWords": "A",
-        "a": 128,
-    }
+    raw_obj = [
+        {
+            "discriminatorWithMultipleWords": "A",
+            "a": 128,
+        },
+        {
+            "discriminatorWithMultipleWords": "B",
+            "b": "foo",
+        },
+    ]
+    obj = [
+        A(
+            discriminator_with_multiple_words="A",
+            a=128,
+        ),
+        B(
+            discriminator_with_multiple_words="B",
+            b="foo",
+        ),
+    ]
 
     serializer = Serializer(
-        Annotated[Union[A, B], Discriminator("discriminator_with_multiple_words")],
+        list[Annotated[Union[A, B], Discriminator("discriminator_with_multiple_words")]],
         camelcase_fields=True,
     )
 
-    assert serializer.load(a) == A(
-        discriminator_with_multiple_words="A",
-        a=128,
-    )
+    assert serializer.dump(obj) == raw_obj
+    assert serializer.load(raw_obj) == obj
```

### Comparing `serpyco_rs-0.9.1/Cargo.lock` & `serpyco_rs-0.9.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 name = "scratch"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8132065adcfd6e02db789d9285a0deb2f3fcb04002865ab67d5fb103533898"
 
 [[package]]
 name = "serpyco-rs"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "atomic_refcell",
  "cfg-if",
  "chrono",
  "dyn-clone",
  "pyo3",
  "pyo3-build-config",
```

### Comparing `serpyco_rs-0.9.1/PKG-INFO` & `serpyco_rs-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serpyco-rs
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

