# Comparing `tmp/facefinder-0.1.1.tar.gz` & `tmp/facefinder-0.1.2.tar.gz`

## Comparing `facefinder-0.1.1.tar` & `facefinder-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.1/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.1/.gitignore
--rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      198 2023-04-24 13:40:08.000000 facefinder-0.1.1/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6651 2023-04-20 14:34:18.000000 facefinder-0.1.1/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.1/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    16403 2023-04-20 14:32:36.000000 facefinder-0.1.1/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.1/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.1/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-04-24 13:41:07.000000 facefinder-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.2/.gitignore
+-rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      198 2023-04-24 13:40:08.000000 facefinder-0.1.2/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6651 2023-04-20 14:34:18.000000 facefinder-0.1.2/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.2/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    16960 2023-04-25 14:34:07.000000 facefinder-0.1.2/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.2/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.2/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-04-25 14:35:01.000000 facefinder-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.2/PKG-INFO
```

### Comparing `facefinder-0.1.1/.github/workflows/CI.yml` & `facefinder-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.1/.gitignore` & `facefinder-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.1/pyproject.toml` & `facefinder-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.1/src/python/facefinder/interact.py` & `facefinder-0.1.2/src/python/facefinder/interact.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.1/src/python/facefinder/metadata.py` & `facefinder-0.1.2/src/python/facefinder/metadata.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.1/src/python/facefinder/metrics.py` & `facefinder-0.1.2/src/python/facefinder/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # Local Imports
 from facefinder import rust
 from . import metadata
 from .interact import InteractiveSession
 
 # Typing imports
-from typing import Callable, Any
+from typing import Callable, Any, Optional
 
 
 def extract_faces(image_path: Path, model: str) -> None:
     with contextlib.redirect_stdout(io.StringIO()):
         return _extract_faces(
             img=str(image_path),
             target_size=metadata.MODEL_TARGET_SIZES[model],
@@ -184,17 +184,20 @@
     )
     input_scores = np.mean(weighted_distances, axis=1)
     return input_scores
 
 
 def get_embedding_metrics(
     model: str,
-    target_path: Path = metadata.PATHS.TARGET_IMAGE,
-    embedding_dir: Path = metadata.PATHS.EMBEDDING_IMAGES,
+    target_path: Optional[Path] = None,
+    embedding_dir: Optional[Path] = None,
 ) -> dict[str, Any]:
+    target_path = target_path or metadata.PATHS.TARGET_IMAGE
+    embedding_dir = embedding_dir or metadata.PATHS.EMBEDDING_IMAGES
+
     # Initial (non-filtered) target/embedding representations
     target_representation = get_representation(target_path, model, skip_face=True)
     paths, representations = get_representations(embedding_dir, model, skip_face=True)
 
     # Filtering representations/paths by distance to target repr
     paths, representations, embedding_target_distances = get_filtered(
         target_representation, representations, paths
@@ -221,17 +224,19 @@
 
 
 def get_input_metrics(
     model: str,
     target_repr: list[float],
     embedding_reprs: list[list[float]],
     embedding_target_distances: list[float],
-    input_dir: Path = metadata.PATHS.UNPROCESSED_IMAGES,
+    input_dir: Optional[Path] = None,
     weight_relevance: int = 1,
 ) -> dict[str, Any]:
+    input_dir = input_dir or metadata.PATHS.UNPROCESSED_IMAGES
+
     # Initial (non-filtered) input representations
     paths, representations = get_representations(input_dir, model)
     x = 0
 
     # Filtering processed images by distance to target
     paths, representations, input_target_distances = get_filtered(
         target_repr, representations, paths
@@ -267,19 +272,23 @@
         "cum_indices": cum_indices,
         "target_indices": target_indices,
     }
 
 
 def get_metrics(
     model: str,
-    target_path: str | Path = metadata.PATHS.TARGET_IMAGE,
-    embedding_dir: str | Path = metadata.PATHS.EMBEDDING_IMAGES,
-    input_dir: str | Path = metadata.PATHS.UNPROCESSED_IMAGES,
+    target_path: Optional[str | Path] = None,
+    embedding_dir: Optional[str | Path] = None,
+    input_dir: Optional[str | Path] = None,
     weight_relevance: int = 1,
 ) -> dict[str, Any]:
+    target_path = target_path or metadata.PATHS.TARGET_IMAGE
+    embedding_dir = embedding_dir or metadata.PATHS.EMBEDDING_IMAGES
+    input_dir = input_dir or metadata.PATHS.UNPROCESSED_IMAGES
+
     embedding_metrics = get_embedding_metrics(model, target_path, embedding_dir)
     input_metrics = get_input_metrics(
         model,
         embedding_metrics["target_representation"],
         embedding_metrics["representations"],
         embedding_metrics["embedding_target_distances"],
         input_dir,
@@ -403,29 +412,35 @@
         "metrics": metrics,
         "metadata": metadata,
     }
 
 
 def get_multimodel_metrics(
     models: list[str],
-    target_path: str | Path = metadata.PATHS.TARGET_IMAGE,
-    embedding_dir: str | Path = metadata.PATHS.EMBEDDING_IMAGES,
-    input_dir: str | Path = metadata.PATHS.UNPROCESSED_IMAGES,
+    target_path: Optional[str | Path] = None,
+    embedding_dir: Optional[str | Path] = None,
+    input_dir: Optional[str | Path] = None,
     weight_relevance: int = 1,
 ) -> dict[str, Any]:
+    target_path = target_path or metadata.PATHS.TARGET_IMAGE
+    embedding_dir = embedding_dir or metadata.PATHS.EMBEDDING_IMAGES
+    input_dir = input_dir or metadata.PATHS.UNPROCESSED_IMAGES
+
     all_metrics = [
         get_metrics(model, target_path, embedding_dir, input_dir, weight_relevance)
         for model in models
     ]
     return merge_metrics(all_metrics)
 
 
 def save_processed_embedding_images(
-    metrics: dict[str, Any], output_dir: Path = metadata.PATHS.EMBEDDING_SCORES_DIR
+    metrics: dict[str, Any], output_dir: Optional[Path] = None
 ) -> None:
+    output_dir = output_dir or metadata.PATHS.EMBEDDING_SCORES_DIR
+
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     n_images = len(metrics["paths"]["embedding"])
     for path, accuracy, coherence in tqdm(
         zip(
             metrics["paths"]["embedding"],
@@ -438,16 +453,18 @@
         image_id = path.name.split("-")[0]
         image_name = f"{accuracy.item():.04f}_{coherence.item():.04f}_{image_id}.png"
         image_path = str(output_dir.joinpath(image_name))
         cv2.imwrite(image_path, cv2.imread(str(path)))
 
 
 def save_processed_input_images(
-    metrics: dict[str, Any], output_dir: Path = metadata.PATHS.PROCESSED_IMAGES
+    metrics: dict[str, Any], output_dir: Optional[Path] = None
 ) -> None:
+    output_dir = output_dir or metadata.PATHS.PROCESSED_IMAGES
+
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     n_images = len(metrics["paths"]["input"])
     for path, score, accuracy, coherence in tqdm(
         zip(
             metrics["paths"]["input"],
```

### Comparing `facefinder-0.1.1/src/python/facefinder/prompting.py` & `facefinder-0.1.2/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.1/Cargo.lock` & `facefinder-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

