# Comparing `tmp/bp_data_fabric-0.0.9.tar.gz` & `tmp/bp_data_fabric-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-0.0.9.tar", last modified: Fri Apr 21 06:23:51 2023, max compression
+gzip compressed data, was "bp_data_fabric-1.0.0.tar", last modified: Wed Apr 26 08:41:51 2023, max compression
```

## Comparing `bp_data_fabric-0.0.9.tar` & `bp_data_fabric-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:23:51.243447 bp_data_fabric-0.0.9/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.9/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:23:51.243108 bp_data_fabric-0.0.9/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.9/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:23:51.241689 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-21 06:23:51.000000 bp_data_fabric-0.0.9/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 06:23:51.242529 bp_data_fabric-0.0.9/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      920 2023-04-20 07:20:57.000000 bp_data_fabric-0.0.9/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2184 2023-04-20 07:22:51.000000 bp_data_fabric-0.0.9/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 06:23:51.243652 bp_data_fabric-0.0.9/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      712 2023-04-21 06:23:36.000000 bp_data_fabric-0.0.9/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:41:51.472012 bp_data_fabric-1.0.0/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.0/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-26 08:41:51.471571 bp_data_fabric-1.0.0/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.0/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:41:51.470043 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:41:51.470967 bp_data_fabric-1.0.0/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1040 2023-04-24 07:05:06.000000 bp_data_fabric-1.0.0/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2476 2023-04-24 09:14:37.000000 bp_data_fabric-1.0.0/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-26 08:41:51.472157 bp_data_fabric-1.0.0/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      712 2023-04-26 08:41:39.000000 bp_data_fabric-1.0.0/setup.py
```

### Comparing `bp_data_fabric-0.0.9/LICENSE` & `bp_data_fabric-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.9/data_fabric/components.py` & `bp_data_fabric-1.0.0/data_fabric/components.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,43 +13,51 @@
         tables: List[dict] = [],
         columns: List[dict] = [],
         data={},
         on_database_change=None,
         on_table_change=None,
         on_generate_query=None,
         on_copy_query=None,
-        on_execute=None
+        on_execute=None,
+        show_data_grid=True,
+        show_charts=True,
     ):
     
 
+    with open('style.css') as f:
+        st.markdown(f'<style>{f.read()}</style>', unsafe_allow_html=True)
+
     render_query_tool(
         query=query,
         title=query_tool_title,
         databases=databases,
         tables=tables,
         columns=columns,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
     )
 
     if query != "":
       st.button("Execute", on_click=on_execute)
+    st.write("")
+    st.write("")
+    if show_data_grid == True:
+        render_data_grid(
+            title=data_grid_title,
+            rows=data.get("rows", []),
+            columns=data.get("columns", []),
+        )
 
-    render_data_grid(
-        title=data_grid_title,
-        rows=data.get("rows", []),
-        columns=data.get("columns", []),
-    )
-
-    render_data_visualizer(
-        title=data_visualization_title,
-        rows=data.get("rows", []),
-    )
+    if show_charts == True:
+        render_data_visualizer(
+            title=data_visualization_title,
+            rows=data.get("rows", []),
+        )
 
 def render_query_tool(
         query: str = "",
         title: str = "",
         databases: List[str] = [],
         tables: List[dict] = [],
         columns: List[dict] = [],
```

### Comparing `bp_data_fabric-0.0.9/setup.py` & `bp_data_fabric-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="0.0.9",
+    version="1.0.0",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

