# Comparing `tmp/dcicutils-7.3.0.1b34.tar.gz` & `tmp/dcicutils-7.3.0.1b35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.0.1b34.tar", max compression
+gzip compressed data, was "dcicutils-7.3.0.1b35.tar", max compression
```

## Comparing `dcicutils-7.3.0.1b34.tar` & `dcicutils-7.3.0.1b35.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1166 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/README.rst
--rw-r--r--   0        0        0        0 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-26 11:54:22.917099 dcicutils-7.3.0.1b34/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87581 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   121536 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-26 11:54:22.921099 dcicutils-7.3.0.1b34/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-26 11:54:22.925099 dcicutils-7.3.0.1b34/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-26 11:54:22.925099 dcicutils-7.3.0.1b34/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0    10080 2023-04-26 11:54:22.925099 dcicutils-7.3.0.1b34/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-26 11:54:22.925099 dcicutils-7.3.0.1b34/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-26 11:54:22.925099 dcicutils-7.3.0.1b34/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3807 2023-04-26 11:54:22.925099 dcicutils-7.3.0.1b34/pyproject.toml
--rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b34/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/README.rst
+-rw-r--r--   0        0        0        0 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-26 13:19:53.416937 dcicutils-7.3.0.1b35/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87972 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-26 13:19:53.420937 dcicutils-7.3.0.1b35/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   121536 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0    10080 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3807 2023-04-26 13:19:53.424937 dcicutils-7.3.0.1b35/pyproject.toml
+-rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 dcicutils-7.3.0.1b35/PKG-INFO
```

### Comparing `dcicutils-7.3.0.1b34/README.rst` & `dcicutils-7.3.0.1b35/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/base.py` & `dcicutils-7.3.0.1b35/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/beanstalk_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/cloudformation_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/codebuild_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/command_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/common.py` & `dcicutils-7.3.0.1b35/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/creds_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/data_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/deployment_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/diff_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/docker_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/ecr_scripts.py` & `dcicutils-7.3.0.1b35/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/ecr_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/ecs_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/env_base.py` & `dcicutils-7.3.0.1b35/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/env_manager.py` & `dcicutils-7.3.0.1b35/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/env_scripts.py` & `dcicutils-7.3.0.1b35/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/env_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/env_utils_legacy.py` & `dcicutils-7.3.0.1b35/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/es_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/exceptions.py` & `dcicutils-7.3.0.1b35/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/ff_mocks.py` & `dcicutils-7.3.0.1b35/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/ff_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/jh_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/kibana/dashboards.json` & `dcicutils-7.3.0.1b35/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/kibana/readme.md` & `dcicutils-7.3.0.1b35/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/lang_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/log_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/misc_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,14 +596,21 @@
     if frac == 0.0:
         seconds = int(intpart)
     if as_type is not None:
         seconds = as_type(seconds)
     return seconds
 
 
+# Pulled this in from "glacier" branch for use in foursight-core (2023-04-26).
+def future_datetime(*, now=None, seconds=0, minutes=0, hours=0, days=0, weeks=0, milliseconds=0):
+    delta = datetime.timedelta(seconds=seconds, minutes=minutes, hours=hours,
+                               days=days, weeks=weeks, milliseconds=milliseconds)
+    return (now or datetime.datetime.now()) + delta
+
+
 REF_TZ = pytz.timezone(os.environ.get("REF_TZ") or "US/Eastern")
 
 
 class DatetimeCoercionFailure(ValueError):
 
     def __init__(self, timespec, timezone):
         self.timespec = timespec
```

### Comparing `dcicutils-7.3.0.1b34/dcicutils/obfuscation_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/opensearch_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/qa_checkers.py` & `dcicutils-7.3.0.1b35/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/qa_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/redis_tools.py` & `dcicutils-7.3.0.1b35/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/redis_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/s3_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.3.0.1b35/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/secrets_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/snapshot_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/task_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/dcicutils/trace_utils.py` & `dcicutils-7.3.0.1b35/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.0.1b34/pyproject.toml` & `dcicutils-7.3.0.1b35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.0.1b34"
+version = "7.3.0.1b35"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.3.0.1b34/PKG-INFO` & `dcicutils-7.3.0.1b35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.0.1b34
+Version: 7.3.0.1b35
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

