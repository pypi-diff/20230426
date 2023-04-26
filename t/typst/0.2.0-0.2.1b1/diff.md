# Comparing `tmp/typst-0.2.0.tar.gz` & `tmp/typst-0.2.1b1.tar.gz`

## Comparing `typst-0.2.0.tar` & `typst-0.2.1b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 typst-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     2752 2023-04-12 02:23:06.000000 typst-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-12 02:23:06.000000 typst-0.2.0/.gitignore
--rw-r--r--   0     1001      123     9723 2023-04-12 02:23:06.000000 typst-0.2.0/LICENSE
--rw-r--r--   0     1001      123      766 2023-04-12 02:23:06.000000 typst-0.2.0/README.md
--rw-r--r--   0     1001      123      421 2023-04-12 02:23:06.000000 typst-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123       74 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/__init__.py
--rw-r--r--   0     1001      123      483 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/__init__.pyi
--rw-r--r--   0     1001      123   331992 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
--rw-r--r--   0     1001      123   253580 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
--rw-r--r--   0     1001      123   251932 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
--rw-r--r--   0     1001      123   340712 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono.ttf
--rw-r--r--   0     1001      123   806856 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_R.ttf
--rw-r--r--   0     1001      123   748600 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_RB.ttf
--rw-r--r--   0     1001      123   533532 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_RBI.ttf
--rw-r--r--   0     1001      123   721340 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_RI.ttf
--rw-r--r--   0     1001      123   499128 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-Bold.otf
--rw-r--r--   0     1001      123   445800 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-BoldItalic.otf
--rw-r--r--   0     1001      123   464808 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-Italic.otf
--rw-r--r--   0     1001      123   547508 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-Regular.otf
--rw-r--r--   0     1001      123  2161432 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCMMath-Book.otf
--rw-r--r--   0     1001      123  1229208 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCMMath-Regular.otf
--rw-r--r--   0     1001      123        1 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/py.typed
--rw-r--r--   0     1001      123     9415 2023-04-12 02:23:06.000000 typst-0.2.0/src/compiler.rs
--rw-r--r--   0     1001      123     3946 2023-04-12 02:23:06.000000 typst-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123    41249 2023-04-12 02:23:06.000000 typst-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 typst-0.2.1b1/Cargo.toml
+-rw-r--r--   0     1001      123     2617 2023-04-26 12:51:16.000000 typst-0.2.1b1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-26 12:51:16.000000 typst-0.2.1b1/.gitignore
+-rw-r--r--   0     1001      123     9723 2023-04-26 12:51:16.000000 typst-0.2.1b1/LICENSE
+-rw-r--r--   0     1001      123      766 2023-04-26 12:51:16.000000 typst-0.2.1b1/README.md
+-rw-r--r--   0     1001      123      421 2023-04-26 12:51:16.000000 typst-0.2.1b1/pyproject.toml
+-rw-r--r--   0     1001      123       74 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/__init__.py
+-rw-r--r--   0     1001      123      483 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/__init__.pyi
+-rw-r--r--   0     1001      123   331992 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0     1001      123   253580 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
+-rw-r--r--   0     1001      123   251932 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/DejaVuSansMono-Oblique.ttf
+-rw-r--r--   0     1001      123   340712 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0     1001      123   806856 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/LinLibertine_R.ttf
+-rw-r--r--   0     1001      123   748600 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/LinLibertine_RB.ttf
+-rw-r--r--   0     1001      123   533532 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/LinLibertine_RBI.ttf
+-rw-r--r--   0     1001      123   721340 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/LinLibertine_RI.ttf
+-rw-r--r--   0     1001      123   499128 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/NewCM10-Bold.otf
+-rw-r--r--   0     1001      123   445800 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/NewCM10-BoldItalic.otf
+-rw-r--r--   0     1001      123   464808 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/NewCM10-Italic.otf
+-rw-r--r--   0     1001      123   547508 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/NewCM10-Regular.otf
+-rw-r--r--   0     1001      123  2161432 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/NewCMMath-Book.otf
+-rw-r--r--   0     1001      123  1229208 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/fonts/NewCMMath-Regular.otf
+-rw-r--r--   0     1001      123        1 2023-04-26 12:51:16.000000 typst-0.2.1b1/python/typst/py.typed
+-rw-r--r--   0     1001      123     9415 2023-04-26 12:51:16.000000 typst-0.2.1b1/src/compiler.rs
+-rw-r--r--   0     1001      123     3946 2023-04-26 12:51:16.000000 typst-0.2.1b1/src/lib.rs
+-rw-r--r--   0     1001      123    41243 2023-04-26 12:51:16.000000 typst-0.2.1b1/Cargo.lock
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 typst-0.2.1b1/PKG-INFO
```

### Comparing `typst-0.2.0/Cargo.toml` & `typst-0.2.1b1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typst-py"
-version = "0.2.0"
+version = "0.2.1-beta.1"
 edition = "2021"
 description = "Python binding to typst"
 license = "Apache-2.0"
 repository = "https://github.com/messense/typst-py"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `typst-0.2.0/.github/workflows/CI.yml` & `typst-0.2.1b1/.github/workflows/CI.yml`

 * *Files 4% similar despite different names*

```diff
@@ -103,18 +103,14 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows, macos, sdist]
+    permissions:
+      id-token: write
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
-      - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --skip-existing *
+      - uses: mxschmitt/action-tmate@v3
```

### Comparing `typst-0.2.0/.gitignore` & `typst-0.2.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/LICENSE` & `typst-0.2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/README.md` & `typst-0.2.1b1/README.md`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/DejaVuSansMono-Bold.ttf` & `typst-0.2.1b1/python/typst/fonts/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf` & `typst-0.2.1b1/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf` & `typst-0.2.1b1/python/typst/fonts/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/DejaVuSansMono.ttf` & `typst-0.2.1b1/python/typst/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/LinLibertine_R.ttf` & `typst-0.2.1b1/python/typst/fonts/LinLibertine_R.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/LinLibertine_RB.ttf` & `typst-0.2.1b1/python/typst/fonts/LinLibertine_RB.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/LinLibertine_RBI.ttf` & `typst-0.2.1b1/python/typst/fonts/LinLibertine_RBI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/LinLibertine_RI.ttf` & `typst-0.2.1b1/python/typst/fonts/LinLibertine_RI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/NewCM10-Bold.otf` & `typst-0.2.1b1/python/typst/fonts/NewCM10-Bold.otf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/NewCM10-BoldItalic.otf` & `typst-0.2.1b1/python/typst/fonts/NewCM10-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/NewCM10-Italic.otf` & `typst-0.2.1b1/python/typst/fonts/NewCM10-Italic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/NewCM10-Regular.otf` & `typst-0.2.1b1/python/typst/fonts/NewCM10-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/NewCMMath-Book.otf` & `typst-0.2.1b1/python/typst/fonts/NewCMMath-Book.otf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/python/typst/fonts/NewCMMath-Regular.otf` & `typst-0.2.1b1/python/typst/fonts/NewCMMath-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/src/compiler.rs` & `typst-0.2.1b1/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/src/lib.rs` & `typst-0.2.1b1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typst-0.2.0/Cargo.lock` & `typst-0.2.1b1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "arrayref"
 version = "0.3.7"
@@ -107,32 +107,25 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chinese-number"
-version = "0.7.0"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "365a2e504d6cb41e85fba5d01a6baf7f13cad4424102859193c4674e7fdff933"
+checksum = "bb8659add27dbba7575c058a3265d81cc078dc2693848445bf3788a883ec82c8"
 dependencies = [
- "chinese-numerals",
  "chinese-variant",
  "enum-ordinalize",
  "num-bigint",
  "num-traits",
 ]
 
 [[package]]
-name = "chinese-numerals"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76a5a40575256b55eebe3e39fa41e53bdaea5d67ac5a7092fa8756020c798d1e"
-
-[[package]]
 name = "chinese-variant"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aeea139b89efab957972956e5d3e4efb66a6c261f726abf6911040cc8ef700f7"
 
 [[package]]
 name = "chrono"
@@ -148,27 +141,27 @@
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "comemo"
-version = "0.2.0"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22bf2c21093020535dd771993fedae8dd55393a4258cca501a9b55a962d350a5"
+checksum = "1ba423e212681b51c5452a458bb24e88165f4c09857a783c802719cc46313f3f"
 dependencies = [
  "comemo-macros",
  "siphasher",
 ]
 
 [[package]]
 name = "comemo-macros"
-version = "0.2.0"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9faa23f4534253fa656b176ff524d5cd7306a6fed3048929f9cc01ab38ab5a5a"
+checksum = "fca5ceeb99665bad04a32fe297d1581a68685e36fb6da92a1c9b7d9693638c01"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -239,17 +232,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "ecow"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e60e2840fbfc397c7972b11a6e6bd99a0248921cc1e31f293c5f6c5ac24831da"
+checksum = "c5c5051925c54d9a42c8652313b5358a7432eed209466b443ed5220431243a14"
 
 [[package]]
 name = "elsa"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e0aca8dce8856e420195bd13b6a64de3334235ccc9214e824b86b12bf26283"
 dependencies = [
@@ -478,17 +471,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
@@ -737,66 +730,66 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
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
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
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
  "pyo3-build-config",
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
  "syn 1.0.109",
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
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -857,30 +850,36 @@
  "getrandom",
  "redox_syscall",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
+name = "regex-syntax"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+
+[[package]]
 name = "resvg"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2e702d1e8e00a3a0717b96244cba840f34f542d8f23097c8903266c4e2975658"
 dependencies = [
  "gif 0.11.4",
  "jpeg-decoder 0.2.6",
@@ -991,22 +990,22 @@
 name = "serde_derive"
 version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.14",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1112,17 +1111,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.14"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcf316d5356ed6847742d036f8a39c3b8435cac10bd528a4bd461928a6ab34d5"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1134,27 +1133,27 @@
  "bincode",
  "bitflags",
  "fancy-regex",
  "flate2",
  "fnv",
  "lazy_static",
  "once_cell",
- "regex-syntax",
+ "regex-syntax 0.6.29",
  "serde",
  "serde_derive",
  "serde_json",
  "thiserror",
  "walkdir",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "thin-vec"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aac81b6fd6beb5884b0cf3321b8117e6e5d47ecb6fc89f414cfdcca8b2fe2dd8"
 
@@ -1171,15 +1170,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.14",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tiny-skia"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d049bfef0eaa2521e75d9ffb5ce86ad54480932ae19b85f78bec6f52c4d30d78"
@@ -1313,15 +1312,15 @@
  "quote",
  "syn 1.0.109",
  "unscanny",
 ]
 
 [[package]]
 name = "typst-py"
-version = "0.2.0"
+version = "0.2.1-beta.1"
 dependencies = [
  "comemo",
  "dirs",
  "elsa",
  "memmap2",
  "once_cell",
  "pyo3",
```

### Comparing `typst-0.2.0/PKG-INFO` & `typst-0.2.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst
-Version: 0.2.0
+Version: 0.2.1b1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python binding to typst
 License: Apache-2.0
 Requires-Python: >=3.7
```

