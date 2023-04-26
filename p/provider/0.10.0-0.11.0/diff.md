# Comparing `tmp/provider-0.10.0.tar.gz` & `tmp/provider-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provider-0.10.0.tar", max compression
+gzip compressed data, was "provider-0.11.0.tar", max compression
```

## Comparing `provider-0.10.0.tar` & `provider-0.11.0.tar`

### file list

```diff
@@ -1,51 +1,49 @@
--rw-r--r--   0        0        0     1901 2023-04-25 16:21:42.296822 provider-0.10.0/README.md
--rw-r--r--   0        0        0        0 2023-04-25 16:21:42.297308 provider-0.10.0/provider/__init__.py
--rw-r--r--   0        0        0     5728 2023-04-25 16:21:42.297389 provider-0.10.0/provider/access.py
--rw-r--r--   0        0        0        0 2023-04-25 16:21:42.297441 provider-0.10.0/provider/cli/__init__.py
--rw-r--r--   0        0        0     2086 2023-04-25 16:21:42.297512 provider-0.10.0/provider/cli/main.py
--rw-r--r--   0        0        0     3020 2023-04-25 16:21:42.297609 provider-0.10.0/provider/config/__init__.py
--rw-r--r--   0        0        0     4377 2023-04-25 16:21:42.297680 provider-0.10.0/provider/config/loaders.py
--rw-r--r--   0        0        0     1128 2023-04-25 16:21:42.297772 provider-0.10.0/provider/config/tests/test_configurer.py
--rw-r--r--   0        0        0      921 2023-04-25 16:21:42.297831 provider-0.10.0/provider/config/tests/test_loaders.py
--rw-r--r--   0        0        0      401 2023-04-25 16:21:42.297888 provider-0.10.0/provider/dataclass.py
--rw-r--r--   0        0        0      769 2023-04-25 16:21:42.297949 provider-0.10.0/provider/diagnostics.py
--rw-r--r--   0        0        0      335 2023-04-25 16:21:42.298010 provider-0.10.0/provider/health.py
--rw-r--r--   0        0        0     5295 2023-04-25 16:21:42.298081 provider-0.10.0/provider/namespace.py
--rw-r--r--   0        0        0     2799 2023-04-25 16:21:42.298150 provider-0.10.0/provider/provider.py
--rw-r--r--   0        0        0     3248 2023-04-25 16:21:42.298218 provider-0.10.0/provider/resources.py
--rw-r--r--   0        0        0     1464 2023-04-25 16:21:42.298282 provider-0.10.0/provider/rpc.py
--rw-r--r--   0        0        0       26 2023-04-25 16:21:42.298371 provider-0.10.0/provider/runtime/__init__.py
--rw-r--r--   0        0        0     3312 2023-04-25 16:21:42.298440 provider-0.10.0/provider/runtime/aws_lambda.py
--rw-r--r--   0        0        0     2609 2023-04-25 16:21:42.298520 provider-0.10.0/provider/runtime/aws_lambda_entrypoint.py
--rw-r--r--   0        0        0      690 2023-04-25 16:21:42.298588 provider-0.10.0/provider/runtime/initialise.py
--rw-r--r--   0        0        0        0 2023-04-25 16:21:42.298644 provider-0.10.0/provider/runtime/tests/__init__.py
--rw-r--r--   0        0        0      111 2023-04-25 16:21:42.298774 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_grant_works.json
--rw-r--r--   0        0        0      365 2023-04-25 16:21:42.298830 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_load_works.json
--rw-r--r--   0        0        0      159 2023-04-25 16:21:42.298889 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_load_works_with_subtasks.json
--rw-r--r--   0        0        0      607 2023-04-25 16:21:42.298956 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe.json
--rw-r--r--   0        0        0      846 2023-04-25 16:21:42.299018 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_config.json
--rw-r--r--   0        0        0      932 2023-04-25 16:21:42.299072 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_errors.json
--rw-r--r--   0        0        0     1560 2023-04-25 16:21:42.299160 provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_resources.json
--rw-r--r--   0        0        0      306 2023-04-25 16:21:42.299229 provider-0.10.0/provider/runtime/tests/aws_lambda_entrypoint_test.py
--rw-r--r--   0        0        0     5998 2023-04-25 16:21:42.299304 provider-0.10.0/provider/runtime/tests/aws_lambda_test.py
--rw-r--r--   0        0        0      260 2023-04-25 16:21:42.299393 provider-0.10.0/provider/runtime/tests/commonfate_provider_dist/README.md
--rw-r--r--   0        0        0        0 2023-04-25 16:21:42.299417 provider-0.10.0/provider/runtime/tests/commonfate_provider_dist/__init__.py
--rw-r--r--   0        0        0      143 2023-04-25 16:21:42.299484 provider-0.10.0/provider/runtime/tests/commonfate_provider_dist/manifest.json
--rw-r--r--   0        0        0      291 2023-04-25 16:21:42.299551 provider-0.10.0/provider/runtime/tests/initialise_test.py
--rw-r--r--   0        0        0        0 2023-04-25 16:21:42.299606 provider-0.10.0/provider/runtime/tests/provider_example/__init__.py
--rw-r--r--   0        0        0      136 2023-04-25 16:21:42.299667 provider-0.10.0/provider/runtime/tests/provider_example/provider.py
--rw-r--r--   0        0        0      861 2023-04-25 16:21:42.299729 provider-0.10.0/provider/schema.py
--rw-r--r--   0        0        0     3051 2023-04-25 16:21:42.299817 provider-0.10.0/provider/target.py
--rw-r--r--   0        0        0     1846 2023-04-25 16:21:42.299888 provider-0.10.0/provider/tasks.py
--rw-r--r--   0        0        0        0 2023-04-25 16:21:42.299961 provider-0.10.0/provider/tests/__init__.py
--rw-r--r--   0        0        0     3449 2023-04-25 16:21:42.300733 provider-0.10.0/provider/tests/access_test.py
--rw-r--r--   0        0        0     1223 2023-04-25 16:21:42.300793 provider-0.10.0/provider/tests/health_test.py
--rw-r--r--   0        0        0      582 2023-04-25 16:21:42.300855 provider-0.10.0/provider/tests/helper.py
--rw-r--r--   0        0        0      545 2023-04-25 16:21:42.300920 provider-0.10.0/provider/tests/provider_test.py
--rw-r--r--   0        0        0     1274 2023-04-25 16:21:42.300985 provider-0.10.0/provider/tests/resources_test.py
--rw-r--r--   0        0        0     1740 2023-04-25 16:21:42.301048 provider-0.10.0/provider/tests/schema_test.py
--rw-r--r--   0        0        0      431 2023-04-25 16:21:42.301103 provider-0.10.0/provider/tests/storage_test.py
--rw-r--r--   0        0        0     1540 2023-04-25 16:21:42.301169 provider-0.10.0/provider/tests/target_test.py
--rw-r--r--   0        0        0      813 2023-04-25 16:21:42.301231 provider-0.10.0/pyproject.toml
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 provider-0.10.0/setup.py
--rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 provider-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0     1901 2023-04-25 16:42:55.406654 provider-0.11.0/README.md
+-rw-r--r--   0        0        0     2799 2023-04-25 16:42:55.406654 provider-0.11.0/provider/__init__.py
+-rw-r--r--   0        0        0     5733 2023-04-25 16:42:55.406654 provider-0.11.0/provider/access.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:42:55.406654 provider-0.11.0/provider/cli/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-25 16:42:55.406654 provider-0.11.0/provider/cli/main.py
+-rw-r--r--   0        0        0     3006 2023-04-25 16:42:55.410655 provider-0.11.0/provider/config/__init__.py
+-rw-r--r--   0        0        0     4377 2023-04-25 16:42:55.410655 provider-0.11.0/provider/config/loaders.py
+-rw-r--r--   0        0        0     1134 2023-04-25 16:42:55.410655 provider-0.11.0/provider/config/tests/test_configurer.py
+-rw-r--r--   0        0        0      921 2023-04-25 16:42:55.410655 provider-0.11.0/provider/config/tests/test_loaders.py
+-rw-r--r--   0        0        0      401 2023-04-25 16:42:55.410655 provider-0.11.0/provider/dataclass.py
+-rw-r--r--   0        0        0      769 2023-04-25 16:42:55.410655 provider-0.11.0/provider/diagnostics.py
+-rw-r--r--   0        0        0      341 2023-04-25 16:42:55.410655 provider-0.11.0/provider/health.py
+-rw-r--r--   0        0        0     5295 2023-04-25 16:42:55.410655 provider-0.11.0/provider/namespace.py
+-rw-r--r--   0        0        0     3248 2023-04-25 16:42:55.410655 provider-0.11.0/provider/resources.py
+-rw-r--r--   0        0        0     1464 2023-04-25 16:42:55.410655 provider-0.11.0/provider/rpc.py
+-rw-r--r--   0        0        0       26 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/__init__.py
+-rw-r--r--   0        0        0     3314 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/aws_lambda.py
+-rw-r--r--   0        0        0     2609 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/aws_lambda_entrypoint.py
+-rw-r--r--   0        0        0      696 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/initialise.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_grant_works.json
+-rw-r--r--   0        0        0      365 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_load_works.json
+-rw-r--r--   0        0        0      159 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_load_works_with_subtasks.json
+-rw-r--r--   0        0        0      607 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe.json
+-rw-r--r--   0        0        0      846 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_config.json
+-rw-r--r--   0        0        0      932 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_errors.json
+-rw-r--r--   0        0        0     1560 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_resources.json
+-rw-r--r--   0        0        0      306 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/aws_lambda_entrypoint_test.py
+-rw-r--r--   0        0        0     6004 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/aws_lambda_test.py
+-rw-r--r--   0        0        0      260 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/commonfate_provider_dist/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/commonfate_provider_dist/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/commonfate_provider_dist/manifest.json
+-rw-r--r--   0        0        0      277 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/initialise_test.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/provider_example/__init__.py
+-rw-r--r--   0        0        0      142 2023-04-25 16:42:55.410655 provider-0.11.0/provider/runtime/tests/provider_example/provider.py
+-rw-r--r--   0        0        0      861 2023-04-25 16:42:55.410655 provider-0.11.0/provider/schema.py
+-rw-r--r--   0        0        0     3051 2023-04-25 16:42:55.410655 provider-0.11.0/provider/target.py
+-rw-r--r--   0        0        0     1852 2023-04-25 16:42:55.410655 provider-0.11.0/provider/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:42:55.410655 provider-0.11.0/provider/tests/__init__.py
+-rw-r--r--   0        0        0     3456 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/access_test.py
+-rw-r--r--   0        0        0     1228 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/health_test.py
+-rw-r--r--   0        0        0      588 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/helper.py
+-rw-r--r--   0        0        0      538 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/provider_test.py
+-rw-r--r--   0        0        0     1274 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/resources_test.py
+-rw-r--r--   0        0        0     1746 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/schema_test.py
+-rw-r--r--   0        0        0      431 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/storage_test.py
+-rw-r--r--   0        0        0     1540 2023-04-25 16:42:55.414655 provider-0.11.0/provider/tests/target_test.py
+-rw-r--r--   0        0        0      813 2023-04-25 16:43:18.754864 provider-0.11.0/pyproject.toml
+-rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 provider-0.11.0/PKG-INFO
```

### Comparing `provider-0.10.0/README.md` & `provider-0.11.0/README.md`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/access.py` & `provider-0.11.0/provider/access.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
 import inspect
 import typing_extensions
 import typing
 
 from pydantic import BaseModel
 
-from provider import namespace, provider, rpc
+import provider
+from provider import namespace, rpc
 from provider import target as cf_target
 
-
 _T = typing.TypeVar("_T")
 
 
 @typing_extensions.dataclass_transform()
 def target(
     kind: typing.Optional[str] = None,
 ) -> typing.Callable[[type[_T]], type[_T]]:
```

### Comparing `provider-0.10.0/provider/cli/main.py` & `provider-0.11.0/provider/cli/main.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/config/__init__.py` & `provider-0.11.0/provider/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 import boto3
 from botocore.exceptions import ClientError
 from dataclasses import dataclass
 from provider.config import loaders
-from provider import provider
+import provider
 
 
 class ConfigError(Exception):
     """
     Raised if the provider is incorrectly configured.
     """
```

### Comparing `provider-0.10.0/provider/config/loaders.py` & `provider-0.11.0/provider/config/loaders.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/config/tests/test_configurer.py` & `provider-0.11.0/provider/config/tests/test_configurer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
-from provider import namespace, provider, config
+import provider
+from provider import namespace, config
 from provider.config import loaders
 
 
 @pytest.fixture(autouse=True)
 def fresh_namespace():
     """clear the registered provider, targets etc between test runs"""
     yield
```

### Comparing `provider-0.10.0/provider/config/tests/test_loaders.py` & `provider-0.11.0/provider/config/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/diagnostics.py` & `provider-0.11.0/provider/diagnostics.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/namespace.py` & `provider-0.11.0/provider/namespace.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/provider.py` & `provider-0.11.0/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/resources.py` & `provider-0.11.0/provider/resources.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/rpc.py` & `provider-0.11.0/provider/rpc.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/runtime/aws_lambda.py` & `provider-0.11.0/provider/runtime/aws_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 import typing
+import provider
 from provider import (
-    provider,
     resources,
     tasks,
     schema,
     access,
     rpc,
 )
 from common_fate_schema.provider import v1alpha1
```

### Comparing `provider-0.10.0/provider/runtime/aws_lambda_entrypoint.py` & `provider-0.11.0/provider/runtime/aws_lambda_entrypoint.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/runtime/initialise.py` & `provider-0.11.0/provider/runtime/initialise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing
-from provider import config, namespace, provider
+from provider import config, namespace
+import provider
 
 
 def initialise_provider(
     configurer: typing.Optional[config.Configurer] = None,
 ) -> provider.Provider:
     """
     Used in the Provider runtimes to load and initialise a provider class.
```

### Comparing `provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe.json` & `provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe.json`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_config.json` & `provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_config.json`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_errors.json` & `provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_errors.json`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_resources.json` & `provider-0.11.0/provider/runtime/tests/__snapshots__/aws_lambda_test/test_provider_describe_with_resources.json`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/runtime/tests/aws_lambda_test.py` & `provider-0.11.0/provider/runtime/tests/aws_lambda_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pydantic import BaseModel
 import pytest
 from syrupy.extensions.json import JSONSnapshotExtension
 
 from provider.runtime import AWSLambdaRuntime
-from provider import namespace, provider, access, target, resources, tasks
+from provider import namespace, access, target, resources, tasks
+import provider
 from provider.tests import helper
 
 
 @pytest.fixture
 def snapshot_json(snapshot):
     """use JSON, rather than AmberSnapshotExtension as our schema is serialized as JSON"""
     return snapshot.use_extension(JSONSnapshotExtension)
```

### Comparing `provider-0.10.0/provider/schema.py` & `provider-0.11.0/provider/schema.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/target.py` & `provider-0.11.0/provider/target.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/tasks.py` & `provider-0.11.0/provider/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing
-from provider import provider, namespace
+from provider import namespace
+import provider
 
 from provider.dataclass import ModelMeta
 
 
 LoaderFunc = typing.Callable[[typing.Any], None]
```

### Comparing `provider-0.10.0/provider/tests/access_test.py` & `provider-0.11.0/provider/tests/access_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass
 from pydantic import BaseModel
 import pytest
-from provider import access, namespace, provider, rpc
+
+from provider import access, namespace, rpc
+import provider
 
 
 @pytest.fixture(autouse=True)
 def fresh_namespace():
     """clear the registered provider, targets etc between test runs"""
     yield
     namespace.clear()
```

### Comparing `provider-0.10.0/provider/tests/health_test.py` & `provider-0.11.0/provider/tests/health_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from syrupy.extensions.json import JSONSnapshotExtension
-
-from provider import diagnostics, namespace, provider, health
+import provider
+from provider import diagnostics, namespace, health
 
 
 @pytest.fixture(autouse=True)
 def fresh_namespace():
     yield
     namespace.clear()
```

### Comparing `provider-0.10.0/provider/tests/helper.py` & `provider-0.11.0/provider/tests/helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing
 
-from provider import config, provider
+import provider
+from provider import config
 from provider.config import loaders
 from provider.runtime import initialise
 
 
 def initialise_test_provider(config_dict: typing.Dict[str, str]) -> provider.Provider:
     """
     A wrapper around commonfate_provider.runtime.initialise
```

### Comparing `provider-0.10.0/provider/tests/provider_test.py` & `provider-0.11.0/provider/tests/provider_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
-from provider import namespace, provider, diagnostics
+from provider import namespace
+import provider
 
 
 @pytest.fixture(autouse=True)
 def fresh_namespace():
     yield
     namespace.clear()
```

### Comparing `provider-0.10.0/provider/tests/resources_test.py` & `provider-0.11.0/provider/tests/resources_test.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/provider/tests/schema_test.py` & `provider-0.11.0/provider/tests/schema_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import pytest
 from syrupy.extensions.json import JSONSnapshotExtension
 
-from provider import access, namespace, provider, resources, schema, target
+import provider
+from provider import access, namespace, resources, schema, target
 
 
 @pytest.fixture(autouse=True)
 def fresh_namespace():
     """clear the registered provider, targets etc between test runs"""
     yield
     namespace.clear()
```

### Comparing `provider-0.10.0/provider/tests/target_test.py` & `provider-0.11.0/provider/tests/target_test.py`

 * *Files identical despite different names*

### Comparing `provider-0.10.0/pyproject.toml` & `provider-0.11.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "provider"
-version = "0.10.0"
+version = "0.11.0"
 description = "Common Fate Provider Development Kit"
 authors = ["Common Fate <hello@commonfate.io>"]
 readme = "README.md"
 packages = [{include = "provider"}]
 include = ["provider/**/*.py"]
 ## TODO: Not excluding test from the build
 exclude = ["provider/tests/**"]
```

### Comparing `provider-0.10.0/setup.py` & `provider-0.11.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,91 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['provider',
- 'provider.cli',
- 'provider.config',
- 'provider.config.tests',
- 'provider.runtime',
- 'provider.runtime.tests',
- 'provider.runtime.tests.commonfate_provider_dist',
- 'provider.runtime.tests.provider_example']
-
-package_data = \
-{'': ['*'], 'provider.runtime.tests': ['__snapshots__/aws_lambda_test/*']}
-
-install_requires = \
-['boto3>=1.26.82,<2.0.0',
- 'click>=8.1.3,<9.0.0',
- 'common-fate-schema>=0.7.0,<0.8.0',
- 'pydantic>=1.10.5,<2.0.0',
- 'toml==0.10.2',
- 'typing-extensions>=4.5.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['provider = provider.cli.main:cli']}
-
-setup_kwargs = {
-    'name': 'provider',
-    'version': '0.10.0',
-    'description': 'Common Fate Provider Development Kit',
-    'long_description': '# Provider Development Kit\n\nCommon Fate Provider Development Kit for Python.\n\n## What is a provider?\n\nA Provider is a Python service which provides a consistent API for managing fine-grain permissions.\n\nManaging permissions in cloud providers, SaaS applications, and CI/CD platforms usually requires access to highly sensitive secrets, like administrative API tokens. The Provider framework allows for access to be granted and revoked to these platforms without requiring direct access to these tokens:\n\n![diagram of Provider framework](./docs/provider.drawio.svg)\n\n## What does the Provider Development Kit do?\n\nThe Provider Development Kit (PDK) makes it easy to develop and deploy Providers.\n\n```python\nclass Provider(provider.Provider):\n    api_url = provider.String()\n\n@access.target()\nclass Target:\n    ...\n\n@access.grant()\ndef grant(p: Provider, subject: str, target: Target):\n    # perform API calls here to grant access\n    ...\n\n@access.revoke()\ndef revoke(p: Provider, subject: str, target: Target):\n    # perform API calls here to revoke access\n    ...\n```\n\nThe PDK handles configuration and packaging into a cloud-native function which can be executed by an application.\n\n## Supported runtimes\n\nCurrently the supported runtimes for Providers are as follows:\n\n- AWS Lambda\n\n## Provider Schemas\n\nEach Provider has a strongly-typed schema. An example schema is shown below:\n\n```json\n{\n  "audit": {\n    "resourceLoaders": {},\n    "resources": {}\n  },\n  "config": {},\n  "target": {\n    "MyTarget": {\n      "schema": {\n        "first": {\n          "description": "first var",\n          "id": "first",\n          "resourceName": null,\n          "title": "First",\n          "type": "string"\n        }\n      }\n    }\n  }\n}\n```\n\nThe schema is based on [JSON Schema](https://json-schema.org/) and allows applications using Providers to interpret the available resources and display the appropriate UI.\n',
-    'author': 'Common Fate',
-    'author_email': 'hello@commonfate.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+Metadata-Version: 2.1
+Name: provider
+Version: 0.11.0
+Summary: Common Fate Provider Development Kit
+Author: Common Fate
+Author-email: hello@commonfate.io
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.26.82,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: common-fate-schema (>=0.7.0,<0.8.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: toml (==0.10.2)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Description-Content-Type: text/markdown
+
+# Provider Development Kit
+
+Common Fate Provider Development Kit for Python.
+
+## What is a provider?
+
+A Provider is a Python service which provides a consistent API for managing fine-grain permissions.
+
+Managing permissions in cloud providers, SaaS applications, and CI/CD platforms usually requires access to highly sensitive secrets, like administrative API tokens. The Provider framework allows for access to be granted and revoked to these platforms without requiring direct access to these tokens:
+
+![diagram of Provider framework](./docs/provider.drawio.svg)
+
+## What does the Provider Development Kit do?
+
+The Provider Development Kit (PDK) makes it easy to develop and deploy Providers.
+
+```python
+class Provider(provider.Provider):
+    api_url = provider.String()
+
+@access.target()
+class Target:
+    ...
+
+@access.grant()
+def grant(p: Provider, subject: str, target: Target):
+    # perform API calls here to grant access
+    ...
+
+@access.revoke()
+def revoke(p: Provider, subject: str, target: Target):
+    # perform API calls here to revoke access
+    ...
+```
+
+The PDK handles configuration and packaging into a cloud-native function which can be executed by an application.
+
+## Supported runtimes
+
+Currently the supported runtimes for Providers are as follows:
+
+- AWS Lambda
+
+## Provider Schemas
+
+Each Provider has a strongly-typed schema. An example schema is shown below:
+
+```json
+{
+  "audit": {
+    "resourceLoaders": {},
+    "resources": {}
+  },
+  "config": {},
+  "target": {
+    "MyTarget": {
+      "schema": {
+        "first": {
+          "description": "first var",
+          "id": "first",
+          "resourceName": null,
+          "title": "First",
+          "type": "string"
+        }
+      }
+    }
+  }
 }
+```
 
+The schema is based on [JSON Schema](https://json-schema.org/) and allows applications using Providers to interpret the available resources and display the appropriate UI.
 
-setup(**setup_kwargs)
```

