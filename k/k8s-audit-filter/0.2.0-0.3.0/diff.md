# Comparing `tmp/k8s_audit_filter-0.2.0-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19455 bytes, number of entries: 11
+Zip file size: 19607 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 k8s_audit_filter/__about__.py
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
 -rw-r--r--  2.0 unx     1117 b- defN 20-Feb-02 00:00 k8s_audit_filter/abstract_classes.py
--rw-r--r--  2.0 unx     2241 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
+-rw-r--r--  2.0 unx     2654 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
 -rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
 -rw-r--r--  2.0 unx     2180 b- defN 20-Feb-02 00:00 k8s_audit_filter/resourses_field.py
 -rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
-?rw-r--r--  2.0 unx     5880 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      946 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.2.0.dist-info/RECORD
-11 files, 51225 bytes uncompressed, 17841 bytes compressed:  65.2%
+?rw-r--r--  2.0 unx     5861 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      946 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/RECORD
+11 files, 51619 bytes uncompressed, 17993 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: k8s_audit_filter/resourses_field.py
 Comment: 
 
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
-Filename: k8s_audit_filter-0.2.0.dist-info/METADATA
+Filename: k8s_audit_filter-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.2.0.dist-info/WHEEL
+Filename: k8s_audit_filter-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.3.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.2.0.dist-info/RECORD
+Filename: k8s_audit_filter-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "0.3.0"
```

## k8s_audit_filter/audit_filter.py

```diff
@@ -1,14 +1,17 @@
+import logging
 from typing import Union
 
 import yaml
 
 from .abstract_classes import Rule
 from .rules import RuleFactory
 
+logger = logging.getLogger(__name__)
+
 
 class AuditFilterException(Exception):
     pass
 
 
 class AuditFilter:
     def __init__(self, config: Union[dict, str, None] = None):
@@ -32,16 +35,23 @@
         else:
             raise AuditFilterException("Invalid config")
 
     def filter(self, log_line: dict) -> bool:
         if not self.rules:
             return True  # no rules, no filter
         for rule in self.rules:
-            if rule.check_rule(log_line):
-                return True
+            try:
+                if rule.check_rule(log_line):
+                    return True
+            except Exception as e:
+                logger.error(
+                    f"Exception: {e}, Type: {e.__class__.__qualname__} "
+                    f"Traceback: {e.__traceback__} Rule: {rule} with log line: {log_line}"
+                )
+                return True  # if rule check fails, we assume it should not be filtered
         return False
 
     def add_rule(self, rule: dict):
         internal_rule = RuleFactory.create(rule)
         self.rules.append(internal_rule)
         self.config.append(internal_rule.as_dict)  # type: ignore
```

## k8s_audit_filter/resourses_field.py

```diff
@@ -12,15 +12,15 @@
         if not self.value:
             return True
         if target["objectRef"].get("apiGroup") and target["objectRef"]["apiGroup"] == self.value:
             return True
         return False
 
 
-class ResourceResourseSubField(Field):
+class ResourceResourceSubField(Field):
     def __init__(self, value: List[str]):
         self.name = "resources"
         self.value: List[str] = value
 
     def check_match(self, target: dict) -> bool:
         for resource in self.value:
             if target["objectRef"].get("resource") and target["objectRef"]["resource"] == resource:
@@ -39,15 +39,15 @@
                 return True
         return False
 
 
 class ResourcesFieldsFactory(Factory):
     mapping = {
         "group": ResourceGroupSubField,
-        "resources": ResourceResourseSubField,
+        "resources": ResourceResourceSubField,
         "resourceNames": ResourceNamesSubField,
     }
 
     @classmethod
     def create(cls, entities: dict):
         fields = []
         for key, value in entities.items():
```

## Comparing `k8s_audit_filter-0.2.0.dist-info/METADATA` & `k8s_audit_filter-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -74,16 +74,16 @@
         audit_filter = AuditFilter('path/to/audit_policy.yaml')  # init AuditFilter class with path to audit policy file
         filtered_log = [line for line in full_log if audit_filter.filter(full_log)]  # filter audit logs
 
         bucket_name = os.environ.get('BUCKET_NAME')
         object_key = 'AUDIT/' + os.environ.get('CLUSTER_ID') + '/' + datetime.now().strftime(
             '%Y-%m-%d-%H:%M:%S') + '-' + get_random_alphanumeric_string(5)
         object_value = '\n'.join(filtered_log)  # prepare data to load
-        client.put_object(Bucket=bucket_name, Key=object_key, Body=object_value,
-                          StorageClass='COLD')  # load data to cloud storage
+        # load data to cloud storage
+        client.put_object(Bucket=bucket_name, Key=object_key, Body=object_value, StorageClass='COLD')
 ```
 
 Also you can update your policy dinamically, just use ```add_rule``` and ```remove_rule``` method:
 
 ```python
 from k8s_audit_filter import AuditFilter
```

## Comparing `k8s_audit_filter-0.2.0.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.3.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

