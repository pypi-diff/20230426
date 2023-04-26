# Comparing `tmp/lammps-2022.6.23.3.0.tar.gz` & `tmp/lammps-2022.6.23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps-2022.6.23.3.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "lammps-2022.6.23.3.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `lammps-2022.6.23.3.0.tar` & `lammps-2022.6.23.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2823 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/.github/workflows/wheel.yml
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/CMakeLists.txt
--rw-r--r--   0        0        0    18059 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/LICENSE
--rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/README.md
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/lammps/__init__.py
--rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/lammps/executable.py
--rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/pyproject.toml
--rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/tests/test_import.py
--rw-r--r--   0        0        0    22969 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.0/PKG-INFO
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2823 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/CMakeLists.txt
+-rw-r--r--   0        0        0    18059 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/LICENSE
+-rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/README.md
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/lammps/__init__.py
+-rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/lammps/executable.py
+-rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/tests/test_import.py
+-rw-r--r--   0        0        0    22969 2022-11-09 12:37:21.000000 lammps-2022.6.23.3.1/PKG-INFO
```

### Comparing `lammps-2022.6.23.3.0/.github/workflows/wheel.yml` & `lammps-2022.6.23.3.1/.github/workflows/wheel.yml`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
           python-version: '3.11'
       - name: Setup MPI
         uses: mpi4py/setup-mpi@v1
         if: matrix.os == 'windows-latest'
         with:
           mpi: msmpi
 
-      - run: python -m pip install cibuildwheel==2.11.3
+      - run: python -m pip install cibuildwheel==2.12.3
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
         env:
           CIBW_BUILD_VERBOSITY: 1
           CIBW_ARCHS: all
           CIBW_BUILD: cp${{ matrix.python }}-${{ matrix.platform_id }}
       - uses: actions/upload-artifact@v3
```

### Comparing `lammps-2022.6.23.3.0/CMakeLists.txt` & `lammps-2022.6.23.3.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.3.0/LICENSE` & `lammps-2022.6.23.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.3.0/README.md` & `lammps-2022.6.23.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.3.0/lammps/__init__.py` & `lammps-2022.6.23.3.1/lammps/__init__.py`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.3.0/lammps/executable.py` & `lammps-2022.6.23.3.1/lammps/executable.py`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.3.0/pyproject.toml` & `lammps-2022.6.23.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core>=0.1.4"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "lammps"
-version = "2022.6.23.3.0"
+version = "2022.6.23.3.1"
 description = "unoffical LAMMPS Molecular Dynamics Python package"
 authors = [
   {name = "The LAMMPS Developers", email = "developers@lammps.org"},
   {name = "Jinzhe Zeng", email = "jinzhe.zeng@rutgers.edu"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `lammps-2022.6.23.3.0/PKG-INFO` & `lammps-2022.6.23.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps
-Version: 2022.6.23.3.0
+Version: 2022.6.23.3.1
 Summary: unoffical LAMMPS Molecular Dynamics Python package
 Keywords: lammps
 Author-Email: The LAMMPS Developers <developers@lammps.org>, Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```

