# Comparing `tmp/ogc_na-0.1.tar.gz` & `tmp/ogc_na-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.1.tar", last modified: Tue Apr 25 11:12:10 2023, max compression
+gzip compressed data, was "ogc_na-0.1.1.tar", last modified: Wed Apr 26 07:04:37 2023, max compression
```

## Comparing `ogc_na-0.1.tar` & `ogc_na-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.092045 ogc_na-0.1/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     5990 2022-12-21 12:24:35.000000 ogc_na-0.1/.gitignore
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)       45 2022-11-07 12:37:19.000000 ogc_na-0.1/MANIFEST.in
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     2635 2023-04-25 11:12:10.092045 ogc_na-0.1/PKG-INFO
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     1879 2023-02-27 10:42:14.000000 ogc_na-0.1/README.md
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.088045 ogc_na-0.1/docs/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     6634 2023-04-04 12:02:11.000000 ogc_na-0.1/docs/examples.md
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      936 2022-12-21 12:24:35.000000 ogc_na-0.1/docs/gen_ref_pages.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     1461 2023-02-27 10:42:14.000000 ogc_na-0.1/docs/index.md
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     7225 2023-01-31 11:09:02.000000 ogc_na-0.1/docs/tutorials.md
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      522 2022-12-21 12:24:35.000000 ogc_na-0.1/mkdocs.yml
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.088045 ogc_na-0.1/ogc/
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.092045 ogc_na-0.1/ogc/na/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      464 2022-12-21 12:24:35.000000 ogc_na-0.1/ogc/na/__init__.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)    17949 2023-04-25 10:37:48.000000 ogc_na-0.1/ogc/na/annotate_schema.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)    12443 2023-04-25 10:37:54.000000 ogc_na-0.1/ogc/na/domain_config.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     3191 2023-04-25 10:38:00.000000 ogc_na-0.1/ogc/na/download.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)    30863 2023-04-25 10:38:06.000000 ogc_na-0.1/ogc/na/ingest_json.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)    14444 2023-04-25 10:38:11.000000 ogc_na-0.1/ogc/na/profile.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     5446 2023-04-25 10:45:48.000000 ogc_na-0.1/ogc/na/provenance.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)    17174 2023-04-25 10:38:23.000000 ogc_na-0.1/ogc/na/update_vocabs.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     6216 2023-04-25 10:38:28.000000 ogc_na-0.1/ogc/na/util.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     3535 2023-04-25 10:38:32.000000 ogc_na-0.1/ogc/na/validation.py
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.092045 ogc_na-0.1/ogc_na.egg-info/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     2635 2023-04-25 11:12:10.000000 ogc_na-0.1/ogc_na.egg-info/PKG-INFO
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      766 2023-04-25 11:12:10.000000 ogc_na-0.1/ogc_na.egg-info/SOURCES.txt
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)        1 2023-04-25 11:12:10.000000 ogc_na-0.1/ogc_na.egg-info/dependency_links.txt
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      353 2023-04-25 11:12:10.000000 ogc_na-0.1/ogc_na.egg-info/requires.txt
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)        4 2023-04-25 11:12:10.000000 ogc_na-0.1/ogc_na.egg-info/top_level.txt
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     1505 2023-04-25 11:01:31.000000 ogc_na-0.1/pyproject.toml
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.092045 ogc_na-0.1/rdf/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      265 2023-04-04 12:02:11.000000 ogc_na-0.1/rdf/catalog-v001.xml
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     2945 2023-04-04 12:02:11.000000 ogc_na-0.1/rdf/domaincfg.vocab.ttl
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      128 2023-01-30 12:20:21.000000 ogc_na-0.1/requirements.txt
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)       38 2023-04-25 11:12:10.092045 ogc_na-0.1/setup.cfg
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)       93 2022-11-07 12:37:19.000000 ogc_na-0.1/setup.py
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.092045 ogc_na-0.1/test/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)        0 2022-11-07 12:37:19.000000 ogc_na-0.1/test/__init__.py
-drwxrwxr-x   0 alx5000   (1000) alx5000   (1000)        0 2023-04-25 11:12:10.092045 ogc_na-0.1/test/data/
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)        0 2023-04-04 12:02:11.000000 ogc_na-0.1/test/data/empty.ttl
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      443 2023-04-04 12:02:11.000000 ogc_na-0.1/test/data/profile_tree.ttl
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      354 2023-04-04 12:02:11.000000 ogc_na-0.1/test/data/profile_tree_cyclic.ttl
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      871 2023-04-04 12:02:11.000000 ogc_na-0.1/test/data/uplift_context_valid.yml
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     1972 2023-04-24 11:32:21.000000 ogc_na-0.1/test/test_annotate_schema.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)      536 2023-04-04 12:02:11.000000 ogc_na-0.1/test/test_ingest_json.py
--rw-rw-r--   0 alx5000   (1000) alx5000   (1000)     2150 2023-04-04 12:02:11.000000 ogc_na-0.1/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.460713 ogc_na-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 07:04:25.000000 ogc_na-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-26 07:04:25.000000 ogc_na-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 07:04:25.000000 ogc_na-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 07:04:37.460713 ogc_na-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-26 07:04:25.000000 ogc_na-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-26 07:04:25.000000 ogc_na-0.1.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-26 07:04:25.000000 ogc_na-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 07:04:25.000000 ogc_na-0.1.1/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-26 07:04:25.000000 ogc_na-0.1.1/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 07:04:25.000000 ogc_na-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:04:37.460713 ogc_na-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 07:04:25.000000 ogc_na-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.460713 ogc_na-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.460713 ogc_na-0.1.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/test_profile.py
```

### Comparing `ogc_na-0.1/.gitignore` & `ogc_na-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/PKG-INFO` & `ogc_na-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.1
+Version: 0.1.1
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1/README.md` & `ogc_na-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/docs/examples.md` & `ogc_na-0.1.1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/docs/gen_ref_pages.py` & `ogc_na-0.1.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/docs/index.md` & `ogc_na-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/docs/tutorials.md` & `ogc_na-0.1.1/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/mkdocs.yml` & `ogc_na-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/annotate_schema.py` & `ogc_na-0.1.1/ogc/na/annotate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,16 @@
             own_context = compact_context
 
         self._parsed_schemas[fn or url] = own_context
         return own_context
 
 
 def dump_annotated_schemas(annotator: SchemaAnnotator, subdir: Path | str = 'annotated',
-                           root_dir: Path | str | None = None) -> list[Path]:
+                           root_dir: Path | str | None = None,
+                           output_fn_transform: Callable[[Path], Path] | None = None) -> list[Path]:
     """
     Creates a "mirror" directory (named `annotated` by default) with the resulting
     schemas annotated by a `SchemaAnnotator`.
 
     :param annotator: a `SchemaAnnotator` with the annotated schemas to read
     :param subdir: a name for the mirror directory
     :param root_dir: root directory for computing relative paths to schemas
@@ -467,14 +468,16 @@
         if isinstance(path, Path):
             outputfn = path.resolve().relative_to(wd)
         else:
             parsed = urlparse(str(path))
             outputfn = parsed.path
 
         outputfn = subdir / outputfn
+        if output_fn_transform:
+            outputfn = output_fn_transform(outputfn)
         outputfn.parent.mkdir(parents=True, exist_ok=True)
 
         with open(outputfn, 'w') as f:
             if schema.is_json:
                 json.dump(schema.schema, f, indent=2)
             else:
                 yaml.dump(schema.schema, f, sort_keys=False)
```

### Comparing `ogc_na-0.1/ogc/na/domain_config.py` & `ogc_na-0.1.1/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/download.py` & `ogc_na-0.1.1/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/ingest_json.py` & `ogc_na-0.1.1/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/profile.py` & `ogc_na-0.1.1/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/provenance.py` & `ogc_na-0.1.1/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/update_vocabs.py` & `ogc_na-0.1.1/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/util.py` & `ogc_na-0.1.1/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc/na/validation.py` & `ogc_na-0.1.1/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.1.1/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.1
+Version: 0.1.1
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.1.1/ogc_na.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 MANIFEST.in
 README.md
 mkdocs.yml
 pyproject.toml
 requirements.txt
 setup.py
+.github/workflows/python-publish.yml
 docs/examples.md
 docs/gen_ref_pages.py
 docs/index.md
 docs/tutorials.md
 ogc/na/__init__.py
 ogc/na/annotate_schema.py
 ogc/na/domain_config.py
```

### Comparing `ogc_na-0.1/pyproject.toml` & `ogc_na-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/rdf/domaincfg.vocab.ttl` & `ogc_na-0.1.1/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/test/data/uplift_context_valid.yml` & `ogc_na-0.1.1/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/test/test_annotate_schema.py` & `ogc_na-0.1.1/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/test/test_ingest_json.py` & `ogc_na-0.1.1/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1/test/test_profile.py` & `ogc_na-0.1.1/test/test_profile.py`

 * *Files identical despite different names*

