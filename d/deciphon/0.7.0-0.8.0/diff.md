# Comparing `tmp/deciphon-0.7.0.tar.gz` & `tmp/deciphon-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon-0.7.0.tar", max compression
+gzip compressed data, was "deciphon-0.8.0.tar", max compression
```

## Comparing `deciphon-0.7.0.tar` & `deciphon-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,30 @@
--rw-r--r--   0        0        0     1063 2023-02-05 23:42:00.945231 deciphon-0.7.0/LICENSE
--rw-r--r--   0        0        0     2996 2023-02-08 11:19:00.538561 deciphon-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-02-05 23:50:26.348804 deciphon-0.7.0/deciphon/__init__.py
--rw-r--r--   0        0        0     1519 2023-02-08 11:12:49.067111 deciphon-0.7.0/deciphon/cli.py
--rw-r--r--   0        0        0      681 2023-02-08 11:01:23.965008 deciphon-0.7.0/deciphon/scan.py
--rw-r--r--   0        0        0      388 2023-02-08 05:24:50.049707 deciphon-0.7.0/deciphon/service_exit.py
--rw-r--r--   0        0        0      637 2023-02-08 10:43:43.335322 deciphon-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 deciphon-0.7.0/setup.py
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 deciphon-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-05 23:42:00.945231 deciphon-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2996 2023-02-08 11:19:00.538561 deciphon-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-05 23:50:26.348804 deciphon-0.8.0/deciphon/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 16:53:57.996737 deciphon-0.8.0/deciphon/api/__init__.py
+-rw-r--r--   0        0        0     4356 2023-03-06 10:42:06.208901 deciphon-0.8.0/deciphon/api/api.py
+-rw-r--r--   0        0        0     2215 2023-03-06 09:47:45.810524 deciphon-0.8.0/deciphon/api/cli.py
+-rw-r--r--   0        0        0     2616 2023-04-25 12:33:55.102304 deciphon-0.8.0/deciphon/cli.py
+-rw-r--r--   0        0        0      501 2023-02-10 13:02:37.810954 deciphon-0.8.0/deciphon/config.py
+-rw-r--r--   0        0        0        0 2023-03-06 10:22:22.559435 deciphon-0.8.0/deciphon/daemon/__init__.py
+-rw-r--r--   0        0        0      622 2023-03-06 10:24:39.743329 deciphon-0.8.0/deciphon/daemon/cli.py
+-rw-r--r--   0        0        0     1691 2023-03-06 10:42:28.436070 deciphon-0.8.0/deciphon/daemon/pressd.py
+-rw-r--r--   0        0        0     2718 2023-03-06 10:42:22.221451 deciphon-0.8.0/deciphon/daemon/scand.py
+-rw-r--r--   0        0        0       72 2023-03-06 09:58:29.086811 deciphon-0.8.0/deciphon/dbfile.py
+-rw-r--r--   0        0        0       84 2023-03-01 11:03:34.003201 deciphon-0.8.0/deciphon/errors.py
+-rw-r--r--   0        0        0       91 2023-03-01 15:13:24.333208 deciphon-0.8.0/deciphon/filepath.py
+-rw-r--r--   0        0        0      483 2023-03-01 11:08:40.980239 deciphon-0.8.0/deciphon/filetype.py
+-rw-r--r--   0        0        0      157 2023-02-08 14:33:19.553381 deciphon-0.8.0/deciphon/fire_and_forget.py
+-rw-r--r--   0        0        0      635 2023-03-06 10:19:46.345162 deciphon-0.8.0/deciphon/h3daemon.py
+-rw-r--r--   0        0        0      196 2023-03-06 10:12:59.866043 deciphon-0.8.0/deciphon/hmmer_press.py
+-rw-r--r--   0        0        0       76 2023-03-06 09:53:17.004469 deciphon-0.8.0/deciphon/hmmfile.py
+-rw-r--r--   0        0        0      775 2023-02-13 10:15:16.068006 deciphon-0.8.0/deciphon/models.py
+-rw-r--r--   0        0        0      522 2023-02-08 14:44:07.024041 deciphon-0.8.0/deciphon/percent.py
+-rw-r--r--   0        0        0       69 2023-03-06 10:02:25.754663 deciphon-0.8.0/deciphon/press.py
+-rw-r--r--   0        0        0      321 2023-03-06 10:33:28.705124 deciphon-0.8.0/deciphon/scan.py
+-rw-r--r--   0        0        0     1929 2023-03-08 14:07:58.009142 deciphon-0.8.0/deciphon/seqfile.py
+-rw-r--r--   0        0        0      670 2023-03-04 10:38:17.846292 deciphon-0.8.0/deciphon/service_exit.py
+-rw-r--r--   0        0        0      157 2023-03-06 10:32:56.579299 deciphon-0.8.0/deciphon/snapfile.py
+-rw-r--r--   0        0        0      556 2023-02-14 10:18:24.072041 deciphon-0.8.0/deciphon/storage.py
+-rw-r--r--   0        0        0      713 2023-04-25 12:31:42.014650 deciphon-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 deciphon-0.8.0/PKG-INFO
```

### Comparing `deciphon-0.7.0/LICENSE` & `deciphon-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon-0.7.0/README.md` & `deciphon-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `deciphon-0.7.0/pyproject.toml` & `deciphon-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 [tool.poetry]
 name = "deciphon"
-version = "0.7.0"
+version = "0.8.0"
 description = "Individually annotate long, error-prone nucleotide sequences into proteins"
 authors = ["Danilo Horta <danilo.horta@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+blx = "*"
 cffi = "*"
-typer = {extras = ["all"], version = "^0.7.0"}
-h3daemon = "^0.7.6"
-deciphon-core = "^0.1.10"
+deciphon-core = "*"
+fasta-reader = "*"
+gmqtt = "*"
+h3daemon = "*"
+hmmer = "*"
+ijson = "*"
+pydantic = "*"
+python = "^3.10"
+requests = "*"
+typer = { extras = ["all"], version = "*" }
+uvloop = "*"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pyright = "^1.1.288"
-blx = "^0.1.8"
+pytest = "*"
+blx = "*"
+pre-commit = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 dcp = 'deciphon.cli:app'
-
-[tool.cibuildwheel]
-skip = ["*i686"]
+dcp-api = 'deciphon.api.cli:app'
```

### Comparing `deciphon-0.7.0/PKG-INFO` & `deciphon-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: deciphon
-Version: 0.7.0
+Version: 0.8.0
 Summary: Individually annotate long, error-prone nucleotide sequences into proteins
 License: MIT
 Author: Danilo Horta
 Author-email: danilo.horta@pm.me
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: blx
 Requires-Dist: cffi
-Requires-Dist: deciphon-core (>=0.1.10,<0.2.0)
-Requires-Dist: h3daemon (>=0.7.6,<0.8.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: deciphon-core
+Requires-Dist: fasta-reader
+Requires-Dist: gmqtt
+Requires-Dist: h3daemon
+Requires-Dist: hmmer
+Requires-Dist: ijson
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: typer[all]
+Requires-Dist: uvloop
 Description-Content-Type: text/markdown
 
 # Welcome to deciphon 👋
 
 > Individually annotate long, error-prone nucleotide sequences into proteins
 
 ### 🏠 [Homepage](https://github.com/EBI-Metagenomics/deciphon-py)
```

