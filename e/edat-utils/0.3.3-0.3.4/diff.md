# Comparing `tmp/edat_utils-0.3.3.tar.gz` & `tmp/edat_utils-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edat_utils-0.3.3.tar", last modified: Thu Apr 13 19:38:02 2023, max compression
+gzip compressed data, was "edat_utils-0.3.4.tar", last modified: Wed Apr 26 18:27:14 2023, max compression
```

## Comparing `edat_utils-0.3.3.tar` & `edat_utils-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:38:02.114336 edat_utils-0.3.3/
--rw-rw-rw-   0        0        0      518 2023-04-13 19:38:02.113324 edat_utils-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       94 2023-04-13 12:22:29.000000 edat_utils-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 19:38:02.105329 edat_utils-0.3.3/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.3.3/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1082 2023-04-13 19:37:50.000000 edat_utils-0.3.3/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.3.3/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1221 2023-04-13 17:37:40.000000 edat_utils-0.3.3/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      967 2023-04-12 14:54:05.000000 edat_utils-0.3.3/edat_utils/schema.py
--rw-rw-rw-   0        0        0      567 2023-04-13 17:34:08.000000 edat_utils-0.3.3/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:38:02.111325 edat_utils-0.3.3/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      518 2023-04-13 19:38:01.000000 edat_utils-0.3.3/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-13 19:38:02.000000 edat_utils-0.3.3/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:38:01.000000 edat_utils-0.3.3/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-13 19:38:01.000000 edat_utils-0.3.3/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 19:38:01.000000 edat_utils-0.3.3/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 19:38:02.115327 edat_utils-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-04-13 19:37:56.000000 edat_utils-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:27:14.572835 edat_utils-0.3.4/
+-rw-rw-rw-   0        0        0      487 2023-04-26 18:27:14.571835 edat_utils-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-26 18:24:30.000000 edat_utils-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 18:27:14.562842 edat_utils-0.3.4/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.3.4/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-04-13 20:04:16.000000 edat_utils-0.3.4/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.3.4/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1221 2023-04-13 17:37:40.000000 edat_utils-0.3.4/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      967 2023-04-12 14:54:05.000000 edat_utils-0.3.4/edat_utils/schema.py
+-rw-rw-rw-   0        0        0      785 2023-04-13 20:03:38.000000 edat_utils-0.3.4/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:27:14.570836 edat_utils-0.3.4/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      487 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:27:14.572835 edat_utils-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-04-13 20:04:23.000000 edat_utils-0.3.4/setup.py
```

### Comparing `edat_utils-0.3.3/edat_utils/generic_controller.py` & `edat_utils-0.3.4/edat_utils/generic_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 
 T = TypeVar("T")
 
 
 class GenericController(Generic[T]):
 
     def get(self, info:Info, filter: EdatFilter, pagination: EdatPagination = None, orders: List[EdatOrder] = None) -> EdatPaginationWindow[T]:             
-        print("###############")
-        print(info)
-        print("###############")
-        table = ''
+        table = EdatUtils.get_table_name(info)
         grouped = True if isinstance(T, EdatGrouped) else False
         fields = EdatUtils.get_fields(info)
         user = EdatUtils.get_user(info)
         query = EdatQueryBuilder.build_query(table, filter, fields, pagination, orders, grouped)
+        print(query)
         rows = EdatQueriyRunner.list(query, user)
         return EdatPaginationWindow(items=rows, total_items_count=len(rows))
```

### Comparing `edat_utils-0.3.3/edat_utils/query_builder.py` & `edat_utils-0.3.4/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.3/edat_utils/query_runner.py` & `edat_utils-0.3.4/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.3/edat_utils/schema.py` & `edat_utils-0.3.4/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.3/edat_utils/utils.py` & `edat_utils-0.3.4/edat_utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from strawberry.types import Info
+import re
 
 EDAT_USER = 'X-EDAT-USER'
 
 
 class EdatUtils:
     @staticmethod
     def get_fields(info: Info):
@@ -12,8 +13,12 @@
     
     @staticmethod
     def get_user(info: Info):
         request = info.context['request']
         user =  None
         if EDAT_USER in request.headers:
             user = request.headers[EDAT_USER]
-        return user
+        return user
+    
+    def get_table_name(info: Info):
+        name = list(info.return_type.__dict__['_type_definition'].type_var_map.values())[0].__name__
+        return re.sub(r'(?<!^)(?=[A-Z])', '_', name).lower()
```

### Comparing `edat_utils-0.3.3/setup.py` & `edat_utils-0.3.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.3.3",
+    version="0.3.4",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

