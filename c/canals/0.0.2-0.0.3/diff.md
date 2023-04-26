# Comparing `tmp/canals-0.0.2.tar.gz` & `tmp/canals-0.0.3.tar.gz`

## Comparing `canals-0.0.2.tar` & `canals-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 canals-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 canals-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.0.2/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 canals-0.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.0.2/canals/__about__.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 canals-0.0.2/canals/__init__.py
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 canals-0.0.2/canals/component.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 canals-0.0.2/canals/pipeline/__init__.py
--rw-r--r--   0        0        0    30093 2020-02-02 00:00:00.000000 canals-0.0.2/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 canals-0.0.2/canals/pipeline/save_load.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 canals-0.0.2/docs/index.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 canals-0.0.2/docs/api-docs/component.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 canals-0.0.2/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/components.md
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/concepts.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/parameters.md
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/pipelines.md
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 canals-0.0.2/docs/concepts/save-load.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.0.2/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.0.2/images/canals-logo-light.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.0.2/test/__init__.py
--rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 canals-0.0.2/test/test_save_load.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_accumulate.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_add_value.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_below.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_double.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_greet.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_merge.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_remainder.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_rename.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_repeat.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_subtract.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 canals-0.0.2/test/components/test_sum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/_test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_complex_pipeline.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_decision_pipeline.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_linear_pipeline.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_looping_pipeline.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_merging_pipeline.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 canals-0.0.2/test/pipelines/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.0.2/LICENSE
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 canals-0.0.2/README.md
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 canals-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 canals-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 canals-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 canals-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.0.3/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 canals-0.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.0.3/canals/__about__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 canals-0.0.3/canals/__init__.py
+-rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 canals-0.0.3/canals/component.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 canals-0.0.3/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0    30093 2020-02-02 00:00:00.000000 canals-0.0.3/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 canals-0.0.3/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 canals-0.0.3/docs/index.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 canals-0.0.3/docs/api-docs/component.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 canals-0.0.3/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/components.md
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/parameters.md
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/save-load.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.0.3/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.0.3/images/canals-logo-light.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 canals-0.0.3/test/test_save_load.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_accumulate.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_add_value.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_below.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_double.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_greet.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_merge.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_remainder.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_rename.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_repeat.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_subtract.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_sum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/_test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_decision_pipeline.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_merging_pipeline.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 canals-0.0.3/README.md
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 canals-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 canals-0.0.3/PKG-INFO
```

### Comparing `canals-0.0.2/.pre-commit-config.yaml` & `canals-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/mkdocs.yml` & `canals-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/.github/workflows/tests.yml` & `canals-0.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/canals/component.py` & `canals-0.0.3/docs/concepts/components.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,152 +1,133 @@
-import logging
+# Creating Components
 
+In order to be recognized as components and work in a Pipeline, Components must follow the contract below.
 
-logger = logging.getLogger(__name__)
+### Decorator
 
+All component classes must be decorated with the `@component` decorator. This allows Canals to discover them.
 
-class ComponentError(Exception):
-    pass
+### `__init__()`
 
+```python
+def __init__(self, [... components init parameters ...]):
+```
 
-def component(class_):
-    """
-    Marks a class as a component. Any class decorated with `@component`
-    can be picked up by a Pipeline, serialized, deserialized, etc.
+The constructor is a mandatory method for Canals components.
 
-    All components MUST follow the contract below.
-    This docstring is the source of truth for components contract.
+In their `__init__`, Components must define:
 
-    ```python
-    def __init__(self, [... components init parameters ...]):
-    ```
-    Mandatory method.
+- `self.inputs = [<expected_input_connection_name(s)>]`:
+    A list with all the connections they can possibly receive input from
 
-    Components should have an `__init__` method where they define:
+- `self.outputs = [<expected_output_connection_name(s)>]`:
+    A list with the connections they might possibly produce as output
 
-    - `self.inputs = [<expected_input_connection_name(s)>]`:
-        A list with all the connections they can possibly receive input from
+- `self.init_parameters = {<init parameters>}`:
+    Any state they wish to be persisted when they are saved.
+    These values will be given to the `__init__` method of a new instance
+    when the pipeline is loaded.
+    The `@component` decorator saves the arguments automatically.
+    Components can assume that the dictionary exists and can alter its content
+    in the `__init__` method if needed.
 
-    - `self.outputs = [<expected_output_connection_name(s)>]`:
-        A list with the connections they might possibly produce as output
+Note that components should take only "basic" Python types as parameters of their
+`__init__` function, or iterables and dictionaries containing only such values.
+Anything else (objects, functions, etc) will raise an exception at init time.
 
-    - `self.init_parameters = {<init parameters>}`:
-        Any state they wish to be persisted when they are marshalled.
-        These values will be given to the `__init__` method of a new instance
-        when the pipeline is unmarshalled.
+_(TODO explain how to use classes and functions in init. In the meantime see `test/components/test_accumulate.py`)_
 
-    If components want to let users customize their input and output connections (be it
-    the connection name, the connection count, etc...) they should provide properly
-    named init parameters:
+If components want to let users customize their input and output connections (be it
+the connection name, the connection count, etc...) they should provide properly
+named init parameters:
 
-    - `input: str` or `inputs: List[str]` (always with proper defaults)
-    - `output: str` or `outputs: List[str]` (always with proper defaults)
+- `input: str` or `inputs: List[str]` (always with proper defaults)
+- `output: str` or `outputs: List[str]` (always with proper defaults)
 
-    All the rest is going to be interpreted as a regular init parameter that
-    has nothing to do with the component connections.
+All the rest is going to be interpreted as a regular init parameter that
+has nothing to do with the component connections.
 
-    The `__init__` must be extrememly lightweight, because it's a frequent
-    operation during the construction and validation of the pipeline. If a component
-    has some heavy state to initialize (models, backends, etc...) refer to the
-    `warm_up()` method.
+The `__init__` must be extrememly lightweight, because it's a frequent
+operation during the construction and validation of the pipeline. If a component
+has some heavy state to initialize (models, backends, etc...) refer to the
+`warm_up()` method.
 
-    ```
-    def warm_up(self):
-    ```
-    Optional method.
+### `warm_up()`
 
-    This method is called by Pipeline before the graph execution.
-    Make sure to avoid double-initializations, because Pipeline will not keep
-    track of which components it called `warm_up()` on.
+```python
+def warm_up(self):
+```
 
-    ```
-    def run(
-        self,
-        name: str,
-        data: List[Tuple[str, Any]],
-        parameters: Dict[str, Dict[str, Any]],
-    ):
-    ```
-    Mandatory method.
+Optional method. If it's defined, this method is called by Pipeline before the graph execution.
+Make sure to avoid double-initializations, because Pipeline will not keep track of which components it called
+`warm_up()` on.
 
-    This is the method where the main functionality of the component should be carried out.
-    It's called by `Pipeline.run()`, which passes the following parameters to it:
+### `run()`
 
-    - `name: str`: the name of the component. Allows the component to find its own parameters in
-        the `parameters` dictionary (see below).
+```python
+def run(
+    self,
+    name: str,
+    data: List[Tuple[str, Any]],
+    parameters: Dict[str, Dict[str, Any]],
+):
+```
 
-    - `data: List[Tuple[str, Any]]`: the input data.
-        Pipeline guarantees that the following assert always passes:
+This is the method that is called by `Pipeline.run()`. When calling it, Pipeline passes the following parameters to it:
 
-        `assert self.inputs == [name for name, value in data]`
+- `name: str`: the name of the component. Allows the component to find its own parameters in
+    the `parameters` dictionary (see below).
 
-        which means that:
-        - `data` is of the same length as `self.inputs`.
-        - `data` contains one tuple for each string stored in `self.inputs`.
-        - no guarantee is given on the values of these tuples: notably, if there was a
-            decision component upstream, some values might be `None`.
+- `data: List[Tuple[str, Any]]`: the input data.
+    Pipeline guarantees that the following assert always passes:
 
-        For example, if a component declares `self.inputs = ["value", "value"]` (think of a
-        `Sum` component), `data` might look like:
+    `assert self.inputs == [name for name, value in data]`
 
-        `[("value", 1), ("value", 10)]`
+    which means that:
+    - `data` is of the same length as `self.inputs`.
+    - `data` contains one tuple for each string stored in `self.inputs`.
+    - no guarantee is given on the values of these tuples: notably, if there was a
+        decision component upstream, some values might be `None`.
 
-        `[("value", None), ("value", 10)]`
+    For example, if a component declares `self.inputs = ["value", "value"]` (think of a
+    `Sum` component), `data` might look like:
 
-        `[("value", None), ("value", None)]`
+    `[("value", 1), ("value", 10)]`
 
-        `[("value", 1), ("value", ["something", "unexpected"])]`
+    `[("value", None), ("value", 10)]`
 
-        but it will never look like:
+    `[("value", None), ("value", None)]`
 
-        `[("value", 1), ("value", 10), ("value", 100)]`
+    `[("value", 1), ("value", ["something", "unexpected"])]`
 
-        `[("value": 15)]`
+    but it will never look like:
 
-        `[("value": 15), ("unexpected", 10)]`
+    `[("value", 1), ("value", 10), ("value", 100)]`
 
-    - `parameters: Dict[str, Dict[str, Any]]`: a dictionary of dictionaries with all
-        the parameters for all components.
-        Note that all components have access to all parameters for all other components: this
-        might come handy to components like `Agent`s, that want to influence the behavior
-        of components downstream.
-        Components can access their own parameters using `name`, but they must **not** assume
-        their name is present in the dictionary.
-        Therefore, the best way to get the parameters is with
-        `my_parameters = parameters.get(name, {})`
+    `[("value": 15)]`
 
-    Pipeline expect the output of this function to be a tuple of two dictionaries.
-    The first item is a dictionary that represents the output and it should always
-    abide to the following format:
+    `[("value": 15), ("unexpected", 10)]`
 
-    `{output_name: output_value for output_name in <subset of self.expected_output>}`
+- `parameters: Dict[str, Dict[str, Any]]`: a dictionary of dictionaries with all
+    the parameters for all components in the Pipeline.
+    Note that all components have access to all parameters for all other components: this
+    might come handy to components that want to influence the behavior
+    of other components downstream.
+    Components can access their own parameters using `name`, but they must **not** assume
+    their name is present in the dictionary.
+    Therefore, the best way to get the parameters is with
+    `my_parameters = parameters.get(name, {})`
 
-    Which means that:
-    - Components are not forced to produce output on all the expected outputs: for example,
-        components taking a decision, like classifiers, can produce output on a subset of
-        the expected output connections and Pipeline will figure out the rest.
-    - Components must not add any key in the data dictionary that is not present in `self.outputs`.
+Pipeline expect the output of this function to be a tuple of two dictionaries.
+The first item is a dictionary that represents the output and it should always
+abide to the following format:
 
-    The second item of the tuple is the `parameters` dictionary. This allows component to
-    propagate downstream any change they might have done to the `parameters` dictionary.
+`{output_name: output_value for output_name in <subset of self.expected_output>}`
 
-    Args:
-        class_: the class that Canals should use as a component.
+Which means that:
+- Components are not forced to produce output on all the expected outputs: for example,
+    components taking a decision, like classifiers, can produce output on a subset of
+    the expected output connections and Pipeline will figure out the rest.
+- Components must not add any key in the data dictionary that is not present in `self.outputs`.
 
-    Returns:
-        A class that can be recognized by Canals as a component.
-
-    Raises:
-        ComponentError: if the class provided has no `run()` method.
-    """
-    logger.debug("Registering %s as a component", class_)
-
-    # '__canals_component__' is used to distinguish components from regular classes.
-    # Its value is set to the desired component name: normally it is the class name, but it can technically be customized.
-    class_.__canals_component__ = class_.__name__
-
-    # Check for run()
-    if not hasattr(class_, "run"):
-        # TODO check the component signature too
-        raise ComponentError("Components must have a 'run()' method. See the docs for more information.")
-
-    return class_
+The second item of the tuple is the `parameters` dictionary. This allows component to
+propagate downstream any change they might have done to the `parameters` dictionary.
```

### Comparing `canals-0.0.2/canals/pipeline/pipeline.py` & `canals-0.0.3/canals/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/canals/pipeline/save_load.py` & `canals-0.0.3/canals/pipeline/save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/docs/index.md` & `canals-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/docs/concepts/concepts.md` & `canals-0.0.3/docs/concepts/concepts.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self,
         input_names: str = ["first_number", "second_number"],
         output_name: str = "value"
     ):
         # self.inputs and self.outputs are required by Canals
         self.inputs = input_names
         self.outputs = [output_name]
-        self.init_parameters = {"input_names": input_names, "output_name": output_name}
+        # self.init_parameters = {"input_names": input_names, "output_name": output_name}
 
     # The signature of the run() method must be exactly this.
     def run(
         self,
         name: str,  # The name of the component in the pipeline
         data: List[Tuple[str, Any]],    # The data from other components
         parameters: Dict[str, Any],     # All the parameters of all the nodes in the pipeline
```

### Comparing `canals-0.0.2/docs/concepts/parameters.md` & `canals-0.0.3/docs/concepts/parameters.md`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/docs/concepts/pipelines.md` & `canals-0.0.3/docs/concepts/pipelines.md`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/docs/concepts/save-load.md` & `canals-0.0.3/docs/concepts/save-load.md`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/images/canals-logo-dark.png` & `canals-0.0.3/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/images/canals-logo-light.png` & `canals-0.0.3/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/test_save_load.py` & `canals-0.0.3/test/test_save_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,36 +36,36 @@
         "pipelines": {
             "pipe1": {
                 "metadata": {"type": "test pipeline", "author": "me"},
                 "max_loops_allowed": 100,
                 "components": {
                     "first_addition": {
                         "type": "AddValue",
-                        "init_parameters": {"add": 1, "input": "value", "output": "value"},
+                        "init_parameters": {"add": 1},
                         "run_parameters": {"add": 6},
                     },
-                    "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
+                    "double": {"type": "Double", "init_parameters": {"input": "value"}},
                     "second_addition": {
                         "type": "AddValue",
-                        "init_parameters": {"add": 1, "input": "value", "output": "value"},
+                        "init_parameters": {"add": 1},
                     },
                     "third_addition": {"refer_to": "pipe1.first_addition"},
                 },
                 "connections": [
                     ("first_addition", "double"),
                     ("double", "second_addition"),
                     ("second_addition", "third_addition"),
                 ],
             },
             "pipe2": {
                 "metadata": {"type": "another test pipeline", "author": "you"},
                 "max_loops_allowed": 100,
                 "components": {
                     "first_addition": {"refer_to": "pipe1.first_addition", "run_parameters": {"add": 4}},
-                    "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
+                    "double": {"type": "Double", "init_parameters": {"input": "value"}},
                     "second_addition": {"refer_to": "pipe1.second_addition"},
                 },
                 "connections": [
                     ("first_addition", "double"),
                     ("double", "second_addition"),
                 ],
             },
```

### Comparing `canals-0.0.2/test/components/__init__.py` & `canals-0.0.3/test/components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/components/test_accumulate.py` & `canals-0.0.3/test/components/test_accumulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Any, List, Tuple, Union, Callable, Optional
 import sys
 import builtins
 from importlib import import_module
 
-from canals import component
+from canals import component  # , non_serializable_component
 
 
 @component
 class Accumulate:
     """
     Accumulates the value flowing through the connection into an internal attribute.
 
@@ -28,18 +28,18 @@
         self.state = 0
 
         if function is None:
             self.function = lambda x, y: x + y
         else:
             self.function = self._load_function(function)
 
-        self.init_parameters = {
-            "connection": connection,
-            "function": self._save_function(function) if function else None,
-        }
+        # 'function' is not serializable normally, so we serialize it manually.
+        if "function" in self.init_parameters.keys():  # type: ignore
+            self.init_parameters["function"] = self._save_function(self.init_parameters["function"])  # type: ignore
+
         self.inputs = [connection]
         self.outputs = [connection]
 
     def _load_function(self, function: Union[Callable, str]):
         """
         Loads the function by trying to import it.
         """
@@ -74,15 +74,15 @@
 
 
 def test_accumulate_default():
     component = Accumulate(connection="test")
     results = component.run(name="test_component", data=[("test", 10)], parameters={})
     assert results == ({"test": 10}, {})
     assert component.state == 10
-    assert component.init_parameters == {"connection": "test", "function": None}
+    assert component.init_parameters == {"connection": "test"}
 
 
 def my_subtract(first, second):
     return first - second
 
 
 def test_accumulate_callable():
```

### Comparing `canals-0.0.2/test/components/test_add_value.py` & `canals-0.0.3/test/components/test_add_value.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,30 +12,28 @@
         Single input, single output component.
 
         :param add: the value to add. This is also a parameter.
         :param input: name of the input connection
         :param output: name of the output connection
         """
         self.add = add
-
-        self.init_parameters = {"add": add, "input": input, "output": output}
         self.inputs = [input]
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         sum = parameters.get(name, {}).get("add", self.add)
         sum += data[0][1]
         return ({self.outputs[0]: sum}, parameters)
 
 
 def test_addvalue_default():
     component = AddValue()
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"value": 11}, {})
-    assert component.init_parameters == {"add": 1, "input": "value", "output": "value"}
+    assert component.init_parameters == {}
 
 
 def test_addvalue_init_params():
     component = AddValue(add=3, input="test_in", output="test_out")
     results = component.run(name="test_component", data=[("test_in", 10)], parameters={})
     assert results == ({"test_out": 13}, {})
     assert component.init_parameters == {"add": 3, "input": "test_in", "output": "test_out"}
```

### Comparing `canals-0.0.2/test/components/test_below.py` & `canals-0.0.3/test/components/test_below.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,14 @@
         :param output_above: the name of the output connection if the value is above the threshold.
         :param output_below: the name of the output connection if the value is below the threshold.
         """
         self.threshold = threshold
         self.output_above = output_above
         self.output_below = output_below
 
-        self.init_parameters = {
-            "threshold": threshold,
-            "input": input,
-            "output_above": output_above,
-            "output_below": output_below,
-        }
         self.inputs = [input]
         self.outputs = [output_above, output_below]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         threshold = parameters.get(name, {}).get("threshold", self.threshold)
         if data[0][1] < threshold:
             return ({self.output_below: data[0][1]}, parameters)
@@ -48,20 +42,15 @@
     component = Below(threshold=10)
     results = component.run(name="test_component", data=[("value", 5)], parameters={})
     assert results == ({"below": 5}, {})
 
     results = component.run(name="test_component", data=[("value", 15)], parameters={})
     assert results == ({"above": 15}, {})
 
-    assert component.init_parameters == {
-        "threshold": 10,
-        "input": "value",
-        "output_above": "above",
-        "output_below": "below",
-    }
+    assert component.init_parameters == {"threshold": 10}
 
 
 def test_below_init_parameters():
     component = Below(threshold=10, input="test", output_above="higher", output_below="lower")
     results = component.run(name="test_component", data=[("test", 5)], parameters={})
     assert results == ({"lower": 5}, {})
```

### Comparing `canals-0.0.2/test/components/test_double.py` & `canals-0.0.3/test/components/test_double.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,29 @@
         Doubles the value in input.
 
         Single input single output component. Doesn't take parameters.
 
         :param input: the name of the input.
         :param output: the name of the output.
         """
-        self.init_parameters = {"input": input, "output": output}
         self.inputs = [input]
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         for _, value in data:
             value *= 2
 
         return ({self.outputs[0]: value}, parameters)
 
 
 def test_double_default():
     component = Double()
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"value": 20}, {})
-    assert component.init_parameters == {"input": "value", "output": "value"}
+    assert component.init_parameters == {}
 
 
 def test_double_init_params():
     component = Double(input="test_in", output="test_out")
     results = component.run(name="test_component", data=[("test_in", 10)], parameters={})
     assert results == ({"test_out": 20}, {})
     assert component.init_parameters == {"input": "test_in", "output": "test_out"}
```

### Comparing `canals-0.0.2/test/components/test_greet.py` & `canals-0.0.3/test/components/test_greet.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         Single input, single output component.
 
         :param message: the message to print. This is also a parameter.
         :param connection: the name of the input and output connection.
         """
         self.message = message
 
-        self.init_parameters = {"connection": connection, "message": message}
         self.inputs = [connection]
         self.outputs = [connection]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         message = parameters.get(name, {}).get("message", self.message)
         logger.info(message)
         return ({data[0][0]: data[0][1]}, parameters)
@@ -33,15 +32,15 @@
 
 def test_greet_default(caplog):
     caplog.set_level(logging.INFO)
     component = Greet()
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"value": 10}, {})
     assert "Greeting component says: Hi!" in caplog.text
-    assert component.init_parameters == {"connection": "value", "message": "\nGreeting component says: Hi!\n"}
+    assert component.init_parameters == {}
 
 
 def test_greet_init_params(caplog):
     caplog.set_level(logging.INFO)
     component = Greet(connection="test", message="Hello!")
     results = component.run(name="test_component", data=[("test", 10)], parameters={})
     assert results == ({"test": 10}, {})
```

### Comparing `canals-0.0.2/test/components/test_merge.py` & `canals-0.0.3/test/components/test_merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,27 @@
 
         Multi input, single output component. Doesn't take any parameter.
 
         :param inputs: the inputs to expect.
         :param output: the name of the output connection.
         """
         self.output = output
-        self.init_parameters = {
-            "inputs": inputs,
-            "output": output,
-        }
         self.inputs = inputs
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         for _, value in data:
             if value is not None:
                 return ({self.outputs[0]: value}, parameters)
 
 
 def test_merge_default():
     component = Merge()
     results = component.run(name="test_component", data=[("value", 5)], parameters={})
     assert results == ({"value": 5}, {})
-    assert component.init_parameters == {
-        "inputs": ["value"],
-        "output": "value",
-    }
+    assert component.init_parameters == {}
 
 
 def test_merge_init_parameters():
     component = Merge(inputs=["test1", "test2", "test3"], output="test")
     results = component.run(name="test_component", data=[("test1", None), ("test2", 5), ("test3", 10)], parameters={})
     assert results == ({"test": 5}, {})
```

### Comparing `canals-0.0.2/test/components/test_remainder.py` & `canals-0.0.3/test/components/test_remainder.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     def __init__(self, divisor: int = 2, input: str = "value", outputs: Optional[List[str]] = None):
         if outputs and len(outputs) != divisor:
             raise ValueError("The divisor must be equal to the number of output connections.")
         if not outputs:
             outputs = [str(remainder) for remainder in range(divisor)]
         self.divisor = divisor
 
-        self.init_parameters = {"divisor": divisor, "input": input, "outputs": outputs}
         self.inputs = [input]
         self.outputs = outputs
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         remainder = data[0][1] % self.divisor
         return ({self.outputs[remainder]: data[0][1]}, parameters)
 
@@ -42,25 +41,25 @@
 def test_remainder_default():
     component = Remainder()
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"0": 10}, {})
 
     results = component.run(name="test_component", data=[("value", 11)], parameters={})
     assert results == ({"1": 11}, {})
-    assert component.init_parameters == {"divisor": 2, "input": "value", "outputs": ["0", "1"]}
+    assert component.init_parameters == {}
 
 
 def test_remainder_default_output_for_divisor():
     component = Remainder(divisor=5)
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"0": 10}, {})
 
     results = component.run(name="test_component", data=[("value", 13)], parameters={})
     assert results == ({"3": 13}, {})
-    assert component.init_parameters == {"divisor": 5, "input": "value", "outputs": ["0", "1", "2", "3", "4"]}
+    assert component.init_parameters == {"divisor": 5}
 
 
 def test_remainder_init_params():
     with pytest.raises(ValueError):
         component = Remainder(divisor=3, input="test", outputs=["one", "two"])
 
     with pytest.raises(ValueError):
```

### Comparing `canals-0.0.2/test/components/test_rename.py` & `canals-0.0.3/test/components/test_rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     :param input: the input connection name.
     :param output: the output connection name.
     """
 
     def __init__(self, input: str, output: str):
         # Contract
-        self.init_parameters = {"input": input, "output": output}
+        # self.init_parameters = {"input": input, "output": output}
         self.inputs = [input]
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         return ({self.outputs[0]: data[0][1]}, parameters)
```

### Comparing `canals-0.0.2/test/components/test_repeat.py` & `canals-0.0.3/test/components/test_repeat.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,30 +12,26 @@
     Doesn't accept parameters.
 
     :param input: the name of the input connection.
     :param outputs: the list of the output connections.
     """
 
     def __init__(self, input: str = "value", outputs: Set[str] = {"first", "second"}):
-        self.init_parameters = {
-            "input": input,
-            "outputs": outputs,
-        }
         self.inputs = [input]
         self.outputs = outputs
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         return ({output: data[0][1] for output in self.outputs}, parameters)
 
 
 def test_repeat_default():
     component = Repeat()
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"first": 10, "second": 10}, {})
-    assert component.init_parameters == {"input": "value", "outputs": {"first", "second"}}
+    assert component.init_parameters == {}
 
 
 def test_repeat_init_params():
     component = Repeat(input="test", outputs={"one", "two"})
     results = component.run(name="test_component", data=[("test", 10)], parameters={})
     assert results == ({"one": 10, "two": 10}, {})
     assert component.init_parameters == {"input": "test", "outputs": {"one", "two"}}
```

### Comparing `canals-0.0.2/test/components/test_subtract.py` & `canals-0.0.3/test/components/test_subtract.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         Double input, single output component. Order of input connections is critical.
         Doesn't have parameters.
 
         :param first_input: name of the connection carrying the value to subtract from.
         :param second_input: name of the connection carrying the value to subtract.
         :param output: name of the output connection.
         """
-        self.init_parameters = {"first_input": first_input, "second_input": second_input, "output": output}
+        # self.init_parameters = {"first_input": first_input, "second_input": second_input, "output": output}
         self.inputs = [first_input, second_input]
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         first_value = [value for name, value in data if name == self.inputs[0]][0]
         second_value = [value for name, value in data if name == self.inputs[1]][0]
```

### Comparing `canals-0.0.2/test/components/test_sum.py` & `canals-0.0.3/test/components/test_sum.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
         Multi input, single output component. Order of input connections is irrelevant.
          Doesn't have parameters.
 
         :param inputs: list of connections to sum.
         :param output: name of the output connection.
         """
-        self.init_parameters = {"inputs": inputs, "output": output}
+        # self.init_parameters = {"inputs": inputs, "output": output}
         self.inputs = inputs
         self.outputs = [output]
 
     def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
         sum = 0
         for _, value in data:
             if value:
@@ -28,15 +28,15 @@
         return ({self.outputs[0]: sum}, parameters)
 
 
 def test_sum_default():
     component = Sum()
     results = component.run(name="test_component", data=[("value", 10)], parameters={})
     assert results == ({"sum": 10}, {})
-    assert component.init_parameters == {"inputs": ["value"], "output": "sum"}
+    assert component.init_parameters == {}
 
 
 def test_sum_init_params():
     component = Sum(inputs=["value", "value"], output="test_out")
     results = component.run(name="test_component", data=[("value", 10), ("value", 4)], parameters={})
     assert results == ({"test_out": 14}, {})
     assert component.init_parameters == {"inputs": ["value", "value"], "output": "test_out"}
```

### Comparing `canals-0.0.2/test/pipelines/_test_looping_and_merge_pipeline.py` & `canals-0.0.3/test/pipelines/_test_looping_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_complex_pipeline.py` & `canals-0.0.3/test/pipelines/test_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_decision_and_merge_pipeline.py` & `canals-0.0.3/test/pipelines/test_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_decision_pipeline.py` & `canals-0.0.3/test/pipelines/test_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_linear_pipeline.py` & `canals-0.0.3/test/pipelines/test_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_looping_pipeline.py` & `canals-0.0.3/test/pipelines/test_looping_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_merging_pipeline.py` & `canals-0.0.3/test/pipelines/test_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/test/pipelines/test_parallel_branches_pipeline.py` & `canals-0.0.3/test/pipelines/test_parallel_branches_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/.gitignore` & `canals-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/LICENSE` & `canals-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/README.md` & `canals-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/pyproject.toml` & `canals-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `canals-0.0.2/PKG-INFO` & `canals-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.0.2
+Version: 0.0.3
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

