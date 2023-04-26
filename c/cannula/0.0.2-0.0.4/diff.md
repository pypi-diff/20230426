# Comparing `tmp/cannula-0.0.2.tar.gz` & `tmp/cannula-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cannula-0.0.2.tar", last modified: Mon May 13 21:20:43 2019, max compression
+gzip compressed data, was "cannula-0.0.4.tar", last modified: Wed Apr 26 15:24:47 2023, max compression
```

## Comparing `cannula-0.0.2.tar` & `cannula-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-13 21:20:43.000000 cannula-0.0.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2019-05-13 21:20:43.000000 cannula-0.0.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2019-05-13 21:20:38.000000 cannula-0.0.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula/middleware/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1643 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/middleware/profile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      193 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/middleware/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11955 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/middleware/mocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2012 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/middleware/debug.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula/datasource/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6737 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/datasource/http.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/datasource/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14412 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/datasource/forms.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8997 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      164 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      360 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      907 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/helpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3774 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1458 2019-05-13 21:20:38.000000 cannula-0.0.2/cannula/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5575 2019-05-13 21:20:38.000000 cannula-0.0.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7562 2019-05-13 21:20:43.000000 cannula-0.0.2/PKG-INFO
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7562 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      541 2019-05-13 21:20:43.000000 cannula-0.0.2/cannula.egg-info/SOURCES.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 15:24:47.215840 cannula-0.0.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-04-26 15:24:41.000000 cannula-0.0.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6057 2023-04-26 15:24:47.215840 cannula-0.0.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5575 2023-04-26 15:24:41.000000 cannula-0.0.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 15:24:47.211840 cannula-0.0.4/cannula/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      226 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8997 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      360 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/context.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 15:24:47.215840 cannula-0.0.4/cannula/datasource/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/datasource/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6737 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/datasource/http.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1458 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 15:24:47.215840 cannula-0.0.4/cannula/middleware/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/middleware/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2012 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/middleware/debug.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11955 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/middleware/mocks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/middleware/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-04-26 15:24:41.000000 cannula-0.0.4/cannula/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 15:24:47.215840 cannula-0.0.4/cannula.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6057 2023-04-26 15:24:47.000000 cannula-0.0.4/cannula.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2023-04-26 15:24:47.000000 cannula-0.0.4/cannula.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 15:24:47.000000 cannula-0.0.4/cannula.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 15:24:47.000000 cannula-0.0.4/cannula.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-04-26 15:24:47.000000 cannula-0.0.4/cannula.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-04-26 15:24:47.000000 cannula-0.0.4/cannula.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      709 2023-04-26 15:24:47.215840 cannula-0.0.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-26 15:24:41.000000 cannula-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cannula-0.0.2/setup.cfg` & `cannula-0.0.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = cannula
 version = attr: cannula.__VERSION__
 author = Robert Myers
 author_email = robert@julython.org
 description = Async GraphQL Helper Library
 url = https://github.com/rmyers/cannula
-long_description = file: README.md, CHANGELOG.md
+long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = graphql
 license = MIT License
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3.6
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	graphql-core-next
+	graphql-core==3.2.3
 
 [flake8]
 max_line_length = 120
 
 [mypy]
 ignore_missing_imports = True
```

### Comparing `cannula-0.0.2/cannula/middleware/profile.py` & `cannula-0.0.4/cannula/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula/middleware/mocks.py` & `cannula-0.0.4/cannula/middleware/mocks.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula/middleware/debug.py` & `cannula-0.0.4/cannula/middleware/debug.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula/datasource/http.py` & `cannula-0.0.4/cannula/datasource/http.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula/api.py` & `cannula-0.0.4/cannula/api.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula/helpers.py` & `cannula-0.0.4/cannula/helpers.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula/schema.py` & `cannula-0.0.4/cannula/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     concat_ast,
 )
 
 LOG = logging.getLogger(__name__)
 QUERY_TYPE = parse("type Query { _empty: String }")
 MUTATION_TYPE = parse("type Mutation { _empty: String }")
 
-object_definition_kind = 'object_type_definition'
-object_extension_kind = 'object_type_extension'
-interface_extension_kind = 'interface_type_extension'
-input_object_extension_kind = 'input_object_type_extension'
-union_extension_kind = 'union_type_extension'
-enum_extension_kind = 'enum_type_extension'
+object_definition_kind = "object_type_definition"
+object_extension_kind = "object_type_extension"
+interface_extension_kind = "interface_type_extension"
+input_object_extension_kind = "input_object_type_extension"
+union_extension_kind = "union_type_extension"
+enum_extension_kind = "enum_type_extension"
 
 extension_kinds = [
     object_extension_kind,
     interface_extension_kind,
     input_object_extension_kind,
     union_extension_kind,
     enum_extension_kind,
@@ -42,25 +42,27 @@
 def assert_has_query_and_mutation(ast: DocumentNode) -> DocumentNode:
     """Assert that schema has query and mutation types defined.
 
     The schema is pretty much useless without them and rather than causing
     an error we'll just add in an empty one so they can be extended.
     """
     object_definitions = [
-        node.name.value for node in ast.definitions if node.kind == object_definition_kind
+        node.name.value
+        for node in ast.definitions
+        if node.kind == object_definition_kind
     ]
-    has_mutation_definition = 'Mutation' in object_definitions
-    has_query_definition = 'Query' in object_definitions
+    has_mutation_definition = "Mutation" in object_definitions
+    has_query_definition = "Query" in object_definitions
 
     if not has_mutation_definition:
-        LOG.debug('Adding default empty Mutation type')
+        LOG.debug("Adding default empty Mutation type")
         ast = concat_ast([ast, MUTATION_TYPE])
 
     if not has_query_definition:
-        LOG.debug('Adding default empty Query type')
+        LOG.debug("Adding default empty Query type")
         ast = concat_ast([ast, QUERY_TYPE])
 
     return ast
 
 
 def maybe_parse(type_def: typing.Union[str, DocumentNode]):
     if isinstance(type_def, str):
@@ -71,54 +73,53 @@
 def build_and_extend_schema(
     type_defs: typing.Union[
         typing.List[str],
         typing.List[DocumentNode],
         typing.Iterator[DocumentNode],
     ],
 ) -> GraphQLSchema:
-
     document_list = [maybe_parse(type_def) for type_def in type_defs]
 
     ast_document = concat_ast(document_list)
 
     ast_document = assert_has_query_and_mutation(ast_document)
 
     schema = build_ast_schema(ast_document)
 
     extension_ast = extract_extensions(ast_document)
 
     if extension_ast.definitions:
-        LOG.debug(f'Extending schema')
+        LOG.debug("Extending schema")
         schema = extend_schema(schema, extension_ast)
 
     return schema
 
 
 def fix_abstract_resolve_type(schema: GraphQLSchema) -> GraphQLSchema:
     # We need to provide a custom 'resolve_type' since the default
     # in method only checks for __typename if the source is a dict.
     # Python mangles the variable name if it starts with `__` so we add
     # `__typename__` attribute which is not mangled.
     # TODO(rmyers): submit PR to fix upstream?
 
     def custom_resolve_type(source, _info):
         if isinstance(source, dict):
-            return str(source.get('__typename'))
-        return getattr(source, '__typename__', None)
+            return str(source.get("__typename"))
+        return getattr(source, "__typename__", None)
 
     for _type_name, graphql_type in schema.type_map.items():
         if isinstance(graphql_type, GraphQLUnionType):
             graphql_type.resolve_type = custom_resolve_type
 
     return schema
 
 
 def load_schema(directory: str) -> typing.List[DocumentNode]:
-    assert os.path.isdir(directory), f'Directory not found: {directory}'
+    assert os.path.isdir(directory), f"Directory not found: {directory}"
     path = pathlib.Path(directory)
 
     def find_graphql_files():
-        for graph in path.glob('**/*.graphql'):
+        for graph in path.glob("**/*.graphql"):
             with open(os.path.join(directory, graph)) as graphfile:
                 yield graphfile.read()
 
     return [parse(schema) for schema in find_graphql_files()]
```

### Comparing `cannula-0.0.2/cannula/errors.py` & `cannula-0.0.4/cannula/errors.py`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/README.md` & `cannula-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cannula-0.0.2/cannula.egg-info/SOURCES.txt` & `cannula-0.0.4/cannula.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 cannula/__init__.py
 cannula/api.py
 cannula/context.py
 cannula/errors.py
@@ -11,13 +12,12 @@
 cannula.egg-info/PKG-INFO
 cannula.egg-info/SOURCES.txt
 cannula.egg-info/dependency_links.txt
 cannula.egg-info/not-zip-safe
 cannula.egg-info/requires.txt
 cannula.egg-info/top_level.txt
 cannula/datasource/__init__.py
-cannula/datasource/forms.py
 cannula/datasource/http.py
 cannula/middleware/__init__.py
 cannula/middleware/debug.py
 cannula/middleware/mocks.py
 cannula/middleware/profile.py
```

