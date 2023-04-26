# Comparing `tmp/neoteroi_mkdocs-1.0.1.tar.gz` & `tmp/neoteroi_mkdocs-1.0.2.tar.gz`

## Comparing `neoteroi_mkdocs-1.0.1.tar` & `neoteroi_mkdocs-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0    59157 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/coverage.xml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0    60021 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    79541 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/junit/pytest-results-3.11.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/py.typed
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/cards/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/cards/domain.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/cards/html.py
--rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/domain.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/git.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/html.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/txt.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/align.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/images.py
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/processors.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/files.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/source.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/text.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/web.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/tables/__init__.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/tables/spantable.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/oad/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/__init__.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/domain.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/timeutil.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/gantt/__init__.py
--rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/gantt/html.py
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/spantable/__init__.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/timeline/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/timeline/domain.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/timeline/html.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/LICENSE
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/README.md
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/py.typed
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/domain.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/py.typed
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/domain.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/git.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/py.typed
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/txt.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/align.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/images.py
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/py.typed
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/files.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/source.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/text.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/web.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/__init__.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/spantable.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/oad/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/oad/py.typed
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/__init__.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/domain.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/py.typed
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/timeutil.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/__init__.py
+-rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/html.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/spantable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/spantable/py.typed
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/domain.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/py.typed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/README.md
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/PKG-INFO
```

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/cards/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/cards/html.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,17 @@
                             if other.name == contributor_info["name"]
                         ),
                         None,
                     )
                     if parent:
                         parent.count += contributor.count
                         continue
+                    else:
+                        # use configured name
+                        contributor.name = contributor_info["name"]
 
                 # should contributor information be merged with another object?
                 if self._merge_contributor_by_email(
                     contributors, contributor, contributor_info
                 ):
                     # skip this item as it was merged with another one
                     continue
```

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/domain.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/domain.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/git.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/git.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/html.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/contribs/txt.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/txt.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/align.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/align.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/images.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/images.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/processors.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/processors.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/utils.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/utils.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/files.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/files.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/text.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/text.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/data/web.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/web.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/tables/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/markdown/tables/spantable.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/spantable.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/oad/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/oad/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/domain.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/domain.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/timeutil.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/timeutil.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/gantt/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/projects/gantt/html.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/spantable/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/spantable/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/timeline/__init__.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/neoteroi/mkdocs/timeline/html.py` & `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/LICENSE` & `neoteroi_mkdocs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/README.md` & `neoteroi_mkdocs-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.1/pyproject.toml` & `neoteroi_mkdocs-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -31,28 +31,22 @@
     "Jinja2",
     "rich",
 ]
 
 [tool.hatch.version]
 path = "neoteroi/mkdocs/__init__.py"
 
+[tool.hatch.build.targets.wheel]
+packages = ["neoteroi"]
+
 [tool.hatch.build.targets.sdist]
-exclude = [
-  "/.github",
-  "/docs",
-  "/deps",
-  "/styles",
-  "/tests",
-  "mkdocs-plugins.code-workspace",
-  "Makefile",
-  "CODE_OF_CONDUCT.md",
-  ".isort.cfg",
-  ".gitignore",
-  ".flake8"
-]
+exclude = ["tests"]
+
+[tool.hatch.build]
+only-packages = true
 
 [project.urls]
 "Homepage" = "https://github.com/Neoteroi/mkdocs-plugins"
 "Bug Tracker" = "https://github.com/Neoteroi/mkdocs-plugins/issues"
 
 [project.entry-points."mkdocs.plugins"]
 "neoteroi.mkdocsoad" = "neoteroi.mkdocs.oad:MkDocsOpenAPIDocumentationPlugin"
```

### Comparing `neoteroi_mkdocs-1.0.1/PKG-INFO` & `neoteroi_mkdocs-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoteroi-mkdocs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plugins for MkDocs and Python Markdown
 Project-URL: Homepage, https://github.com/Neoteroi/mkdocs-plugins
 Project-URL: Bug Tracker, https://github.com/Neoteroi/mkdocs-plugins/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: Markdown,MkDocs,OpenAPI,Swagger,documentation,extensions,plugins
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neoteroi-mkdocs Version: 1.0.1 Summary: Plugins for
+Metadata-Version: 2.1 Name: neoteroi-mkdocs Version: 1.0.2 Summary: Plugins for
 MkDocs and Python Markdown Project-URL: Homepage, https://github.com/Neoteroi/
 mkdocs-plugins Project-URL: Bug Tracker, https://github.com/Neoteroi/mkdocs-
 plugins/issues Author-email: Roberto Prevato
 prevato@gmail.com> License-File: LICENSE Keywords:
 Markdown,MkDocs,OpenAPI,Swagger,documentation,extensions,plugins Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
```

