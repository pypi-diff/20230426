# Comparing `tmp/unscrewed-0.1a1.tar.gz` & `tmp/unscrewed-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unscrewed-0.1a1.tar", last modified: Sat Apr 22 21:33:35 2023, max compression
+gzip compressed data, was "unscrewed-0.1a2.tar", last modified: Tue Apr 25 13:42:49 2023, max compression
```

## Comparing `unscrewed-0.1a1.tar` & `unscrewed-0.1a2.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0       61 2023-04-22 17:51:30.002054 unscrewed-0.1a1/.coveragerc
--rw-r--r--   0        0        0     1080 2023-04-22 18:44:01.080252 unscrewed-0.1a1/.github/workflows/testing.yml
--rw-r--r--   0        0        0       65 2023-04-22 17:51:30.002306 unscrewed-0.1a1/.gitignore
--rw-r--r--   0        0        0     1607 2023-04-22 17:53:59.572215 unscrewed-0.1a1/LICENSE
--rw-r--r--   0        0        0      844 2023-04-22 21:27:17.007030 unscrewed-0.1a1/README.md
--rw-r--r--   0        0        0      519 2023-04-22 17:59:53.851899 unscrewed-0.1a1/pyproject.toml
--rw-r--r--   0        0        0      233 2023-04-22 17:58:13.522790 unscrewed-0.1a1/unscrewed/__init__.py
--rw-r--r--   0        0        0     2782 2023-04-22 19:00:06.696884 unscrewed-0.1a1/unscrewed/fetcher.py
--rw-r--r--   0        0        0        0 2023-04-22 17:54:11.423042 unscrewed-0.1a1/unscrewed/tests/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-22 18:01:43.786173 unscrewed-0.1a1/unscrewed/tests/nipraxis_registry.yaml
--rw-r--r--   0        0        0     1080 2023-04-22 19:04:36.240333 unscrewed-0.1a1/unscrewed/tests/test_local_cache.py
--rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 unscrewed-0.1a1/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-04-25 11:53:10.459190 unscrewed-0.1a2/.coveragerc
+-rw-r--r--   0        0        0     1023 2023-04-25 11:55:24.997879 unscrewed-0.1a2/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       75 2023-04-25 11:40:40.561778 unscrewed-0.1a2/.gitignore
+-rw-r--r--   0        0        0     1607 2023-04-22 17:53:59.572215 unscrewed-0.1a2/LICENSE
+-rw-r--r--   0        0        0      804 2023-04-25 13:27:55.967217 unscrewed-0.1a2/README.md
+-rw-r--r--   0        0        0      608 2023-04-22 22:06:45.853086 unscrewed-0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      233 2023-04-25 13:40:33.420259 unscrewed-0.1a2/src/unscrewed/__init__.py
+-rw-r--r--   0        0        0     2938 2023-04-25 11:38:47.181746 unscrewed-0.1a2/src/unscrewed/fetcher.py
+-rw-r--r--   0        0        0     1277 2023-04-22 22:13:47.363875 unscrewed-0.1a2/src/unscrewed/update_config.py
+-rw-r--r--   0        0        0        0 2023-04-22 17:54:11.423042 unscrewed-0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-25 13:30:59.686272 unscrewed-0.1a2/tests/test_local_cache.py
+-rw-r--r--   0        0        0     8042 2023-04-25 13:16:57.185863 unscrewed-0.1a2/tests/testreg/24719.f3_beh_CHYM.csv
+-rw-r--r--   0        0        0       90 2023-04-25 13:15:52.622216 unscrewed-0.1a2/tests/testreg/README.md
+-rw-r--r--   0        0        0      110 2023-04-25 13:17:16.241902 unscrewed-0.1a2/tests/testreg/ds114_sub009_t2r1_cond.txt
+-rw-r--r--   0        0        0     1613 2023-04-25 13:17:16.243076 unscrewed-0.1a2/tests/testreg/ds114_sub009_t2r1_conv.txt
+-rw-r--r--   0        0        0    76598 2023-04-25 13:18:15.926463 unscrewed-0.1a2/tests/testreg/dsfe_logo.png
+-rw-r--r--   0        0        0      144 2023-04-25 13:17:16.243732 unscrewed-0.1a2/tests/testreg/new_cond.txt
+-rw-r--r--   0        0        0      601 2023-04-25 13:35:44.796094 unscrewed-0.1a2/tests/testreg_registry.yaml
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 unscrewed-0.1a2/PKG-INFO
```

### Comparing `unscrewed-0.1a1/.github/workflows/testing.yml` & `unscrewed-0.1a2/.github/workflows/testing.yml`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,15 @@
         run: |
           pip install pytest-cov
       - name: Install package
         run: |
           pip install .
       - name: Run tests
         run: |
-          mkdir tmp
-          cd tmp
-          pytest --log-level DEBUG --cov-config=../.coveragerc --cov=$PKG_NAME --doctest-modules --pyargs $PKG_NAME
+          pytest --log-level DEBUG --cov-config=.coveragerc --cov=$PKG_NAME --doctest-modules tests
       - name: Collect code coverage data
         run: |
-          coverage xml --data-file=tmp/.coverage
+          coverage xml --data-file=.coverage
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
```

### Comparing `unscrewed-0.1a1/LICENSE` & `unscrewed-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `unscrewed-0.1a1/README.md` & `unscrewed-0.1a2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 ```bash
 pip install unscrewed
 ```
 
 ## Usage
 
 First prepare a `registry.yaml` file, like the one in
-`unscrewed/tests/nipraxis_registry.yaml`.  Put it in your package, say in the
-`your_package` directory (that contains the `__init__.py` file.  Maybe call it
-`registry.yaml`.
+`unscrewed/tests/testreg_registry.yaml`.  Put it in your package, say in the
+`your_package` directory (that contains the `__init__.py` file).  Maybe call
+it `registry.yaml`.
 
 In some module, say `your_package/data.py`
 
 ```python
 import pkg_resources
 
 import unscrewed
 
 _config_file = pkg_resources.resource_filename("your_package", "registry.yaml")
-_fetcher = unscrewed.Fetcher(_config_file)
-fetch_file = _fetcher.fetch_file
+fetcher = unscrewed.Fetcher(_config_file)
 ```
 
 Say you have a file `my_data_file.nii` configured in your `registry.yaml` file above.
 
 Now you can fetch it like this:
 
 ```python
-from your_package.data import fetch_file
+from your_package.data import fetcher
 
-fname = fetch_file('my_data_file.nii')
+fname = fetcher('my_data_file.nii')
 ```
```

### Comparing `unscrewed-0.1a1/pyproject.toml` & `unscrewed-0.1a2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 license = {file = "LICENSE"}
 dependencies = ["pooch", "pyyaml"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.urls]
-Home = "https://unscrewed.org"
+Home = "https://github.com/matthew-brett/unscrewed"
+
+[project.scripts]
+us-update-config = "unscrewed.update_config:cli"
```

### Comparing `unscrewed-0.1a1/unscrewed/fetcher.py` & `unscrewed-0.1a2/src/unscrewed/fetcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 """ Fetch data from repository, or maybe local cache
 """
 
-import os
-import io
+from os import environ
+from io import StringIO
 from pathlib import Path
 
 import yaml
 
 import pooch
 
 
 class Fetcher:
 
     def __init__(self, config):
-        self.config = self._get_config(config)
-        self.registry = self._get_registry()
+        self.config = self._read_config(config)
+        self.registry = self._build_registry(self.config)
+        self.data_version = self.config['data_version']
 
-    def _get_config(self, config):
+    def _read_config(self, config):
+        """ Read configuration from filename, Path, fileobj or mapping.
+        """
         if isinstance(config, str):
             config = Path(config)
         if isinstance(config, Path):
-            config = io.StringIO(config.read_text())
+            config = StringIO(config.read_text())
         if hasattr(config, 'read'):
             config = yaml.load(config, Loader=yaml.SafeLoader)
         return config
 
-    def _get_registry(self):
-        """ Build and return Pooch image registry object
+    def _build_registry(self, config):
+        """ Build and return Pooch registry object
         """
-        config = self.config
         return pooch.create(
             # Use the default cache folder for the operating system
             path=pooch.os_cache(config['pkg_name']),
             # The remote data is on Github
             base_url=config.get('base_url', ''),
             version=config.get('data_version'),
-            # If this is a development version, get the data from the "main" branch
+            # If this is a development version, get the data from the
+            # specified branch (default 'main')
             version_dev=config.get('version_dev', 'main'),
             registry=config.get('files'),
             urls=config.get('urls'),
-            # The name of an environment variable that can overwrite the cache path.
+            # The name of an environment variable that can overwrite the cache
+            # path.
             env=config.get('cache_env_var')
         )
 
     def _from_staging_cache(self, rel_url, staging_cache):
         known_hash = self.registry.registry.get(rel_url)
         if not known_hash:
             return None
-        data_version = self.config['data_version']
-        pth = Path(staging_cache).resolve() / data_version / rel_url
+        pth = Path(staging_cache).resolve() / self.data_version / rel_url
         action, verb = pooch.core.download_action(pth, known_hash)
         if action == 'update':
             pooch.utils.get_logger().info(
-                f"'{rel_url}' in '{staging_cache}/{data_version}' "
+                f"'{rel_url}' in '{staging_cache}/{self.data_version}' "
                 "but hash does not match; looking in local cache / registry.")
             return None
         if action == 'fetch':
             return str(pth)
 
-    def fetch_file(self, rel_url):
+    def __call__(self, rel_url):
         """ Fetch data file from local cache, or registry
 
         Parameters
         ----------
         rel_url : str
             Location of file to fetch, relative to repository base URLs.  Use
             forward slashes to separate paths, on Windows or Unix.
 
         Returns
         -------
         local_fname : str
             The absolute path (including the file name) of the file in the local
             storage.
         """
-        staging_cache = os.environ.get(self.config.get('staging_env_var'))
+        staging_cache = environ.get(self.config.get('staging_env_var'))
         if staging_cache:
             cache_fname = self._from_staging_cache(rel_url, staging_cache)
             if cache_fname:
                 return cache_fname
         return self.registry.fetch(rel_url)
```

### Comparing `unscrewed-0.1a1/unscrewed/tests/test_local_cache.py` & `unscrewed-0.1a2/tests/test_local_cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 import shutil
 from pathlib import Path
 from hashlib import sha1
 
 import unscrewed.fetcher as usf
 
 
-CAMERA_HASH = 'af7257977f30797d4b3ea7dd15fa362d4fe8c37e'
+LOGO_SHA = 'cd8157960cf256e53c4e9722c7c34b8d38eb24ec'
 
 
-def assert_hash(fname, hash):
+def assert_hash(fname, sha):
     with open(fname, 'rb') as fobj:
         contents = fobj.read()
-    assert sha1(contents).hexdigest() == hash
+    assert sha1(contents).hexdigest() == sha
 
 
 def test_camera(tmp_path, monkeypatch):
     local_cache = tmp_path / 'unscrewed-local'
     staging_cache = tmp_path / 'unscrewed-staging'
-    monkeypatch.delenv("NIPRAXIS_STAGING_CACHE", raising=False)
-    monkeypatch.setenv("NIPRAXIS_LOCAL_CACHE", str(local_cache))
-    config = Path(__file__).parent / 'nipraxis_registry.yaml'
+    monkeypatch.delenv("TESTREG_STAGING_CACHE", raising=False)
+    monkeypatch.setenv("TESTREG_LOCAL_CACHE", str(local_cache))
+    config = Path(__file__).parent / 'testreg_registry.yaml'
     fetcher = usf.Fetcher(config)
-    fname = fetcher.fetch_file('camera.txt')
+    fname = fetcher('dsfe_logo.png')
+    assert_hash(fname, LOGO_SHA)
     assert fname.startswith(str(local_cache))
-    monkeypatch.setenv("NIPRAXIS_STAGING_CACHE", str(staging_cache))
-    fname = fetcher.fetch_file('camera.txt')
+    monkeypatch.setenv("TESTREG_STAGING_CACHE", str(staging_cache))
+    fname = fetcher('dsfe_logo.png')
     assert fname.startswith(str(local_cache))
     shutil.move(local_cache, staging_cache)
-    fname = fetcher.fetch_file('camera.txt')
+    fname = fetcher('dsfe_logo.png')
     assert fname.startswith(str(staging_cache))
```

### Comparing `unscrewed-0.1a1/PKG-INFO` & `unscrewed-0.1a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: unscrewed
-Version: 0.1a1
+Version: 0.1a2
 Summary: Unscrewed data packaging
 Author-email: Matthew Brett <matthew.brett@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pooch
 Requires-Dist: pyyaml
 Requires-Dist: pytest ; extra == "test"
-Project-URL: Home, https://unscrewed.org
+Project-URL: Home, https://github.com/matthew-brett/unscrewed
 Provides-Extra: test
 
 # Unscrewed
 
 Utility for making and updating a data fetcher component of your project.
 
 ## Install
@@ -21,33 +21,32 @@
 ```bash
 pip install unscrewed
 ```
 
 ## Usage
 
 First prepare a `registry.yaml` file, like the one in
-`unscrewed/tests/nipraxis_registry.yaml`.  Put it in your package, say in the
-`your_package` directory (that contains the `__init__.py` file.  Maybe call it
-`registry.yaml`.
+`unscrewed/tests/testreg_registry.yaml`.  Put it in your package, say in the
+`your_package` directory (that contains the `__init__.py` file).  Maybe call
+it `registry.yaml`.
 
 In some module, say `your_package/data.py`
 
 ```python
 import pkg_resources
 
 import unscrewed
 
 _config_file = pkg_resources.resource_filename("your_package", "registry.yaml")
-_fetcher = unscrewed.Fetcher(_config_file)
-fetch_file = _fetcher.fetch_file
+fetcher = unscrewed.Fetcher(_config_file)
 ```
 
 Say you have a file `my_data_file.nii` configured in your `registry.yaml` file above.
 
 Now you can fetch it like this:
 
 ```python
-from your_package.data import fetch_file
+from your_package.data import fetcher
 
-fname = fetch_file('my_data_file.nii')
+fname = fetcher('my_data_file.nii')
 ```
```

