# Comparing `tmp/graal-0.4.5rc2.tar.gz` & `tmp/graal-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graal-0.4.5rc2.tar", max compression
+gzip compressed data, was "graal-0.4.6.tar", max compression
```

## Comparing `graal-0.4.5rc2.tar` & `graal-0.4.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      240 2023-04-21 09:54:58.442339 graal-0.4.5rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-21 09:54:58.442339 graal-0.4.5rc2/LICENSE
--rw-r--r--   0        0        0     1425 2023-04-21 09:54:58.442339 graal-0.4.5rc2/NEWS
--rw-r--r--   0        0        0    13761 2023-04-21 09:54:58.442339 graal-0.4.5rc2/README.md
--rw-r--r--   0        0        0      876 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/__init__.py
--rw-r--r--   0        0        0       91 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/_version.py
--rw-r--r--   0        0        0      876 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/__init__.py
--rw-r--r--   0        0        0      883 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/analyzer.py
--rw-r--r--   0        0        0     4594 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/bandit.py
--rw-r--r--   0        0        0     4543 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/cloc.py
--rw-r--r--   0        0        0     2479 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/flake8.py
--rw-r--r--   0        0        0     2317 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/jadolint.py
--rw-r--r--   0        0        0     2243 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/linguist.py
--rw-r--r--   0        0        0     5383 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/lizard.py
--rw-r--r--   0        0        0     2360 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/nomos.py
--rw-r--r--   0        0        0     2852 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/pylint.py
--rw-r--r--   0        0        0     2620 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/reverse.py
--rw-r--r--   0        0        0     4563 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/scancode.py
--rw-r--r--   0        0        0     4504 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/analyzers/scc.py
--rw-r--r--   0        0        0    11691 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/cocom.py
--rw-r--r--   0        0        0     8463 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/codep.py
--rw-r--r--   0        0        0     6344 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/colang.py
--rw-r--r--   0        0        0     8182 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/colic.py
--rw-r--r--   0        0        0     9186 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/coqua.py
--rw-r--r--   0        0        0     5662 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/backends/core/covuln.py
--rwxr-xr-x   0        0        0     4425 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/bin/graal.py
--rw-r--r--   0        0        0    23643 2023-04-21 09:54:58.442339 graal-0.4.5rc2/graal/graal.py
--rw-r--r--   0        0        0     1584 2023-04-21 09:54:58.446339 graal-0.4.5rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/base_analyzer.py
--rw-r--r--   0        0        0     2056 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/base_repo.py
--rw-r--r--   0        0        0     1575 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/data/Dockerfile
--rw-r--r--   0        0        0   132358 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/data/graaltest-dockerfile.zip
--rw-r--r--   0        0        0   126651 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/data/graaltest.zip
--rw-r--r--   0        0        0     4482 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/data/sample_code.py
--rwxr-xr-x   0        0        0     1174 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/run_tests.py
--rw-r--r--   0        0        0     1222 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_analyzer.py
--rw-r--r--   0        0        0     5650 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_bandit.py
--rw-r--r--   0        0        0     3341 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_cloc.py
--rw-r--r--   0        0        0    14713 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_cocom.py
--rw-r--r--   0        0        0    14625 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_codep.py
--rw-r--r--   0        0        0     8707 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_colang.py
--rw-r--r--   0        0        0    13445 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_colic.py
--rw-r--r--   0        0        0    20057 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_coqua.py
--rw-r--r--   0        0        0     7611 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_covuln.py
--rw-r--r--   0        0        0     2846 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_flake8.py
--rw-r--r--   0        0        0    29236 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_graal.py
--rw-r--r--   0        0        0     6391 2023-04-21 09:54:58.446339 graal-0.4.5rc2/tests/test_jadolint.py
--rw-r--r--   0        0        0     2456 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_linguist.py
--rw-r--r--   0        0        0     4980 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_lizard.py
--rw-r--r--   0        0        0     2321 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_nomos.py
--rw-r--r--   0        0        0     3181 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_pylint.py
--rw-r--r--   0        0        0     2481 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_reverse.py
--rw-r--r--   0        0        0     3538 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_scancode.py
--rw-r--r--   0        0        0     4022 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/test_scc.py
--rw-r--r--   0        0        0     1191 2023-04-21 09:54:58.450339 graal-0.4.5rc2/tests/utils.py
--rw-r--r--   0        0        0    15214 1970-01-01 00:00:00.000000 graal-0.4.5rc2/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-04-26 14:46:33.918412 graal-0.4.6/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-26 14:46:33.918412 graal-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1677 2023-04-26 14:46:33.918412 graal-0.4.6/NEWS
+-rw-r--r--   0        0        0    13761 2023-04-26 14:46:33.918412 graal-0.4.6/README.md
+-rw-r--r--   0        0        0      876 2023-04-26 14:46:33.918412 graal-0.4.6/graal/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-26 14:46:33.918412 graal-0.4.6/graal/_version.py
+-rw-r--r--   0        0        0      876 2023-04-26 14:46:33.918412 graal-0.4.6/graal/backends/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-26 14:46:33.918412 graal-0.4.6/graal/backends/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/analyzer.py
+-rw-r--r--   0        0        0     4594 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/bandit.py
+-rw-r--r--   0        0        0     4543 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/cloc.py
+-rw-r--r--   0        0        0     2479 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/flake8.py
+-rw-r--r--   0        0        0     2317 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/jadolint.py
+-rw-r--r--   0        0        0     2243 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/linguist.py
+-rw-r--r--   0        0        0     5383 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/lizard.py
+-rw-r--r--   0        0        0     2360 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/nomos.py
+-rw-r--r--   0        0        0     2852 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/pylint.py
+-rw-r--r--   0        0        0     2620 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/reverse.py
+-rw-r--r--   0        0        0     4563 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/scancode.py
+-rw-r--r--   0        0        0     4504 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/analyzers/scc.py
+-rw-r--r--   0        0        0    11691 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/cocom.py
+-rw-r--r--   0        0        0     8463 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/codep.py
+-rw-r--r--   0        0        0     6344 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/colang.py
+-rw-r--r--   0        0        0     8182 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/colic.py
+-rw-r--r--   0        0        0     9186 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/coqua.py
+-rw-r--r--   0        0        0     5662 2023-04-26 14:46:33.922412 graal-0.4.6/graal/backends/core/covuln.py
+-rwxr-xr-x   0        0        0     4425 2023-04-26 14:46:33.922412 graal-0.4.6/graal/bin/graal.py
+-rw-r--r--   0        0        0    23643 2023-04-26 14:46:33.922412 graal-0.4.6/graal/graal.py
+-rw-r--r--   0        0        0     1579 2023-04-26 14:46:33.922412 graal-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 14:46:33.922412 graal-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-26 14:46:33.922412 graal-0.4.6/tests/base_analyzer.py
+-rw-r--r--   0        0        0     2056 2023-04-26 14:46:33.922412 graal-0.4.6/tests/base_repo.py
+-rw-r--r--   0        0        0     1575 2023-04-26 14:46:33.922412 graal-0.4.6/tests/data/Dockerfile
+-rw-r--r--   0        0        0   132358 2023-04-26 14:46:33.922412 graal-0.4.6/tests/data/graaltest-dockerfile.zip
+-rw-r--r--   0        0        0   126651 2023-04-26 14:46:33.926412 graal-0.4.6/tests/data/graaltest.zip
+-rw-r--r--   0        0        0     4482 2023-04-26 14:46:33.926412 graal-0.4.6/tests/data/sample_code.py
+-rwxr-xr-x   0        0        0     1174 2023-04-26 14:46:33.926412 graal-0.4.6/tests/run_tests.py
+-rw-r--r--   0        0        0     1222 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_analyzer.py
+-rw-r--r--   0        0        0     5650 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_bandit.py
+-rw-r--r--   0        0        0     3341 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_cloc.py
+-rw-r--r--   0        0        0    14713 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_cocom.py
+-rw-r--r--   0        0        0    14625 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_codep.py
+-rw-r--r--   0        0        0     8707 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_colang.py
+-rw-r--r--   0        0        0    13445 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_colic.py
+-rw-r--r--   0        0        0    20057 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_coqua.py
+-rw-r--r--   0        0        0     7611 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_covuln.py
+-rw-r--r--   0        0        0     2846 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_flake8.py
+-rw-r--r--   0        0        0    29236 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_graal.py
+-rw-r--r--   0        0        0     6391 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_jadolint.py
+-rw-r--r--   0        0        0     2456 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_linguist.py
+-rw-r--r--   0        0        0     4980 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_lizard.py
+-rw-r--r--   0        0        0     2321 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_nomos.py
+-rw-r--r--   0        0        0     3181 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_pylint.py
+-rw-r--r--   0        0        0     2481 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_reverse.py
+-rw-r--r--   0        0        0     3538 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_scancode.py
+-rw-r--r--   0        0        0     4022 2023-04-26 14:46:33.926412 graal-0.4.6/tests/test_scc.py
+-rw-r--r--   0        0        0     1191 2023-04-26 14:46:33.926412 graal-0.4.6/tests/utils.py
+-rw-r--r--   0        0        0    15211 1970-01-01 00:00:00.000000 graal-0.4.6/PKG-INFO
```

### Comparing `graal-0.4.5rc2/LICENSE` & `graal-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/NEWS` & `graal-0.4.6/NEWS`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Releases
 
+  ## graal 0.4.6 - (2023-04-26)
+  
+  * Update Poetry's package dependencies
+
+## graal 0.4.5 - (2023-04-21)
+
+**Dependencies updateds:**
+
+ * Update package dependencies\
+   Update package dependencies and pin `markdown-it-py` to a specific
+   version.
+
+
   ## graal 0.4.4 - (2023-02-03)
   
   * Update Poetry's package dependencies
 
   ## graal 0.4.3 - (2023-02-01)
   
   * Update Poetry's package dependencies
```

### Comparing `graal-0.4.5rc2/README.md` & `graal-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/__init__.py` & `graal-0.4.6/graal/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/__init__.py` & `graal-0.4.6/graal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/__init__.py` & `graal-0.4.6/graal/backends/core/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/analyzer.py` & `graal-0.4.6/graal/backends/core/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/bandit.py` & `graal-0.4.6/graal/backends/core/analyzers/bandit.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/cloc.py` & `graal-0.4.6/graal/backends/core/analyzers/cloc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/flake8.py` & `graal-0.4.6/graal/backends/core/analyzers/flake8.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/jadolint.py` & `graal-0.4.6/graal/backends/core/analyzers/jadolint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/linguist.py` & `graal-0.4.6/graal/backends/core/analyzers/linguist.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/lizard.py` & `graal-0.4.6/graal/backends/core/analyzers/lizard.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/nomos.py` & `graal-0.4.6/graal/backends/core/analyzers/nomos.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/pylint.py` & `graal-0.4.6/graal/backends/core/analyzers/pylint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/reverse.py` & `graal-0.4.6/graal/backends/core/analyzers/reverse.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/scancode.py` & `graal-0.4.6/graal/backends/core/analyzers/scancode.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/analyzers/scc.py` & `graal-0.4.6/graal/backends/core/analyzers/scc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/cocom.py` & `graal-0.4.6/graal/backends/core/cocom.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/codep.py` & `graal-0.4.6/graal/backends/core/codep.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/colang.py` & `graal-0.4.6/graal/backends/core/colang.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/colic.py` & `graal-0.4.6/graal/backends/core/colic.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/coqua.py` & `graal-0.4.6/graal/backends/core/coqua.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/backends/core/covuln.py` & `graal-0.4.6/graal/backends/core/covuln.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/bin/graal.py` & `graal-0.4.6/graal/bin/graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/graal/graal.py` & `graal-0.4.6/graal/graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/pyproject.toml` & `graal-0.4.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graal"
-version = "0.4.5-rc.2"
+version = "0.4.6"
 description = "A generic source code analyzer"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `graal-0.4.5rc2/tests/base_analyzer.py` & `graal-0.4.6/tests/base_analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/base_repo.py` & `graal-0.4.6/tests/base_repo.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/data/Dockerfile` & `graal-0.4.6/tests/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/data/graaltest-dockerfile.zip` & `graal-0.4.6/tests/data/graaltest-dockerfile.zip`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/data/graaltest.zip` & `graal-0.4.6/tests/data/graaltest.zip`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/data/sample_code.py` & `graal-0.4.6/tests/data/sample_code.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/run_tests.py` & `graal-0.4.6/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_analyzer.py` & `graal-0.4.6/tests/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_bandit.py` & `graal-0.4.6/tests/test_bandit.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_cloc.py` & `graal-0.4.6/tests/test_cloc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_cocom.py` & `graal-0.4.6/tests/test_cocom.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_codep.py` & `graal-0.4.6/tests/test_codep.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_colang.py` & `graal-0.4.6/tests/test_colang.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_colic.py` & `graal-0.4.6/tests/test_colic.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_coqua.py` & `graal-0.4.6/tests/test_coqua.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_covuln.py` & `graal-0.4.6/tests/test_covuln.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_flake8.py` & `graal-0.4.6/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_graal.py` & `graal-0.4.6/tests/test_graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_jadolint.py` & `graal-0.4.6/tests/test_jadolint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_linguist.py` & `graal-0.4.6/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_lizard.py` & `graal-0.4.6/tests/test_lizard.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_nomos.py` & `graal-0.4.6/tests/test_nomos.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_pylint.py` & `graal-0.4.6/tests/test_pylint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_reverse.py` & `graal-0.4.6/tests/test_reverse.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_scancode.py` & `graal-0.4.6/tests/test_scancode.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/test_scc.py` & `graal-0.4.6/tests/test_scc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/tests/utils.py` & `graal-0.4.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.5rc2/PKG-INFO` & `graal-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graal
-Version: 0.4.5rc2
+Version: 0.4.6
 Summary: A generic source code analyzer
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

