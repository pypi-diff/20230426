# Comparing `tmp/accurating-0.4.6.tar.gz` & `tmp/accurating-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.6.tar", max compression
+gzip compressed data, was "accurating-0.4.7.tar", max compression
```

## Comparing `accurating-0.4.6.tar` & `accurating-0.4.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.6/LICENSE
--rw-r--r--   0        0        0     6245 2023-04-23 19:14:57.625128 accurating-0.4.6/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.6/accurating/__init__.py
--rw-r--r--   0        0        0     8412 2023-04-26 05:54:52.763633 accurating-0.4.6/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.6/accurating/tests/__init__.py
--rw-r--r--   0        0        0     3171 2023-04-26 06:21:18.601104 accurating-0.4.6/accurating/tests/model_test.py
--rw-r--r--   0        0        0      632 2023-04-26 06:01:50.420875 accurating-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     6853 1970-01-01 00:00:00.000000 accurating-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.7/LICENSE
+-rw-r--r--   0        0        0     6245 2023-04-23 19:14:57.625128 accurating-0.4.7/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.7/accurating/__init__.py
+-rw-r--r--   0        0        0     8441 2023-04-26 06:45:07.226315 accurating-0.4.7/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.7/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3135 2023-04-26 06:46:15.146580 accurating-0.4.7/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      632 2023-04-26 06:47:02.358765 accurating-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     6853 1970-01-01 00:00:00.000000 accurating-0.4.7/PKG-INFO
```

### Comparing `accurating-0.4.6/LICENSE` & `accurating-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.6/README.md` & `accurating-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `accurating-0.4.6/accurating/model.py` & `accurating-0.4.7/accurating/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,16 @@
         lr *= 1.5 ** (1.0 / 12)
 
     def postprocess():
         rating = {}
         for id, name in enumerate(data.player_name):
             rating[name] = {}
             for season in range(season_count):
-                rating[name][season] = float(params['rating'][id, season])
+                rating[name][season] = float(
+                    params['rating'][id, season]) * 100.0
         ret = Model(rating=rating)
         return ret
 
     return postprocess()
 
 
 def data_from_dicts(matches) -> MatchResultArrays:
```

### Comparing `accurating-0.4.6/accurating/tests/model_test.py` & `accurating-0.4.7/accurating/tests/model_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     )
     model = accurating.fit(test_data, config)
     elos = [[model.rating[f'p{pl}'][season]
              for season in range(2)] for pl in range(3)]
     elos = np.array(elos)
 
     elos = elos - jnp.min(elos, axis=0, keepdims=True)
-    err = jnp.linalg.norm(elos - jnp.array(true_elos))
-    assert err < 0.000001, f'FAIL err={err}; results={model}'
+    err = jnp.linalg.norm(elos - jnp.array(true_elos) * 100.0)
+    assert err < 0.0001, f'FAIL err={err}; results={model}'
 
 
 def test_data_from_dicts():
     json_str = """
     [
       {
         "p1": "Leon",
@@ -93,13 +93,13 @@
         smoothing=0.1,
         max_steps=100,
         do_log=True,
         initial_lr=1.0,
     )
     model = accurating.fit(data, cfg)
     # ratings = np.array([[model.rating[pl][s] for s in range(len(season))] for pl in player_name])
-    assert_almost_equal(model.rating['Alusia'][0], -7.955777374991861e-17)
-    assert_almost_equal(model.rating['Alusia'][1], -9.539554751084385e-17)
-    assert_almost_equal(model.rating['Caesar'][0], -0.1345060654581596)
-    assert_almost_equal(model.rating['Caesar'][1], 0.2690122721761437)
-    assert_almost_equal(model.rating['Leon'][0], 0.1345060654581597)
-    assert_almost_equal(model.rating['Leon'][1], -0.26901227217614354)
+    assert_almost_equal(model.rating['Alusia'][0], 0.0)
+    assert_almost_equal(model.rating['Alusia'][1], 0.0)
+    assert_almost_equal(model.rating['Caesar'][0], -13.45060654581596)
+    assert_almost_equal(model.rating['Caesar'][1], 26.90122721761437)
+    assert_almost_equal(model.rating['Leon'][0], 13.45060654581597)
+    assert_almost_equal(model.rating['Leon'][1], -26.901227217614354)
```

### Comparing `accurating-0.4.6/pyproject.toml` & `accurating-0.4.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.6"
+version = "0.4.7"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
```

### Comparing `accurating-0.4.6/PKG-INFO` & `accurating-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.6
+Version: 0.4.7
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

