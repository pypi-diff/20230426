# Comparing `tmp/tfs-pandas-3.6.0.tar.gz` & `tmp/tfs-pandas-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/tfs/tfs/dist/.tmp-slo_bz1h/tfs-pandas-3.6.0.tar", last modified: Thu Apr 20 12:48:49 2023, max compression
+gzip compressed data, was "/home/runner/work/tfs/tfs/dist/.tmp-phjd970e/tfs-pandas-3.7.0.tar", last modified: Wed Apr 26 07:28:09 2023, max compression
```

## Comparing `tfs-pandas-3.6.0.tar` & `tfs-pandas-3.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-20 12:48:31.000000 tfs-pandas-3.6.0/tfs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 12:48:49.000000 tfs-pandas-3.6.0/tfs_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-26 07:27:53.000000 tfs-pandas-3.7.0/tfs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 07:28:09.000000 tfs-pandas-3.7.0/tfs_pandas.egg-info/top_level.txt
```

### Comparing `tfs-pandas-3.6.0/LICENSE` & `tfs-pandas-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/PKG-INFO` & `tfs-pandas-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfs-pandas
-Version: 3.6.0
+Version: 3.7.0
 Summary: Read and write tfs files.
 Home-page: https://github.com/pylhc/tfs
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tfs-pandas-3.6.0/README.md` & `tfs-pandas-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/setup.py` & `tfs-pandas-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tests/test_compression.py` & `tfs-pandas-3.7.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tests/test_frame.py` & `tfs-pandas-3.7.0/tests/test_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,25 @@
     def test_merge_headers_raises_on_invalid_how_key(self, caplog, how):
         headers_left = OrderedDict()
         headers_right = OrderedDict()
 
         with pytest.raises(ValueError):
             merge_headers(headers_left, headers_right, how=how)
 
+    def test_access_errors(self):
+        df = TfsDataFrame(index=["A", "B", "A"], columns=["A", "B", "A"], headers={"HEADER": 10})
+        with pytest.raises(AttributeError):
+            df.does_not_exist
+
+        with pytest.raises(KeyError):
+            df["does also not exist"]
+
+        with pytest.raises(KeyError):  # raises KeyError in pandas, TypeError in dict
+            df[[1, 2, 3]]
+
 
 class TestTfsDataFrameMerging:
     @pytest.mark.parametrize("how_headers", [None, "left", "right"])
     @pytest.mark.parametrize("how", ["left", "right", "outer", "inner"])
     @pytest.mark.parametrize("on", ["NAME", "S", "NUMBER", "CO", "CORMS", "BPM_RES"])
     def test_correct_merging(self, _tfs_file_x_pathlib, _tfs_file_y_pathlib, how_headers, how, on):
         dframe_x = tfs.read(_tfs_file_x_pathlib)
```

### Comparing `tfs-pandas-3.6.0/tests/test_hdf.py` & `tfs-pandas-3.7.0/tests/test_hdf.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tests/test_reader.py` & `tfs-pandas-3.7.0/tests/test_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,22 +52,14 @@
         assert "BPM RES" in df.columns
 
     def test_tfs_read_no_validation_doesnt_warn(self, caplog):
         nan_tfs_path = pathlib.Path(__file__).parent / "inputs" / "has_nans.tfs"
         _ = read_tfs(nan_tfs_path, index="NAME", validate=False)
         assert "contains non-physical values at Index:" not in caplog.text
 
-    def tfs_indx_pathlib_input(self, _tfs_file_pathlib: pathlib.Path):
-        test_file = read_tfs(_tfs_file_pathlib)
-        assert test_file.indx["BPMYB.5L2.B1"] == test_file.set_index("NAME")["BPMYB.5L2.B1"]
-
-    def tfs_indx_str_input(self, _tfs_file_str: str):
-        test_file = read_tfs(_tfs_file_str)
-        assert test_file.indx["BPMYB.5L2.B1"] == test_file.set_index("NAME")["BPMYB.5L2.B1"]
-
     def test_id_to_type_handles_madx_string_identifier(self):
         madx_str_id = "%20s"
         assert tfs.reader._id_to_type(madx_str_id) is str
 
     def test_tfs_read_write_read_pathlib_input(self, _tfs_file_pathlib: pathlib.Path, tmp_path):
         original = read_tfs(_tfs_file_pathlib)
         write_location = tmp_path / "test_file.tfs"
```

### Comparing `tfs-pandas-3.6.0/tests/test_tools.py` & `tfs-pandas-3.7.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tests/test_writer.py` & `tfs-pandas-3.7.0/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs/__init__.py` & `tfs-pandas-3.7.0/tfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tfs.hdf import read_hdf, write_hdf
 from tfs.reader import read_tfs
 from tfs.writer import write_tfs
 
 __title__ = "tfs-pandas"
 __description__ = "Read and write tfs files."
 __url__ = "https://github.com/pylhc/tfs"
-__version__ = "3.6.0"
+__version__ = "3.7.0"
 __author__ = "pylhc"
 __author_email__ = "pylhc@github.com"
 __license__ = "MIT"
 
 # aliases
 read = read_tfs
 write = write_tfs
```

### Comparing `tfs-pandas-3.6.0/tfs/collection.py` & `tfs-pandas-3.7.0/tfs/collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Collection
 ----------
 
 Advanced **TFS** files reading and writing functionality.
 """
+from typing import Tuple, List, Dict
+
 import pathlib
 
 from pandas import DataFrame
 
 from tfs.frame import TfsDataFrame
 from tfs.reader import read_tfs
 from tfs.writer import write_tfs
@@ -18,31 +20,35 @@
     Metaclass for TfsCollection. It takes the class attributes declared as
     `Tfs(...)` and replaces it for a property getter and setter. Check
     TfsCollection docs.
     """
 
     def __new__(mcs, cls_name, bases, dct: dict):
         new_dict = dict(dct)
+        new_dict["_stored_definitions"] = {}
         new_dict["_two_plane_names"] = []
         # for name in dct:
         for key, value in dct.items():
             try:
-                args = value.args
-                kwargs = value.kwargs
+                new_props = value.get_property()
             except AttributeError:
                 continue
-            new_props = _define_property(args, kwargs)
+
             try:
                 prop_x, prop_y = new_props
-                new_dict.pop(key)
-                new_dict["_two_plane_names"].append(key)
-                new_dict[key + "_x"] = prop_x
-                new_dict[key + "_y"] = prop_y
             except TypeError:
                 new_dict[key] = new_props
+                new_dict["_stored_definitions"][key] = value
+            else:
+                new_dict.pop(key)
+                new_dict["_two_plane_names"].append(key)
+                for plane, prop in zip("xy", (prop_x, prop_y)):
+                    new_key = f"{key}_{plane}"
+                    new_dict[new_key] = prop
+                    new_dict["_stored_definitions"][new_key] = value.get_planed_copy(plane)
         return super().__new__(mcs, cls_name, bases, new_dict)
 
 
 class TfsCollection(metaclass=_MetaTfsCollection):
     """
     Abstract class to lazily load and write **TFS** files.
 
@@ -96,170 +102,226 @@
     file is not in the provided directory (only the first time, but is better to always take it
     into account!).
 
     When a ``TfsDataFrame`` is assigned to one attribute, it will be set as the buffer value. If the
     ``self.allow_write`` attribute is set to ``True``, an assignment on one of the attributes will
     trigger the corresponding file write.
     """
+    INDEX = "NAME"
 
     def __init__(self, directory: pathlib.Path, allow_write: bool = None):
         self.directory = pathlib.Path(directory) if isinstance(directory, str) else directory
         self.allow_write = False if allow_write is None else allow_write
         self.maybe_call = _MaybeCall(self)
+        self.filenames = TfsCollection._FilenameGetter(self)
+        self.defined_properties = tuple(self._stored_definitions.keys())
         self._buffer = {}
 
-    def get_filename(self, *args, **kwargs):
+    def get_filename(self, name: str) -> str:
+        """ Return the actual filename of the property `name`.
+
+        Arguments:
+            name (str): Property name of the file.
+
+        Returns:
+            A `str` of the actual name of the file in `directory`.
+            The path to the file is then `self.directory / filename`.
+        """
+        definition: Tfs = self._stored_definitions.get(name)
+        if not definition:
+            raise AttributeError(f"TfsCollection does not have any property named {name}.")
+        return self._get_filename(*definition.args, **definition.kwargs)
+
+    def get_path(self, name: str) -> pathlib.Path:
+        """ Return the actual file path of the property `name` (convenience function).
+
+        Arguments:
+            name (str): Property name of the file.
+
+        Returns:
+            A `pathlib.Path` of the actual name of the file in `directory`.
+            The path to the file is then `self.directory / filename`.
+        """
+        return self.directory / self.get_filename(name)
+
+    def _get_filename(self, *args, **kwargs):
         """
         Return the filename to be loaded or written.
 
         This function will get as parameters any parameter given to the Tfs(...) attributes. It must
         return the filename to be written according to those parameters. If ``two_planes=False`` is
         not present in the Tfs(...) definition, it will also be given the keyword argument
         ``plane="x"`` or ``plane="y"``.
         """
         raise NotImplementedError("This is an abstract method, it should be implemented in subclasses.")
 
-    def write_to(self, *args, **kwargs):
+    def _write_to(self, *args, **kwargs):
         """
         Returns the filename and `TfsDataFrame` to be written on assignments.
 
         If this function is overwritten, it will replace ``get_filename(...)`` in file writes to
-        find out the filename of the file to be written. It also gets the value assigned as first
-        parameter. It must return a tuple (filename, tfs_data_frame).
+        find out the filename of the file to be written.
+        Which means you can define different locations for reading and writing.
+        It also gets the value assigned as first parameter. It must return a tuple (filename, tfs_data_frame).
         """
         raise NotImplementedError("This is an abstract method, it should be implemented in subclasses.")
 
     def clear(self):
         """
         Clear the file buffer.
 
         Any subsequent attribute access will try to load the corresponding file again.
         """
         self._buffer = {}
 
+    def flush(self):
+        """
+        Write the current state of the TFSDataFrames into their respective files.
+        """
+        if not self.allow_write:
+            raise IOError("Cannot flush TfsCollection, as `allow_write` is set to `False`.")
+
+        for filename, data_frame in self._buffer.items():
+            write_tfs(self.directory / filename, data_frame)
+
     def read_tfs(self, filename: str) -> TfsDataFrame:
         """
         Reads the **TFS** file from ``self.directory`` with the given filename.
 
-        This function can be overwritten to use something instead of ``tfs-pandas`` to load the
-        files.
+        This function can be overwritten to use something instead of ``tfs-pandas``
+        to load the files. It does not set the TfsDataframe into the buffer
+        (that is the job of `_load_tfs`)!
 
         Arguments:
             filename (str): The name of the file to load.
 
         Returns:
             A ``TfsDataFrame`` built from reading the requested file.
         """
         tfs_data_df = read_tfs(self.directory / filename)
-        if "NAME" in tfs_data_df:
-            tfs_data_df = tfs_data_df.set_index("NAME", drop=False)
+        if self.INDEX and self.INDEX in tfs_data_df:
+            tfs_data_df = tfs_data_df.set_index(self.INDEX, drop=False)
         return tfs_data_df
 
+    def write_tfs(self, filename: str, data_frame: DataFrame):
+        """
+        Write the **TFS** file to ``self.directory`` with the given filename.
+
+        This function can be overwritten to use something instead of ``tfs-pandas``
+        to write out the files. It does not  check for `allow_write` and
+        does not set the Dataframe into the buffer (that is the job of `_write_tfs`)!
+
+        Arguments:
+            filename (str): The name of the file to load.
+            data_frame (TfsDataFrame): TfsDataframe to write
+
+        """
+        write_tfs(self.directory / filename, data_frame)
+
     def __getattr__(self, attr: str) -> object:
         if attr in self._two_plane_names:
             return TfsCollection._TwoPlanes(self, attr)
         raise AttributeError(f"{self.__class__.__name__} object has no attribute {attr}")
 
+    def __getitem__(self, item):
+        return getattr(self, item)
+
+    def __setitem__(self, key, value):
+        return setattr(self, key, value)
+
     def _load_tfs(self, filename: str):
         try:
             return self._buffer[filename]
         except KeyError:
             tfs_data = self.read_tfs(filename)
-            if "NAME" in tfs_data:
-                tfs_data = tfs_data.set_index("NAME", drop=False)
+            if self.INDEX and self.INDEX in tfs_data:
+                tfs_data = tfs_data.set_index(self.INDEX, drop=False)
             self._buffer[filename] = tfs_data
             return self._buffer[filename]
 
     def _write_tfs(self, filename: str, data_frame: DataFrame):
         if self.allow_write:
-            write_tfs(self.directory / filename, data_frame)
+            self.write_tfs(filename, data_frame)
         self._buffer[filename] = data_frame
 
     class _TwoPlanes(object):
         def __init__(self, parent, attr):
             self.parent = parent
             self.attr = attr
 
         def __getitem__(self, plane: str):
-            return getattr(self.parent, self.attr + "_" + plane.lower())
+            return getattr(self.parent, f"{self.attr}_{plane.lower()}")
 
         def __setitem__(self, plane: str, value):
-            setattr(self.parent, self.attr + "_" + plane.lower(), value)
+            setattr(self.parent, f"{self.attr}_{plane.lower()}", value)
+
+    class _FilenameGetter:
+        def __init__(self, parent: 'TfsCollection'):
+            self.parent = parent
+
+        def __getitem__(self, item) -> str:
+            return self.parent.get_filename(item)
+
+        def __getattr__(self, attr) -> str:
+            return self[attr]
+
+        def __call__(self, exist: bool = False) -> Dict[str, str]:
+            all_filenames = {name: self.parent.get_filename(name)
+                             for name in self.parent.defined_properties}
+            if not exist:
+                return all_filenames
+            return {name: filename for name, filename in all_filenames.items()
+                    if (self.parent.directory / filename).is_file()}
 
 
 class Tfs:
     """Class to mark attributes as **TFS** attributes.
 
-    Any parameter given to this class will be passed to the ``get_filename()`` and ``write_to()``
-    methods, together with the plane if ``two_planes=False`` is not present.
+    Any parameter given to this class will be passed to the ``_get_filename()`` method,
+    together with the plane if ``two_planes=False`` is not present.
     """
+    PLANES = "x", "y"
 
     def __init__(self, *args, **kwargs):
+        self._two_planes = kwargs.pop("two_planes", True)
         self.args = args
         self.kwargs = kwargs
 
+    def get_planed_copy(self, plane: str):
+        return self.__class__(*self.args, plane=plane, **self.kwargs)
 
-# Private methods to define the properties ##################################
-
-
-def _define_property(args, kwargs):
-    if "two_planes" not in kwargs:
-        return _define_property_two_planes(args, kwargs)
-    elif kwargs["two_planes"]:
-        kwargs.pop("two_planes")
-        return _define_property_two_planes(args, kwargs)
-    else:
-        kwargs.pop("two_planes")
+    def get_property(self):
+        if self._two_planes:
+            return self._get_property_two_planes()
+        else:
+            return self._get_property_single_plane()
+
+    def _get_property_two_planes(self) -> Tuple[property, property]:
+        properties = [None, None]
+        for idx, plane in enumerate(self.PLANES):
+            planed = self.get_planed_copy(plane)
+            properties[idx] = planed._get_property_single_plane()
+        return tuple(properties)
+
+    def _get_property_single_plane(self) -> property:
+        def getter_funct(other: TfsCollection):
+            filename = other._get_filename(*self.args, **self.kwargs)
+            return other._load_tfs(filename)
 
-        def getter_funct(self):
-            return _getter(self, *args, **kwargs)
-
-        def setter_funct(self, tfs_data):
-            return _setter(self, tfs_data, *args, **kwargs)
+        def setter_funct(other: TfsCollection, value):
+            try:
+                filename, data_frame = other._write_to(value, *self.args, **self.kwargs)
+                other._write_tfs(filename, data_frame)
+            except NotImplementedError:
+                filename = other._get_filename(*self.args, **self.kwargs)
+                other._write_tfs(filename, value)
 
         return property(fget=getter_funct, fset=setter_funct)
 
 
-def _define_property_two_planes(args, kwargs) -> tuple:
-    x_kwargs = dict(kwargs)
-    y_kwargs = dict(kwargs)
-    x_kwargs["plane"] = "x"
-    y_kwargs["plane"] = "y"
-
-    def x_getter_funct(self):
-        return _getter(self, *args, **x_kwargs)
-
-    def x_setter_funct(self, tfs_data):
-        return _setter(self, tfs_data, *args, **x_kwargs)
-
-    def y_getter_funct(self):
-        return _getter(self, *args, **y_kwargs)
-
-    def y_setter_funct(self, tfs_data):
-        return _setter(self, tfs_data, *args, **y_kwargs)
-
-    property_x = property(fget=x_getter_funct, fset=x_setter_funct)
-    property_y = property(fget=y_getter_funct, fset=y_setter_funct)
-    return property_x, property_y
-
-
-def _getter(self, *args, **kwargs):
-    filename = self.get_filename(*args, **kwargs)
-    return self._load_tfs(filename)
-
-
-def _setter(self, value, *args, **kwargs):
-    try:
-        filename, data_frame = self.write_to(value, *args, **kwargs)
-        self._write_tfs(filename, data_frame)
-    except NotImplementedError:
-        filename = self.get_filename(*args, **kwargs)
-        self._write_tfs(filename, value)
-
-
 class _MaybeCall:
     """
     Handles the maybe_call feature of the TfsCollection.
 
     This class defines the `maybe_call` attribute in the instances of `TfsCollection`. To avoid
     repetitive try / except blocks, this class allows you to do:
     ``meas.maybe_call.beta["x"](some_funct, args, kwargs)``.
@@ -275,15 +337,15 @@
 
     class MaybeCallAttr:
         def __init__(self, parent, attr):
             self.parent = parent
             self.attr = attr
 
         def __getitem__(self, item):
-            return _MaybeCall.MaybeCallAttr(self.parent, self.attr + "_" + item)
+            return _MaybeCall.MaybeCallAttr(self.parent, f"{self.attr}_{item}")
 
         def __call__(self, function_call, *args, **kwargs):
             try:
                 tfs_file = getattr(self.parent, self.attr)
             except IOError:
-                return lambda funct: None  # Empty function
+                return None
             return function_call(tfs_file, *args, **kwargs)
```

### Comparing `tfs-pandas-3.6.0/tfs/constants.py` & `tfs-pandas-3.7.0/tfs/constants.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs/frame.py` & `tfs-pandas-3.7.0/tfs/frame.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs/hdf.py` & `tfs-pandas-3.7.0/tfs/hdf.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs/reader.py` & `tfs-pandas-3.7.0/tfs/reader.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs/tools.py` & `tfs-pandas-3.7.0/tfs/tools.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs/writer.py` & `tfs-pandas-3.7.0/tfs/writer.py`

 * *Files identical despite different names*

### Comparing `tfs-pandas-3.6.0/tfs_pandas.egg-info/PKG-INFO` & `tfs-pandas-3.7.0/tfs_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfs-pandas
-Version: 3.6.0
+Version: 3.7.0
 Summary: Read and write tfs files.
 Home-page: https://github.com/pylhc/tfs
 Author: pylhc
 Author-email: pylhc@github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

