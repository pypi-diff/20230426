# Comparing `tmp/llmbda_fastapi-0.0.4.tar.gz` & `tmp/llmbda_fastapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmbda_fastapi-0.0.4.tar", last modified: Wed Apr 26 10:02:51 2023, max compression
+gzip compressed data, was "llmbda_fastapi-0.0.5.tar", last modified: Wed Apr 26 11:15:57 2023, max compression
```

## Comparing `llmbda_fastapi-0.0.4.tar` & `llmbda_fastapi-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:02:51.495324 llmbda_fastapi-0.0.4/
--rw-rw-rw-   0        0        0     2537 2023-04-26 10:02:51.495324 llmbda_fastapi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2335 2023-04-24 08:52:38.000000 llmbda_fastapi-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 10:02:51.478784 llmbda_fastapi-0.0.4/llmbda_fastapi/
--rw-rw-rw-   0        0        0      143 2023-04-26 10:02:45.000000 llmbda_fastapi-0.0.4/llmbda_fastapi/__init__.py
--rw-rw-rw-   0        0        0     3978 2023-04-24 08:41:21.000000 llmbda_fastapi-0.0.4/llmbda_fastapi/chains.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:02:51.494320 llmbda_fastapi-0.0.4/llmbda_fastapi/frontend/
--rw-rw-rw-   0        0        0       54 2023-04-24 10:31:44.000000 llmbda_fastapi-0.0.4/llmbda_fastapi/frontend/__init__.py
--rw-rw-rw-   0        0        0     5555 2023-04-24 06:58:04.000000 llmbda_fastapi-0.0.4/llmbda_fastapi/frontend/input_components.py
--rw-rw-rw-   0        0        0     3184 2023-04-26 09:57:55.000000 llmbda_fastapi-0.0.4/llmbda_fastapi/transformations.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:02:51.492320 llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/
--rw-rw-rw-   0        0        0     2537 2023-04-26 10:02:51.000000 llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-26 10:02:51.000000 llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:02:51.000000 llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-04-26 10:02:51.000000 llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-26 10:02:51.000000 llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:02:51.496322 llmbda_fastapi-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-24 11:12:55.000000 llmbda_fastapi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.526163 llmbda_fastapi-0.0.5/
+-rw-rw-rw-   0        0        0     2537 2023-04-26 11:15:57.526163 llmbda_fastapi-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2335 2023-04-24 08:52:38.000000 llmbda_fastapi-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.511614 llmbda_fastapi-0.0.5/llmbda_fastapi/
+-rw-rw-rw-   0        0        0      143 2023-04-26 11:15:47.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/__init__.py
+-rw-rw-rw-   0        0        0     3978 2023-04-24 08:41:21.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/chains.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.525163 llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/
+-rw-rw-rw-   0        0        0       54 2023-04-24 10:31:44.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/__init__.py
+-rw-rw-rw-   0        0        0     5555 2023-04-24 06:58:04.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/input_components.py
+-rw-rw-rw-   0        0        0     3730 2023-04-26 11:13:25.000000 llmbda_fastapi-0.0.5/llmbda_fastapi/transformations.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:15:57.521613 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     2537 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-26 11:15:57.000000 llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 11:15:57.527167 llmbda_fastapi-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-24 11:12:55.000000 llmbda_fastapi-0.0.5/setup.py
```

### Comparing `llmbda_fastapi-0.0.4/PKG-INFO` & `llmbda_fastapi-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmbda_fastapi
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 
 # Llmbda FastAPI
```

### Comparing `llmbda_fastapi-0.0.4/README.md` & `llmbda_fastapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.4/llmbda_fastapi/chains.py` & `llmbda_fastapi-0.0.5/llmbda_fastapi/chains.py`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.4/llmbda_fastapi/frontend/input_components.py` & `llmbda_fastapi-0.0.5/llmbda_fastapi/frontend/input_components.py`

 * *Files identical despite different names*

### Comparing `llmbda_fastapi-0.0.4/llmbda_fastapi/transformations.py` & `llmbda_fastapi-0.0.5/llmbda_fastapi/transformations.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,45 @@
     id_list = []
     for route in api_routes:
         if isinstance(route, APIRoute):
             id_list.append(route.unique_id + id_suffix)
             input_schema = {}
             if route.body_field:
                 input_schema = json.loads(route.body_field.type_.schema_json())
-                        
+
+            for k, v in input_schema["properties"].items():
+                if "title" in v:
+                    if "metadata" not in v:
+                        v['metadata'] = {}
+                    v['metadata']['title'] = v['title']
+                    del v['title']
+                if "description" in v:
+                    if "metadata" not in v:
+                        v['metadata'] = {}
+                    v['metadata']['description'] = v['description']
+                    del v['description']
+
             output_schema = {}
             if route.response_field:
                 output_schema = json.loads(route.response_field.type_.schema_json())
 
             if url.endswith("/"):
-                full_path = url + route.path
-            else:
-                full_path = url + "/" + route.path
+                url = url[:-1]
+            route_path = route.path
+            if route_path.startswith("/"):
+                route_path = route_path[1:]
+            full_path = url + "/" + route_path
 
             tfs_list.append({
                 "_id" : route.unique_id + id_suffix,
                 "transformation_id" : route.unique_id + id_suffix,
                 "name" : route.summary if route.summary else route.name,
                 "description" : route.description,
                 "studio_api_path" : full_path,
                 "execution_type" : "studio-api",
-                "tags" : route.tags,
                 "input_schema" : input_schema,
                 "output_schema" : output_schema,
             })
     return tfs_list, id_list
 
 def list_transformations():
     url = f"https://api-{RELEVANCE_AUTH_TOKEN.split(':')[2]}.stack.tryrelevance.com"
```

### Comparing `llmbda_fastapi-0.0.4/llmbda_fastapi.egg-info/PKG-INFO` & `llmbda_fastapi-0.0.5/llmbda_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmbda-fastapi
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 
 # Llmbda FastAPI
```

### Comparing `llmbda_fastapi-0.0.4/setup.py` & `llmbda_fastapi-0.0.5/setup.py`

 * *Files identical despite different names*

