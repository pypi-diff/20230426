# Comparing `tmp/nornir_srl-0.0.2.tar.gz` & `tmp/nornir_srl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_srl-0.0.2.tar", max compression
+gzip compressed data, was "nornir_srl-0.0.3.tar", max compression
```

## Comparing `nornir_srl-0.0.2.tar` & `nornir_srl-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7763 2023-04-07 13:39:14.312735 nornir_srl-0.0.2/README.md
--rw-r--r--   0        0        0       22 2022-11-20 12:27:33.451929 nornir_srl-0.0.2/nornir_srl/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 18:28:42.918760 nornir_srl-0.0.2/nornir_srl/connections/__init__.py
--rw-r--r--   0        0        0     3372 2023-04-06 23:26:57.017816 nornir_srl-0.0.2/nornir_srl/connections/helpers.py
--rw-r--r--   0        0        0    13026 2023-04-07 11:04:13.339840 nornir_srl-0.0.2/nornir_srl/connections/srlinux.py
--rw-r--r--   0        0        0     7904 2023-04-07 10:50:01.483750 nornir_srl-0.0.2/nornir_srl/fsc.py
--rw-r--r--   0        0        0        0 2022-10-30 22:33:33.108689 nornir_srl-0.0.2/nornir_srl/tasks/__init__.py
--rw-r--r--   0        0        0      373 2022-11-25 22:31:43.343296 nornir_srl-0.0.2/nornir_srl/tasks/helpers.py
--rw-r--r--   0        0        0     8844 2023-01-03 20:18:09.232105 nornir_srl-0.0.2/nornir_srl/tasks/srl_config.py
--rw-r--r--   0        0        0      846 2023-04-07 13:56:19.686468 nornir_srl-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     9143 2023-04-07 13:56:30.822740 nornir_srl-0.0.2/setup.py
--rw-r--r--   0        0        0     8773 2023-04-07 13:56:30.823404 nornir_srl-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    12129 2023-04-25 19:19:50.485815 nornir_srl-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2022-11-20 12:27:33.451929 nornir_srl-0.0.3/nornir_srl/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 18:28:42.918760 nornir_srl-0.0.3/nornir_srl/connections/__init__.py
+-rw-r--r--   0        0        0     3781 2023-04-25 18:20:26.447734 nornir_srl-0.0.3/nornir_srl/connections/helpers.py
+-rw-r--r--   0        0        0    19453 2023-04-25 19:12:50.201512 nornir_srl-0.0.3/nornir_srl/connections/srlinux.py
+-rw-r--r--   0        0        0     9599 2023-04-25 18:56:11.575576 nornir_srl-0.0.3/nornir_srl/fsc.py
+-rw-r--r--   0        0        0        0 2022-10-30 22:33:33.108689 nornir_srl-0.0.3/nornir_srl/tasks/__init__.py
+-rw-r--r--   0        0        0      373 2022-11-25 22:31:43.343296 nornir_srl-0.0.3/nornir_srl/tasks/helpers.py
+-rw-r--r--   0        0        0     8844 2023-01-03 20:18:09.232105 nornir_srl-0.0.3/nornir_srl/tasks/srl_config.py
+-rw-r--r--   0        0        0      846 2023-04-25 19:22:17.657001 nornir_srl-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13559 2023-04-25 19:23:33.933824 nornir_srl-0.0.3/setup.py
+-rw-r--r--   0        0        0    13139 2023-04-25 19:23:33.934759 nornir_srl-0.0.3/PKG-INFO
```

### Comparing `nornir_srl-0.0.2/nornir_srl/connections/helpers.py` & `nornir_srl-0.0.3/nornir_srl/connections/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,28 +68,40 @@
 
 def filter_fields(d: Dict, *fields: str) -> Dict:
     return  { 
             k:v for k,v in d.items()
                 if k in [ f.replace('_', '-') for f in fields ]
         }
     
-
 def strip_modules(d: Dict) -> Dict:
-    stripped = {}
-    for k,v in d.items():
-        k = '/'.join([e.split(':')[-1] for e in k.split('/')])
-        stripped[k] = v
-    for k, v in stripped.items():
-        if isinstance(v, dict):
-            stripped[k] = strip_modules(v)
-        elif isinstance(v, list):
-            stripped[k] = [strip_modules(d) for d in v if isinstance(d, dict)]
-        elif isinstance(v, str):
-            stripped[k] = v.split(':')[-1] if v.startswith('srl_nokia') else v
-    return stripped
+    if isinstance(d, list):
+        return [strip_modules(x) for x in d]
+    elif isinstance(d, dict):
+        return {strip_modules(k): strip_modules(v) for k, v in d.items()}
+    elif isinstance(d, str):
+        if d.startswith("srl_nokia-") and ":" in d:
+            return d[(d.index(":") + 1):]
+        return d
+    else:
+        return d
+
+
+#def strip_modules(d: Dict) -> Dict:
+#    stripped = {}
+#    for k,v in d.items():
+#        k = '/'.join([e.split(':')[-1] for e in k.split('/')])
+#        stripped[k] = copy.deepcopy(v)
+#    for k, v in stripped.items():
+#        if isinstance(v, dict):
+#            stripped[k] = strip_modules(v)
+#        elif isinstance(v, list):
+#            stripped[k] = [strip_modules(d) for d in v if isinstance(d, dict)]
+#        elif isinstance(v, str):
+#            stripped[k] = v.split(':')[-1] if v.startswith('srl_nokia') else v
+#    return stripped
 
 def get_fields_at_depth(d:Dict, depth:int) -> Dict:
     if depth == 1:
         return {k: v for k,v in d.items() if isinstance(v, (str, int, float, list))}
     return {k: get_fields_at_depth(v, depth-1) for k,v in d.items() if isinstance(v, dict)}
 
 def flatten_dict(d: Dict, depth:Optional[int]) -> Dict:
```

### Comparing `nornir_srl-0.0.2/nornir_srl/tasks/srl_config.py` & `nornir_srl-0.0.3/nornir_srl/tasks/srl_config.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.0.2/pyproject.toml` & `nornir_srl-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_srl"
-version = "0.0.2"
+version = "0.0.3"
 description = "Nornir connection plugin for SRLinux"
 authors = ["Walter De Smedt <walter.de.smedt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/wdesmedt/nornir_srl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

