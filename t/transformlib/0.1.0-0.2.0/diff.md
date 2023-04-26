# Comparing `tmp/transformlib-0.1.0.tar.gz` & `tmp/transformlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformlib-0.1.0.tar", last modified: Mon Apr 24 21:00:46 2023, max compression
+gzip compressed data, was "transformlib-0.2.0.tar", last modified: Tue Apr 25 15:33:09 2023, max compression
```

## Comparing `transformlib-0.1.0.tar` & `transformlib-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.508098 transformlib-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 21:00:46.508098 transformlib-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 21:00:33.000000 transformlib-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:00:46.508098 transformlib-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 21:00:33.000000 transformlib-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.504098 transformlib-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.504098 transformlib-0.1.0/src/transformlib/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.508098 transformlib-0.1.0/src/transformlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.508098 transformlib-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:00:33.000000 transformlib-0.1.0/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-24 21:00:33.000000 transformlib-0.1.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 21:00:33.000000 transformlib-0.1.0/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 15:33:09.363041 transformlib-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 15:32:54.000000 transformlib-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:33:09.363041 transformlib-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-25 15:32:54.000000 transformlib-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.359041 transformlib-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/src/transformlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-25 15:32:54.000000 transformlib-0.2.0/src/transformlib/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/src/transformlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 15:33:09.000000 transformlib-0.2.0/src/transformlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:33:09.363041 transformlib-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 15:32:54.000000 transformlib-0.2.0/tests/test_transform.py
```

### Comparing `transformlib-0.1.0/PKG-INFO` & `transformlib-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: transformlib
-Version: 0.1.0
+Version: 0.2.0
 Summary: Enables the user to organize transformations of data as a regular Python package.
 Home-page: https://github.com/laegsgaardTroels/transformlib
 Author: Troels Lægsgaard
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # transformlib
 [![CI Checks](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-package.yml/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-package.yml)
 [![pages-build-deployment](https://github.com/laegsgaardTroels/transformlib/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/pages/pages-build-deployment)
+[![Upload Python Package](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-publish.yml)
 
 Enables the user to organize transformations of data as a regular Python package.
```

### Comparing `transformlib-0.1.0/README.md` & `transformlib-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,5 +1,6 @@
 # transformlib
 [![CI Checks](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-package.yml/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-package.yml)
 [![pages-build-deployment](https://github.com/laegsgaardTroels/transformlib/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/pages/pages-build-deployment)
+[![Upload Python Package](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-publish.yml)
 
 Enables the user to organize transformations of data as a regular Python package.
```

### Comparing `transformlib-0.1.0/setup.py` & `transformlib-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name='transformlib',
     author='Troels Lægsgaard',
-    version='0.1.0',
+    version='0.2.0',
     description=(
         "Enables the user to organize transformations of data as a regular Python package."
     ),
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/laegsgaardTroels/transformlib",
     package_dir={"": "src"},
```

### Comparing `transformlib-0.1.0/src/transformlib/__init__.py` & `transformlib-0.2.0/src/transformlib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,18 @@
     Node,
     Output, Input,
     PySparkDataFrameOutput, PySparkDataFrameInput,
     PandasDataFrameOutput, PandasDataFrameInput,
 )
 from .transform import Transform, transform
 from .pipeline import Pipeline
+from . import config
 
 __all__ = [
     'Node',
     'Output', 'Input',
     'Transform', 'transform',
     'PySparkDataFrameOutput', 'PySparkDataFrameInput',
     'PandasDataFrameOutput', 'PandasDataFrameInput',
-    'Pipeline'
+    'Pipeline',
+    'config'
 ]
```

### Comparing `transformlib-0.1.0/src/transformlib/__main__.py` & `transformlib-0.2.0/src/transformlib/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from pathlib import Path
 import argparse
 import logging
 import sys
+from pathlib import Path
 
 from transformlib import Pipeline
 
 
 def main() -> None:
     """A Command Line Inferface (CLI) for running transforms."""
     parser = argparse.ArgumentParser(
@@ -24,13 +24,14 @@
         help="Should the Transform be run with logging set to INFO.",
     )
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.INFO)
     pipeline = Pipeline(transforms=[])
     for path in args.path:
+        print(path)
         pipeline.add_transforms_from_path(path)
     pipeline.run()
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `transformlib-0.1.0/src/transformlib/node.py` & `transformlib-0.2.0/src/transformlib/node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,39 @@
+import os
+from pathlib import Path
+from typing import Optional
+from typing import Union
+
 from transformlib import config
 
-from typing import Union
-from pathlib import Path
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class Node:
     """The `Node` base class is a node in a directed asyclic graph (DAG) of data transformations."""
 
     def __init__(
         self,
-        path: Union[str, Path],
-        root_dir: Union[str, Path] = config.ROOT_DIR,
+        relative_path: Union[str, Path],
+        data_dir: Optional[Union[str, Path]] = None,
     ):
-        self.path = path
-        self.root_dir = root_dir
+        self.relative_path = relative_path
+        if data_dir is None:
+            self.data_dir = os.getenv(config.DATA_DIR, config.DEFAULT_DATA_DIR)
+        else:
+            self.data_dir = data_dir
 
     @property
-    def _path(self):
-        return Path(self.root_dir) / self.path
+    def path(self):
+        return Path(self.data_dir) / self.relative_path
 
     def __repr__(self):
-        return f'{self.__class__.__name__}(path={self.path})'
+        return f'{self.__class__.__name__}({self.relative_path})'
 
     def __str__(self):
         return self.path
 
     def __eq__(self, other):
         return self.path == other.path
 
@@ -36,70 +42,70 @@
 
 
 class Output(Node):
     """An `Output` is a sink in a DAG of data transformations."""
 
     def __init__(
         self,
-        path: str,
-        root_dir: str = config.ROOT_DIR,
-        **write_kwargs
+        relative_path: str,
+        data_dir: Optional[Union[str, Path]] = None,
+        **save_kwargs
     ):
-        super().__init__(path, root_dir)
-        self.write_kwargs = write_kwargs
+        super().__init__(relative_path=relative_path, data_dir=data_dir)
+        self.save_kwargs = save_kwargs
 
     def save(self, obj, **save_kwargs):
-        """Saves an object containing data to the `config.ROOT_DIR`."""
+        """Saves an object containing data to the `config.DATA_DIR`."""
         raise NotImplementedError(
             f"The save method is not implemented for {self.__class__.__name__}"
         )
 
 
 class Input(Node):
     """An `Input` is a source in a DAG of data transformations."""
 
     def __init__(
         self,
-        path: str,
-        root_dir: str = config.ROOT_DIR,
+        relative_path: str,
+        data_dir: Optional[Union[str, Path]] = None,
         **load_kwargs
     ):
-        super().__init__(path, root_dir)
+        super().__init__(relative_path=relative_path, data_dir=data_dir)
         self.load_kwargs = load_kwargs
 
     def load(self, obj, **load_kwargs) -> None:
-        """Loads an object containing data from the `config.ROOT_DIR`."""
+        """Loads an object containing data from the `config.DATA_DIR`."""
         raise NotImplementedError(
             f"The load method is not implemented for {self.__class__.__name__}"
         )
 
 
 class PySparkDataFrameOutput(Output):
     """Used for PySpark DataFrame Output of a Transform."""
 
-    def save(self, df: 'pyspark.sql.DataFrame', **write_kwargs) -> None:
+    def save(self, df: 'pyspark.sql.DataFrame', **save_kwargs) -> None:
         """Save and output PySpark DataFrame from a fixed path.
 
         The default save mode is set to 'overwrite' because this is most
         commonly used.
 
         >>> from transformlib import PySparkDataFrameOutput
         >>> PySparkDataFrameOutput('/path/to/output.csv', format='csv')
         PySparkDataFrameOutput(path=/path/to/output.csv)
 
         Args:
             df (pyspark.sql.DataFrame): A DataFrame which is to be saved in the output
                 location.
-            **write_kwargs: The key value arguments to the DataFrameReader class
+            **save_kwargs: The key value arguments to the DataFrameReader class
                 in pyspark.sql.
         """
-        write_kwargs = write_kwargs or self.write_kwargs
-        if 'mode' not in write_kwargs:
-            write_kwargs['mode'] = 'overwrite'
-        df.write.save(path=self.path, **write_kwargs)
+        save_kwargs = save_kwargs or self.save_kwargs
+        if 'mode' not in save_kwargs:
+            save_kwargs['mode'] = 'overwrite'
+        df.write.save(path=str(self.path), **save_kwargs)
 
 
 class PySparkDataFrameInput(Input):
     """Used for PySpark DataFrame Input to a Transform."""
 
     def load(self, **load_kwargs) -> 'pyspark.sql.DataFrame':
         """Load an input PySpark DataFrame from a fixed path.
@@ -115,37 +121,37 @@
 
         Returns:
             pyspark.sql.DataFrame: The DataFrame that the input is pointing to.
         """
         import pyspark
         spark = pyspark.sql.SparkSession.builder.getOrCreate()
         load_kwargs = load_kwargs or self.load_kwargs
-        return spark.read.load(path=self.path, **load_kwargs)
+        return spark.read.load(path=str(self.path), **load_kwargs)
 
 
 class PandasDataFrameOutput(Output):
     """Used for pandas DataFrame Output of a Transform."""
 
-    def save(self, df: 'pandas.DataFrame', format='csv', **write_kwargs) -> None:
+    def save(self, df: 'pandas.DataFrame', format='csv', **save_kwargs) -> None:
         """Save the output Pandas DataFrame from a fixed path.
 
         >>> from transformlib import PandasDataFrameOutput
         >>> PandasDataFrameOutput('/path/to/input.csv', format='csv')
         PandasDataFrameOutput(path=/path/to/input.csv)
 
         Args:
             df (pandas.DataFrame): A pandas DataFrame which is to be saved in the
                 output location.
-            **write_kwargs: The key value arguments to the DataFrameReader class
+            **save_kwargs: The key value arguments to the DataFrameReader class
                 in pyspark.sql.
         """
         if format == 'csv':
-            df.to_csv(self._path, **write_kwargs)
+            df.to_csv(self.path, **save_kwargs)
         elif format == 'parquet':
-            df.to_parquet(self._path, **write_kwargs)
+            df.to_parquet(self.path, **save_kwargs)
         else:
             raise NotImplementedError(f"The save method is not implemented for {format}")
 
 
 class PandasDataFrameInput(Input):
     """Used for pandas DataFrame Input to a Transform."""
 
@@ -157,12 +163,12 @@
         PandasDataFrameInput(path=/path/to/output.csv)
 
         Returns:
             pandas.DataFrame: The DataFrame that the input is pointing to.
         """
         import pandas as pd
         if format == 'csv':
-            return pd.read_csv(self._path, **load_kwargs)
+            return pd.read_csv(self.path, **load_kwargs)
         elif format == 'parquet':
-            return pd.read_parquet(self._path, **load_kwargs)
+            return pd.read_parquet(self.path, **load_kwargs)
         else:
             raise NotImplementedError(f"The save method is not implemented for {format}")
```

### Comparing `transformlib-0.1.0/src/transformlib/pipeline.py` & `transformlib-0.2.0/src/transformlib/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,19 +49,15 @@
     def tasks(self):
         """A topologically ordered list of transforms."""
         if len(set(self.transforms)) != len(self.transforms):
             raise TransformlibDuplicateTransformException(f"Duplicate {self.transforms}")
         return _get_tasks(self.transforms)  # Topologically sort the transforms.
 
     def __repr__(self):
-        return (
-            'Pipeline('
-            + ', '.join(map(repr, self.tasks))
-            + ')'
-        )
+        return f"Pipeline({', '.join(map(repr, self.tasks))})"
 
     def run(self) -> None:
         """Used to run all the transforms in the pipeline."""
         logger.info(f'Beginning running of {self}.')
         start = time.perf_counter()
         for transform in self.tasks:
             transform.run()
```

### Comparing `transformlib-0.1.0/src/transformlib/transform.py` & `transformlib-0.2.0/src/transformlib/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,20 @@
         return tuple(self.outputs + self.inputs)
 
     def __call__(self, *args, **kwargs):
         return self.func(*args, **kwargs)
 
     def __repr__(self):
         return (
-            f'{self.__class__}('
+            f'{self.__class__.__name__}('
             + ', '.join(map(
                 lambda key: key + '=' + repr(self.output_kwargs[key]),
                 self.output_kwargs
             ))
+            + (', ' if self.input_kwargs else '')
             + ', '.join(map(
                 lambda key: key + '=' + repr(self.input_kwargs[key]),
                 self.input_kwargs
             ))
             + ')'
         )
```

### Comparing `transformlib-0.1.0/src/transformlib.egg-info/PKG-INFO` & `transformlib-0.2.0/src/transformlib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: transformlib
-Version: 0.1.0
+Version: 0.2.0
 Summary: Enables the user to organize transformations of data as a regular Python package.
 Home-page: https://github.com/laegsgaardTroels/transformlib
 Author: Troels Lægsgaard
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # transformlib
 [![CI Checks](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-package.yml/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-package.yml)
 [![pages-build-deployment](https://github.com/laegsgaardTroels/transformlib/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/pages/pages-build-deployment)
+[![Upload Python Package](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/laegsgaardTroels/transformlib/actions/workflows/python-publish.yml)
 
 Enables the user to organize transformations of data as a regular Python package.
```

### Comparing `transformlib-0.1.0/src/transformlib.egg-info/SOURCES.txt` & `transformlib-0.2.0/src/transformlib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 src/transformlib/transform.py
 src/transformlib.egg-info/PKG-INFO
 src/transformlib.egg-info/SOURCES.txt
 src/transformlib.egg-info/dependency_links.txt
 src/transformlib.egg-info/entry_points.txt
 src/transformlib.egg-info/requires.txt
 src/transformlib.egg-info/top_level.txt
+tests/test_main.py
 tests/test_node.py
 tests/test_pipeline.py
 tests/test_transform.py
```

### Comparing `transformlib-0.1.0/tests/test_pipeline.py` & `transformlib-0.2.0/tests/test_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 
 from tests.utils import ReusedPySparkTestCase
-from transformlib import Transform
-from transformlib import Pipeline
+from transformlib import (
+    Transform,
+    Pipeline
+)
 from transformlib.exceptions import (
     TransformlibDuplicateTransformException,
     TransformlibCycleException
 )
 from transformlib.pipeline import _tsort
```

### Comparing `transformlib-0.1.0/tests/test_transform.py` & `transformlib-0.2.0/tests/test_transform.py`

 * *Files identical despite different names*

