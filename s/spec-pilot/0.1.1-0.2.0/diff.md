# Comparing `tmp/spec_pilot-0.1.1.tar.gz` & `tmp/spec_pilot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec_pilot-0.1.1.tar", last modified: Wed Apr 26 03:49:20 2023, max compression
+gzip compressed data, was "spec_pilot-0.2.0.tar", last modified: Wed Apr 26 16:41:34 2023, max compression
```

## Comparing `spec_pilot-0.1.1.tar` & `spec_pilot-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:49:20.567332 spec_pilot-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-26 03:49:20.567332 spec_pilot-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 03:49:20.567332 spec_pilot-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:49:20.567332 spec_pilot-0.1.1/spec_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-26 03:49:20.000000 spec_pilot-0.1.1/spec_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-26 03:49:20.000000 spec_pilot-0.1.1/spec_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:49:20.000000 spec_pilot-0.1.1/spec_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 03:49:20.000000 spec_pilot-0.1.1/spec_pilot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 03:49:20.000000 spec_pilot-0.1.1/spec_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 03:49:20.000000 spec_pilot-0.1.1/spec_pilot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:49:20.567332 spec_pilot-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/src/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/src/spec_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/src/spec_pilot.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-26 03:49:09.000000 spec_pilot-0.1.1/src/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/spec_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 16:41:34.000000 spec_pilot-0.2.0/spec_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:41:34.427957 spec_pilot-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/spec_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/spec_pilot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 16:41:14.000000 spec_pilot-0.2.0/src/validator.py
```

### Comparing `spec_pilot-0.1.1/LICENSE` & `spec_pilot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spec_pilot-0.1.1/setup.py` & `spec_pilot-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         os.system("python -m spacy download en_core_web_sm")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="spec_pilot",
-    version="0.1.1",
+    version="0.2.0",
     author="jmfwolf",
     author_email="jmfwolf@hacksomniac.com",
     description="A tool to generate OpenAPI specifications using natural language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jmfwolf/spec-pilot",
     packages=find_packages(),
```

### Comparing `spec_pilot-0.1.1/src/generator.py` & `spec_pilot-0.2.0/src/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,73 +1,86 @@
 import pystache
 import os
 import yaml
 
+
 def init_project(project_name):
     if project_name == "":
         project_name = input("Enter project name: ")
     os.mkdir(project_name)
     os.mkdir(os.path.join(project_name, "schemas"))
     os.mkdir(os.path.join(project_name, "paths"))
     os.mkdir(os.path.join(project_name, "parameters"))
     os.mkdir(os.path.join(project_name, "responses"))
     os.mkdir(os.path.join(project_name, "tags"))
     os.mkdir(os.path.join(project_name, "servers"))
     os.mkdir(os.path.join(project_name, "info"))
-    #openapi_file_path = os.path.join(project_name, "openapi.yml")
-    #open(openapi_file_path, "w").close()
+    # openapi_file_path = os.path.join(project_name, "openapi.yml")
+    # open(openapi_file_path, "w").close()
+
 
 def render_template(template_file, context, output_file):
     with open(template_file, 'r') as f:
         template = f.read()
     rendered = pystache.render(template, context)
 
     with open(output_file, 'w') as f:
         f.write(rendered)
 
+
 def check_version(version):
     if version != 'v2.0' and version != 'v3.0':
         raise ValueError("Version must be either 'v2.0' or 'v3.0'")
 
+
 def generate_schema(context, output_file='schema.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/schema.mustache", context, output_file)
 
+
 def generate_path_object(context, output_file='path_object.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/path_object.mustache", context, output_file)
 
+
 def generate_parameter(context, output_file='parameter.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/parameter.mustache", context, output_file)
 
+
 def generate_info(context, output_file='info.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/info.mustache", context, output_file)
 
+
 def generate_header(context, output_file='header.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/header.mustache", context, output_file)
 
+
 def generate_media_type(context, output_file='media_type.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/media_type.mustache", context, output_file)
 
+
 def generate_response(context, output_file='response.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/response.mustache", context, output_file)
 
+
 def generate_tag(context, output_file='tag.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/tag.mustache", context, output_file)
 
+
 def generate_server(context, output_file='server.yaml', version='v2.0'):
     check_version(version)
     render_template(f"templates/{version}/server.mustache", context, output_file)
-    
+
+
 def generate_openapi_spec(project_name, version='v3.0', output_file='openapi_spec.yaml'):
     check_version(version)
 
     openapi_spec = {
         'openapi': '3.0.0' if version == 'v3.0' else '2.0',
         'info': {},
         'paths': {},
@@ -109,25 +122,28 @@
                     openapi_spec['info']['contact'] = content
                 elif subdir.endswith("licenses"):
                     openapi_spec['info']['license'] = content
 
     with open(os.path.join(project_name, output_file), 'w') as f:
         yaml.dump(openapi_spec, f, sort_keys=False, default_flow_style=False)
 
+
 def demo():
     # Example usage
     project_name = "demo"
     init_project(project_name)
     schema_context = {
         'schemaName': 'Book',
         'type': 'object',
         'properties': [
-            {'name': 'title', 'type': 'string', 'description': 'The title of the book', 'example': 'The Catcher in the Rye'},
+            {'name': 'title', 'type': 'string', 'description': 'The title of the book',
+             'example': 'The Catcher in the Rye'},
             {'name': 'author', 'type': 'string', 'description': 'The author of the book', 'example': 'J.D. Salinger'},
-            {'name': 'publication_date', 'type': 'string', 'description': 'The publication date of the book', 'example': '1951-07-16', 'format': 'date'}
+            {'name': 'publication_date', 'type': 'string', 'description': 'The publication date of the book',
+             'example': '1951-07-16', 'format': 'date'}
         ],
         'required': ['title', 'author'],
         'description': 'A book in the library.'
     }
 
     generate_schema(schema_context, os.path.join(f"{project_name}/schemas", 'book.yaml'), version='v3.0')
 
@@ -158,15 +174,16 @@
         'responses': [
             {
                 'statusCode': '201',
                 'description': 'Book successfully created',
                 'mediaType': 'application/json',
                 'schemaName': 'book',
                 'schemaFile': '#/components/schemas/book',
-                'example': {'title': 'The Catcher in the Rye', 'author': 'J.D. Salinger', 'publication_date': '1951-07-16'}
+                'example': {'title': 'The Catcher in the Rye', 'author': 'J.D. Salinger',
+                            'publication_date': '1951-07-16'}
             }
         ]
     }
     generate_path_object(path_object_context, os.path.join(f"{project_name}/paths", 'books.yaml'), version='v3.0')
 
     parameter_context = {
         'parameterName': 'bookId',
@@ -219,8 +236,7 @@
         'description': 'Operations related to books'
     }
 
     generate_tag(tags_context, os.path.join(f"{project_name}/tags", 'books.yaml'), version='v3.0')
 
     generate_info(info_context, os.path.join(f"{project_name}/info", 'info.yaml'), version='v3.0')
     generate_openapi_spec("demo")
-
```

### Comparing `spec_pilot-0.1.1/src/spec_parser.py` & `spec_pilot-0.2.0/src/spec_parser.py`

 * *Files identical despite different names*

### Comparing `spec_pilot-0.1.1/src/spec_pilot.py` & `spec_pilot-0.2.0/src/spec_pilot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 import argparse
 import os
 import sys
 import json
-from generator import init_project, generate_openapi_spec, demo
+from generator import init_project, generate_openapi_spec, demo, render_template
 from spec_parser import process_natural_language_input
 from validator import vacuum
 
+
 def main():
     parser = argparse.ArgumentParser(description="Spec-Pilot: Generate OpenAPI specifications using natural language")
     parser.add_argument("--init", metavar="project_name",
                         help="Initialize a new OpenAPI project with the specified project name")
-    parser.add_argument("--generate", metavar="project_name",
+    parser.add_argument("-g", "--generate", metavar="project_name",
                         help="Generate the OpenAPI specification for the specified project")
-    parser.add_argument("--demo", help="Generate the OpenAPI specification for the specified project", action="store_true")
+    parser.add_argument("--demo", help="Demonstration project",
+                        action="store_true")
     parser.add_argument("--nlp", metavar="input_text",
                         help="Process a natural language input to modify the OpenAPI specification")
-    parser.add_argument("--validate", metavar="spec_file",
+    parser.add_argument("-v", "--validate", metavar="spec_file",
                         help="Validate the provided OpenAPI specification file")
+    parser.add_argument("-c", "--create", nargs=3, metavar=("template", "asset_name", "output_path"),
+                        help="Create a new OpenAPI asset from the specified template with the given asset_name and save it to the output_path")
 
     args = parser.parse_args()
 
     if args.init:
         init_project(args.init)
     elif args.generate:
         generate_openapi_spec(args.generate)
     elif args.demo:
         demo()
+    elif args.create:
+        template, asset_name, output_path = args.create
+        render_template(template, asset_name, output_path)
     elif args.nlp:
         if not os.path.exists("openapi_spec.json"):
             sys.exit("Error: openapi_spec.json not found. Please provide an existing OpenAPI specification to modify.")
-        
+
         with open("openapi_spec.json", "r") as f:
             openapi_spec = json.load(f)
-        
+
         modified_openapi_spec = process_natural_language_input(args.nlp, openapi_spec)
-        
+
         if modified_openapi_spec:
             with open("openapi_spec.json", "w") as f:
                 json.dump(modified_openapi_spec, f, indent=2)
         else:
             print("Error: Unable to process the provided natural language input.")
     elif args.validate:
         vacuum(["validate", args.validate])
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `spec_pilot-0.1.1/src/validator.py` & `spec_pilot-0.2.0/src/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import subprocess
 import sys
 
+
 def check_vacuum():
     try:
         subprocess.check_call(["which", "vacuum"])
         return True
     except subprocess.CalledProcessError:
         return False
 
+
 def install_vacuum():
     try:
         subprocess.check_call(["/bin/sh", "-c", "curl -fsSL https://quobix.com/scripts/install_vacuum.sh | sh "])
     except subprocess.CalledProcessError:
         sys.exit("Failed to install vacuum")
 
+
 def vacuum(args):
     try:
         subprocess.check_call(["vacuum"] + args)
     except subprocess.CalledProcessError as e:
         sys.exit("Error running vacuum: " + str(e))
 
+
 if not check_vacuum():
     install_vacuum()
 
+
 def main():
     vacuum(["help"])
 
+
 if __name__ == "__main__":
     main()
```

