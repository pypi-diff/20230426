# Comparing `tmp/pyaiken-0.4.0.tar.gz` & `tmp/pyaiken-0.5.0.tar.gz`

## Comparing `pyaiken-0.4.0.tar` & `pyaiken-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 pyaiken-0.4.0/Cargo.toml
--rw-r--r--   0     1001      123      329 2023-02-24 12:29:03.000000 pyaiken-0.4.0/.ci/deploy_to_pypi.sh
--rw-r--r--   0     1001      123     1506 2023-02-24 12:29:03.000000 pyaiken-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     6782 2023-02-24 12:29:03.000000 pyaiken-0.4.0/.gitignore
--rw-r--r--   0     1001      123     1053 2023-02-24 12:29:03.000000 pyaiken-0.4.0/LICENSE.txt
--rw-r--r--   0     1001      123     2090 2023-02-24 12:29:03.000000 pyaiken-0.4.0/README.md
--rw-r--r--   0     1001      123      919 2023-02-24 12:29:03.000000 pyaiken-0.4.0/pyproject.toml
--rwxr-xr-x   0     1001      123      833 2023-02-24 12:29:34.000000 pyaiken-0.4.0/run-maturin-action.sh
--rw-r--r--   0     1001      123     3617 2023-02-24 12:29:03.000000 pyaiken-0.4.0/src/lib.rs
--rw-r--r--   0        0        0    26640 2023-02-24 12:30:54.000000 pyaiken-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 pyaiken-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 pyaiken-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      123      329 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.ci/deploy_to_pypi.sh
+-rw-r--r--   0     1001      123     1506 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     6782 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.gitignore
+-rw-r--r--   0     1001      123      527 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.travis.yml
+-rw-r--r--   0     1001      123     1053 2023-04-26 07:33:32.000000 pyaiken-0.5.0/LICENSE.txt
+-rw-r--r--   0     1001      123     2049 2023-04-26 07:33:32.000000 pyaiken-0.5.0/README.md
+-rw-r--r--   0     1001      123      894 2023-04-26 07:33:32.000000 pyaiken-0.5.0/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-04-26 07:34:01.000000 pyaiken-0.5.0/run-maturin-action.sh
+-rw-r--r--   0     1001      123     3689 2023-04-26 07:33:32.000000 pyaiken-0.5.0/src/lib.rs
+-rw-r--r--   0        0        0    30683 2023-04-26 07:35:09.000000 pyaiken-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 pyaiken-0.5.0/PKG-INFO
```

### Comparing `pyaiken-0.4.0/.github/workflows/CI.yml` & `pyaiken-0.5.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyaiken-0.4.0/.gitignore` & `pyaiken-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyaiken-0.4.0/LICENSE.txt` & `pyaiken-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyaiken-0.4.0/README.md` & `pyaiken-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pyaiken
 =======
-[![CI](https://github.com/ImperatorLang/pyaiken/actions/workflows/CI.yml/badge.svg)](https://github.com/ImperatorLang/pyaiken/actions/workflows/CI.yml)
+[![CI](https://github.com/OpShin/pyaiken/actions/workflows/CI.yml/badge.svg)](https://github.com/OpShin/pyaiken/actions/workflows/CI.yml)
 [![PyPI version](https://badge.fury.io/py/pyaiken.svg)](https://pypi.org/project/pyaiken/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pyaiken.svg)](https://pypi.org/project/pyaiken/)
 
 This package supplies python bindings for the package [aiken](https://github.com/aiken-lang/aiken).
-The bindings are added on a per-need basis, currently only serving the development of [eopsin](https://github.com/ImperatorLang/eopsin)
+The bindings are added on a per-need basis, currently only serving the development of [opshin](https://github.com/opshin)
 
 
 ### Installation
 
 Install python3. Then run the following command.
 
 ```bash
@@ -43,25 +43,25 @@
 # Evaluate a UPLC program with the given arguments (all in textual representation) and cpu and memory budget (optional, in this order)
 # Returns either computed UPLC value on success or thrown error on failure,
 # logs generated through trace
 # and the consumed cpu and memory steps
 ((suc, err), logs, (cpu, mem)) = uplc.eval("(program 1.0.0 (lam x x))", ["(con data #01)"], 1000000, None)
 
 print((suc, err), logs, (cpu, mem))
-# prints "('(con data #01)', None), [], (9907900, 13999500)"
+# prints "('(con data #01)', None), [], (92100, 500)"
 
 ```
 
 ### Building
 
 In case you need to build this package from source, install Python3 and Rust and proceed as follows.
 
 ```bash
-git clone https://github.com/ImperatorLang/pyaiken
+git clone https://github.com/OpShin/pyaiken
 cd pyaiken
 python3 -m venv .env
 source .env/bin/activate  # or in whichever environment you want to have it installed
 pip install maturin
 maturin build
 ```
 
-The package will be installed in the active python environment.
+The package will be installed in the active python environment.
```

### Comparing `pyaiken-0.4.0/pyproject.toml` & `pyaiken-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 [project]
 name = "pyaiken"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 description = "Python bindings for aiken"
 keywords=["python", "rust", "cardano", "smart contract", "blockchain"]
 license = {file = "LICENSE.txt"}
 long-description = {file = "README.md"}
 authors = [
   {email = "n.muendler@posteo.de"},
   {name = "Niels Mündler"}
 ]
 maintainers = [
   {name = "Niels Mündler", email = "n.muendler@posteo.de"}
 ]
-url = "https://github.com/imperatorlang/uplc"
+url = "https://github.com/opshin/uplc"
```

### Comparing `pyaiken-0.4.0/run-maturin-action.sh` & `pyaiken-0.5.0/run-maturin-action.sh`

 * *Files 1% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain stable
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set stable
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
 export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.14.14/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v0.14.17/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
 python3 -m pip install cffi || true
 echo "::endgroup::"
 maturin build --release --sdist -o dist --find-interpreter
```

### Comparing `pyaiken-0.4.0/src/lib.rs` & `pyaiken-0.5.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -104,15 +104,18 @@
     let mem = match budget.1 {
         Some(budget) => budget,
         None => ExBudget::default().mem
     };
 
     let budget = ExBudget { mem: mem, cpu: cpu };
 
-    let (term, cost, logs) = program.eval(budget);
+    let mut res = program.eval(budget);
+    let cost = res.cost();
+    let logs = res.logs();
+    let term = res.result();
 
     return Ok((
         match term {
             Ok(term) => {
                 (Some(term.to_string()), None)
             }
             Err(err) => {
```

### Comparing `pyaiken-0.4.0/Cargo.lock` & `pyaiken-0.5.0/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -26,45 +26,34 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
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
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 
 [[package]]
 name = "arrayvec"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
 
 [[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi",
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "backtrace"
@@ -78,14 +67,23 @@
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
+name = "backtrace-ext"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "537beee3be4a18fb023b570f80e3ae28003db9167a751266b259926e25539d50"
+dependencies = [
+ "backtrace",
+]
+
+[[package]]
 name = "base58"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6107fe1be6682a68940da878d9e9f5e90ca5745b3dec9fd1bb393c8777d4f581"
 
 [[package]]
 name = "bech32"
@@ -120,15 +118,15 @@
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
@@ -136,28 +134,49 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "flat-rs"
-version = "0.0.27"
+version = "1.0.2-alpha"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cfc458c5529a33581b2c5139b03885a823c55713e6db2ff0447bff87393e097"
+checksum = "bde678538a2859f832d89c93fb7f46cce855b96d4f0945f0149880dcd19d9dc2"
 dependencies = [
  "anyhow",
  "thiserror",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -185,44 +204,64 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "is-terminal"
+version = "0.4.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+dependencies = [
+ "hermit-abi",
+ "io-lifetimes",
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "is_ci"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "616cde7c720bb2bb5824a224687d8f77bfd38922027f01d825cd7453be5099fb"
 
 [[package]]
 name = "itertools"
@@ -231,23 +270,29 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.142"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -277,62 +322,63 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miette"
-version = "5.5.0"
+version = "5.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4afd9b301defa984bbdbe112b4763e093ed191750a0d914a78c1106b2d0fe703"
+checksum = "92a992891d5579caa9efd8e601f82e30a1caa79a27a5db075dde30ecb9eab357"
 dependencies = [
- "atty",
  "backtrace",
+ "backtrace-ext",
+ "is-terminal",
  "miette-derive",
  "once_cell",
  "owo-colors",
  "supports-color",
  "supports-hyperlinks",
  "supports-unicode",
  "terminal_size",
  "textwrap",
  "thiserror",
  "unicode-width",
 ]
 
 [[package]]
 name = "miette-derive"
-version = "5.5.0"
+version = "5.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97c2401ab7ac5282ca5c8b518a87635b1a93762b0b90b9990c509888eeccba29"
+checksum = "4c65c625186a9bcce6699394bee511e1b1aec689aa7e3be1bf4e996e75834153"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "minicbor"
-version = "0.18.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a20020e8e2d1881d8736f64011bb5ff99f1db9947ce3089706945c8915695cb"
+checksum = "d7005aaf257a59ff4de471a9d5538ec868a21586534fff7f85dd97d4043a6139"
 dependencies = [
  "half",
  "minicbor-derive",
 ]
 
 [[package]]
 name = "minicbor-derive"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8608fb1c805b5b6b3d5ab7bd95c40c396df622b64d77b2d621a5eae1eed050ee"
+checksum = "1154809406efdb7982841adb6311b3d095b46f78342dd646736122fe6b19e267"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
@@ -398,72 +444,72 @@
 name = "owo-colors"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1b04fb49957986fdce4d6ee7a65027d55d4b6d2265e5848bbb507b58ccfdb6f"
 
 [[package]]
 name = "pallas-addresses"
-version = "0.16.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31a4845f1022856fd77af2ff563bce420470ec589e1f6f08897492b4948f78d0"
+checksum = "185e42a5022488c5bd15fb843d48382ee5d7bc2bfef2454ee8a9dec7ab1fc1eb"
 dependencies = [
  "base58",
  "bech32",
  "hex",
  "pallas-codec",
  "pallas-crypto",
  "thiserror",
 ]
 
 [[package]]
 name = "pallas-codec"
-version = "0.16.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36db2e36825d8c037a54a5be551e5b903f8007b1b1259bc7a737c3aeb904c9b7"
+checksum = "7194c1ee4fa15ba9f40955ee2599449ac648234337af53de7a7322d4d49fce73"
 dependencies = [
  "hex",
  "minicbor",
  "serde",
 ]
 
 [[package]]
 name = "pallas-crypto"
-version = "0.16.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42e34ccf8a9664e6d999ff90a19450cfabc565dc8eff6b394376383e4762083f"
+checksum = "f7984a500ca763bc88c606d208fa852b691fd946128c31473085da737cd7f73b"
 dependencies = [
  "cryptoxide",
  "hex",
  "pallas-codec",
  "rand_core",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "pallas-primitives"
-version = "0.16.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df74101aa78f8702d7e45ea22260ab8d2597e83b847924db3fbef1eb6f806c41"
+checksum = "6c8e089d1d1366bd20c7ec79916dae51391b9989dd05efb4d24e10e61ada3880"
 dependencies = [
  "base58",
  "bech32",
  "hex",
  "log",
  "pallas-codec",
  "pallas-crypto",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "pallas-traverse"
-version = "0.16.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "457ff2429dbc77dabba9fa0e4077c277b8a09a59b3db9bc262d79b307005b0af"
+checksum = "989aede160bf9d84b598b881d7645cdb5de3cdaa74af7b28d0486a2b8d4eb979"
 dependencies = [
  "hex",
  "pallas-addresses",
  "pallas-codec",
  "pallas-crypto",
  "pallas-primitives",
  "thiserror",
@@ -485,15 +531,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "peg"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a07f2cafdc3babeebc087e499118343442b742cc7c31b4d054682cc598508554"
@@ -541,24 +587,24 @@
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyaiken"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "hex",
  "miette",
  "pyo3",
  "uplc",
 ]
 
@@ -604,33 +650,33 @@
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
@@ -644,46 +690,60 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
+name = "rustix"
+version = "0.37.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0661814f891c57c930a610266415528da53c4933e6dea5fb350cbfe048a9ece"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
 
 [[package]]
 name = "rustversion"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5583e89e108996506031660fe09baa5011b9dd0341b89029313006d1fb508d70"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
@@ -694,46 +754,46 @@
 checksum = "4124a35fe33ae14259c490fd70fa199a32b9ce9502f2ee6bc4f81ec06fa65894"
 dependencies = [
  "secp256k1-sys",
 ]
 
 [[package]]
 name = "secp256k1-sys"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642a62736682fdd8c71da0eb273e453c8ac74e33b9fb310e22ba5b03ec7651ff"
+checksum = "70a129b9e9efbfb223753b9163c4ab3b13cff7fd9c7f010fbac25ab4099fa07e"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.93"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -760,61 +820,72 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "supports-color"
-version = "1.3.1"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ba6faf2ca7ee42fdd458f4347ae0a9bd6bcc445ad7cb57ad82b383f18870d6f"
+checksum = "4950e7174bffabe99455511c39707310e7e9b440364a2fcb1cc21521be57b354"
 dependencies = [
- "atty",
+ "is-terminal",
  "is_ci",
 ]
 
 [[package]]
 name = "supports-hyperlinks"
-version = "1.2.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "590b34f7c5f01ecc9d78dba4b3f445f31df750a67621cf31626f3b7441ce6406"
+checksum = "f84231692eb0d4d41e4cdd0cabfdd2e6cd9e255e65f80c9aa7c98dd502b4233d"
 dependencies = [
- "atty",
+ "is-terminal",
 ]
 
 [[package]]
 name = "supports-unicode"
-version = "1.0.2"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8b945e45b417b125a8ec51f1b7df2f8df7920367700d1f98aedd21e5735f8b2"
+checksum = "4b6c2cb240ab5dd21ed4906895ee23fe5a48acdbd15a3ce388e7b62a9b66baf7"
 dependencies = [
- "atty",
+ "is-terminal",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "terminal_size"
 version = "0.1.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "633c1a546cee861a1a6d0dc69ebeca693bf4296661ba7852b9d21d159e0506df"
 dependencies = [
@@ -831,43 +902,43 @@
  "smawk",
  "unicode-linebreak",
  "unicode-width",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-linebreak"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5faade31a542b8b35855fff6e8def199853b2da8da256da52f52f1316ee3137"
 dependencies = [
@@ -891,24 +962,25 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "uplc"
-version = "0.0.29"
+version = "1.0.2-alpha"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "492ae1252003b75b6edd46f19cf563a716b4667235f8050a54ee2fe45289a0ba"
+checksum = "5a0e70f2d2394d8f1ecbd764a2135ec79cb4546393319ef10be099891e817242"
 dependencies = [
  "anyhow",
  "cryptoxide",
  "flat-rs",
  "hex",
  "indexmap",
  "itertools",
+ "miette",
  "num-bigint",
  "num-integer",
  "num-traits",
  "pallas-addresses",
  "pallas-codec",
  "pallas-crypto",
  "pallas-primitives",
@@ -960,72 +1032,138 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "yansi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
```

### Comparing `pyaiken-0.4.0/PKG-INFO` & `pyaiken-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: pyaiken
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 Summary: Python bindings for aiken
 Keywords: python,rust,cardano,smart contract,blockchain
 Author: Niels Mündler
 Author-email: n.muendler@posteo.de
 Maintainer-email: Niels Mündler <n.muendler@posteo.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 pyaiken
 =======
-[![CI](https://github.com/ImperatorLang/pyaiken/actions/workflows/CI.yml/badge.svg)](https://github.com/ImperatorLang/pyaiken/actions/workflows/CI.yml)
+[![CI](https://github.com/OpShin/pyaiken/actions/workflows/CI.yml/badge.svg)](https://github.com/OpShin/pyaiken/actions/workflows/CI.yml)
 [![PyPI version](https://badge.fury.io/py/pyaiken.svg)](https://pypi.org/project/pyaiken/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pyaiken.svg)](https://pypi.org/project/pyaiken/)
 
 This package supplies python bindings for the package [aiken](https://github.com/aiken-lang/aiken).
-The bindings are added on a per-need basis, currently only serving the development of [eopsin](https://github.com/ImperatorLang/eopsin)
+The bindings are added on a per-need basis, currently only serving the development of [opshin](https://github.com/opshin)
 
 
 ### Installation
 
 Install python3. Then run the following command.
 
 ```bash
@@ -63,25 +63,26 @@
 # Evaluate a UPLC program with the given arguments (all in textual representation) and cpu and memory budget (optional, in this order)
 # Returns either computed UPLC value on success or thrown error on failure,
 # logs generated through trace
 # and the consumed cpu and memory steps
 ((suc, err), logs, (cpu, mem)) = uplc.eval("(program 1.0.0 (lam x x))", ["(con data #01)"], 1000000, None)
 
 print((suc, err), logs, (cpu, mem))
-# prints "('(con data #01)', None), [], (9907900, 13999500)"
+# prints "('(con data #01)', None), [], (92100, 500)"
 
 ```
 
 ### Building
 
 In case you need to build this package from source, install Python3 and Rust and proceed as follows.
 
 ```bash
-git clone https://github.com/ImperatorLang/pyaiken
+git clone https://github.com/OpShin/pyaiken
 cd pyaiken
 python3 -m venv .env
 source .env/bin/activate  # or in whichever environment you want to have it installed
 pip install maturin
 maturin build
 ```
 
 The package will be installed in the active python environment.
+
```

